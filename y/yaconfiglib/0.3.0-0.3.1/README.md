# Comparing `tmp/yaconfiglib-0.3.0.tar.gz` & `tmp/yaconfiglib-0.3.1.tar.gz`

## Comparing `yaconfiglib-0.3.0.tar` & `yaconfiglib-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/examples/config.toml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/examples/hiera.yaml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/examples/includeme.yaml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/examples/jinja.yaml.j2
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/example.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/__init__.py
--rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/loader.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/backends/__init__.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/backends/base.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/backends/jinja2.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/backends/toml.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/backends/yaml.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/utils/__init__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/utils/enum.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/utils/jinja2.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/utils/log.py
--rw-r--r--   0        0        0    16694 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/utils/merge.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/utils/source.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/LICENSE
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/README.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/examples/config.toml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/examples/hiera.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/examples/includeme.yaml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/examples/jinja.yaml.j2
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/example.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/yaconfiglib/__init__.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/yaconfiglib/loader.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/yaconfiglib/backends/__init__.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/yaconfiglib/backends/base.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/yaconfiglib/backends/jinja2.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/yaconfiglib/backends/toml.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/yaconfiglib/backends/yaml.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/yaconfiglib/utils/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/yaconfiglib/utils/enum.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/yaconfiglib/utils/jinja2.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/yaconfiglib/utils/log.py
+-rw-r--r--   0        0        0    16694 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/yaconfiglib/utils/merge.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/src/yaconfiglib/utils/source.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/LICENSE
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/README.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 yaconfiglib-0.3.1/PKG-INFO
```

### Comparing `yaconfiglib-0.3.0/src/example.py` & `yaconfiglib-0.3.1/src/example.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import sys
 from dataclasses import dataclass
 
 import yaml
 
-from yaconfiglib import YamlConfig
 from yaconfiglib.loader import ConfigLoader
 from yaconfiglib.loader import ConfigLoaderMergeMethod as MergeMethod
 from yaconfiglib.utils.log import LogLevel
 from yaconfiglib.utils.merge import typed_merge
 
 
 @dataclass
@@ -29,19 +28,17 @@
     dict(field_1=1, field_2=2),
     init=True,
 )
 
 
 logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
 
-loader = YamlConfig()
-
-yaml.SafeLoader.add_constructor("!load", loader)
 
 configloader = ConfigLoader()
+yaml.SafeLoader.add_constructor("!load", configloader)
 
 hieraconf = configloader.load(
     """#!test.yaml
 pathname:
   stem: root
 """,
     "examples/hiera.yaml",
@@ -52,15 +49,15 @@
 
 config = yaml.safe_load(
     "test: !load {pathname: examples/includeme.yaml, transform: '{ pathname.name: value.include }', key_factory: '%pathname.as_posix()', type: map }"
 )
 print(yaml.dump(config, indent=2))
 
 
-jinjaconfig = loader.load("examples/jinja.yaml.j2", configloader=configloader)
+jinjaconfig = configloader.load("examples/jinja.yaml.j2")
 print(yaml.dump(jinjaconfig, indent=2))
 
 pyproject = configloader.load("pyproject.toml")
 print(yaml.dump(pyproject, indent=2))
 
 
 a = MergeMethod(1)
```

### Comparing `yaconfiglib-0.3.0/src/yaconfiglib/loader.py` & `yaconfiglib-0.3.1/src/yaconfiglib/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .utils.enum import IntEnum
 from .utils.log import Logger, LogLevel, getLogger
 from .utils.merge import Merge, MergeMethod, is_array
 from .utils.source import SourceLike, parse_sources
 
 _LOGGER = logging.getLogger("yaconfiglib")
 
-__all__ = ["ConfigLoader"]
+__all__ = ["ConfigLoader", "ConfigLoaderMergeMethod"]
 
 
 class _ConfigLoaderMergeMethod(IntEnum):
     Last = 4
     List = 5
     Hash = 6
 
@@ -89,18 +89,15 @@
 else:
     ConfigLoaderMergeMethod = MergeMethod.extend(
         _ConfigLoaderMergeMethod,
         name=_ConfigLoaderMergeMethod.__name__.removeprefix("_"),
     )
 
 
-class ConfigLoader:
-
-    DEFAULT_PATH_GENERATOR = LocalPath
-    DEFAULT_ENCODING = "utf-8"
+class ConfigLoader(ConfigBackend):
 
     def __init__(
         self,
         base_dir: str | Path = "",
         *,
         encoding: str = None,
         path_factory: typing.Callable[[str], Path] = None,
@@ -114,15 +111,15 @@
     ) -> None:
         self.merge = (
             merge if isinstance(merge, Merge) else ConfigLoaderMergeMethod(merge)
         )
         self.merge_options = {} if merge_options is None else merge_options
         self.interpolate = False if interpolate is None else bool(interpolate)
         self.logger = getLogger(logger)
-        self.path_factory = path_factory or self.DEFAULT_PATH_GENERATOR
+        self.path_factory = path_factory or self.DEFAULT_PATH_FACTORY
         self.base_dir = base_dir or ""
         self.encoding = encoding or self.DEFAULT_ENCODING
         self.recursive = False if recursive is None else recursive
         self.configloader_factory = configloader_factory or (
             lambda path: ConfigBackend.get_class_by_path(path)()
         )
         self.key_factory = key_factory or (lambda path, value: path.stem)
```

### Comparing `yaconfiglib-0.3.0/src/yaconfiglib/backends/jinja2.py` & `yaconfiglib-0.3.1/src/yaconfiglib/backends/jinja2.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         self,
         path: Path,
         encoding: str = None,
         configloader: ConfigBackend = None,
         envoriment: Environment = None,
         **kwargs,
     ) -> None:
+        encoding = encoding or self.DEFAULT_ENCODING
         template = jinja2.load_template(
             path.read_text(encoding=encoding),
             environment=envoriment or jinja2.DEFAULT_ENV,
         )
         pathname = PosixPathname(path.as_posix())
         rendered = template.render(pathname=pathname)
         mempath = MemPath(
```

### Comparing `yaconfiglib-0.3.0/src/yaconfiglib/utils/enum.py` & `yaconfiglib-0.3.1/src/yaconfiglib/utils/enum.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.0/src/yaconfiglib/utils/jinja2.py` & `yaconfiglib-0.3.1/src/yaconfiglib/utils/jinja2.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.0/src/yaconfiglib/utils/log.py` & `yaconfiglib-0.3.1/src/yaconfiglib/utils/log.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.0/src/yaconfiglib/utils/merge.py` & `yaconfiglib-0.3.1/src/yaconfiglib/utils/merge.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.0/src/yaconfiglib/utils/source.py` & `yaconfiglib-0.3.1/src/yaconfiglib/utils/source.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.0/LICENSE` & `yaconfiglib-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.3.0/pyproject.toml` & `yaconfiglib-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "yaconfiglib"
-version = "0.3.0"
+version = "0.3.1"
 authors = [{ name = "Jose A" }]
 description = "Another Config lib for python, basically load config/yaml/toml/... files and add some features like relative import and templating."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `yaconfiglib-0.3.0/PKG-INFO` & `yaconfiglib-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yaconfiglib
-Version: 0.3.0
+Version: 0.3.1
 Summary: Another Config lib for python, basically load config/yaml/toml/... files and add some features like relative import and templating.
 Project-URL: Homepage, https://github.com/jose-pr/yaconfiglib/
 Project-URL: Issues, https://github.com/jose-pr/yaconfiglib/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

