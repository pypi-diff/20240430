# Comparing `tmp/pdm_backend-2.2.1.tar.gz` & `tmp/pdm_backend-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_backend-2.2.1.tar", last modified: Thu Apr 18 03:32:59 2024, max compression
+gzip compressed data, was "pdm_backend-2.3.0.tar", last modified: Tue Apr 30 07:43:23 2024, max compression
```

## Comparing `pdm_backend-2.2.1.tar` & `pdm_backend-2.3.0.tar`

### file list

```diff
@@ -1,185 +1,185 @@
--rw-r--r--   0        0        0     1067 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/LICENSE
--rw-r--r--   0        0        0     1711 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/README.md
--rw-r--r--   0        0        0     2326 2024-04-18 03:32:59.568298 pdm_backend-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     3286 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/__init__.py
--rw-r--r--   0        0        0      197 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/LICENSE
--rw-r--r--   0        0        0    10174 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/LICENSE.BSD
--rw-r--r--   0        0        0      496 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     9590 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2676 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0    10347 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/markers.py
--rw-r--r--   0        0        0    33036 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/metadata.py
--rw-r--r--   0        0        0        0 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     2933 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39824 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18950 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     5268 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16256 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/version.py
--rw-r--r--   0        0        0     1113 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
--rw-r--r--   0        0        0    21011 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/pyproject_metadata/py.typed
--rw-r--r--   0        0        0     1072 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/LICENSE
--rw-r--r--   0        0        0      396 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/py.typed
--rw-r--r--   0        0        0     1072 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli_w/LICENSE
--rw-r--r--   0        0        0      177 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli_w/__init__.py
--rw-r--r--   0        0        0     6132 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli_w/_writer.py
--rw-r--r--   0        0        0       26 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli_w/py.typed
--rw-r--r--   0        0        0       70 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/vendor.txt
--rw-r--r--   0        0        0    12629 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/base.py
--rw-r--r--   0        0        0     9872 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/config.py
--rw-r--r--   0        0        0     3674 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/editable.py
--rw-r--r--   0        0        0      452 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/exceptions.py
--rw-r--r--   0        0        0      108 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/hooks/__init__.py
--rw-r--r--   0        0        0     4593 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/hooks/base.py
--rw-r--r--   0        0        0     6459 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/hooks/setuptools.py
--rw-r--r--   0        0        0     5296 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/hooks/version/__init__.py
--rw-r--r--   0        0        0    10153 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/hooks/version/scm.py
--rw-r--r--   0        0        0     1037 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/intree.py
--rw-r--r--   0        0        0    14959 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/macosx_platform.py
--rw-r--r--   0        0        0        0 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/py.typed
--rw-r--r--   0        0        0     3050 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/sdist.py
--rw-r--r--   0        0        0     1381 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/structures.py
--rw-r--r--   0        0        0     8985 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/utils.py
--rw-r--r--   0        0        0    12797 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/wheel.py
--rw-r--r--   0        0        0       72 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/__init__.py
--rw-r--r--   0        0        0      929 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/conftest.py
--rw-r--r--   0        0        0      856 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/hooks/hook_class.py
--rw-r--r--   0        0        0      599 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/hooks/hook_module.py
--rw-r--r--   0        0        0      599 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/hooks/local_hook.py
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/LICENSE
--rw-r--r--   0        0        0      138 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
--rw-r--r--   0        0        0      234 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
--rw-r--r--   0        0        0      558 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
--rw-r--r--   0        0        0      478 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/LICENSE
--rw-r--r--   0        0        0       22 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/my_package/__init__.py
--rw-r--r--   0        0        0      478 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
--rw-r--r--   0        0        0      138 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/pdm.lock
--rw-r--r--   0        0        0      230 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/pdm_build.py
--rw-r--r--   0        0        0      554 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/pyproject.toml
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-combined-extras/LICENSE
--rw-r--r--   0        0        0       26 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      379 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/README.md
--rw-r--r--   0        0        0       16 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
--rw-r--r--   0        0        0       22 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
--rw-r--r--   0        0        0      433 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-metadata-test/LICENSE
--rw-r--r--   0        0        0        0 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-metadata-test/README.md
--rw-r--r--   0        0        0      407 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-metadata-test/pyproject.toml
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       60 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      402 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-no-license/README.md
--rw-r--r--   0        0        0      406 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-no-license/pyproject.toml
--rw-r--r--   0        0        0       36 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-no-license/src/foo_module.py
--rw-r--r--   0        0        0        0 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-no-version/README.md
-lrwxr-xr-x   0        0        0        0 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
--rw-r--r--   0        0        0      330 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-no-version/pyproject.toml
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/LICENSE
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/README.md
--rw-r--r--   0        0        0       16 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/data_out.json
--rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/my_package/data.json
--rw-r--r--   0        0        0     7700 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/pdm.lock
--rw-r--r--   0        0        0      555 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/pyproject.toml
--rw-r--r--   0        0        0     4259 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/requirements.txt
--rw-r--r--   0        0        0      604 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
--rw-r--r--   0        0        0       21 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/single_module.py
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/LICENSE
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/README.md
--rw-r--r--   0        0        0       16 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/data_out.json
--rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/my_package/data.json
--rw-r--r--   0        0        0     7700 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/pdm.lock
--rw-r--r--   0        0        0      642 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/pyproject.toml
--rw-r--r--   0        0        0     4259 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/requirements.txt
--rw-r--r--   0        0        0      604 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/requirements_simple.txt
--rwxr-xr-x   0        0        0       32 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/scripts/data/my_script.sh
--rw-r--r--   0        0        0       21 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/single_module.py
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/README.md
--rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
--rw-r--r--   0        0        0       16 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
--rw-r--r--   0        0        0      574 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/LICENSE
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/README.md
--rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
--rw-r--r--   0        0        0     7700 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/pdm.lock
--rw-r--r--   0        0        0      513 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/my_package/data.json
--rwxr-xr-x   0        0        0        0 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/my_package/executable
--rw-r--r--   0        0        0     2461 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      598 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0     4259 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      604 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0       21 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-pep420-package/LICENSE
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-pep420-package/README.md
--rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
--rw-r--r--   0        0        0        3 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
--rw-r--r--   0        0        0      464 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-pep420-package/pyproject.toml
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-purelib-with-build/LICENSE
--rw-r--r--   0        0        0      277 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-purelib-with-build/my_build.py
--rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
--rw-r--r--   0        0        0      138 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
--rw-r--r--   0        0        0      549 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
--rw-r--r--   0        0        0       26 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-reuse-spec/README.md
--rw-r--r--   0        0        0      413 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
--rw-r--r--   0        0        0       36 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/LICENSE
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/README.md
--rw-r--r--   0        0        0       16 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/data_out.json
--rw-r--r--   0        0        0      500 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/single_module.py
--rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      395 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-pymodule/LICENSE
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-pymodule/README.md
--rw-r--r--   0        0        0      406 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
--rw-r--r--   0        0        0       36 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
--rw-r--r--   0        0        0       36 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-using-scm/.gitignore
--rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-using-scm/LICENSE
--rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-using-scm/README.md
--rw-r--r--   0        0        0       36 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-using-scm/foo/__init__.py
--rw-r--r--   0        0        0      369 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-using-scm/pyproject.toml
--rw-r--r--   0        0        0      156 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-using-scm/version.py
--rw-r--r--   0        0        0    21084 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/test_api.py
--rw-r--r--   0        0        0     5324 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/test_file_finder.py
--rw-r--r--   0        0        0     1632 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/test_hooks.py
--rw-r--r--   0        0        0     3058 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/test_metadata.py
--rw-r--r--   0        0        0      748 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/test_utils.py
--rw-r--r--   0        0        0     1176 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/test_wheel.py
--rw-r--r--   0        0        0      318 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/testutils.py
--rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 pdm_backend-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-30 07:43:16.058700 pdm_backend-2.3.0/LICENSE
+-rw-r--r--   0        0        0     1711 2024-04-30 07:43:16.058700 pdm_backend-2.3.0/README.md
+-rw-r--r--   0        0        0     2386 2024-04-30 07:43:23.946769 pdm_backend-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3286 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/__init__.py
+-rw-r--r--   0        0        0      197 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/LICENSE
+-rw-r--r--   0        0        0    10174 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/LICENSE.BSD
+-rw-r--r--   0        0        0      496 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     9590 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2676 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10347 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0    33036 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     2933 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39824 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18950 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     5268 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16256 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     1113 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
+-rw-r--r--   0        0        0    21011 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/pyproject_metadata/py.typed
+-rw-r--r--   0        0        0     1072 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli/LICENSE
+-rw-r--r--   0        0        0      396 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2024-04-30 07:43:16.062700 pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0     1072 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli_w/LICENSE
+-rw-r--r--   0        0        0      177 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli_w/__init__.py
+-rw-r--r--   0        0        0     6132 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli_w/_writer.py
+-rw-r--r--   0        0        0       26 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli_w/py.typed
+-rw-r--r--   0        0        0       70 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/_vendor/vendor.txt
+-rw-r--r--   0        0        0    12723 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/base.py
+-rw-r--r--   0        0        0     9872 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/config.py
+-rw-r--r--   0        0        0     3674 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/editable.py
+-rw-r--r--   0        0        0      452 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/exceptions.py
+-rw-r--r--   0        0        0      108 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/hooks/__init__.py
+-rw-r--r--   0        0        0     4604 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/hooks/base.py
+-rw-r--r--   0        0        0     6459 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/hooks/setuptools.py
+-rw-r--r--   0        0        0     5407 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/hooks/version/__init__.py
+-rw-r--r--   0        0        0     9619 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/hooks/version/scm.py
+-rw-r--r--   0        0        0     1037 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/intree.py
+-rw-r--r--   0        0        0        0 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/py.typed
+-rw-r--r--   0        0        0     3050 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/sdist.py
+-rw-r--r--   0        0        0     1381 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/structures.py
+-rw-r--r--   0        0        0     6907 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/utils.py
+-rw-r--r--   0        0        0    12418 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/src/pdm/backend/wheel.py
+-rw-r--r--   0        0        0       72 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/conftest.py
+-rw-r--r--   0        0        0      856 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/hooks/hook_class.py
+-rw-r--r--   0        0        0      599 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/hooks/hook_module.py
+-rw-r--r--   0        0        0      599 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/hooks/local_hook.py
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension-in-src/LICENSE
+-rw-r--r--   0        0        0      138 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
+-rw-r--r--   0        0        0      234 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
+-rw-r--r--   0        0        0      558 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension/LICENSE
+-rw-r--r--   0        0        0       22 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
+-rw-r--r--   0        0        0      138 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension/pdm.lock
+-rw-r--r--   0        0        0      230 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension/pdm_build.py
+-rw-r--r--   0        0        0      554 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-combined-extras/LICENSE
+-rw-r--r--   0        0        0       26 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      379 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-explicit-package-dir/README.md
+-rw-r--r--   0        0        0       16 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
+-rw-r--r--   0        0        0       22 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
+-rw-r--r--   0        0        0      433 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-metadata-test/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-metadata-test/README.md
+-rw-r--r--   0        0        0      407 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-metadata-test/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       60 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      402 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-no-license/README.md
+-rw-r--r--   0        0        0      406 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-no-license/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-no-license/src/foo_module.py
+-rw-r--r--   0        0        0        0 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-no-version/README.md
+lrwxr-xr-x   0        0        0        0 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
+-rw-r--r--   0        0        0      330 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-no-version/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/README.md
+-rw-r--r--   0        0        0       16 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/data_out.json
+-rw-r--r--   0        0        0       22 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/my_package/data.json
+-rw-r--r--   0        0        0     7700 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/pdm.lock
+-rw-r--r--   0        0        0      555 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/pyproject.toml
+-rw-r--r--   0        0        0     4259 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/requirements.txt
+-rw-r--r--   0        0        0      604 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/single_module.py
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/README.md
+-rw-r--r--   0        0        0       16 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/data_out.json
+-rw-r--r--   0        0        0       22 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/my_package/data.json
+-rw-r--r--   0        0        0     7700 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/pdm.lock
+-rw-r--r--   0        0        0      642 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/pyproject.toml
+-rw-r--r--   0        0        0     4259 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/requirements.txt
+-rw-r--r--   0        0        0      604 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/requirements_simple.txt
+-rwxr-xr-x   0        0        0       32 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/scripts/data/my_script.sh
+-rw-r--r--   0        0        0       21 2024-04-30 07:43:16.066700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/single_module.py
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-deep-path/README.md
+-rw-r--r--   0        0        0       22 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
+-rw-r--r--   0        0        0       16 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
+-rw-r--r--   0        0        0      574 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-tests/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-tests/README.md
+-rw-r--r--   0        0        0       22 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
+-rw-r--r--   0        0        0     7700 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-tests/pdm.lock
+-rw-r--r--   0        0        0      513 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package/my_package/data.json
+-rwxr-xr-x   0        0        0        0 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package/my_package/executable
+-rw-r--r--   0        0        0     2461 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      598 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0     4259 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      604 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-pep420-package/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-pep420-package/README.md
+-rw-r--r--   0        0        0       22 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
+-rw-r--r--   0        0        0        3 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
+-rw-r--r--   0        0        0      464 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-pep420-package/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-purelib-with-build/LICENSE
+-rw-r--r--   0        0        0      277 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-purelib-with-build/my_build.py
+-rw-r--r--   0        0        0       22 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
+-rw-r--r--   0        0        0      138 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
+-rw-r--r--   0        0        0      549 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
+-rw-r--r--   0        0        0       26 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-reuse-spec/README.md
+-rw-r--r--   0        0        0      413 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package-include/README.md
+-rw-r--r--   0        0        0       16 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package-include/data_out.json
+-rw-r--r--   0        0        0      500 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package-include/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package-include/single_module.py
+-rw-r--r--   0        0        0       22 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      395 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-pymodule/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-pymodule/README.md
+-rw-r--r--   0        0        0      406 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
+-rw-r--r--   0        0        0       36 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-using-scm/.gitignore
+-rw-r--r--   0        0        0       12 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-using-scm/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-using-scm/README.md
+-rw-r--r--   0        0        0       36 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-using-scm/foo/__init__.py
+-rw-r--r--   0        0        0      369 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-using-scm/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/fixtures/projects/demo-using-scm/version.py
+-rw-r--r--   0        0        0     7409 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/pdm/backend/hooks/version/test_scm.py
+-rw-r--r--   0        0        0    21084 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/test_api.py
+-rw-r--r--   0        0        0     5324 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/test_file_finder.py
+-rw-r--r--   0        0        0     1632 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/test_hooks.py
+-rw-r--r--   0        0        0     3058 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/test_metadata.py
+-rw-r--r--   0        0        0      748 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1176 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/test_wheel.py
+-rw-r--r--   0        0        0      318 2024-04-30 07:43:16.070700 pdm_backend-2.3.0/tests/testutils.py
+-rw-r--r--   0        0        0     2673 1970-01-01 00:00:00.000000 pdm_backend-2.3.0/PKG-INFO
```

### Comparing `pdm_backend-2.2.1/LICENSE` & `pdm_backend-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/README.md` & `pdm_backend-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/pyproject.toml` & `pdm_backend-2.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [project]
 name = "pdm-backend"
 description = "The build backend used by PDM that supports latest packaging standards"
 authors = [
     { name = "Frost Ming", email = "me@frostming.com" },
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "packaging",
     "PEP 517",
     "build",
 ]
 dynamic = []
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "importlib-metadata>=3.6; python_version < \"3.10\"",
 ]
-version = "2.2.1"
+version = "2.3.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/pdm-project/pdm-backend"
 Repository = "https://github.com/pdm-project/pdm-backend"
@@ -105,16 +105,18 @@
 test = [
     "pytest",
     "pytest-cov",
     "pytest-xdist",
     "setuptools",
 ]
 dev = [
-    "editables",
-    "vendoring; python_version ~= '3.8'",
+    "editables>=0.3",
+    "pre-commit>=2.21.0",
+    "vendoring>=1.2.0; python_version ~= \"3.8\"",
+    "ruff>=0.4.1",
 ]
 docs = [
     "mkdocs>=1.4.2",
     "mkdocstrings[python]>=0.19.0",
     "mkdocs-material>=8.5.10",
     "mkdocs-version-annotations>=1.0.0",
 ]
```

### Comparing `pdm_backend-2.2.1/src/pdm/backend/__init__.py` & `pdm_backend-2.3.0/src/pdm/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/LICENSE.APACHE` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/LICENSE.BSD` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_elffile.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_manylinux.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_musllinux.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_parser.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_structures.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_tokenizer.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/markers.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/metadata.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/requirements.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/specifiers.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/tags.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/utils.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/version.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/pyproject_metadata/LICENSE` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/pyproject_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/pyproject_metadata/__init__.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/pyproject_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/LICENSE` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/_parser.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/_re.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli_w/LICENSE` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli_w/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli_w/_writer.py` & `pdm_backend-2.3.0/src/pdm/backend/_vendor/tomli_w/_writer.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/base.py` & `pdm_backend-2.3.0/src/pdm/backend/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,23 @@
 import glob
 import os
 import shutil
 import sys
 import warnings
 from fnmatch import fnmatch
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Iterable, Mapping, TypeVar, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Iterable,
+    Literal,
+    Mapping,
+    TypeVar,
+    cast,
+)
 
 from pdm.backend.config import Config
 from pdm.backend.exceptions import PDMWarning, ValidationError
 from pdm.backend.hooks import BuildHookInterface, Context
 from pdm.backend.hooks.version import DynamicVersionBuildHook
 from pdm.backend.structures import FileMap
 from pdm.backend.utils import expand_vars, import_module_at_path, is_python_package
@@ -77,20 +85,23 @@
     for path in os.listdir(root):
         path = os.path.join(root, path)
         if is_python_package(path):
             result.append(path)
     return result
 
 
+Target = Literal["sdist", "wheel", "editable"]
+
+
 class Builder:
     """Base class for building and distributing a package from given path."""
 
     DEFAULT_EXCLUDES = [".pdm-build"]
 
-    target: str
+    target: Target
     hooks: list[BuildHookInterface] = [DynamicVersionBuildHook()]
 
     def __init__(
         self,
         location: str | Path,
         config_settings: Mapping[str, Any] | None = None,
     ) -> None:
```

### Comparing `pdm_backend-2.2.1/src/pdm/backend/config.py` & `pdm_backend-2.3.0/src/pdm/backend/config.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/editable.py` & `pdm_backend-2.3.0/src/pdm/backend/editable.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/hooks/base.py` & `pdm_backend-2.3.0/src/pdm/backend/hooks/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING, Any, Iterable
 
 from pdm.backend.config import Config
 
 if TYPE_CHECKING:
     from typing import Protocol
 
-    from pdm.backend.base import Builder
+    from pdm.backend.base import Builder, Target
 else:
     Protocol = object
 
 
 @dataclasses.dataclass()
 class Context:
     """The context object for the build hook,
@@ -40,15 +40,15 @@
 
     @property
     def root(self) -> Path:
         """The project root directory"""
         return self.builder.location
 
     @property
-    def target(self) -> str:
+    def target(self) -> Target:
         """The target to build, one of 'sdist', 'wheel', 'editable'"""
         return self.builder.target
 
     @property
     def config_settings(self) -> dict[str, str]:
         """The config settings passed to the hook"""
         return self.builder.config_settings
```

### Comparing `pdm_backend-2.2.1/src/pdm/backend/hooks/setuptools.py` & `pdm_backend-2.3.0/src/pdm/backend/hooks/setuptools.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/hooks/version/__init__.py` & `pdm_backend-2.3.0/src/pdm/backend/hooks/version/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,28 +71,32 @@
 
     def resolve_version_from_scm(
         self,
         context: Context,
         write_to: str | None = None,
         write_template: str = "{}\n",
         tag_regex: str | None = None,
+        tag_filter: str | None = None,
         version_format: str | None = None,
         fallback_version: str | None = None,
     ) -> str:
         if "PDM_BUILD_SCM_VERSION" in os.environ:
             version = os.environ["PDM_BUILD_SCM_VERSION"]
         else:
             if version_format is not None:
                 version_formatter, _ = evaluate_module_attribute(
                     version_format, context.root
                 )
             else:
                 version_formatter = None
             version = get_version_from_scm(
-                context.root, tag_regex=tag_regex, version_formatter=version_formatter
+                context.root,
+                tag_regex=tag_regex,
+                version_formatter=version_formatter,
+                tag_filter=tag_filter,
             )
             if version is None:
                 if fallback_version is not None:
                     version = fallback_version
                 else:
                     raise ConfigError(
                         "Cannot find the version from SCM or SCM isn't detected. \n"
```

### Comparing `pdm_backend-2.2.1/src/pdm/backend/hooks/version/scm.py` & `pdm_backend-2.3.0/src/pdm/backend/hooks/version/scm.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 import shlex
 import shutil
 import subprocess
 import warnings
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from pathlib import Path
-from typing import TYPE_CHECKING, Callable, Iterable, NamedTuple
+from typing import TYPE_CHECKING, Callable, NamedTuple
 
 from pdm.backend._vendor.packaging.version import Version
 
 if TYPE_CHECKING:
     from _typeshed import StrPath
 
 DEFAULT_TAG_REGEX = re.compile(
     r"^(?:[\w-]+-)?(?P<version>[vV]?\d+(?:\.\d+){0,2}[^\+]*)(?:\+.*)?$"
 )
 
 
 @dataclass(frozen=True)
 class Config:
     tag_regex: re.Pattern
+    tag_filter: str | None
 
 
 def _subprocess_call(
     cmd: str | list[str],
     cwd: StrPath | None = None,
     extra_env: dict[str, str] | None = None,
 ) -> tuple[int, str, str]:
@@ -160,36 +161,35 @@
 
     if tagdict.suffix:
         warnings.warn(f"tag {tag!r} will be stripped of its suffix {tagdict.suffix!r}")
 
     return Version(version)
 
 
-def tags_to_versions(config: Config, tags: Iterable[str]) -> list[Version]:
-    """
-    take tags that might be prefixed with a keyword and return only the version part
-    :param tags: an iterable of tags
-    :param config: optional configuration object
-    """
-    return [tag_to_version(config, tag) for tag in tags if tag]
-
-
 def git_parse_version(root: StrPath, config: Config) -> SCMVersion | None:
-    GIT = shutil.which("git")
-    if not GIT:
+    git = shutil.which("git")
+    if not git:
         return None
 
-    ret, repo, _ = _subprocess_call([GIT, "rev-parse", "--show-toplevel"], root)
+    ret, repo, _ = _subprocess_call([git, "rev-parse", "--show-toplevel"], root)
     if ret or not repo:
         return None
 
     if os.path.isfile(os.path.join(repo, ".git/shallow")):
         warnings.warn(f"{repo!r} is shallow and may cause errors")
-    describe_cmd = [GIT, "describe", "--dirty", "--tags", "--long", "--match", "*.*"]
-    ret, output, err = _subprocess_call(describe_cmd, repo)
+    describe_cmd = [
+        git,
+        "describe",
+        "--dirty",
+        "--tags",
+        "--long",
+        "--match",
+        config.tag_filter or "*.*",
+    ]
+    ret, output, _ = _subprocess_call(describe_cmd, repo)
     branch = _git_get_branch(repo)
 
     if ret:
         rev_node = _git_get_node(repo)
         dirty = _git_is_dirty(repo)
         if rev_node is None:
             return meta(config, "0.0", 0, dirty)
@@ -197,62 +197,52 @@
             config, "0.0", _git_count_all_nodes(repo), dirty, f"g{rev_node}", branch
         )
     else:
         tag, number, node, dirty = _git_parse_describe(output)
         return meta(config, tag, number or None, dirty, node, branch)
 
 
-def get_latest_normalizable_tag(root: StrPath) -> str:
-    # Gets all tags containing a '.' from oldest to newest
-    cmd = [
-        "hg",
-        "log",
-        "-r",
-        "ancestors(.) and tag('re:\\.')",
-        "--template",
-        "{tags}\n",
-    ]
-    _, output, _ = _subprocess_call(cmd, root)
-    outlines = output.split()
-    if not outlines:
-        return "null"
-    tag = outlines[-1].split()[-1]
-    return tag
+def get_distance_revset(tag: str | None) -> str:
+    return (
+        "(branch(.)"  # look for revisions in this branch only
+        " and {rev}::."  # after the last tag
+        # ignore commits that only modify .hgtags and nothing else:
+        " and (merge() or file('re:^(?!\\.hgtags).*$'))"
+        " and not {rev})"  # ignore the tagged commit itself
+    ).format(rev=f"tag({tag!r})" if tag is not None else "null")
 
 
-def hg_get_graph_distance(root: StrPath, rev1: str, rev2: str = ".") -> int:
-    cmd = ["hg", "log", "-q", "-r", f"{rev1}::{rev2}"]
+def hg_get_graph_distance(root: StrPath, tag: str | None) -> int:
+    cmd = ["hg", "log", "-q", "-r", get_distance_revset(tag)]
     _, out, _ = _subprocess_call(cmd, root)
-    return len(out.strip().splitlines()) - 1
+    return len(out.strip().splitlines())
 
 
 def _hg_tagdist_normalize_tagcommit(
-    config: Config, root: StrPath, tag: str, dist: int, node: str, branch: str
+    config: Config,
+    root: StrPath,
+    tag: str,
+    dist: int,
+    node: str,
+    branch: str,
+    dirty: bool,
 ) -> SCMVersion:
-    dirty = node.endswith("+")
-    node = "h" + node.strip("+")
-
     # Detect changes since the specified tag
-    revset = (
-        "(branch(.)"  # look for revisions in this branch only
-        " and tag({tag!r})::."  # after the last tag
-        # ignore commits that only modify .hgtags and nothing else:
-        " and (merge() or file('re:^(?!\\.hgtags).*$'))"
-        " and not tag({tag!r}))"  # ignore the tagged commit itself
-    ).format(tag=tag)
     if tag != "0.0":
         _, commits, _ = _subprocess_call(
-            ["hg", "log", "-r", revset, "--template", "{node|short}"],
+            ["hg", "log", "-r", get_distance_revset(tag), "--template", "{node|short}"],
             root,
         )
     else:
         commits = "True"
 
     if commits or dirty:
-        return meta(config, tag, distance=dist, node=node, dirty=dirty, branch=branch)
+        return meta(
+            config, tag, distance=dist or None, node=node, dirty=dirty, branch=branch
+        )
     else:
         return meta(config, tag)
 
 
 def guess_next_version(tag_version: Version) -> str:
     version = _strip_local(str(tag_version))
     return _bump_dev(version) or _bump_regex(version)
@@ -276,40 +266,48 @@
     match = re.match(r"(.*?)(\d+)$", version)
     assert match is not None
     prefix, tail = match.groups()
     return "%s%d" % (prefix, int(tail) + 1)
 
 
 def hg_parse_version(root: StrPath, config: Config) -> SCMVersion | None:
-    if not shutil.which("hg"):
+    hg = shutil.which("hg")
+    if not hg:
         return None
-    _, output, _ = _subprocess_call("hg id -i -b -t", root)
-    identity_data = output.split()
-    if not identity_data:
-        return None
-    node = identity_data.pop(0)
-    branch = identity_data.pop(0)
-    if "tip" in identity_data:
-        # tip is not a real tag
-        identity_data.remove("tip")
-    tags = tags_to_versions(config, identity_data)
-    dirty = node[-1] == "+"
-    if tags:
-        return meta(config, tags[0], dirty=dirty, branch=branch)
-
-    if node.strip("+") == "0" * 12:
-        return meta(config, "0.0", dirty=dirty, branch=branch)
 
+    tag_filter = config.tag_filter or "\\."
+    _, output, _ = _subprocess_call(
+        [
+            hg,
+            "log",
+            "-r",
+            ".",
+            "--template",
+            f"{{latesttag(r're:{tag_filter}')}}-{{node|short}}-{{branch}}",
+        ],
+        root,
+    )
+    tag: str | None
+    tag, node, branch = output.rsplit("-", 2)
+    # If no tag exists passes the tag filter.
+    if tag == "null":
+        tag = None
+
+    _, id_output, _ = _subprocess_call(
+        [hg, "id", "-i"],
+        root,
+    )
+    dirty = id_output.endswith("+")
     try:
-        tag = get_latest_normalizable_tag(root)
         dist = hg_get_graph_distance(root, tag)
-        if tag == "null":
+        if tag is None:
             tag = "0.0"
-            dist = int(dist) + 1
-        return _hg_tagdist_normalize_tagcommit(config, root, tag, dist, node, branch)
+        return _hg_tagdist_normalize_tagcommit(
+            config, root, tag, dist, node, branch, dirty=dirty
+        )
     except ValueError:
         return None  # unpacking failed, old hg
 
 
 def format_version(version: SCMVersion) -> str:
     if version.distance is None:
         main_version = str(version.version)
@@ -328,17 +326,21 @@
     return main_version + local_version
 
 
 def get_version_from_scm(
     root: str | Path,
     *,
     tag_regex: str | None = None,
+    tag_filter: str | None = None,
     version_formatter: Callable[[SCMVersion], str] | None = None,
 ) -> str | None:
-    config = Config(tag_regex=re.compile(tag_regex) if tag_regex else DEFAULT_TAG_REGEX)
+    config = Config(
+        tag_regex=re.compile(tag_regex) if tag_regex else DEFAULT_TAG_REGEX,
+        tag_filter=tag_filter,
+    )
     for func in (git_parse_version, hg_parse_version):
-        version = func(root, config)  # type: ignore
+        version = func(root, config)
         if version:
             if version_formatter is None:
                 version_formatter = format_version
             return version_formatter(version)
     return None
```

### Comparing `pdm_backend-2.2.1/src/pdm/backend/intree.py` & `pdm_backend-2.3.0/src/pdm/backend/intree.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/sdist.py` & `pdm_backend-2.3.0/src/pdm/backend/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/structures.py` & `pdm_backend-2.3.0/src/pdm/backend/structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/src/pdm/backend/utils.py` & `pdm_backend-2.3.0/src/pdm/backend/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,29 +3,25 @@
 import ast
 import contextlib
 import functools
 import importlib.util
 import os
 import re
 import sys
-import sysconfig
 import types
 import urllib.parse
-import warnings
 from contextlib import contextmanager
 from fnmatch import fnmatchcase
 from pathlib import Path
 from typing import Any, Callable, Generator, Iterable, Match
 
-from pdm.backend._vendor.packaging import tags
 from pdm.backend._vendor.packaging.markers import Marker
 from pdm.backend._vendor.packaging.requirements import Requirement
 from pdm.backend._vendor.packaging.version import InvalidVersion, Version
 from pdm.backend.exceptions import ConfigError
-from pdm.backend.macosx_platform import calculate_macosx_platform_tag
 
 
 def safe_version(version: str) -> str:
     """
     Convert an arbitrary string to a standard version string
     """
     try:
@@ -107,87 +103,29 @@
 
             # Keep searching subdirectories, as there may be more packages
             # down there, even if the parent was excluded.
             dirs.append(dir)
 
 
 @contextmanager
-def cd(path: str) -> Generator[None, None, None]:
+def cd(path: str | Path) -> Generator[None, None, None]:
     _old_cwd = os.getcwd()
     os.chdir(path)
     try:
         yield
     finally:
         os.chdir(_old_cwd)
 
 
 def normalize_path(filename: str | Path) -> str:
     """Normalize a file/dir name for comparison purposes"""
     filename = os.path.abspath(filename) if sys.platform == "cygwin" else filename
     return os.path.normcase(os.path.realpath(os.path.normpath(filename)))
 
 
-def get_platform(build_dir: str | Path) -> str:
-    """Return our platform name 'win32', 'linux_x86_64'"""
-    result = sysconfig.get_platform()
-    if result.startswith("macosx") and os.path.exists(build_dir):
-        result = calculate_macosx_platform_tag(build_dir, result)
-    if result in ("linux_x86_64", "linux-x86_64") and sys.maxsize == 2147483647:
-        # pip pull request #3497
-        result = "linux_i686"
-    return result
-
-
-def get_flag(
-    var: str, fallback: bool, expected: bool = True, warn: bool = True
-) -> bool:
-    """Use a fallback value for determining SOABI flags if the needed config
-    var is unset or unavailable."""
-    val = sysconfig.get_config_var(var)
-    if val is None:
-        if warn:
-            warnings.warn(
-                "Config variable '{}' is unset, Python ABI tag may "
-                "be incorrect".format(var),
-                RuntimeWarning,
-                2,
-            )
-        return fallback
-    return val == expected
-
-
-def get_abi_tag() -> str | None:
-    """Return the ABI tag based on SOABI (if available) or emulate SOABI
-    (CPython 2, PyPy)."""
-    soabi = sysconfig.get_config_var("SOABI")
-    impl = tags.interpreter_name()
-    is_cpython = impl == "cp"
-    if not soabi and impl in ("cp", "pp") and hasattr(sys, "maxunicode"):
-        d = ""
-        m = ""
-        u = ""
-        if get_flag("Py_DEBUG", hasattr(sys, "gettotalrefcount"), warn=is_cpython):
-            d = "d"
-        if sys.version_info < (3, 8) and get_flag(
-            "WITH_PYMALLOC", is_cpython, warn=is_cpython
-        ):
-            m = "m"
-        if sys.version_info < (3, 3) and get_flag(
-            "Py_UNICODE_SIZE", sys.maxunicode == 0x10FFFF, expected=4, warn=is_cpython
-        ):
-            u = "u"
-        return f"{impl}{tags.interpreter_version()}{d}{m}{u}"
-    elif soabi and soabi.startswith("cpython-"):
-        return "cp" + soabi.split("-")[1]
-    elif soabi:
-        return soabi.replace(".", "_").replace("-", "_")
-    else:
-        return None
-
-
 def is_relative_path(target: Path, other: Path) -> bool:
     try:
         target.relative_to(other)
     except ValueError:
         return False
     else:
         return True
@@ -273,11 +211,14 @@
         )
     with cm:
         module = importlib.import_module(matched.group(1))
         attrs = matched.group(2).split(".")
         obj: Any = functools.reduce(getattr, attrs, module)
         args_group = matched.group(3)
         if args_group:
+            # make tuple
+            args_group = args_group.strip()[:-1] + ",)"
             args = ast.literal_eval(args_group)
+
         else:
             args = ()
         return obj, args
```

### Comparing `pdm_backend-2.2.1/src/pdm/backend/wheel.py` & `pdm_backend-2.3.0/src/pdm/backend/wheel.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,45 +3,39 @@
 import csv
 import hashlib
 import io
 import os
 import posixpath
 import shutil
 import stat
-import sys
 import tempfile
 import time
 import zipfile
 from base64 import urlsafe_b64encode
+from importlib.metadata import version as get_version
 from pathlib import Path
 from typing import IO, Any, Iterable, Mapping, NamedTuple, cast
 
 from pdm.backend._vendor.packaging import tags
 from pdm.backend._vendor.packaging.specifiers import SpecifierSet
 from pdm.backend._vendor.packaging.utils import _build_tag_regex, canonicalize_name
 from pdm.backend.base import Builder
 from pdm.backend.hooks import Context
 from pdm.backend.hooks.setuptools import SetuptoolsBuildHook
 from pdm.backend.structures import FileMap
 from pdm.backend.utils import (
-    get_abi_tag,
-    get_platform,
     normalize_file_permissions,
     safe_version,
     to_filename,
 )
 
 SCHEME_NAMES = frozenset(
     ["purelib", "platlib", "include", "platinclude", "scripts", "data"]
 )
 
-if sys.version_info < (3, 8):
-    from importlib_metadata import version as get_version
-else:
-    from importlib.metadata import version as get_version
 
 WHEEL_FILE_FORMAT = """\
 Wheel-Version: 1.0
 Generator: pdm-backend ({version})
 Root-Is-Purelib: {is_purelib}
 Tag: {tag}
 """
@@ -203,38 +197,35 @@
 
         return build_number
 
     def _get_tag(self) -> str:
         impl, abi, platform = self._get_platform_tags()
         is_purelib = self.config.build_config.is_purelib
         if not is_purelib:
+            sys_tag = next(tags.sys_tags())
             if not platform:
-                platform = get_platform(self.location / "build")
+                platform = sys_tag.platform
             if not impl:
-                impl = tags.interpreter_name() + tags.interpreter_version()
+                impl = sys_tag.interpreter
             if not abi:
-                abi = str(get_abi_tag()).lower()
+                abi = sys_tag.abi
         else:
             if not platform:
                 platform = "any"
-            abi = "none"
+            if not abi:
+                abi = "none"
             if not impl:
                 requires_python = self.config.metadata.get("requires-python", "")
                 if SpecifierSet(requires_python).contains("2.7"):
                     impl = "py2.py3"
                 else:
                     impl = "py3"
 
         platform = platform.lower().replace("-", "_").replace(".", "_")  # type: ignore
         tag = (impl, abi, platform)
-        if not is_purelib:
-            supported_tags = [(t.interpreter, t.abi, platform) for t in tags.sys_tags()]
-            assert (
-                tag in supported_tags
-            ), f"would build wheel with unsupported tag {tag}"
         return "-".join(tag)  # type: ignore[arg-type]
 
     def _write_dist_info(self, parent: Path) -> Path:
         """write the dist-info directory and return the path to it"""
         dist_info = parent / self.dist_info_name
         dist_info.mkdir(0o700, exist_ok=True)
         meta = self.config.metadata
```

### Comparing `pdm_backend-2.2.1/tests/conftest.py` & `pdm_backend-2.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/hooks/hook_class.py` & `pdm_backend-2.3.0/tests/fixtures/hooks/hook_class.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/hooks/hook_module.py` & `pdm_backend-2.3.0/tests/fixtures/hooks/hook_module.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/hooks/local_hook.py` & `pdm_backend-2.3.0/tests/fixtures/hooks/local_hook.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/pyproject.toml` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-cextension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/pdm.lock` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/pyproject.toml` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/requirements.txt` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/pdm.lock` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/pyproject.toml` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/requirements.txt` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/requirements_simple.txt` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package-include/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/pdm.lock` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-tests/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/pyproject.toml` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package-with-tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package/pdm.lock` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package/requirements.txt` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-package/requirements_simple.txt` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-package/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml` & `pdm_backend-2.3.0/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/test_api.py` & `pdm_backend-2.3.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/test_file_finder.py` & `pdm_backend-2.3.0/tests/test_file_finder.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/test_hooks.py` & `pdm_backend-2.3.0/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/test_metadata.py` & `pdm_backend-2.3.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/test_utils.py` & `pdm_backend-2.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/tests/test_wheel.py` & `pdm_backend-2.3.0/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.1/PKG-INFO` & `pdm_backend-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pdm-backend
-Version: 2.2.1
+Version: 2.3.0
 Summary: The build backend used by PDM that supports latest packaging standards
 Keywords: packaging,PEP 517,build
 Author-Email: Frost Ming <me@frostming.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Homepage, https://github.com/pdm-project/pdm-backend
 Project-URL: Repository, https://github.com/pdm-project/pdm-backend
 Project-URL: Documentation, https://backend.pdm-project.org
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: importlib-metadata>=3.6; python_version < "3.10"
 Description-Content-Type: text/markdown
 
 # PDM-Backend
 
 The build backend used by [PDM] that supports latest packaging standards.
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: pdm-backend Version: 2.2.1 Summary: The build
+Metadata-Version: 2.1 Name: pdm-backend Version: 2.3.0 Summary: The build
 backend used by PDM that supports latest packaging standards Keywords:
 packaging,PEP 517,build Author-Email: Frost Ming
 frostming.com> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Project-URL:
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Project-URL:
 Homepage, https://github.com/pdm-project/pdm-backend Project-URL: Repository,
 https://github.com/pdm-project/pdm-backend Project-URL: Documentation, https://
-backend.pdm-project.org Requires-Python: >=3.7 Requires-Dist: importlib-
+backend.pdm-project.org Requires-Python: >=3.8 Requires-Dist: importlib-
 metadata>=3.6; python_version < "3.10" Description-Content-Type: text/markdown
 # PDM-Backend The build backend used by [PDM] that supports latest packaging
 standards. [![PyPI](https://img.shields.io/pypi/v/pdm-backend?label=PyPI)]
 (https://pypi.org/project/pdm-backend) [![Tests](https://github.com/pdm-
 project/pdm-backend/actions/workflows/ci.yml/badge.svg)](https://github.com/
 pdm-project/pdm-backend/actions/workflows/ci.yml) [![pre-commit.ci status]
 (https://results.pre-commit.ci/badge/github/pdm-project/pdm-backend/main.svg)]
```

