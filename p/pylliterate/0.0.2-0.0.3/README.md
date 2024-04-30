# Comparing `tmp/pylliterate-0.0.2.tar.gz` & `tmp/pylliterate-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylliterate-0.0.2.tar", max compression
+gzip compressed data, was "pylliterate-0.0.3.tar", max compression
```

## Comparing `pylliterate-0.0.2.tar` & `pylliterate-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1079 2024-04-24 01:28:01.016185 pylliterate-0.0.2/LICENSE
--rw-r--r--   0        0        0    10157 2024-04-25 20:23:18.036017 pylliterate-0.0.2/pylliterate/__init__.py
--rw-r--r--   0        0        0      273 2024-04-24 20:27:28.869868 pylliterate-0.0.2/pylliterate/__main__.py
--rw-r--r--   0        0        0     3817 2024-04-25 20:23:18.036017 pylliterate-0.0.2/pylliterate/cli.py
--rw-r--r--   0        0        0     3145 2024-04-25 20:23:18.038504 pylliterate-0.0.2/pylliterate/config.py
--rw-r--r--   0        0        0    14790 2024-04-25 20:23:18.038504 pylliterate-0.0.2/pylliterate/core.py
--rw-r--r--   0        0        0      644 2024-04-25 20:23:18.039636 pylliterate-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8542 2024-04-25 20:23:18.035310 pylliterate-0.0.2/Readme.md
--rw-r--r--   0        0        0     9483 1970-01-01 00:00:00.000000 pylliterate-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-24 01:28:01.016185 pylliterate-0.0.3/LICENSE
+-rw-r--r--   0        0        0    10157 2024-04-25 20:23:18.036017 pylliterate-0.0.3/pylliterate/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-24 20:27:28.869868 pylliterate-0.0.3/pylliterate/__main__.py
+-rw-r--r--   0        0        0     3817 2024-04-25 20:23:18.036017 pylliterate-0.0.3/pylliterate/cli.py
+-rw-r--r--   0        0        0     3145 2024-04-25 20:23:18.038504 pylliterate-0.0.3/pylliterate/config.py
+-rw-r--r--   0        0        0    14790 2024-04-25 20:23:18.038504 pylliterate-0.0.3/pylliterate/core.py
+-rw-r--r--   0        0        0      665 2024-04-30 05:05:03.220100 pylliterate-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8544 2024-04-30 05:00:19.884025 pylliterate-0.0.3/Readme.md
+-rw-r--r--   0        0        0     9050 1970-01-01 00:00:00.000000 pylliterate-0.0.3/PKG-INFO
```

### Comparing `pylliterate-0.0.2/LICENSE` & `pylliterate-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.2/pylliterate/__init__.py` & `pylliterate-0.0.3/pylliterate/__init__.py`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.2/pylliterate/cli.py` & `pylliterate-0.0.3/pylliterate/cli.py`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.2/pylliterate/config.py` & `pylliterate-0.0.3/pylliterate/config.py`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.2/pylliterate/core.py` & `pylliterate-0.0.3/pylliterate/core.py`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.2/Readme.md` & `pylliterate-0.0.3/Readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # Pylliterate: python illiterate programing
 
-> Disclaimer: This code is a copy **with improvements** of the original [illiterate](https://github.com/apiad/illiterate) project because was discontinued since 2022.
-
 [<img alt="PyPI" src="https://img.shields.io/pypi/v/pylliterate">](https://pypi.org/project/pylliterate)
 [<img alt="PyPI - License" src="https://img.shields.io/pypi/l/pylliterate">](https://github.com/gaspect/pylliterate)
 [<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/pylliterate">](https://pypi.org/project/pylliterate)
 [<img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/gaspect/pylliterate?style=social">](https://github.com/gaspect/pylliterate/stargazers)
 [<img alt="GitHub forks" src="https://img.shields.io/github/forks/gaspect/pylliterate?style=social">](https://github.com/gaspect/pylliterate/network/members)
 
 > Unobtrusive literate programming experience for Python pragmatists
@@ -117,7 +115,10 @@
 You can mix pylliterate with regular markdown simply by hand-crafting all the documentation you want in pure Markdown and then conveniently designing your `mkdocs.yml`.
 You can also see the `mkdocs.yml` in this repository to get an idea of how that configuration looks, but beware, I'm using some custom
 themes and other stuff you might or might not want.
 
 ## Next steps
 
 This project is quite small, but it is a self-fulfilling prophecy. The remaining [documentation](https://gaspect.github.io/pylliterate) has been written with `pylliterate`. Just keep reading, and you'll see for yourself what does this mean.
+
+
+> Disclaimer: This code is a copy **with improvements** of the original [illiterate](https://github.com/apiad/illiterate) project because was discontinued since 2022.
```

### Comparing `pylliterate-0.0.2/PKG-INFO` & `pylliterate-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,27 @@
 Metadata-Version: 2.1
 Name: pylliterate
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unobtrusive literate programming experience for Python pragmatists
 License: MIT
 Author: Jesús Enrique Fuentes
 Author-email: jesusefg12@gmail.com
+Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: PyYAML (==6.0.1)
-Requires-Dist: pydantic (==2.7.1)
-Requires-Dist: rich (==9.0.1)
-Requires-Dist: typer (==0.12.3)
-Requires-Dist: watchdog (==2.3.1)
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
+Requires-Dist: rich (>=9.0.1,<10.0.0)
+Requires-Dist: typer (>=0.12.3,<0.13.0)
+Requires-Dist: watchdog (>=2.3.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Pylliterate: python illiterate programing
 
-> Disclaimer: This code is a copy **with improvements** of the original [illiterate](https://github.com/apiad/illiterate) project because was discontinued since 2022.
-
 [<img alt="PyPI" src="https://img.shields.io/pypi/v/pylliterate">](https://pypi.org/project/pylliterate)
 [<img alt="PyPI - License" src="https://img.shields.io/pypi/l/pylliterate">](https://github.com/gaspect/pylliterate)
 [<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/pylliterate">](https://pypi.org/project/pylliterate)
 [<img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/gaspect/pylliterate?style=social">](https://github.com/gaspect/pylliterate/stargazers)
 [<img alt="GitHub forks" src="https://img.shields.io/github/forks/gaspect/pylliterate?style=social">](https://github.com/gaspect/pylliterate/network/members)
 
 > Unobtrusive literate programming experience for Python pragmatists
@@ -145,7 +134,10 @@
 You can also see the `mkdocs.yml` in this repository to get an idea of how that configuration looks, but beware, I'm using some custom
 themes and other stuff you might or might not want.
 
 ## Next steps
 
 This project is quite small, but it is a self-fulfilling prophecy. The remaining [documentation](https://gaspect.github.io/pylliterate) has been written with `pylliterate`. Just keep reading, and you'll see for yourself what does this mean.
 
+
+> Disclaimer: This code is a copy **with improvements** of the original [illiterate](https://github.com/apiad/illiterate) project because was discontinued since 2022.
+
```

