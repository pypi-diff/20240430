# Comparing `tmp/vision_mamba-0.0.1.tar.gz` & `tmp/vision_mamba-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_mamba-0.0.1.tar", max compression
+gzip compressed data, was "vision_mamba-0.0.5.tar", max compression
```

## Comparing `vision_mamba-0.0.1.tar` & `vision_mamba-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-01-21 23:06:37.273005 vision_mamba-0.0.1/LICENSE
--rw-r--r--   0        0        0      723 2024-01-21 23:09:48.533885 vision_mamba-0.0.1/README.md
--rw-r--r--   0        0        0     1372 2024-01-21 23:10:38.148353 vision_mamba-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-21 23:07:22.657815 vision_mamba-0.0.1/vision_mamba/__init__.py
--rw-r--r--   0        0        0     2701 2024-01-21 23:08:42.615017 vision_mamba-0.0.1/vision_mamba/model.py
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 vision_mamba-0.0.1/setup.py
--rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 vision_mamba-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-01-21 23:06:37.273005 vision_mamba-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1767 2024-04-30 03:23:54.672675 vision_mamba-0.0.5/README.md
+-rw-r--r--   0        0        0     1364 2024-04-30 03:28:16.769518 vision_mamba-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-30 03:23:54.692729 vision_mamba-0.0.5/vision_mamba/__init__.py
+-rw-r--r--   0        0        0     7822 2024-04-30 03:24:57.742893 vision_mamba-0.0.5/vision_mamba/model.py
+-rw-r--r--   0        0        0     2487 1970-01-01 00:00:00.000000 vision_mamba-0.0.5/setup.py
+-rw-r--r--   0        0        0     2771 1970-01-01 00:00:00.000000 vision_mamba-0.0.5/PKG-INFO
```

### Comparing `vision_mamba-0.0.1/LICENSE` & `vision_mamba-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_mamba-0.0.1/pyproject.toml` & `vision_mamba-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-mamba"
-version = "0.0.1"
+version = "0.0.5"
 description = "Vision Mamba - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/VisionMamba"
 documentation = "https://github.com/kyegomez/VisionMamba"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/VisionMamba"
@@ -18,25 +18,24 @@
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.9"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-swarms = "*"
+python = "^3.9"
 zetascale = "*"
 einops = "*"
 torch = "*"
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.6"
 types-toml = "^0.10.8.1"
 types-redis = "^4.3.21.6"
-types-pytz = "^2023.3.0.0"
+types-pytz = ">=2023.3,<2025.0"
 black = "^23.1.0"
 types-chardet = "^5.0.4.6"
 mypy-protobuf = "^3.0.0"
 
 
 [tool.autopep8]
 max_line_length = 80
```

