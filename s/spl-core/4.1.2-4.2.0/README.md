# Comparing `tmp/spl_core-4.1.2.tar.gz` & `tmp/spl_core-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_core-4.1.2.tar", max compression
+gzip compressed data, was "spl_core-4.2.0.tar", max compression
```

## Comparing `spl_core-4.1.2.tar` & `spl_core-4.2.0.tar`

### file list

```diff
@@ -1,68 +1,60 @@
--rw-r--r--   0        0        0     1099 2024-04-18 13:58:45.985234 spl_core-4.1.2/LICENSE
--rw-r--r--   0        0        0      824 2024-04-18 13:58:45.985234 spl_core-4.1.2/README.md
--rw-r--r--   0        0        0     4335 2024-04-18 13:58:47.185249 spl_core-4.1.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-18 13:58:47.185249 spl_core-4.1.2/src/spl_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/common/__init__.py
--rw-r--r--   0        0        0     2054 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/common/cmake.py
--rw-r--r--   0        0        0     2019 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/common/command_line_executor.py
--rw-r--r--   0        0        0      462 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/common/path.py
--rw-r--r--   0        0        0        0 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/gcov_maid/__init__.py
--rw-r--r--   0        0        0     1455 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/gcov_maid/gcov_maid.py
--rw-r--r--   0        0        0        0 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/kconfig/__init__.py
--rw-r--r--   0        0        0     9795 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/kconfig/kconfig.py
--rw-r--r--   0        0        0        0 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/__init__.py
--rw-r--r--   0        0        0     7342 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/creator.py
--rw-r--r--   0        0        0      239 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/cookiecutter.json
--rw-r--r--   0        0        0       33 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.flake8
--rw-r--r--   0        0        0      599 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.gitignore
--rw-r--r--   0        0        0      269 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-kits.json
--rw-r--r--   0        0        0      718 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-variants.json
--rw-r--r--   0        0        0      626 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/extensions.json
--rw-r--r--   0        0        0     1103 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/launch.json
--rw-r--r--   0        0        0     1369 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/settings.json
--rw-r--r--   0        0        0     2853 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/tasks.json
--rw-r--r--   0        0        0     1400 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/CMakeLists.txt
--rw-r--r--   0        0        0      598 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/KConfig
--rw-r--r--   0        0        0     1108 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/LICENSE
--rw-r--r--   0        0        0      513 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/Pipfile
--rw-r--r--   0        0        0      337 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/README.md
--rw-r--r--   0        0        0       73 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.bat
--rw-r--r--   0        0        0    10528 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.ps1
--rw-r--r--   0        0        0     6705 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/conf.py
--rw-r--r--   0        0        0   123927 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/Doxyfile.in
--rw-r--r--   0        0        0       90 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/common/index.rst
--rw-r--r--   0        0        0      594 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/components/index.rst
--rw-r--r--   0        0        0     1072 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/LICENSE
--rw-r--r--   0        0        0    63071 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/doxygen-awesome.css
--rw-r--r--   0        0        0       44 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/software_architecture/index.rst
--rw-r--r--   0        0        0       95 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/software_requirements/index.rst
--rw-r--r--   0        0        0     1217 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/test_report_template.txt
--rw-r--r--   0        0        0     1021 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/index.rst
--rw-r--r--   0        0        0       46 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/install-mandatory.bat
--rw-r--r--   0        0        0      127 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/pytest.ini
--rw-r--r--   0        0        0     1077 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/scoopfile.json
--rw-r--r--   0        0        0     1518 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_build.py
--rw-r--r--   0        0        0      941 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_unittests.py
--rw-r--r--   0        0        0      617 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/utils.py
--rw-r--r--   0        0        0      348 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/tools/setup/git-config.ps1
--rw-r--r--   0        0        0      123 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/CMakeLists.txt
--rw-r--r--   0        0        0     7588 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/_images/screenshot.png
--rw-r--r--   0        0        0      477 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/design.rst
--rw-r--r--   0        0        0      135 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/index.rst
--rw-r--r--   0        0        0      433 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/src/component.c
--rw-r--r--   0        0        0       40 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/src/component.h
--rw-r--r--   0        0        0     1048 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/test/test_component.cc
--rw-r--r--   0        0        0       68 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/CMakeLists.txt
--rw-r--r--   0        0        0      311 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/doc/index.rst
--rw-r--r--   0        0        0      272 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/src/main.c
--rw-r--r--   0        0        0      714 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/clang/toolchain.cmake
--rw-r--r--   0        0        0      183 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/gcc/toolchain.cmake
--rw-r--r--   0        0        0       57 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/variant/cookiecutter.json
--rw-r--r--   0        0        0       94 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/config.cmake
--rw-r--r--   0        0        0       24 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/config.txt
--rw-r--r--   0        0        0       77 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/parts.cmake
--rw-r--r--   0        0        0      532 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/variant.py
--rw-r--r--   0        0        0     1279 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/workspace_artifacts.py
--rw-r--r--   0        0        0     3221 2024-04-18 13:58:45.997234 spl_core-4.1.2/src/spl_core/test_utils/base_variant_test_runner.py
--rw-r--r--   0        0        0     5599 2024-04-18 13:58:45.997234 spl_core-4.1.2/src/spl_core/test_utils/spl_build.py
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 spl_core-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-29 17:57:39.664572 spl_core-4.2.0/LICENSE
+-rw-r--r--   0        0        0      824 2024-04-29 17:57:39.664572 spl_core-4.2.0/README.md
+-rw-r--r--   0        0        0     4378 2024-04-29 17:57:40.592574 spl_core-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-29 17:57:40.592574 spl_core-4.2.0/src/spl_core/__init__.py
+-rw-r--r--   0        0        0      361 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/__run.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/common/__init__.py
+-rw-r--r--   0        0        0     2079 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/common/command_line_executor.py
+-rw-r--r--   0        0        0      462 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/common/path.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/gcov_maid/__init__.py
+-rw-r--r--   0        0        0     1455 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/gcov_maid/gcov_maid.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kconfig/__init__.py
+-rw-r--r--   0        0        0     9795 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kconfig/kconfig.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/__init__.py
+-rw-r--r--   0        0        0     2741 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/create.py
+-rw-r--r--   0        0        0      553 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/.vscode/cmake-variants.json
+-rw-r--r--   0        0        0      589 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/KConfig
+-rw-r--r--   0        0        0      117 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/greeter/CMakeLists.txt
+-rw-r--r--   0        0        0    11090 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/greeter/doc/_images/screenshot.png
+-rw-r--r--   0        0        0      500 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/greeter/doc/index.rst
+-rw-r--r--   0        0        0      431 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/greeter/src/greeter.c
+-rw-r--r--   0        0        0       99 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/greeter/src/greeter.h
+-rw-r--r--   0        0        0      482 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/greeter/test/test_greeter.cc
+-rw-r--r--   0        0        0       68 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/main/CMakeLists.txt
+-rw-r--r--   0        0        0      303 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/main/doc/index.rst
+-rw-r--r--   0        0        0      215 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/src/main/src/main.c
+-rw-r--r--   0        0        0      437 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/test/EnglishVariant/test__EnglishVariant.py
+-rw-r--r--   0        0        0      436 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/test/German/test__GermanVariant.py
+-rw-r--r--   0        0        0       94 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/variants/EnglishVariant/config.cmake
+-rw-r--r--   0        0        0       61 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/variants/EnglishVariant/parts.cmake
+-rw-r--r--   0        0        0       94 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/variants/GermanVariant/config.cmake
+-rw-r--r--   0        0        0      188 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/variants/GermanVariant/config.txt
+-rw-r--r--   0        0        0       61 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/application/variants/GermanVariant/parts.cmake
+-rw-r--r--   0        0        0      638 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/.gitignore
+-rw-r--r--   0        0        0      269 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/cmake-kits.json
+-rw-r--r--   0        0        0      624 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/extensions.json
+-rw-r--r--   0        0        0     1103 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/launch.json
+-rw-r--r--   0        0        0     1369 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/settings.json
+-rw-r--r--   0        0        0     3434 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/tasks.json
+-rw-r--r--   0        0        0     1817 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/CMakeLists.txt
+-rw-r--r--   0        0        0       73 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/build.bat
+-rw-r--r--   0        0        0    11057 2024-04-29 17:57:39.668572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/build.ps1
+-rw-r--r--   0        0        0     6775 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/conf.py
+-rw-r--r--   0        0        0   123953 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/Doxyfile.in
+-rw-r--r--   0        0        0       91 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/common/index.rst
+-rw-r--r--   0        0        0      590 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/components/index.rst
+-rw-r--r--   0        0        0     1072 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/doxygen-awesome/LICENSE
+-rw-r--r--   0        0        0    63045 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/doxygen-awesome/doxygen-awesome.css
+-rw-r--r--   0        0        0       44 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/software_architecture/index.rst
+-rw-r--r--   0        0        0       95 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/software_requirements/index.rst
+-rw-r--r--   0        0        0     1213 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/test_report_template.txt
+-rw-r--r--   0        0        0     1044 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/index.rst
+-rw-r--r--   0        0        0       85 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/pipfile
+-rw-r--r--   0        0        0      159 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/pytest.ini
+-rw-r--r--   0        0        0      219 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/scoopfile.json
+-rw-r--r--   0        0        0      713 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/tools/toolchains/clang/toolchain.cmake
+-rw-r--r--   0        0        0      183 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/kickstart/templates/project/tools/toolchains/gcc/toolchain.cmake
+-rw-r--r--   0        0        0     1225 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/main.py
+-rw-r--r--   0        0        0     3221 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/test_utils/base_variant_test_runner.py
+-rw-r--r--   0        0        0     5599 2024-04-29 17:57:39.672572 spl_core-4.2.0/src/spl_core/test_utils/spl_build.py
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 spl_core-4.2.0/PKG-INFO
```

### Comparing `spl_core-4.1.2/LICENSE` & `spl_core-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.2/README.md` & `spl_core-4.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 ```
 
 ## Project Creator
 
 With the integrated project creator you can create a new SPL workspace, e.g.:
 
 ```powershell
-pipenv run python src/project_creator/creator.py workspace --name MyProject --variant FLV1/SYS1 --out_dir C:\dev
+pipenv run python src/project_creator/creator.py workspace --name MyProject --variant MyVariant --out_dir C:\dev
 ```
 
 Note: one can use the `--variant` argument several times to create a project with multiple variants.
```

### Comparing `spl_core-4.1.2/pyproject.toml` & `spl_core-4.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spl-core"
-version = "4.1.2"
+version = "4.2.0"
 description = "Software Product Line Support for CMake"
 authors = ["Avengineers <karsten.guenther@kamg.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/avengineers/spl-core"
 documentation = "https://spl-core.readthedocs.io"
 classifiers = [
@@ -25,52 +25,49 @@
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 py-app-dev = "^2.1.0"
 cookiecutter = {version="==2.1.1"}
 gcovr = "*"
 hammocking = "*"
 kconfiglib = "*"
+typer = {extras = ["all"], version = "^0.12.3"}
+doxysphinx = "^3.3.7"
+sphinx = "^7.3.5"
+sphinx-rtd-theme = "^2.0.0"
+sphinxcontrib-mermaid = "^0.9.2"
+sphinx-needs = "^2.0.0"
+sphinx-test-reports = "^1.0.2"
+sphinx-rtd-size = "^0.2.0"
+sphinxcontrib-datatemplates = "^0.11.0"
+sphinxcontrib-plantuml = "^0.29"
+sphinx-copybutton = "^0.5.2"
+sphinx-new-tab-link = "^0.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.0"
 black = "^23.1.0"
 pre-commit = "^3.1.1"
 ruff = "^0.3.0"
 jinja2 = "*"
 testfixtures = "*"
 junitparser = "*"
 mashumaro = "*"
 loguru = "*"
 m2r = "*"
 flake8 = "*"
-sphinx = "*"
-sphinx-rtd-theme = "*"
-sphinxcontrib-mermaid = "*"
-sphinx-needs = "*"
-sphinx-test-reports = "*"
-doxysphinx = "*"
-sphinx-rtd-size = "*"
-sphinxcontrib-datatemplates = "*"
-sphinxcontrib-plantuml = "*"
-sphinx-copybutton = "*"
-sphinx-new-tab-link = "*"
 pipenv = "*"
 pypeline-runner = "^0.2.1"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
-sphinx = ">=4.0"
-sphinxcontrib-mermaid = "^0.8.1"
 mlx-traceability = "^10.0.0"
-sphinx-copybutton = "^0.5.2"
-sphinx-new-tab-link = "^0.2.2"
 sphinx-book-theme = "^1.1.2"
 sphinx-design = "^0.5.0"
 
 [tool.semantic_release]
 version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variables = [
     "src/spl_core/__init__.py:__version__",
@@ -91,15 +88,15 @@
 match = "develop"
 
 [tool.semantic_release.branches.noop]
 match = "(?!develop$)"
 prerelease = true
 
 [tool.pytest.ini_options]
-addopts = " --verbose --capture=tee-sys --junitxml=out/test-report.xml"
+addopts = " -vv --capture=tee-sys --junitxml=out/test-report.xml"
 pythonpath = ["src", "tests"]
 testpaths = ["tests"]
 junit_logging = "all"
 
 [tool.coverage.run]
 branch = true
 
@@ -135,15 +132,16 @@
     "E",   # pycodestyle
     "W",   # pycodestyle
     "UP",  # pyupgrade
     "I",   # isort
     "RUF", # ruff specific
 ]
 exclude = [
-    "bootstrap.py"
+    "bootstrap.py",
+    "src/spl_core/kickstart/templates/project/conf.py"
 ]
 
 [tool.ruff.lint.per-file-ignores]
 "tests/**/*" = [
     "D100",
     "D101",
     "D102",
```

### Comparing `spl_core-4.1.2/src/spl_core/common/command_line_executor.py` & `spl_core-4.2.0/src/spl_core/common/command_line_executor.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 
         Returns:
         - A subprocess.CompletedProcess object representing the result of the command execution.
         """
         command = " ".join([cmd] if isinstance(cmd, str) else cmd)
         output = ""
         try:
-            print(f"Running command: {command}")
+            print("=" * 120)
+            print(f"= Running command: {command}")
+            print("=" * 120)
             with subprocess.Popen(
                 command,
                 cwd=str(self.current_working_directory or Path.cwd()),
                 stdout=subprocess.PIPE,
                 stderr=subprocess.STDOUT,
                 bufsize=1,
                 text=True,
```

### Comparing `spl_core-4.1.2/src/spl_core/gcov_maid/gcov_maid.py` & `spl_core-4.2.0/src/spl_core/gcov_maid/gcov_maid.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.2/src/spl_core/kconfig/kconfig.py` & `spl_core-4.2.0/src/spl_core/kconfig/kconfig.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/extensions.json` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/extensions.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'recommendations'": "{insert: [(14, 'waderyan.gitblame'), (15, 'sandcastle.vscode-open')]}"}*

```diff
@@ -9,10 +9,12 @@
         "visualstudioexptteam.vscodeintellicode",
         "haugerbr.project-tasks",
         "avengineers.show-link-list",
         "ms-python.vscode-pylance",
         "ms-python.python",
         "donjayamanne.python-environment-manager",
         "felipecaputo.git-project-manager",
-        "ms-vscode.powershell"
+        "ms-vscode.powershell",
+        "waderyan.gitblame",
+        "sandcastle.vscode-open"
     ]
 }
```

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/launch.json` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/settings.json` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/tasks.json` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/.vscode/tasks.json`

 * *Files 6% similar despite different names*

```diff
@@ -135,45 +135,81 @@
 00000860: 7661 7269 616e 7422 2c0a 2020 2020 2020  variant",.      
 00000870: 2020 2020 2020 2264 6574 6169 6c22 3a20        "detail": 
 00000880: 2246 6561 7475 7265 2063 6f6e 6669 6775  "Feature configu
 00000890: 7261 7469 6f6e 2075 7369 6e67 204b 436f  ration using KCo
 000008a0: 6e66 6967 222c 0a20 2020 2020 2020 2020  nfig",.         
 000008b0: 2020 2022 7479 7065 223a 2022 7368 656c     "type": "shel
 000008c0: 6c22 2c0a 2020 2020 2020 2020 2020 2020  l",.            
-000008d0: 2263 6f6d 6d61 6e64 223a 2022 7069 7065  "command": "pipe
-000008e0: 6e76 2072 756e 2067 7569 636f 6e66 6967  nv run guiconfig
-000008f0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00000900: 6f70 7469 6f6e 7322 3a20 7b0a 2020 2020  options": {.    
-00000910: 2020 2020 2020 2020 2020 2020 2265 6e76              "env
-00000920: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00000930: 2020 2020 2020 2020 2022 4b43 4f4e 4649           "KCONFI
-00000940: 475f 434f 4e46 4947 223a 2022 7661 7269  G_CONFIG": "vari
-00000950: 616e 7473 2f24 7b69 6e70 7574 3a76 6172  ants/${input:var
-00000960: 6961 6e74 7d2f 636f 6e66 6967 2e74 7874  iant}/config.txt
-00000970: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00000980: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00000990: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-000009a0: 7072 6f62 6c65 6d4d 6174 6368 6572 223a  problemMatcher":
-000009b0: 205b 5d0a 2020 2020 2020 2020 7d0a 2020   [].        }.  
-000009c0: 2020 5d2c 0a20 2020 2022 696e 7075 7473    ],.    "inputs
-000009d0: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
-000009e0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-000009f0: 223a 2022 7069 636b 5374 7269 6e67 222c  ": "pickString",
-00000a00: 0a20 2020 2020 2020 2020 2020 2022 6964  .            "id
-00000a10: 223a 2022 7661 7269 616e 7422 2c0a 2020  ": "variant",.  
-00000a20: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00000a30: 6970 7469 6f6e 223a 2022 5768 6963 6820  iption": "Which 
-00000a40: 7661 7269 616e 7420 646f 2079 6f75 2077  variant do you w
-00000a50: 616e 7420 746f 2073 656c 6563 743f 222c  ant to select?",
-00000a60: 0a20 2020 2020 2020 2020 2020 2022 6f70  .            "op
-00000a70: 7469 6f6e 7322 3a20 5b0a 7b25 2d20 666f  tions": [.{%- fo
-00000a80: 7220 7661 7269 616e 7420 696e 2063 6f6f  r variant in coo
-00000a90: 6b69 6563 7574 7465 722e 7661 7269 616e  kiecutter.varian
-00000aa0: 7473 2e76 616c 7565 7328 2920 2d25 7d0a  ts.values() -%}.
-00000ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ac0: 227b 7b20 7661 7269 616e 745b 2266 6c61  "{{ variant["fla
-00000ad0: 766f 7222 5d20 7d7d 2f7b 7b20 7661 7269  vor"] }}/{{ vari
-00000ae0: 616e 745b 2273 7562 7379 7374 656d 225d  ant["subsystem"]
-00000af0: 207d 7d22 2c0a 7b25 2d20 656e 6466 6f72   }}",.{%- endfor
-00000b00: 202d 257d 0a20 2020 2020 2020 2020 2020   -%}.           
-00000b10: 205d 0a20 2020 2020 2020 207d 0a20 2020   ].        }.   
-00000b20: 205d 0a7d 0a                              ].}.
+000008d0: 2263 6f6d 6d61 6e64 223a 2022 2e76 656e  "command": ".ven
+000008e0: 762f 5363 7269 7074 732f 706f 6574 7279  v/Scripts/poetry
+000008f0: 2072 756e 2067 7569 636f 6e66 6967 222c   run guiconfig",
+00000900: 0a20 2020 2020 2020 2020 2020 2022 6f70  .            "op
+00000910: 7469 6f6e 7322 3a20 7b0a 2020 2020 2020  tions": {.      
+00000920: 2020 2020 2020 2020 2020 2265 6e76 223a            "env":
+00000930: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000940: 2020 2020 2020 2022 4b43 4f4e 4649 475f         "KCONFIG_
+00000950: 434f 4e46 4947 223a 2022 7661 7269 616e  CONFIG": "varian
+00000960: 7473 2f24 7b69 6e70 7574 3a76 6172 6961  ts/${input:varia
+00000970: 6e74 7d2f 636f 6e66 6967 2e74 7874 220a  nt}/config.txt".
+00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000990: 7d0a 2020 2020 2020 2020 2020 2020 7d2c  }.            },
+000009a0: 0a20 2020 2020 2020 2020 2020 2022 7072  .            "pr
+000009b0: 6f62 6c65 6d4d 6174 6368 6572 223a 205b  oblemMatcher": [
+000009c0: 5d0a 2020 2020 2020 2020 7d2c 0a20 2020  ].        },.   
+000009d0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+000009e0: 2020 2022 6c61 6265 6c22 3a20 226f 7065     "label": "ope
+000009f0: 6e20 7265 706f 7274 2068 746d 6c22 2c0a  n report html",.
+00000a00: 2020 2020 2020 2020 2020 2020 2263 6f6d              "com
+00000a10: 6d61 6e64 223a 2022 247b 776f 726b 7370  mand": "${worksp
+00000a20: 6163 6546 6f6c 6465 727d 2f62 7569 6c64  aceFolder}/build
+00000a30: 2f24 7b69 6e70 7574 3a76 6172 6961 6e74  /${input:variant
+00000a40: 7d2f 7465 7374 2f73 7263 2f24 7b69 6e70  }/test/src/${inp
+00000a50: 7574 3a63 6f6d 706f 6e65 6e74 7d2f 7265  ut:component}/re
+00000a60: 706f 7274 732f 6874 6d6c 2f69 6e64 6578  ports/html/index
+00000a70: 2e68 746d 6c22 2c0a 2020 2020 2020 2020  .html",.        
+00000a80: 2020 2020 2274 7970 6522 3a20 2273 6865      "type": "she
+00000a90: 6c6c 222c 0a20 2020 2020 2020 2020 2020  ll",.           
+00000aa0: 2022 7072 6573 656e 7461 7469 6f6e 223a   "presentation":
+00000ab0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000ac0: 2020 2022 7265 7665 616c 223a 2022 616c     "reveal": "al
+00000ad0: 7761 7973 220a 2020 2020 2020 2020 2020  ways".          
+00000ae0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00000af0: 2022 6772 6f75 7022 3a20 7b0a 2020 2020   "group": {.    
+00000b00: 2020 2020 2020 2020 2020 2020 226b 696e              "kin
+00000b10: 6422 3a20 2262 7569 6c64 222c 0a20 2020  d": "build",.   
+00000b20: 2020 2020 2020 2020 2020 2020 2022 6973               "is
+00000b30: 4465 6661 756c 7422 3a20 6661 6c73 650a  Default": false.
+00000b40: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00000b50: 2020 2020 2020 7d0a 2020 2020 5d2c 0a20        }.    ],. 
+00000b60: 2020 2022 696e 7075 7473 223a 205b 0a20     "inputs": [. 
+00000b70: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00000b80: 2020 2020 2022 7479 7065 223a 2022 7069       "type": "pi
+00000b90: 636b 5374 7269 6e67 222c 0a20 2020 2020  ckString",.     
+00000ba0: 2020 2020 2020 2022 6964 223a 2022 7661         "id": "va
+00000bb0: 7269 616e 7422 2c0a 2020 2020 2020 2020  riant",.        
+00000bc0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00000bd0: 223a 2022 5768 6963 6820 7661 7269 616e  ": "Which varian
+00000be0: 7420 646f 2079 6f75 2077 616e 7420 746f  t do you want to
+00000bf0: 2073 656c 6563 743f 222c 0a20 2020 2020   select?",.     
+00000c00: 2020 2020 2020 2022 6f70 7469 6f6e 7322         "options"
+00000c10: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+00000c20: 2020 2020 2245 6e67 6c69 7368 5661 7269      "EnglishVari
+00000c30: 616e 7422 2c0a 2020 2020 2020 2020 2020  ant",.          
+00000c40: 2020 2020 2020 2247 6572 6d61 6e56 6172        "GermanVar
+00000c50: 6961 6e74 220a 2020 2020 2020 2020 2020  iant".          
+00000c60: 2020 5d0a 2020 2020 2020 2020 7d2c 0a20    ].        },. 
+00000c70: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00000c80: 2020 2020 2022 7479 7065 223a 2022 7069       "type": "pi
+00000c90: 636b 5374 7269 6e67 222c 0a20 2020 2020  ckString",.     
+00000ca0: 2020 2020 2020 2022 6964 223a 2022 636f         "id": "co
+00000cb0: 6d70 6f6e 656e 7422 2c0a 2020 2020 2020  mponent",.      
+00000cc0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00000cd0: 6f6e 223a 2022 5768 6963 6820 636f 6d70  on": "Which comp
+00000ce0: 6f6e 656e 7420 646f 2079 6f75 2077 616e  onent do you wan
+00000cf0: 7420 746f 2073 656c 6563 743f 222c 0a20  t to select?",. 
+00000d00: 2020 2020 2020 2020 2020 2022 6f70 7469             "opti
+00000d10: 6f6e 7322 3a20 5b0a 2020 2020 2020 2020  ons": [.        
+00000d20: 2020 2020 2020 2020 2267 7265 6574 6572          "greeter
+00000d30: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000d40: 2020 2022 6d61 696e 220a 2020 2020 2020     "main".      
+00000d50: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00000d60: 7d0a 2020 2020 5d0a 7d0a                 }.    ].}.
```

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/CMakeLists.txt` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/CMakeLists.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 # cmake project definition
 cmake_minimum_required(VERSION 3.24.0)
 cmake_policy(VERSION 3.24)
 
+# configure the current variant to be build
 set(BUILD_KIT prod CACHE STRING "Target Group to build.")
 
 include(${CMAKE_SOURCE_DIR}/variants/${VARIANT}/config.cmake)
 
 if(BUILD_KIT STREQUAL prod)
     project(${VARIANT} C ASM)
+    set(VARIANT_ADDITIONAL_COMPILE_C_FLAGS -Dstatic_scope_file=static)
 else()
+    # In case of test the project is a C++ project due to GTest usage
     project(${VARIANT} C ASM CXX)
-    set(VARIANT_ADDITIONAL_COMPILE_C_FLAGS -Dstatic= -save-temps)
+
+    # define static to nothing on file scope to allow access to
+    # static variables and function in unit test cases.
+    # Furthermore store temporary files during compilation to
+    # get preprocessed files.
+    set(VARIANT_ADDITIONAL_COMPILE_C_FLAGS -Dstatic_scope_file= -save-temps)
 endif()
 
 # Fetch all external dependencies into modules directory
 set(FETCHCONTENT_BASE_DIR ${CMAKE_SOURCE_DIR}/build/modules CACHE INTERNAL "")
 set(FETCHCONTENT_QUIET FALSE)
 include(FetchContent)
```

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/KConfig` & `spl_core-4.2.0/src/spl_core/kickstart/templates/application/KConfig`

 * *Files 24% similar despite different names*

```diff
@@ -13,11 +13,11 @@
         prompt "LINKER_BYPRODUCTS_EXTENSIONS"
         default "map"
         help
           The extensions of other byproducts generated by the linker (e.g. map)
 endmenu
 
 menu "Feature Model"
-    config USE_COMPONENT
-        bool "Enable features of component"
+    config LANG_DE
+        bool "German language selection"
         default n
 endmenu
```

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/LICENSE` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/doxygen-awesome/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 - present Marquardt GmbH and members of AVENGINEERS
+Copyright (c) 2021 - 2023 jothepro
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.ps1` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/build.ps1`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 For more information on Execution Policies:
 https://go.microsoft.com/fwlink/?LinkID=135170
 #>
 
 param(
     [Parameter(Mandatory = $false, HelpMessage = 'Install all dependencies required to build. (Switch, default: false)')]
     [switch]$install = $false,
+    [Parameter(Mandatory = $false, HelpMessage = 'Build the target.')]
+    [switch]$build = $false,
     [Parameter(Mandatory = $false, HelpMessage = 'Clean build, wipe out all build artifacts. (Switch, default: false)')]
     [switch]$clean = $false,
     [Parameter(Mandatory = $false, HelpMessage = 'Build kit to be used. (String, default: "prod")')]
     [string]$buildKit = "prod",
     [Parameter(Mandatory = $false, HelpMessage = 'Target to be built. (String, default: "all")')]
     [string]$target = "all",
     [Parameter(Mandatory = $false, HelpMessage = 'Variants (of the product) to be built (List of strings, leave empty to be asked or "all" for automatic build of all variants)')]
@@ -70,14 +72,46 @@
     }
 }
 
 function Test-RunningInCIorTestEnvironment {
     return [Boolean]($Env:JENKINS_URL -or $Env:PYTEST_CURRENT_TEST -or $Env:GITHUB_ACTIONS)
 }
 
+# Consider CI environment variables (e.g. on Jenkins BRANCH_NAME and CHANGE_TARGET) to filter tests in release branch builds
+function Get-ReleaseBranchPytestFilter {
+    $ChangeId = $env:CHANGE_ID
+    $BranchName = $env:BRANCH_NAME
+    $ChangeTarget = $env:CHANGE_TARGET
+
+    $targetBranch = ''
+
+    if (-not $ChangeId -and $BranchName -and $BranchName.StartsWith("release/")) {
+        $targetBranch = $BranchName
+    }
+
+    if ($ChangeId -and $ChangeTarget -and $ChangeTarget.StartsWith("release/") ) {
+        $targetBranch = $ChangeTarget
+    }
+
+    $filter = ''
+    if ($targetBranch -and ($targetBranch -match 'release/([^/]+/[^/]+)(.*)')) {
+        $filter = $Matches[1]
+    }
+
+    return $filter
+}
+
+function Invoke-Bootstrap {
+    # Download bootstrap scripts from external repository
+    Invoke-RestMethod https://raw.githubusercontent.com/avengineers/bootstrap-installer/v1.5.0/install.ps1 | Invoke-Expression
+    # Execute bootstrap script
+    . .\.bootstrap\bootstrap.ps1
+}
+
+
 # Build with given parameters
 Function Invoke-Build {
     param (
         [Parameter(Mandatory = $false)]
         [bool]$clean = $false,
         [Parameter(Mandatory = $false)]
         [string]$buildKit = "prod",
@@ -106,17 +140,17 @@
                 Write-Output "Removing build folder '$buildFolder' ..."
                 Remove-Item $buildFolder -Force -Recurse
             }
         }
 
         # Filter pytest test cases
         $filterCmd = ''
-        # Consider environment variable BRANCH_NAME (e.g. on Jenkins) to filter tests in release branch builds
-        if ($Env:BRANCH_NAME -and ($Env:BRANCH_NAME -match 'release/([^/]+/[^/]+)(.*)')) {
-            $filterCmd = "-k " + $Matches[1]
+        $releaseBranchFilter = Get-ReleaseBranchPytestFilter
+        if ($releaseBranchFilter) {
+            $filterCmd = "-k '$releaseBranchFilter'"
         }
         # otherwise consider command line option '-filter' if given
         elseif ($filter) {
             $filterCmd = "-k '$filter'"
         }
 
         # Test result of pytest
@@ -131,15 +165,15 @@
         Invoke-CommandLine -CommandLine "python -m pipenv run python -m pytest test --junitxml=$pytestJunitXml $filterCmd"
     }
     else {
         if ((-Not $variants) -or ($variants -eq 'all')) {
             $dirs = Get-Childitem -Include config.cmake -Path variants -Recurse | Resolve-Path -Relative
             $variantsList = @()
             Foreach ($dir in $dirs) {
-                $variant = (get-item $dir).Directory.Parent.BaseName + "/" + (get-item $dir).Directory.BaseName
+                $variant = (get-item $dir).Directory.BaseName
                 $variantsList += $variant
             }
             $variantsSelected = @()
             if (-Not $variants) {
                 # variant selection by user if not specified
                 Write-Information -Tags "Info:" -MessageData "no '--variant <variant>' was given, please select from list:"
                 Foreach ($variant in $variantsList) {
@@ -154,15 +188,15 @@
             }
         }
         else {
             $variantsSelected = $Variants.Replace('\', '/').Replace('./variant/', '').Replace('./variants/', '').Split(',')
         }
 
         # Select 'test' build kit based on target
-        if ($target.Contains("unittests") -or $target.Contains("reports")) {
+        if ($target.Contains("unittests") -or $target.Contains("reports") -or $target.Contains("docs")) {
             $buildKit = "test"
         }
 
         Foreach ($variant in $variantsSelected) {
             Write-Output "Building target '$target' with build kit '$buildKit' for variant '$variant' ..."
 
             $buildFolder = "build/$variant/$buildKit"
@@ -207,29 +241,25 @@
 # Stop on first error
 $ErrorActionPreference = "Stop"
 
 Push-Location $PSScriptRoot
 Write-Output "Running in ${pwd}"
 
 try {
+    if (Test-RunningInCIorTestEnvironment -or $Env:USER_PATH_FIRST) {
+        Initialize-EnvPath
+    }
+
     if ($install) {
-        # Installation of Scoop, Python and pipenv via bootstrap
-        if (-Not (Test-Path -Path '.bootstrap')) {
-            New-Item -ItemType Directory '.bootstrap'
-        }
-        Invoke-RestMethod "https://raw.githubusercontent.com/avengineers/bootstrap/v1.3.0/bootstrap.ps1" -OutFile ".\.bootstrap\bootstrap.ps1"
-        Invoke-CommandLine ". .\.bootstrap\bootstrap.ps1" -Silent $true
-        Write-Output "For installation changes to take effect, please close and re-open your current shell."
+        # bootstrap environment
+        Invoke-Bootstrap
     }
-    else {
+
+    if ($build) {
         # Call build system
-        if (Test-RunningInCIorTestEnvironment -or $Env:USER_PATH_FIRST) {
-            Initialize-EnvPath
-        }
-        # Call CMake
         Invoke-Build `
             -target $target `
             -buildKit $buildKit `
             -variants $variants `
             -clean $clean `
             -reconfigure $reconfigure `
             -ninjaArgs $ninjaArgs `
```

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/conf.py` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# -*- coding: utf-8 -*-
 """ Configuration  """
 
+import datetime
 import json
 import os
-import datetime
 import re
 
 day = datetime.date.today()
 # meta data #################################################################
 
-project = "Project"
+project = "Hello SPL"
 copyright = f"{day.year} Avengineers"
 release = f"{day}"
 
 # file handling #############################################################
 # @see https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 templates_path = [
@@ -60,16 +59,19 @@
     "sticky_navigation": True,
     "navigation_depth": 6,
     "includehidden": True,
     "titles_only": False,
 }
 
 # EXTENSIONS AND THEIR CONFIGS ##############################################
-extensions = ["sphinx_rtd_size"]
 
+# extensions and their configuration #########################################
+extensions = []
+
+extensions.append("sphinx_rtd_size")
 sphinx_rtd_size_width = "90%"
 
 # mermaid config - @see https://pypi.org/project/sphinxcontrib-mermaid/ #####
 extensions.append("sphinxcontrib.mermaid")
 
 # sphinx_needs ###############################################################
 extensions.append("sphinx_needs")
@@ -166,22 +168,22 @@
     "build_config": {},
     "config": {},
 }
 
 # Check if the SPHINX_BUILD_CONFIGURATION_FILE environment variable exists
 # and if so, load the JSON file and set the 'html_context' variable
 if "SPHINX_BUILD_CONFIGURATION_FILE" in os.environ:
-    with open(os.environ["SPHINX_BUILD_CONFIGURATION_FILE"], "r") as file:
+    with open(os.environ["SPHINX_BUILD_CONFIGURATION_FILE"]) as file:
         html_context["build_config"] = json.load(file)
         include_patterns.extend(html_context["build_config"].get("include_patterns", []))
 
 # Check if the SPHINX_BUILD_CONFIGURATION_FILE environment variable exists
 # and if so, load the JSON file and set the 'html_context' variable
 if "AUTOCONF_JSON_FILE" in os.environ:
-    with open(os.environ["AUTOCONF_JSON_FILE"], "r") as file:
+    with open(os.environ["AUTOCONF_JSON_FILE"]) as file:
         html_context["config"] = json.load(file)["features"]
 
 if "VARIANT" in os.environ:
     html_context["build_config"]["variant"] = os.environ["VARIANT"]
 
 
 def rstjinja(app, docname, source):
```

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/Doxyfile.in` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/Doxyfile.in`

 * *Files 0% similar despite different names*

```diff
@@ -1312,15 +1312,15 @@
 # for information on how to generate the default header that doxygen normally
 # uses.
 # Note: The header is subject to change so you typically have to regenerate the
 # default header when upgrading to a newer version of doxygen. For a description
 # of the possible markers and block names see the documentation.
 # This tag requires that the tag GENERATE_HTML is set to YES.
 
-HTML_HEADER            = 
+HTML_HEADER            =
 
 # The HTML_FOOTER tag can be used to specify a user-defined HTML footer for each
 # generated HTML page. If the tag is left blank doxygen will generate a standard
 # footer. See HTML_HEADER for more information on how to generate a default
 # footer and what special commands can be used inside the footer. See also
 # section "Doxygen usage" for information on how to generate the default footer
 # that doxygen normally uses.
@@ -2352,15 +2352,15 @@
 # defined before the preprocessor is started (similar to the -D option of e.g.
 # gcc). The argument of the tag is a list of macros of the form: name or
 # name=definition (no spaces). If the definition and the "=" are omitted, "=1"
 # is assumed. To prevent a macro definition from being undefined via #undef or
 # recursively expanded use the := operator instead of the = operator.
 # This tag requires that the tag ENABLE_PREPROCESSING is set to YES.
 
-PREDEFINED             =
+PREDEFINED             = "static_scope_file=static"
 
 # If the MACRO_EXPANSION and EXPAND_ONLY_PREDEF tags are set to YES then this
 # tag can be used to specify a list of macro names that should be expanded. The
 # macro definition that is found in the sources will be used. Use the PREDEFINED
 # tag if you want to use a different macro definition that overrules the
 # definition found in the source code.
 # This tag requires that the tag ENABLE_PREPROCESSING is set to YES.
```

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/components/index.rst` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/components/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Components
 ==========
 
 {% for component_info in build_config.components_info %}
 {% if component_info.has_docs %}
 
-{{ component_info.long_name }}
---------------------
+{{ component_info.long_name or component_info.name }}
+-----------------------------------------------------
 
 .. toctree::
     :maxdepth: 2
 
     /{{ component_info.path }}/doc/index
 {% if (build_config.target == 'reports') and component_info.has_reports %}
-    /{{ component_info.reports_output_dir }}/unit_test_spec
     /{{ component_info.reports_output_dir }}/unit_test_results
     /{{ component_info.reports_output_dir }}/doxygen/html/index
     /{{ component_info.reports_output_dir }}/coverage
 {% endif %}
 
 
 {% endif %}
```

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/doxygen-awesome.css` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/doxygen-awesome/doxygen-awesome.css`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         --page-secondary-foreground-color: #859399;
         --separator-color: #38393b;
         --side-nav-background: #252628;
 
         --code-background: #2a2c2f;
 
         --tablehead-background: #2a2c2f;
-    
+
         --blockquote-background: #222325;
         --blockquote-foreground: #7e8c92;
 
         --warning-color: #2e1917;
         --warning-color-dark: #ad2617;
         --warning-color-darker: #f5b1aa;
         --note-color: #3b2e04;
@@ -884,15 +884,15 @@
     #doc-content > div > div.contents,
     .PageDoc > div.contents {
         display: flex;
         flex-direction: row-reverse;
         flex-wrap: nowrap;
         align-items: flex-start;
     }
-    
+
     div.contents .textblock {
         min-width: 200px;
         flex-grow: 1;
     }
 }
 
 div.contents, div.header .title, div.header .summary {
@@ -976,29 +976,29 @@
  {
     filter: brightness(89%) hue-rotate(180deg) invert();
 }
 
 h2.groupheader {
     border-bottom: 0px;
     color: var(--page-foreground-color);
-    box-shadow: 
-        100px 0 var(--page-background-color), 
+    box-shadow:
+        100px 0 var(--page-background-color),
         -100px 0 var(--page-background-color),
         100px 0.75px var(--separator-color),
         -100px 0.75px var(--separator-color),
-        500px 0 var(--page-background-color), 
+        500px 0 var(--page-background-color),
         -500px 0 var(--page-background-color),
         500px 0.75px var(--separator-color),
         -500px 0.75px var(--separator-color),
-        900px 0 var(--page-background-color), 
+        900px 0 var(--page-background-color),
         -900px 0 var(--page-background-color),
         900px 0.75px var(--separator-color),
         -900px 0.75px var(--separator-color),
         1400px 0 var(--page-background-color),
-        -1400px 0 var(--page-background-color), 
+        -1400px 0 var(--page-background-color),
         1400px 0.75px var(--separator-color),
         -1400px 0.75px var(--separator-color),
         1900px 0 var(--page-background-color),
         -1900px 0 var(--page-background-color),
         1900px 0.75px var(--separator-color),
         -1900px 0.75px var(--separator-color);
 }
@@ -1161,16 +1161,16 @@
         margin: 0;
         padding: var(--spacing-large) 0;
         display: block;
     }
 
     div.contents .toc.interactive > h3::before {
         content: "";
-        width: 0; 
-        height: 0; 
+        width: 0;
+        height: 0;
         border-left: 4px solid transparent;
         border-right: 4px solid transparent;
         border-top: 5px solid var(--primary-color);
         display: inline-block;
         margin-right: var(--spacing-small);
         margin-bottom: calc(var(--navigation-font-size) / 4);
         transform: rotate(-90deg);
@@ -1853,16 +1853,16 @@
     color: var(--page-secondary-foreground-color);
 }
 
 table.memberdecls img[src="closed.png"],
 table.memberdecls img[src="open.png"],
 div.dynheader img[src="open.png"],
 div.dynheader img[src="closed.png"] {
-    width: 0; 
-    height: 0; 
+    width: 0;
+    height: 0;
     border-left: 4px solid transparent;
     border-right: 4px solid transparent;
     border-top: 5px solid var(--primary-color);
     margin-top: 8px;
     display: block;
     float: left;
     margin-left: -10px;
@@ -1872,15 +1872,15 @@
 table.memberdecls img {
     margin-right: 10px;
 }
 
 table.memberdecls img[src="closed.png"],
 div.dynheader img[src="closed.png"] {
     transform: rotate(-90deg);
-    
+
 }
 
 .compoundTemplParams {
     font-family: var(--font-family-monospace);
     color: var(--primary-dark-color);
     font-size: var(--code-font-size);
 }
@@ -1915,15 +1915,15 @@
         padding-top: 0;
     }
 
     table.memberdecls .mdescLeft {
         margin-bottom: calc(0px - var(--page-font-size));
     }
 
-    table.memberdecls .memItemRight, 
+    table.memberdecls .memItemRight,
     table.memberdecls .mdescRight,
     table.memberdecls .memTemplItemRight {
         border-top: 0;
         padding-top: 0;
         padding-right: var(--spacing-large);
         overflow-x: auto;
     }
@@ -2101,16 +2101,16 @@
     border-radius: var(--border-radius-small);
 }
 
 .classindex dl.even {
     background-color: transparent;
 }
 
-/* 
- Class Index Doxygen 1.8 
+/*
+ Class Index Doxygen 1.8
 */
 
 table.classindex {
     margin-left: 0;
     margin-right: 0;
     width: 100%;
 }
@@ -2247,15 +2247,15 @@
 .contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) tbody::-webkit-scrollbar-thumb,
 div.contents .toc::-webkit-scrollbar-thumb,
 .contents .dotgraph::-webkit-scrollbar-thumb,
 .contents .tabs-overview-container::-webkit-scrollbar-thumb {
     background-color: transparent;
     border: var(--webkit-scrollbar-padding) solid transparent;
     border-radius: calc(var(--webkit-scrollbar-padding) + var(--webkit-scrollbar-padding));
-    background-clip: padding-box;  
+    background-clip: padding-box;
 }
 
 #nav-tree:hover::-webkit-scrollbar-thumb,
 div.fragment:hover::-webkit-scrollbar-thumb,
 pre.fragment:hover::-webkit-scrollbar-thumb,
 div.memproto:hover::-webkit-scrollbar-thumb,
 .contents center:hover::-webkit-scrollbar-thumb,
```

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/test_report_template.txt` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/doc/test_report_template.txt`

 * *Files 7% similar despite different names*

```diff
@@ -38,9 +38,7 @@
    :id: {id}{links_string}
    :tags: {tags}
    :file: {file}
    :auto_suites:
    :auto_cases:
 
    {content}
-
-
```

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/index.rst` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -30,9 +30,10 @@
 
     doc/software_requirements/index
     doc/software_architecture/index
     doc/components/index
 {% if build_config.target == 'reports' %}
     {{ build_config.reports_output_dir }}/coverage
 {% endif %}
+    doc/results/index
 
 {% endif %}
```

### Comparing `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/clang/toolchain.cmake` & `spl_core-4.2.0/src/spl_core/kickstart/templates/project/tools/toolchains/clang/toolchain.cmake`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 # TODO: caching required due to cmake tools extension issue: https://github.com/microsoft/vscode-cmake-tools/issues/1188
 # TODO: get debugging running (lldb-mi not found in any current package, switching back to gcc)
 set(CMAKE_C_COMPILER clang CACHE STRING "C Compiler")
-# TODO: clarify why llvm-cov produces invalid gcov files (contain blank lines), releated GCOVR issue: https://github.com/gcovr/gcovr/issues/331
+# TODO: clarify why llvm-cov produces invalid gcov files (contain blank lines), related GCOVR issue: https://github.com/gcovr/gcovr/issues/331
 set(GCOVR_ADDITIONAL_OPTIONS --gcov-executable \"llvm-cov gcov\" --gcov-ignore-parse-errors --html-title \"Code Coverage Report \(tool suite: LLVM Clang\)\")
 
 set(CMAKE_CXX_COMPILER clang++ CACHE STRING "CXX Compiler")
 set(CMAKE_ASM_COMPILER ${CMAKE_C_COMPILER} CACHE STRING "ASM Compiler")
```

### Comparing `spl_core-4.1.2/src/spl_core/test_utils/base_variant_test_runner.py` & `spl_core-4.2.0/src/spl_core/test_utils/base_variant_test_runner.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.2/src/spl_core/test_utils/spl_build.py` & `spl_core-4.2.0/src/spl_core/test_utils/spl_build.py`

 * *Files identical despite different names*

