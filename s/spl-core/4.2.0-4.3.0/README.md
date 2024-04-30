# Comparing `tmp/spl_core-4.2.0.tar.gz` & `tmp/spl_core-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_core-4.2.0.tar", max compression
+gzip compressed data, was "spl_core-4.3.0.tar", max compression
```

## Comparing `spl_core-4.2.0.tar` & `spl_core-4.3.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1099 2024-04-29 17:57:39.664572 spl_core-4.2.0/LICENSE
--rw-r--r--   0        0        0      824 2024-04-29 17:57:39.664572 spl_core-4.2.0/README.md
--rw-r--r--   0        0        0     4378 2024-04-29 17:57:40.592574 spl_core-4.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-29 17:57:40.592574 spl_core-4.2.0/src/spl_core/__init__.py
--rw-r--r--   0        0        0      361 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/__run.py
--rw-r--r--   0        0        0        0 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/common/__init__.py
--rw-r--r--   0        0        0     2079 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/common/command_line_executor.py
--rw-r--r--   0        0        0      462 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/common/path.py
--rw-r--r--   0        0        0        0 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/gcov_maid/__init__.py
--rw-r--r--   0        0        0     1455 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/gcov_maid/gcov_maid.py
--rw-r--r--   0        0        0        0 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kconfig/__init__.py
--rw-r--r--   0        0        0     9795 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kconfig/kconfig.py
--rw-r--r--   0        0        0        0 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/__init__.py
--rw-r--r--   0        0        0     2741 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/create.py
--rw-r--r--   0        0        0      553 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/.vscode/cmake-variants.json
--rw-r--r--   0        0        0      589 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/KConfig
--rw-r--r--   0        0        0      117 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/greeter/CMakeLists.txt
--rw-r--r--   0        0        0    11090 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/greeter/doc/_images/screenshot.png
--rw-r--r--   0        0        0      500 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/greeter/doc/index.rst
--rw-r--r--   0        0        0      431 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/greeter/src/greeter.c
--rw-r--r--   0        0        0       99 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/greeter/src/greeter.h
--rw-r--r--   0        0        0      482 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/greeter/test/test_greeter.cc
--rw-r--r--   0        0        0       68 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/main/CMakeLists.txt
--rw-r--r--   0        0        0      303 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/main/doc/index.rst
--rw-r--r--   0        0        0      215 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/main/src/main.c
--rw-r--r--   0        0        0      437 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/test/EnglishVariant/test__EnglishVariant.py
--rw-r--r--   0        0        0      436 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/test/German/test__GermanVariant.py
--rw-r--r--   0        0        0       94 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/variants/EnglishVariant/config.cmake
--rw-r--r--   0        0        0       61 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/variants/EnglishVariant/parts.cmake
--rw-r--r--   0        0        0       94 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/variants/GermanVariant/config.cmake
--rw-r--r--   0        0        0      188 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/variants/GermanVariant/config.txt
--rw-r--r--   0        0        0       61 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/variants/GermanVariant/parts.cmake
--rw-r--r--   0        0        0      638 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/.gitignore
--rw-r--r--   0        0        0      269 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/cmake-kits.json
--rw-r--r--   0        0        0      624 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/extensions.json
--rw-r--r--   0        0        0     1103 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/launch.json
--rw-r--r--   0        0        0     1369 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/settings.json
--rw-r--r--   0        0        0     3434 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/tasks.json
--rw-r--r--   0        0        0     1817 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/CMakeLists.txt
--rw-r--r--   0        0        0       73 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/build.bat
--rw-r--r--   0        0        0    11057 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/build.ps1
--rw-r--r--   0        0        0     6775 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/conf.py
--rw-r--r--   0        0        0   123953 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/Doxyfile.in
--rw-r--r--   0        0        0       91 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/common/index.rst
--rw-r--r--   0        0        0      590 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/components/index.rst
--rw-r--r--   0        0        0     1072 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/doxygen-awesome/LICENSE
--rw-r--r--   0        0        0    63045 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/doxygen-awesome/doxygen-awesome.css
--rw-r--r--   0        0        0       44 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/software_architecture/index.rst
--rw-r--r--   0        0        0       95 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/software_requirements/index.rst
--rw-r--r--   0        0        0     1213 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/test_report_template.txt
--rw-r--r--   0        0        0     1044 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/index.rst
--rw-r--r--   0        0        0       85 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/pipfile
--rw-r--r--   0        0        0      159 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/pytest.ini
--rw-r--r--   0        0        0      219 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/scoopfile.json
--rw-r--r--   0        0        0      713 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/tools/toolchains/clang/toolchain.cmake
--rw-r--r--   0        0        0      183 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/tools/toolchains/gcc/toolchain.cmake
--rw-r--r--   0        0        0     1225 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/main.py
--rw-r--r--   0        0        0     3221 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/test_utils/base_variant_test_runner.py
--rw-r--r--   0        0        0     5599 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/test_utils/spl_build.py
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 spl_core-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-30 06:31:19.631405 spl_core-4.3.0/LICENSE
+-rw-r--r--   0        0        0      824 2024-04-30 06:31:19.631405 spl_core-4.3.0/README.md
+-rw-r--r--   0        0        0     4431 2024-04-30 06:31:20.471400 spl_core-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-30 06:31:20.471400 spl_core-4.3.0/src/spl_core/__init__.py
+-rw-r--r--   0        0        0      361 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/__run.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/common/__init__.py
+-rw-r--r--   0        0        0     2079 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/common/command_line_executor.py
+-rw-r--r--   0        0        0      462 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/common/path.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/gcov_maid/__init__.py
+-rw-r--r--   0        0        0     1455 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/gcov_maid/gcov_maid.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kconfig/__init__.py
+-rw-r--r--   0        0        0     9795 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kconfig/kconfig.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/__init__.py
+-rw-r--r--   0        0        0     2741 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/create.py
+-rw-r--r--   0        0        0      553 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/.vscode/cmake-variants.json
+-rw-r--r--   0        0        0      589 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/KConfig
+-rw-r--r--   0        0        0      117 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/src/greeter/CMakeLists.txt
+-rw-r--r--   0        0        0    11090 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/src/greeter/doc/_images/screenshot.png
+-rw-r--r--   0        0        0      500 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/src/greeter/doc/index.rst
+-rw-r--r--   0        0        0      431 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/src/greeter/src/greeter.c
+-rw-r--r--   0        0        0       99 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/src/greeter/src/greeter.h
+-rw-r--r--   0        0        0      482 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/src/greeter/test/test_greeter.cc
+-rw-r--r--   0        0        0       68 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/src/main/CMakeLists.txt
+-rw-r--r--   0        0        0      303 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/src/main/doc/index.rst
+-rw-r--r--   0        0        0      215 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/src/main/src/main.c
+-rw-r--r--   0        0        0      437 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/test/EnglishVariant/test__EnglishVariant.py
+-rw-r--r--   0        0        0      436 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/test/German/test__GermanVariant.py
+-rw-r--r--   0        0        0       94 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/variants/EnglishVariant/config.cmake
+-rw-r--r--   0        0        0       61 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/variants/EnglishVariant/parts.cmake
+-rw-r--r--   0        0        0       94 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/variants/GermanVariant/config.cmake
+-rw-r--r--   0        0        0      188 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/variants/GermanVariant/config.txt
+-rw-r--r--   0        0        0       61 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/application/variants/GermanVariant/parts.cmake
+-rw-r--r--   0        0        0      638 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/.gitignore
+-rw-r--r--   0        0        0      269 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/.vscode/cmake-kits.json
+-rw-r--r--   0        0        0      624 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/.vscode/extensions.json
+-rw-r--r--   0        0        0     1103 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/.vscode/launch.json
+-rw-r--r--   0        0        0     1369 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/.vscode/settings.json
+-rw-r--r--   0        0        0     3434 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/.vscode/tasks.json
+-rw-r--r--   0        0        0     1817 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/CMakeLists.txt
+-rw-r--r--   0        0        0       73 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/build.bat
+-rw-r--r--   0        0        0    11057 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/build.ps1
+-rw-r--r--   0        0        0     6775 2024-04-30 06:31:19.635405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/conf.py
+-rw-r--r--   0        0        0   123953 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/doc/Doxyfile.in
+-rw-r--r--   0        0        0       91 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/doc/common/index.rst
+-rw-r--r--   0        0        0      590 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/doc/components/index.rst
+-rw-r--r--   0        0        0     1072 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/doc/doxygen-awesome/LICENSE
+-rw-r--r--   0        0        0    63045 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/doc/doxygen-awesome/doxygen-awesome.css
+-rw-r--r--   0        0        0       44 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/doc/software_architecture/index.rst
+-rw-r--r--   0        0        0       95 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/doc/software_requirements/index.rst
+-rw-r--r--   0        0        0     1213 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/doc/test_report_template.txt
+-rw-r--r--   0        0        0     1044 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/index.rst
+-rw-r--r--   0        0        0       85 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/pipfile
+-rw-r--r--   0        0        0      159 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/pytest.ini
+-rw-r--r--   0        0        0      219 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/scoopfile.json
+-rw-r--r--   0        0        0      713 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/tools/toolchains/clang/toolchain.cmake
+-rw-r--r--   0        0        0      183 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/kickstart/templates/project/tools/toolchains/gcc/toolchain.cmake
+-rw-r--r--   0        0        0     1225 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/main.py
+-rw-r--r--   0        0        0     3221 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/test_utils/base_variant_test_runner.py
+-rw-r--r--   0        0        0     5599 2024-04-30 06:31:19.639405 spl_core-4.3.0/src/spl_core/test_utils/spl_build.py
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 spl_core-4.3.0/PKG-INFO
```

### Comparing `spl_core-4.2.0/LICENSE` & `spl_core-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/README.md` & `spl_core-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/pyproject.toml` & `spl_core-4.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spl-core"
-version = "4.2.0"
+version = "4.3.0"
 description = "Software Product Line Support for CMake"
 authors = ["Avengineers <karsten.guenther@kamg.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/avengineers/spl-core"
 documentation = "https://spl-core.readthedocs.io"
 classifiers = [
@@ -14,14 +14,17 @@
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
 ]
 packages = [
     { include = "spl_core", from = "src" },
 ]
 
+[tool.poetry.scripts]
+please = "spl_core.main:main"
+
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/avengineers/spl-core/issues"
 "Changelog" = "https://github.com/avengineers/spl-core/blob/develop/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 py-app-dev = "^2.1.0"
```

### Comparing `spl_core-4.2.0/src/spl_core/common/command_line_executor.py` & `spl_core-4.3.0/src/spl_core/common/command_line_executor.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/gcov_maid/gcov_maid.py` & `spl_core-4.3.0/src/spl_core/gcov_maid/gcov_maid.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kconfig/kconfig.py` & `spl_core-4.3.0/src/spl_core/kconfig/kconfig.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/create.py` & `spl_core-4.3.0/src/spl_core/kickstart/create.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/application/.vscode/cmake-variants.json` & `spl_core-4.3.0/src/spl_core/kickstart/templates/application/.vscode/cmake-variants.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/application/KConfig` & `spl_core-4.3.0/src/spl_core/kickstart/templates/application/KConfig`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/greeter/doc/_images/screenshot.png` & `spl_core-4.3.0/src/spl_core/kickstart/templates/application/src/greeter/doc/_images/screenshot.png`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/.gitignore` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/extensions.json` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/launch.json` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/settings.json` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/tasks.json` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/CMakeLists.txt` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/build.ps1` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/build.ps1`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/conf.py` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/conf.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/Doxyfile.in` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/doc/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/components/index.rst` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/doc/components/index.rst`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/doxygen-awesome/LICENSE` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/doc/doxygen-awesome/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/doxygen-awesome/doxygen-awesome.css` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/doc/doxygen-awesome/doxygen-awesome.css`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/test_report_template.txt` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/doc/test_report_template.txt`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/index.rst` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/index.rst`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/kickstart/templates/project/tools/toolchains/clang/toolchain.cmake` & `spl_core-4.3.0/src/spl_core/kickstart/templates/project/tools/toolchains/clang/toolchain.cmake`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/main.py` & `spl_core-4.3.0/src/spl_core/main.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/test_utils/base_variant_test_runner.py` & `spl_core-4.3.0/src/spl_core/test_utils/base_variant_test_runner.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/src/spl_core/test_utils/spl_build.py` & `spl_core-4.3.0/src/spl_core/test_utils/spl_build.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.2.0/PKG-INFO` & `spl_core-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spl-core
-Version: 4.2.0
+Version: 4.3.0
 Summary: Software Product Line Support for CMake
 Home-page: https://github.com/avengineers/spl-core
 License: MIT
 Author: Avengineers
 Author-email: karsten.guenther@kamg.de
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

