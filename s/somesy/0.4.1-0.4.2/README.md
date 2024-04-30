# Comparing `tmp/somesy-0.4.1.tar.gz` & `tmp/somesy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somesy-0.4.1.tar", max compression
+gzip compressed data, was "somesy-0.4.2.tar", max compression
```

## Comparing `somesy-0.4.1.tar` & `somesy-0.4.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0      872 2024-04-08 16:10:30.881035 somesy-0.4.1/.reuse/dep5
--rw-r--r--   0        0        0     1473 2024-04-08 16:10:30.885035 somesy-0.4.1/AUTHORS.md
--rw-r--r--   0        0        0     1916 2024-04-08 16:10:30.885035 somesy-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     1036 2024-04-08 16:10:30.885035 somesy-0.4.1/CITATION.cff
--rw-r--r--   0        0        0     5446 2024-04-08 16:10:30.885035 somesy-0.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2271 2024-04-08 16:10:30.885035 somesy-0.4.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1190 2024-04-08 16:10:30.885035 somesy-0.4.1/LICENSE
-drwxr-xr-x   0        0        0        0 2024-04-08 16:10:30.885035 somesy-0.4.1/LICENSES/
--rw-r--r--   0        0        0     7048 2024-04-08 16:10:30.885035 somesy-0.4.1/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0     1078 2024-04-08 16:10:30.885035 somesy-0.4.1/LICENSES/MIT.txt
--rw-r--r--   0        0        0    10070 2024-04-08 16:10:30.885035 somesy-0.4.1/README.md
--rw-r--r--   0        0        0     2087 2024-04-08 16:10:30.885035 somesy-0.4.1/codemeta.json
--rw-r--r--   0        0        0     1113 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/_template_authors.md
--rw-r--r--   0        0        0       22 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/changelog.md
--rw-r--r--   0        0        0       28 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/code_of_conduct.md
--rw-r--r--   0        0        0       25 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/contributing.md
--rw-r--r--   0        0        0       20 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/credits.md
--rw-r--r--   0        0        0       55 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/css/style.css
--rw-r--r--   0        0        0    13699 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/dev_guide.md
--rw-r--r--   0        0        0      179 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/index.md
--rw-r--r--   0        0        0      473 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/license.md
--rw-r--r--   0        0        0    25303 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/manual.md
--rw-r--r--   0        0        0      229 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/overrides/main.html
--rw-r--r--   0        0        0      699 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/overrides/partials/copyright.html
--rw-r--r--   0        0        0       30 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/quickstart.md
--rw-r--r--   0        0        0     2084 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/scripts/coverage_status.py
--rw-r--r--   0        0        0      994 2024-04-08 16:10:30.885035 somesy-0.4.1/docs/scripts/gen_ref_pages.py
--rw-r--r--   0        0        0     5592 2024-04-08 16:10:30.885035 somesy-0.4.1/mkdocs.yml
--rw-r--r--   0        0        0     3958 2024-04-08 16:10:30.885035 somesy-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      229 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/__init__.py
--rw-r--r--   0        0        0       61 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/cff/__init__.py
--rw-r--r--   0        0        0     3225 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/cff/writer.py
--rw-r--r--   0        0        0       31 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/cli/__init__.py
--rw-r--r--   0        0        0     1925 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/cli/fill.py
--rw-r--r--   0        0        0     3766 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/cli/init.py
--rw-r--r--   0        0        0     6523 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/cli/sync.py
--rw-r--r--   0        0        0     2141 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/cli/util.py
--rw-r--r--   0        0        0      140 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/codemeta/__init__.py
--rw-r--r--   0        0        0     6035 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/codemeta/writer.py
--rw-r--r--   0        0        0      122 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/commands/__init__.py
--rw-r--r--   0        0        0     1402 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/commands/init_config.py
--rw-r--r--   0        0        0     2469 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/commands/sync.py
--rw-r--r--   0        0        0       26 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/core/__init__.py
--rw-r--r--   0        0        0     4106 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/core/core.py
--rw-r--r--   0        0        0     3226 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/core/log.py
--rw-r--r--   0        0        0    19681 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/core/models.py
--rw-r--r--   0        0        0    19373 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/core/types.py
--rw-r--r--   0        0        0    14417 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/core/writer.py
--rw-r--r--   0        0        0       73 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/fortran/__init__.py
--rw-r--r--   0        0        0     1902 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/fortran/models.py
--rw-r--r--   0        0        0     4097 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/fortran/writer.py
--rw-r--r--   0        0        0      474 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/json_wrapper.py
--rw-r--r--   0        0        0       67 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/julia/__init__.py
--rw-r--r--   0        0        0     1793 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/julia/models.py
--rw-r--r--   0        0        0     2097 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/julia/writer.py
--rw-r--r--   0        0        0     1790 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/main.py
--rw-r--r--   0        0        0       70 2024-04-08 16:10:30.885035 somesy-0.4.1/src/somesy/mkdocs/__init__.py
--rw-r--r--   0        0        0      909 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/mkdocs/models.py
--rw-r--r--   0        0        0     3457 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/mkdocs/writer.py
--rw-r--r--   0        0        0       85 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/package_json/__init__.py
--rw-r--r--   0        0        0     4209 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/package_json/models.py
--rw-r--r--   0        0        0     4612 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/package_json/writer.py
--rw-r--r--   0        0        0      419 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/pom_xml/__init__.py
--rw-r--r--   0        0        0     7569 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/pom_xml/writer.py
--rw-r--r--   0        0        0    15126 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/pom_xml/xmlproxy.py
--rw-r--r--   0        0        0      123 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/pyproject/__init__.py
--rw-r--r--   0        0        0     6315 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/pyproject/models.py
--rw-r--r--   0        0        0     6858 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/pyproject/writer.py
--rw-r--r--   0        0        0       64 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/rust/__init__.py
--rw-r--r--   0        0        0     4286 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/rust/models.py
--rw-r--r--   0        0        0     4753 2024-04-08 16:10:30.889035 somesy-0.4.1/src/somesy/rust/writer.py
--rw-r--r--   0        0        0     6721 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0      627 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/data/CITATION.cff
--rw-r--r--   0        0        0     2063 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/data/Cargo.toml
--rw-r--r--   0        0        0     2210 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/data/Project.toml
--rw-r--r--   0        0        0      287 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/data/blank_pom.xml
--rw-r--r--   0        0        0      561 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/data/example_1.xml
--rw-r--r--   0        0        0     1372 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/data/example_pom.xml
--rw-r--r--   0        0        0     2117 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/data/fpm.toml
--rw-r--r--   0        0        0      692 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/data/mkdocs.yml
--rw-r--r--   0        0        0     2854 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/data/package.json
--rw-r--r--   0        0        0     1438 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/data/pom.xml
--rw-r--r--   0        0        0     2426 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/data/pyproject.setuptools.toml
--rw-r--r--   0        0        0     2411 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/data/pyproject.toml
--rw-r--r--   0        0        0     1540 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/data/somesy.toml
--rw-r--r--   0        0        0      732 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/input/test_cff_validate.py
--rw-r--r--   0        0        0     3780 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/input/test_core_core.py
--rw-r--r--   0        0        0      719 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/input/test_fortran_validate.py
--rw-r--r--   0        0        0      711 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/input/test_julia_validate.py
--rw-r--r--   0        0        0      648 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/input/test_mkdocs_validate.py
--rw-r--r--   0        0        0      846 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/input/test_package_json_validate.py
--rw-r--r--   0        0        0     1209 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/input/test_pyproject_validate.py
--rw-r--r--   0        0        0     1701 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/input/test_rust_validate.py
--rw-r--r--   0        0        0     4435 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/output/test_cff_writer.py
--rw-r--r--   0        0        0     1359 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/output/test_codemeta.py
--rw-r--r--   0        0        0     1678 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/output/test_fortran_writer.py
--rw-r--r--   0        0        0     3515 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/output/test_julia_writer.py
--rw-r--r--   0        0        0     1187 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/output/test_mkdocs_writer.py
--rw-r--r--   0        0        0     3926 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/output/test_package_json_writer.py
--rw-r--r--   0        0        0     3852 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/output/test_pom_writer.py
--rw-r--r--   0        0        0     5387 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/output/test_pyproject_writer.py
--rw-r--r--   0        0        0     4294 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/output/test_rust_writer.py
--rw-r--r--   0        0        0     1167 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/processing/test_cli_util.py
--rw-r--r--   0        0        0     3419 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/processing/test_core_models.py
--rw-r--r--   0        0        0     5705 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/processing/test_xmlwrapper.py
--rw-r--r--   0        0        0      880 2024-04-08 16:10:30.889035 somesy-0.4.1/tests/test_main.py
--rw-r--r--   0        0        0    11683 1970-01-01 00:00:00.000000 somesy-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      872 2024-04-30 09:43:30.755883 somesy-0.4.2/.reuse/dep5
+-rw-r--r--   0        0        0     1473 2024-04-30 09:43:30.755883 somesy-0.4.2/AUTHORS.md
+-rw-r--r--   0        0        0     2108 2024-04-30 09:43:30.755883 somesy-0.4.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1036 2024-04-30 09:43:30.755883 somesy-0.4.2/CITATION.cff
+-rw-r--r--   0        0        0     5446 2024-04-30 09:43:30.755883 somesy-0.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2271 2024-04-30 09:43:30.755883 somesy-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1190 2024-04-30 09:43:30.755883 somesy-0.4.2/LICENSE
+drwxr-xr-x   0        0        0        0 2024-04-30 09:43:30.755883 somesy-0.4.2/LICENSES/
+-rw-r--r--   0        0        0     7048 2024-04-30 09:43:30.755883 somesy-0.4.2/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0     1078 2024-04-30 09:43:30.755883 somesy-0.4.2/LICENSES/MIT.txt
+-rw-r--r--   0        0        0    10070 2024-04-30 09:43:30.755883 somesy-0.4.2/README.md
+-rw-r--r--   0        0        0     2087 2024-04-30 09:43:30.755883 somesy-0.4.2/codemeta.json
+-rw-r--r--   0        0        0     1113 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/_template_authors.md
+-rw-r--r--   0        0        0       22 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/changelog.md
+-rw-r--r--   0        0        0       28 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/code_of_conduct.md
+-rw-r--r--   0        0        0       25 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/contributing.md
+-rw-r--r--   0        0        0       20 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/credits.md
+-rw-r--r--   0        0        0       55 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/css/style.css
+-rw-r--r--   0        0        0    13699 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/dev_guide.md
+-rw-r--r--   0        0        0      179 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/index.md
+-rw-r--r--   0        0        0      473 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/license.md
+-rw-r--r--   0        0        0    25303 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/manual.md
+-rw-r--r--   0        0        0      229 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/overrides/main.html
+-rw-r--r--   0        0        0      699 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/overrides/partials/copyright.html
+-rw-r--r--   0        0        0       30 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/quickstart.md
+-rw-r--r--   0        0        0     2084 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/scripts/coverage_status.py
+-rw-r--r--   0        0        0      994 2024-04-30 09:43:30.755883 somesy-0.4.2/docs/scripts/gen_ref_pages.py
+-rw-r--r--   0        0        0     5592 2024-04-30 09:43:30.755883 somesy-0.4.2/mkdocs.yml
+-rw-r--r--   0        0        0     3958 2024-04-30 09:43:30.755883 somesy-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/cff/__init__.py
+-rw-r--r--   0        0        0     3225 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/cff/writer.py
+-rw-r--r--   0        0        0       31 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/cli/__init__.py
+-rw-r--r--   0        0        0     1925 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/cli/fill.py
+-rw-r--r--   0        0        0     3766 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/cli/init.py
+-rw-r--r--   0        0        0     6523 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/cli/sync.py
+-rw-r--r--   0        0        0     2369 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/cli/util.py
+-rw-r--r--   0        0        0      140 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/codemeta/__init__.py
+-rw-r--r--   0        0        0     6035 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/codemeta/writer.py
+-rw-r--r--   0        0        0      122 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/commands/__init__.py
+-rw-r--r--   0        0        0     1402 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/commands/init_config.py
+-rw-r--r--   0        0        0     2469 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/commands/sync.py
+-rw-r--r--   0        0        0       26 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/core/__init__.py
+-rw-r--r--   0        0        0     4106 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/core/core.py
+-rw-r--r--   0        0        0     3226 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/core/log.py
+-rw-r--r--   0        0        0    19681 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/core/models.py
+-rw-r--r--   0        0        0    19373 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/core/types.py
+-rw-r--r--   0        0        0    14417 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/core/writer.py
+-rw-r--r--   0        0        0       73 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/fortran/__init__.py
+-rw-r--r--   0        0        0     1902 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/fortran/models.py
+-rw-r--r--   0        0        0     4097 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/fortran/writer.py
+-rw-r--r--   0        0        0      474 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/json_wrapper.py
+-rw-r--r--   0        0        0       67 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/julia/__init__.py
+-rw-r--r--   0        0        0     1793 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/julia/models.py
+-rw-r--r--   0        0        0     2097 2024-04-30 09:43:30.755883 somesy-0.4.2/src/somesy/julia/writer.py
+-rw-r--r--   0        0        0     1790 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/main.py
+-rw-r--r--   0        0        0       70 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/mkdocs/__init__.py
+-rw-r--r--   0        0        0      909 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/mkdocs/models.py
+-rw-r--r--   0        0        0     3457 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/mkdocs/writer.py
+-rw-r--r--   0        0        0       85 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/package_json/__init__.py
+-rw-r--r--   0        0        0     4209 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/package_json/models.py
+-rw-r--r--   0        0        0     4612 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/package_json/writer.py
+-rw-r--r--   0        0        0      419 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/pom_xml/__init__.py
+-rw-r--r--   0        0        0     7569 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/pom_xml/writer.py
+-rw-r--r--   0        0        0    15126 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/pom_xml/xmlproxy.py
+-rw-r--r--   0        0        0      123 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/pyproject/__init__.py
+-rw-r--r--   0        0        0     6315 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/pyproject/models.py
+-rw-r--r--   0        0        0     6858 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/pyproject/writer.py
+-rw-r--r--   0        0        0       64 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/rust/__init__.py
+-rw-r--r--   0        0        0     4286 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/rust/models.py
+-rw-r--r--   0        0        0     4753 2024-04-30 09:43:30.759883 somesy-0.4.2/src/somesy/rust/writer.py
+-rw-r--r--   0        0        0     6721 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0      627 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/data/CITATION.cff
+-rw-r--r--   0        0        0     2063 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/data/Cargo.toml
+-rw-r--r--   0        0        0     2210 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/data/Project.toml
+-rw-r--r--   0        0        0      287 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/data/blank_pom.xml
+-rw-r--r--   0        0        0      561 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/data/example_1.xml
+-rw-r--r--   0        0        0     1372 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/data/example_pom.xml
+-rw-r--r--   0        0        0     2117 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/data/fpm.toml
+-rw-r--r--   0        0        0      692 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/data/mkdocs.yml
+-rw-r--r--   0        0        0     2854 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/data/package.json
+-rw-r--r--   0        0        0     1438 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/data/pom.xml
+-rw-r--r--   0        0        0     2426 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/data/pyproject.setuptools.toml
+-rw-r--r--   0        0        0     2411 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/data/pyproject.toml
+-rw-r--r--   0        0        0     1540 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/data/somesy.toml
+-rw-r--r--   0        0        0      732 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/input/test_cff_validate.py
+-rw-r--r--   0        0        0     3780 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/input/test_core_core.py
+-rw-r--r--   0        0        0      719 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/input/test_fortran_validate.py
+-rw-r--r--   0        0        0      711 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/input/test_julia_validate.py
+-rw-r--r--   0        0        0      648 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/input/test_mkdocs_validate.py
+-rw-r--r--   0        0        0      846 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/input/test_package_json_validate.py
+-rw-r--r--   0        0        0     1209 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/input/test_pyproject_validate.py
+-rw-r--r--   0        0        0     1701 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/input/test_rust_validate.py
+-rw-r--r--   0        0        0     4435 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/output/test_cff_writer.py
+-rw-r--r--   0        0        0     1359 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/output/test_codemeta.py
+-rw-r--r--   0        0        0     1678 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/output/test_fortran_writer.py
+-rw-r--r--   0        0        0     3515 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/output/test_julia_writer.py
+-rw-r--r--   0        0        0     1187 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/output/test_mkdocs_writer.py
+-rw-r--r--   0        0        0     3926 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/output/test_package_json_writer.py
+-rw-r--r--   0        0        0     3852 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/output/test_pom_writer.py
+-rw-r--r--   0        0        0     5387 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/output/test_pyproject_writer.py
+-rw-r--r--   0        0        0     4294 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/output/test_rust_writer.py
+-rw-r--r--   0        0        0     1167 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/processing/test_cli_util.py
+-rw-r--r--   0        0        0     3419 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/processing/test_core_models.py
+-rw-r--r--   0        0        0     5705 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/processing/test_xmlwrapper.py
+-rw-r--r--   0        0        0      880 2024-04-30 09:43:30.759883 somesy-0.4.2/tests/test_main.py
+-rw-r--r--   0        0        0    11683 1970-01-01 00:00:00.000000 somesy-0.4.2/PKG-INFO
```

### Comparing `somesy-0.4.1/.reuse/dep5` & `somesy-0.4.2/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/AUTHORS.md` & `somesy-0.4.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/CHANGELOG.md` & `somesy-0.4.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Changelog
 
 Here we provide notes that summarize the most important changes in each released version.
 
 Please consult the changelog to inform yourself about breaking changes and security issues.
 
-## [v0.4.1](https://github.com/Materials-Data-Science-and-Informatics/somesy/tree/v0.4.1) <small>(2024-02-??)</small> { id="0.4.1" }
+## [v0.4.2](https://github.com/Materials-Data-Science-and-Informatics/somesy/tree/v0.4.2) <small>(2024-04-30)</small> { id="0.4.2" }
+
+* fix rich logging bug for error messages and tracebacks
+
+## [v0.4.1](https://github.com/Materials-Data-Science-and-Informatics/somesy/tree/v0.4.1) <small>(2024-04-08)</small> { id="0.4.1" }
 
 * fix package.json and mkdocs.yml validation bug about optional fields
 
-## [v0.4.0](https://github.com/Materials-Data-Science-and-Informatics/somesy/tree/v0.4.0) <small>(2024-02-??)</small> { id="0.4.0" }
+## [v0.4.0](https://github.com/Materials-Data-Science-and-Informatics/somesy/tree/v0.4.0) <small>(2024-03-08)</small> { id="0.4.0" }
 
 * added separate `documentation` URL to Project metadata model
 * added support for Julia `Project.toml` file
 * added support for Fortran `fpm.toml` file
 * added support for Java `pom.xml` file
 * added support for MkDocs `mkdocs.yml` file
 * added support for Rust `Cargo.toml` file
```

### Comparing `somesy-0.4.1/CITATION.cff` & `somesy-0.4.2/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cff-version: 1.2.0
 type: software
 message: If you use this software, please cite it using this metadata.
 
 title: somesy
-version: 0.4.1
+version: 0.4.2
 abstract: A CLI tool for synchronizing software project metadata.
 url: https://materials-data-science-and-informatics.github.io/somesy
 repository-code: https://github.com/Materials-Data-Science-and-Informatics/somesy
 license: MIT
 keywords:
 - metadata
 - FAIR
```

### Comparing `somesy-0.4.1/CODE_OF_CONDUCT.md` & `somesy-0.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/CONTRIBUTING.md` & `somesy-0.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/LICENSE` & `somesy-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/LICENSES/CC0-1.0.txt` & `somesy-0.4.2/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/LICENSES/MIT.txt` & `somesy-0.4.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/README.md` & `somesy-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/codemeta.json` & `somesy-0.4.2/codemeta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.4.2'"}*

```diff
@@ -64,9 +64,9 @@
             "familyName": "Soylu",
             "givenName": "Mustafa"
         }
     ],
     "name": "somesy",
     "softwareHelp": "https://materials-data-science-and-informatics.github.io/somesy",
     "url": "https://materials-data-science-and-informatics.github.io/somesy",
-    "version": "0.4.1"
+    "version": "0.4.2"
 }
```

### Comparing `somesy-0.4.1/docs/_template_authors.md` & `somesy-0.4.2/docs/_template_authors.md`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/docs/dev_guide.md` & `somesy-0.4.2/docs/dev_guide.md`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/docs/manual.md` & `somesy-0.4.2/docs/manual.md`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/docs/overrides/partials/copyright.html` & `somesy-0.4.2/docs/overrides/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/docs/scripts/coverage_status.py` & `somesy-0.4.2/docs/scripts/coverage_status.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/docs/scripts/gen_ref_pages.py` & `somesy-0.4.2/docs/scripts/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/mkdocs.yml` & `somesy-0.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/pyproject.toml` & `somesy-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "somesy"
-version = "0.4.1"
+version = "0.4.2"
 description = "A CLI tool for synchronizing software project metadata."
 authors = ["Mustafa Soylu <m.soylu@fz-juelich.de>", "Anton Pirogov <a.pirogov@fz-juelich.de>"]
 maintainers = ["Mustafa Soylu <m.soylu@fz-juelich.de>"]
 license = "MIT"
 
 readme = "README.md"
 repository = "https://github.com/Materials-Data-Science-and-Informatics/somesy"
```

### Comparing `somesy-0.4.1/src/somesy/cff/writer.py` & `somesy-0.4.2/src/somesy/cff/writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/cli/fill.py` & `somesy-0.4.2/src/somesy/cli/fill.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/cli/init.py` & `somesy-0.4.2/src/somesy/cli/init.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/cli/sync.py` & `somesy-0.4.2/src/somesy/cli/sync.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/cli/util.py` & `somesy-0.4.2/src/somesy/cli/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Utility functions for CLI commands."""
 import logging
 import traceback
 from typing import Optional
 
 import typer
 import wrapt
+from rich.markup import escape
 from rich.pretty import pretty_repr
 
 from somesy.core.core import discover_input
 from somesy.core.log import SomesyLogLevel, get_log_level, set_log_level
 from somesy.core.models import SomesyConfig, SomesyInput
 
 logger = logging.getLogger("somesy")
@@ -29,16 +30,20 @@
 @wrapt.decorator
 def wrap_exceptions(wrapped, instance, args, kwargs):
     """Format and log exceptions for cli commands."""
     try:
         return wrapped(*args, **kwargs)
 
     except Exception as e:
-        logger.error(f"[bold red]Error: {e}[/bold red]")
-        logger.debug(f"[red]{traceback.format_exc()}[/red]")
+        # Escape the error message to prevent Rich from misinterpreting it
+        escaped_error_message = escape(str(e))
+        escaped_traceback = escape(traceback.format_exc())
+
+        logger.error(f"[bold red]Error: {escaped_error_message}[/bold red]")
+        logger.debug(f"[red]{escaped_traceback}[/red]")
         raise typer.Exit(code=1) from e
 
 
 def resolved_somesy_input(**cli_args) -> SomesyInput:
     """Return a combined `SomesyInput` based on config file and passed CLI args.
 
     Will also adjust log levels accordingly.
```

### Comparing `somesy-0.4.1/src/somesy/codemeta/writer.py` & `somesy-0.4.2/src/somesy/codemeta/writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/commands/init_config.py` & `somesy-0.4.2/src/somesy/commands/init_config.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/commands/sync.py` & `somesy-0.4.2/src/somesy/commands/sync.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/core/core.py` & `somesy-0.4.2/src/somesy/core/core.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/core/log.py` & `somesy-0.4.2/src/somesy/core/log.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/core/models.py` & `somesy-0.4.2/src/somesy/core/models.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/core/types.py` & `somesy-0.4.2/src/somesy/core/types.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/core/writer.py` & `somesy-0.4.2/src/somesy/core/writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/fortran/models.py` & `somesy-0.4.2/src/somesy/fortran/models.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/fortran/writer.py` & `somesy-0.4.2/src/somesy/fortran/writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/julia/models.py` & `somesy-0.4.2/src/somesy/julia/models.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/julia/writer.py` & `somesy-0.4.2/src/somesy/julia/writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/main.py` & `somesy-0.4.2/src/somesy/main.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/mkdocs/models.py` & `somesy-0.4.2/src/somesy/mkdocs/models.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/mkdocs/writer.py` & `somesy-0.4.2/src/somesy/mkdocs/writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/package_json/models.py` & `somesy-0.4.2/src/somesy/package_json/models.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/package_json/writer.py` & `somesy-0.4.2/src/somesy/package_json/writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/pom_xml/writer.py` & `somesy-0.4.2/src/somesy/pom_xml/writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/pom_xml/xmlproxy.py` & `somesy-0.4.2/src/somesy/pom_xml/xmlproxy.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/pyproject/models.py` & `somesy-0.4.2/src/somesy/pyproject/models.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/pyproject/writer.py` & `somesy-0.4.2/src/somesy/pyproject/writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/rust/models.py` & `somesy-0.4.2/src/somesy/rust/models.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/src/somesy/rust/writer.py` & `somesy-0.4.2/src/somesy/rust/writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/conftest.py` & `somesy-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/data/CITATION.cff` & `somesy-0.4.2/tests/data/CITATION.cff`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/data/Cargo.toml` & `somesy-0.4.2/tests/data/Cargo.toml`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/data/Project.toml` & `somesy-0.4.2/tests/data/Project.toml`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/data/example_1.xml` & `somesy-0.4.2/tests/data/example_1.xml`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/data/example_pom.xml` & `somesy-0.4.2/tests/data/example_pom.xml`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/data/fpm.toml` & `somesy-0.4.2/tests/data/fpm.toml`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/data/mkdocs.yml` & `somesy-0.4.2/tests/data/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/data/package.json` & `somesy-0.4.2/tests/data/package.json`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/data/pom.xml` & `somesy-0.4.2/tests/data/pom.xml`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/data/pyproject.setuptools.toml` & `somesy-0.4.2/tests/data/pyproject.setuptools.toml`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/data/pyproject.toml` & `somesy-0.4.2/tests/data/pyproject.toml`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/data/somesy.toml` & `somesy-0.4.2/tests/data/somesy.toml`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/input/test_cff_validate.py` & `somesy-0.4.2/tests/input/test_cff_validate.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/input/test_core_core.py` & `somesy-0.4.2/tests/input/test_core_core.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/input/test_fortran_validate.py` & `somesy-0.4.2/tests/input/test_fortran_validate.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/input/test_julia_validate.py` & `somesy-0.4.2/tests/input/test_julia_validate.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/input/test_mkdocs_validate.py` & `somesy-0.4.2/tests/input/test_mkdocs_validate.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/input/test_package_json_validate.py` & `somesy-0.4.2/tests/input/test_package_json_validate.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/input/test_pyproject_validate.py` & `somesy-0.4.2/tests/input/test_pyproject_validate.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/input/test_rust_validate.py` & `somesy-0.4.2/tests/input/test_rust_validate.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/output/test_cff_writer.py` & `somesy-0.4.2/tests/output/test_cff_writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/output/test_codemeta.py` & `somesy-0.4.2/tests/output/test_codemeta.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/output/test_fortran_writer.py` & `somesy-0.4.2/tests/output/test_fortran_writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/output/test_julia_writer.py` & `somesy-0.4.2/tests/output/test_julia_writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/output/test_mkdocs_writer.py` & `somesy-0.4.2/tests/output/test_mkdocs_writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/output/test_package_json_writer.py` & `somesy-0.4.2/tests/output/test_package_json_writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/output/test_pom_writer.py` & `somesy-0.4.2/tests/output/test_pom_writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/output/test_pyproject_writer.py` & `somesy-0.4.2/tests/output/test_pyproject_writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/output/test_rust_writer.py` & `somesy-0.4.2/tests/output/test_rust_writer.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/processing/test_cli_util.py` & `somesy-0.4.2/tests/processing/test_cli_util.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/processing/test_core_models.py` & `somesy-0.4.2/tests/processing/test_core_models.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/processing/test_xmlwrapper.py` & `somesy-0.4.2/tests/processing/test_xmlwrapper.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/tests/test_main.py` & `somesy-0.4.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `somesy-0.4.1/PKG-INFO` & `somesy-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somesy
-Version: 0.4.1
+Version: 0.4.2
 Summary: A CLI tool for synchronizing software project metadata.
 Home-page: https://materials-data-science-and-informatics.github.io/somesy
 License: MIT
 Keywords: metadata,FAIR
 Author: Mustafa Soylu
 Author-email: m.soylu@fz-juelich.de
 Maintainer: Mustafa Soylu
```

