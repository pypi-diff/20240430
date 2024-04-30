# Comparing `tmp/vr180_convert-0.1.0.tar.gz` & `tmp/vr180_convert-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vr180_convert-0.1.0.tar", max compression
+gzip compressed data, was "vr180_convert-0.2.0.tar", max compression
```

## Comparing `vr180_convert-0.1.0.tar` & `vr180_convert-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1061 2024-04-19 12:21:49.405093 vr180_convert-0.1.0/LICENSE
--rw-r--r--   0        0        0     6186 2024-04-19 12:21:49.405093 vr180_convert-0.1.0/README.md
--rw-r--r--   0        0        0     3819 2024-04-19 12:21:50.329093 vr180_convert-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      707 2024-04-19 12:21:50.329093 vr180_convert-0.1.0/src/vr180_convert/__init__.py
--rw-r--r--   0        0        0      113 2024-04-19 12:21:49.421093 vr180_convert-0.1.0/src/vr180_convert/__main__.py
--rw-r--r--   0        0        0     4979 2024-04-19 12:21:49.421093 vr180_convert-0.1.0/src/vr180_convert/cli.py
--rw-r--r--   0        0        0        0 2024-04-19 12:21:49.421093 vr180_convert-0.1.0/src/vr180_convert/py.typed
--rw-r--r--   0        0        0     5702 2024-04-19 12:21:49.421093 vr180_convert-0.1.0/src/vr180_convert/remapper.py
--rw-r--r--   0        0        0     1889 2024-04-19 12:21:49.421093 vr180_convert-0.1.0/src/vr180_convert/testing.py
--rw-r--r--   0        0        0    11723 2024-04-19 12:21:49.421093 vr180_convert-0.1.0/src/vr180_convert/transformer.py
--rw-r--r--   0        0        0     7584 1970-01-01 00:00:00.000000 vr180_convert-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-04-30 08:11:19.111633 vr180_convert-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8872 2024-04-30 08:11:19.111633 vr180_convert-0.2.0/README.md
+-rw-r--r--   0        0        0     3834 2024-04-30 08:11:19.931634 vr180_convert-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      707 2024-04-30 08:11:19.935634 vr180_convert-0.2.0/src/vr180_convert/__init__.py
+-rw-r--r--   0        0        0      113 2024-04-30 08:11:19.127633 vr180_convert-0.2.0/src/vr180_convert/__main__.py
+-rw-r--r--   0        0        0    12797 2024-04-30 08:11:19.127633 vr180_convert-0.2.0/src/vr180_convert/cli.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:11:19.127633 vr180_convert-0.2.0/src/vr180_convert/py.typed
+-rw-r--r--   0        0        0    12090 2024-04-30 08:11:19.127633 vr180_convert-0.2.0/src/vr180_convert/remapper.py
+-rw-r--r--   0        0        0     1889 2024-04-30 08:11:19.127633 vr180_convert-0.2.0/src/vr180_convert/testing.py
+-rw-r--r--   0        0        0    18069 2024-04-30 08:11:19.127633 vr180_convert-0.2.0/src/vr180_convert/transformer.py
+-rw-r--r--   0        0        0    10270 1970-01-01 00:00:00.000000 vr180_convert-0.2.0/PKG-INFO
```

### Comparing `vr180_convert-0.1.0/LICENSE` & `vr180_convert-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.1.0/pyproject.toml` & `vr180_convert-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vr180-convert"
-version = "0.1.0"
+version = "0.2.0"
 description = "Simple VR180 image converter"
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/vr180-convert"
 documentation = "https://vr180-convert.readthedocs.io"
 classifiers = [
@@ -33,15 +33,15 @@
 opencv-python = "^4.9.0.80"
 attrs = "^23.2.0"
 scikit-learn = "^1.4.2"
 numpy-quaternion = "^2023.0.3"
 strenum = "^0.4.15"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.0"
+pytest = "^8.0.0"
 pytest-cov = "^3.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = { version = ">=0.16", python = ">=3.11"}
@@ -87,25 +87,26 @@
     "if TYPE_CHECKING",
     "raise NotImplementedError",
     'if __name__ == "__main__":',
 ]
 
 [tool.ruff]
 target-version = "py38"
-line-length = 88
+line-length = 110
 unsafe-fixes = true
 ignore = [
     "D203", # 1 blank line required before class docstring
     "D212", # Multi-line docstring summary should start at the first line
     "D100", # Missing docstring in public module
     "D104", # Missing docstring in public package
     "D107", # Missing docstring in `__init__`
     "D401", # First line of docstring should be in imperative mood
     "D101",
     "D102",
+    "D417",
 ]
 select = [
     "B",   # flake8-bugbear
     "D",   # flake8-docstrings
     "C4",  # flake8-comprehensions
     "S",   # flake8-bandit
     "F",   # pyflake
```

### Comparing `vr180_convert-0.1.0/src/vr180_convert/__init__.py` & `vr180_convert-0.2.0/src/vr180_convert/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 from .remapper import apply, apply_lr, get_map
 from .transformer import (
     DenormalizeTransformer,
     EquirectangularEncoder,
     Euclidean3DRotator,
     Euclidean3DTransformer,
     FisheyeDecoder,
```

### Comparing `vr180_convert-0.1.0/src/vr180_convert/testing.py` & `vr180_convert-0.2.0/src/vr180_convert/testing.py`

 * *Files identical despite different names*

