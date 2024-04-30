# Comparing `tmp/lephare-0.1.2.tar.gz` & `tmp/lephare-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lephare-0.1.2.tar", last modified: Sat Apr  6 06:55:39 2024, max compression
+gzip compressed data, was "lephare-0.1.4.tar", last modified: Tue Apr 30 19:03:46 2024, max compression
```

## Comparing `lephare-0.1.2.tar` & `lephare-0.1.4.tar`

### file list

```diff
@@ -1,142 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.749007 lephare-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-06 06:55:31.000000 lephare-0.1.2/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-06 06:55:31.000000 lephare-0.1.2/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-06 06:55:31.000000 lephare-0.1.2/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-06 06:55:31.000000 lephare-0.1.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.729007 lephare-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.729007 lephare-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.733007 lephare-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/workflows/compile-cpp.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-06 06:55:31.000000 lephare-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 06:55:31.000000 lephare-0.1.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-06 06:55:31.000000 lephare-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-06 06:55:31.000000 lephare-0.1.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-06 06:55:31.000000 lephare-0.1.2/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-06 06:55:31.000000 lephare-0.1.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-06 06:55:31.000000 lephare-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-06 06:55:39.749007 lephare-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-06 06:55:31.000000 lephare-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.733007 lephare-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.733007 lephare-0.1.2/docs/doxygen/
--rw-r--r--   0 runner    (1001) docker     (127)   112662 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/doxygen/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/keywords.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/legacy_install.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.733007 lephare-0.1.2/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Building_list_of_onesources.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Data_retrieval.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Example_SED_manipulation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Example_cosmo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16531 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Example_full_run.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Example_of_usage_of_magSvc.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.737007 lephare-0.1.2/docs/notebooks/data/
--rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/data/COSMOS.para
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/data/output.para
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.737007 lephare-0.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-04-06 06:55:31.000000 lephare-0.1.2/examples/color.py
--rw-r--r--   0 runner    (1001) docker     (127)    39348 2024-04-06 06:55:31.000000 lephare-0.1.2/examples/figuresLPP.py
--rw-r--r--   0 runner    (1001) docker     (127)    31984 2024-04-06 06:55:31.000000 lephare-0.1.2/examples/figuresLPZ.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-06 06:55:31.000000 lephare-0.1.2/examples/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-06 06:55:31.000000 lephare-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 06:55:39.749007 lephare-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-06 06:55:31.000000 lephare-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.729007 lephare-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.737007 lephare-0.1.2/src/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/_flt.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/_photoz.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/data_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/filterSvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/magSvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/mag_gal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/sedtolib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/zphota.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/src/lephare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/src/lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3003 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/PDF.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/PDF.h
--rw-r--r--   0 runner    (1001) docker     (127)    72114 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/SED.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/SED.h
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/SEDLib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/SEDLib.h
--rw-r--r--   0 runner    (1001) docker     (127)    18941 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/_bindings.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/cosmology.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/cosmology.h
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/ext.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/ext.h
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/ext_curv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/filter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/filter_extinc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20113 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/flt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/flt.h
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/globals.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/globals.h
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/keyword.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/keyword.h
--rw-r--r--   0 runner    (1001) docker     (127)    31597 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/mag.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/mag.h
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/mag_gal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/oneElLambda.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/oneElLambda.h
--rw-r--r--   0 runner    (1001) docker     (127)    80040 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/onesource.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/onesource.h
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/opa.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/opa.h
--rw-r--r--   0 runner    (1001) docker     (127)    61007 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/photoz_lib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/photoz_lib.h
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/sedtolib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/zphota.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)    41606 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/calzetti.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/tests/data/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/examples/COSMOS.para
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.729007 lephare-0.1.2/tests/data/filt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/tests/data/filt/subaru/
--rw-r--r--   0 runner    (1001) docker     (127)    25919 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/filt/subaru/IB527.pb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/tests/data/sed/
--rw-r--r--   0 runner    (1001) docker     (127)    54522 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/sed/WDgd71.sed.ext
--rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/sed/o5v.sed.ext
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/tau10.out
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/test_data_registry.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/test_file_names.list
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/tests/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_cosmology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_dataRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_keyword.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_oneElLambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_onesource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_sed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.970774 lephare-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 19:03:40.000000 lephare-0.1.4/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-30 19:03:40.000000 lephare-0.1.4/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 19:03:40.000000 lephare-0.1.4/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-30 19:03:40.000000 lephare-0.1.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.950774 lephare-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.950774 lephare-0.1.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.954774 lephare-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/workflows/compile-cpp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-30 19:03:40.000000 lephare-0.1.4/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-30 19:03:40.000000 lephare-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 19:03:40.000000 lephare-0.1.4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-30 19:03:40.000000 lephare-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-30 19:03:40.000000 lephare-0.1.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-30 19:03:40.000000 lephare-0.1.4/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-30 19:03:40.000000 lephare-0.1.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-30 19:03:40.000000 lephare-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-30 19:03:46.970774 lephare-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-30 19:03:40.000000 lephare-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.954774 lephare-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.954774 lephare-0.1.4/docs/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (127)   112662 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/doxygen/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/keywords.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/legacy_install.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.954774 lephare-0.1.4/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Building_list_of_onesources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Data_retrieval.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Example_SED_manipulation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Example_cosmo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Example_full_run.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Example_of_usage_of_magSvc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.958774 lephare-0.1.4/docs/notebooks/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/data/COSMOS.para
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks/data/output.para
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-30 19:03:40.000000 lephare-0.1.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.958774 lephare-0.1.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-04-30 19:03:40.000000 lephare-0.1.4/examples/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39348 2024-04-30 19:03:40.000000 lephare-0.1.4/examples/figuresLPP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31984 2024-04-30 19:03:40.000000 lephare-0.1.4/examples/figuresLPZ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-30 19:03:40.000000 lephare-0.1.4/examples/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-30 19:03:40.000000 lephare-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:03:46.970774 lephare-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-30 19:03:40.000000 lephare-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.946774 lephare-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.958774 lephare-0.1.4/src/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/_flt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/_photoz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/filterSvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/magSvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/mag_gal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/sedtolib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lephare/zphota.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.970774 lephare-0.1.4/src/lephare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 19:03:46.000000 lephare-0.1.4/src/lephare.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.966774 lephare-0.1.4/src/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3003 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/PDF.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/PDF.h
+-rw-r--r--   0 runner    (1001) docker     (127)    72115 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/SED.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/SED.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/SEDLib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/SEDLib.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/_bindings.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/cosmology.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/cosmology.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/ext.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/ext.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/ext_curv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/filter_extinc.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20186 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/flt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/flt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/globals.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/globals.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/keyword.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/keyword.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31598 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/mag.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/mag.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/mag_gal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/oneElLambda.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/oneElLambda.h
+-rw-r--r--   0 runner    (1001) docker     (127)    80072 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/onesource.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/onesource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/opa.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/opa.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61669 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/photoz_lib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/photoz_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/sedtolib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-04-30 19:03:40.000000 lephare-0.1.4/src/lib/zphota.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.966774 lephare-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.966774 lephare-0.1.4/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41606 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/calzetti.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.966774 lephare-0.1.4/tests/data/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/examples/COSMOS.para
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.950774 lephare-0.1.4/tests/data/filt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.966774 lephare-0.1.4/tests/data/filt/subaru/
+-rw-r--r--   0 runner    (1001) docker     (127)    25919 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/filt/subaru/IB527.pb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.966774 lephare-0.1.4/tests/data/sed/
+-rw-r--r--   0 runner    (1001) docker     (127)    54522 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/sed/WDgd71.sed.ext
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/sed/o5v.sed.ext
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/tau10.out
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/test_data_registry.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/test_file_names.list
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.970774 lephare-0.1.4/tests/data/vega/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24434 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/vega/SunLCB.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24455 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/data/vega/VegaLCB.sed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:03:46.970774 lephare-0.1.4/tests/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_data_retrieval_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_oneElLambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_onesource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-30 19:03:40.000000 lephare-0.1.4/tests/lephare/test_sed.py
```

### Comparing `lephare-0.1.2/.copier-answers.yml` & `lephare-0.1.4/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/.gitattributes` & `lephare-0.1.4/.gitattributes`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/.github/ISSUE_TEMPLATE/1-bug_report.md` & `lephare-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/.github/ISSUE_TEMPLATE/2-feature_request.md` & `lephare-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/.github/pull_request_template.md` & `lephare-0.1.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/.github/workflows/build-documentation.yml` & `lephare-0.1.4/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/.github/workflows/compile-cpp.yml` & `lephare-0.1.4/.github/workflows/compile-cpp.yml`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 jobs:
   build:
     name: Build C++
     runs-on: ${{ matrix.os }}
     strategy: 
       matrix:
-        os: [ubuntu-latest, macos-latest, macos-14]
+        os: [ubuntu-22.04, macos-12, macos-14]
 
     steps:
     - uses: actions/checkout@v4
       with:
         submodules: resursive
 
     - uses: maxim-lobanov/setup-xcode@v1
```

### Comparing `lephare-0.1.2/.github/workflows/pre-commit-ci.yml` & `lephare-0.1.4/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/.github/workflows/publish-to-pypi.yml` & `lephare-0.1.4/.github/workflows/publish-to-pypi.yml`

 * *Files 25% similar despite different names*

```diff
@@ -21,49 +21,49 @@
     name: Build wheels on ${{ matrix.os }}-${{ matrix.python_version}}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         include:
 
           # Linux 64 bit manylinux2014
-          - os: ubuntu-latest
+          - os: ubuntu-22.04
             python: 39
             platform_id: manylinux_x86_64
             manylinux_image: manylinux2014
             python_version: "3.9"
-          - os: ubuntu-latest
+          - os: ubuntu-22.04
             python: 310
             platform_id: manylinux_x86_64
             manylinux_image: manylinux2014
             python_version: "3.10"
-          - os: ubuntu-latest
+          - os: ubuntu-22.04
             python: 311
             platform_id: manylinux_x86_64
             manylinux_image: manylinux2014
             python_version: "3.11"
-          - os: ubuntu-latest
+          - os: ubuntu-22.04
             python: 312
             platform_id: manylinux_x86_64
             manylinux_image: manylinux2014
             python_version: "3.12"
 
           # MacOS x86_64
-          - os: macos-latest
+          - os: macos-12
             python: 39
             platform_id: macosx_x86_64
             python_version: "3.9"
-          - os: macos-latest
+          - os: macos-12
             python: 310
             platform_id: macosx_x86_64
             python_version: "3.10"
-          - os: macos-latest
+          - os: macos-12
             python: 311
             platform_id: macosx_x86_64
             python_version: "3.11"
-          - os: macos-latest
+          - os: macos-12
             python: 312
             platform_id: macosx_x86_64
             python_version: "3.12"
 
           # MacOS arm64
           - os: macos-14
             python: 39
```

### Comparing `lephare-0.1.2/.github/workflows/smoke-test.yml` & `lephare-0.1.4/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/.github/workflows/testing-and-coverage.yml` & `lephare-0.1.4/.github/workflows/testing-and-coverage.yml`

 * *Files 22% similar despite different names*

```diff
@@ -9,32 +9,46 @@
   pull_request:
     branches: [ main ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
+    env:
+      INCLUDE_COVERAGE: TRUE
     strategy:
       matrix:
         python-version: ['3.9', '3.10', '3.11', '3.12']
 
     steps:
     - uses: actions/checkout@v4
       with:
         submodules: recursive
+
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
+
     - name: Install dependencies
       run: |
         sudo apt-get update
+        sudo apt-get install -yy lcov
         python -m pip install --upgrade pip
-        pip install -e .[dev]
+        python -m pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+
     - name: Run unit tests with pytest
       run: |
-        python -m pytest tests --cov=lephare --cov-report=xml
+        python -m pytest -s tests --cov=lephare --cov-report=lcov
+
+    - name: Collect C++ coverage
+      run: |
+        lcov --output-file coverage.cpp --capture --directory build
+        lcov --output-file coverage.cpp --extract coverage.cpp $PWD/src/"*"
+        cat coverage.lcov coverage.cpp > coverage.txt
+
     - name: Upload coverage report to codecov
       uses: codecov/codecov-action@v4
       with:
+        files: coverage.txt
         token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `lephare-0.1.2/.gitignore` & `lephare-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/.pre-commit-config.yaml` & `lephare-0.1.4/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 repos:
     # Compare the local template version to the latest remote template version
     # This hook should always pass. It will print a message if the local version 
     # is out of date.
   - repo: https://github.com/lincc-frameworks/pre-commit-hooks
-    rev: v0.1.1
+    rev: v0.1.2
     hooks:
       - id: check-lincc-frameworks-template-version
         name: Check template version
         description: Compare current template version against latest
         verbose: true
     # Run clang-format to apply style rules to c++ code
   - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v18.1.1
+    rev: v18.1.3
     hooks:
     - id: clang-format
       name: clang-format
       types_or: [c++, c]
     # Clear output from jupyter notebooks so that only the input cells are committed.
   - repo: local
     hooks:
@@ -24,47 +24,47 @@
         description: Clear output from Jupyter notebooks.
         files: \.ipynb$
         stages: [commit]
         language: system
         entry: jupyter nbconvert --clear-output
     # Prevents committing directly branches named 'main' and 'master'.
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
       - id: no-commit-to-branch
         name: Prevent main branch commits
         description: Prevent the user from committing directly to the primary branch.
       - id: check-added-large-files
         name: Check for large files
         description: Prevent the user from committing very large files.
         args: ['--maxkb=500']
     # Verify that pyproject.toml is well formed
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.1
+    rev: v0.16
     hooks:
       - id: validate-pyproject
         name: Validate pyproject.toml
         description: Verify that pyproject.toml adheres to the established schema.
     # Verify that GitHub workflows are well formed
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.0
+    rev: 0.28.2
     hooks:
       - id: check-github-workflows
         args: ["--verbose"]
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.2.1
+    rev: v0.3.7
     hooks:
       - id: ruff
         name: Lint code using ruff; sort and organize imports 
         types_or: [ python, pyi ]
         args: ["--fix"]
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.2.1
+    rev: v0.3.7
     hooks:
       - id: ruff-format
         name: Format code using ruff
         types_or: [ python, pyi, jupyter ]
     # Make sure Sphinx can build the documentation while explicitly omitting 
     # notebooks from the docs, so users don't have to wait through the execution 
     # of each notebook or each commit. By default, these will be checked in the
```

### Comparing `lephare-0.1.2/.readthedocs.yml` & `lephare-0.1.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/.setup_dev.sh` & `lephare-0.1.4/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/CMakeLists.txt` & `lephare-0.1.4/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -60,14 +60,22 @@
     set(ENV{CPPFLAGS} "-I/usr/local/opt/llvm/include")
     set(CMAKE_CPP_COMPILER "clang++")
     set(CMAKE_C_COMPILER "clang")
 else()
     add_compile_options("-mno-vzeroupper" "-mavx2" "-floop-unroll-and-jam" )
 endif()
 
+# only set these flags if in `INCLUDE_COVERAGE` env var is set (to any value)
+if(DEFINED ENV{INCLUDE_COVERAGE})
+  message(STATUS "Building with code coverage enabled.")
+  SET(GCC_COVERAGE_COMPILE_FLAGS "-g -O0 -coverage -fprofile-arcs -ftest-coverage")
+  SET(GCC_COVERAGE_LINK_FLAGS    "-coverage -lgcov")
+  SET( CMAKE_CXX_FLAGS  "${CMAKE_CXX_FLAGS} ${GCC_COVERAGE_COMPILE_FLAGS}" )
+  SET( CMAKE_EXE_LINKER_FLAGS  "${CMAKE_EXE_LINKER_FLAGS} ${GCC_COVERAGE_LINK_FLAGS}" )
+endif()
 
 add_library(lepharelib STATIC ${SOURCES})
 find_package(OpenMP)
 if(OpenMP_CXX_FOUND)
     target_link_libraries(lepharelib PUBLIC OpenMP::OpenMP_CXX)
 endif()
```

### Comparing `lephare-0.1.2/LICENSE` & `lephare-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/PKG-INFO` & `lephare-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lephare
-Version: 0.1.2
+Version: 0.1.4
 Summary: LEPHARE photometric redshift estimator
 Home-page: https://gitlab.lam.fr/Galaxies/LEPHARE
 Author: Johann Cohen-Tanugi
-Author-email: Johann Cohen-Tanugi <johann.cohentanugi@gmail.com>
+Author-email: Stéphane Arnouts <stephane.arnouts@lam.fr>, Olivier Ilbert <olivier.ilbert@lam.fr>, Johann Cohen-Tanugi <johann.cohen-tanugi@in2p3.fr>, Raphael Shirley <rshirley@mpe.mpg.de>
 License: MIT License
         
         Copyright (c) 2023 Johann Cohen-Tanugi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -94,14 +94,15 @@
 >> conda activate <env_name>
 ```
 
 Once you have created a new environment, you can install this project for local
 development using the following commands:
 
 ```
+>> git submodule update --init --recursive
 >> pip install -e .'[dev]'
 >> pre-commit install
 >> conda install pandoc
 ```
 
 Notes:
 1. The single quotes around `'[dev]'` may not be required for your operating system.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lephare-0.1.2/README.md` & `lephare-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 >> conda activate <env_name>
 ```
 
 Once you have created a new environment, you can install this project for local
 development using the following commands:
 
 ```
+>> git submodule update --init --recursive
 >> pip install -e .'[dev]'
 >> pre-commit install
 >> conda install pandoc
 ```
 
 Notes:
 1. The single quotes around `'[dev]'` may not be required for your operating system.
@@ -63,8 +64,8 @@
 
 If using this code in scientific research please cite the following papers:
 
 
 This project was automatically generated using the LINCC-Frameworks 
 [python-project-template](https://github.com/lincc-frameworks/python-project-template).
 For more information about the project template see the 
-[documentation](https://lincc-ppt.readthedocs.io/en/latest/).
+[documentation](https://lincc-ppt.readthedocs.io/en/latest/).
```

### Comparing `lephare-0.1.2/docs/Makefile` & `lephare-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/docs/conf.py` & `lephare-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/docs/doxygen/Doxyfile` & `lephare-0.1.4/docs/doxygen/Doxyfile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/docs/index.rst` & `lephare-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/docs/keywords.rst` & `lephare-0.1.4/docs/keywords.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/docs/legacy_install.rst` & `lephare-0.1.4/docs/legacy_install.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/docs/notebooks/Building_list_of_onesources.ipynb` & `lephare-0.1.4/docs/notebooks/Building_list_of_onesources.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988425925925926%*

 * *Differences: {"'cells'": "{15: {'source': ['photz.run_photoz(photozlist[:10], a0, a1)']}, 16: {'source': ['t = "*

 * *            'photz.build_output_tables(photozlist[:10], para_out="./data/output.para", '*

 * *            'filename="toto.fits")\']}}'}*

```diff
@@ -254,25 +254,25 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d55446a1-2a6f-4376-9654-58e4f7895800",
             "metadata": {},
             "outputs": [],
             "source": [
-                "photz.run_photoz(photozlist[:100], a0, a1)"
+                "photz.run_photoz(photozlist[:10], a0, a1)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "3b61d3eb-f7c9-4e09-903a-3f2838e9d644",
             "metadata": {},
             "outputs": [],
             "source": [
-                "t = photz.build_output_tables(photozlist[:100], para_out=\"./data/output.para\", filename=\"toto.fits\")"
+                "t = photz.build_output_tables(photozlist[:10], para_out=\"./data/output.para\", filename=\"toto.fits\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d9ddffc7-e936-44f7-abf8-41087d176898",
             "metadata": {},
```

### Comparing `lephare-0.1.2/docs/notebooks/Data_retrieval.ipynb` & `lephare-0.1.4/docs/notebooks/Data_retrieval.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.950447849495701%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'In order to run lephare we must download some input "*

 * *            "data. \\n'), (3, '\\n'), (4, 'In this short notebook we a simple example which uses "*

 * *            'pooch to check if the required files have already been downloaded and to download '*

 * *            "them if not.')], delete: [2]}}, 8: {'id': '044c490f-c022-43b2-b12e-4e256b7050f6', "*

 * *            "'metadata': {replace: OrderedDict([('tags', [])])}, 'source': {insert: [(0, "*

 * *            "'lephare.data_retr […]*

```diff
@@ -3,15 +3,17 @@
         {
             "cell_type": "markdown",
             "id": "694d217b-ec1a-42b7-b8e6-dde10c3490b1",
             "metadata": {},
             "source": [
                 "# Data retrieval example\n",
                 "\n",
-                "In order to run lephare we must download some input data. In this short notebook we a simple example which uses pooch to check if the required files have already been downloaded and to download them if not."
+                "In order to run lephare we must download some input data. \n",
+                "\n",
+                "In this short notebook we a simple example which uses pooch to check if the required files have already been downloaded and to download them if not."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "571cf701-c5d0-44b6-b815-2e7bc038016d",
             "metadata": {
@@ -45,14 +47,29 @@
                 "            print(line)\n",
                 "        print(\"...\")\n",
                 "        for line in print_list[-number_lines:]:\n",
                 "            print(line)"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "3279e220",
+            "metadata": {},
+            "source": [
+                "## Getting a list of file names to download\n",
+                "\n",
+                "There are a couple ways to do this:\n",
+                "1. Using a list file, such as `QSO_MOD.list`\n",
+                "2. Using a list of target subdirectories, such as `[\"sed/GAL/\", \"filt/lsst/\"]`\n",
+                "\n",
+                "_(If you don't know what subset of data you need, we have included methods\n",
+                "    of downloading all of the data at once in the last section of this notebook.)_"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "9e5124e7-1a30-473a-82da-3914dd1014b3",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
@@ -88,92 +105,124 @@
                 "\n",
                 "# target_dirs = [\"sed/GAL/\", \"filt/lsst/\"]\n",
                 "# file_names = lephare.data_retrieval.filter_files_by_prefix(registry_file, target_dirs)\n",
                 "# partial_print(file_names, 4)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "99446731-e9c6-46a5-b7b3-63a683d37df8",
+            "cell_type": "markdown",
+            "id": "583a5bf5",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "# A third way to get data is to grab the zip file from OSF,\n",
-                "# which can be found in: https://osf.io/mvpks/files/osfstorage\n",
-                "\n",
-                "# TODO: extend this in a future PR"
+                "## Download the registry file\n",
+                "This will default to the default registry location at the default base url,\n",
+                "then output as the default registry file name, but these can be overridden\n",
+                "with the url and outfile keywords."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "044c490f-c022-43b2-b12e-4e256b7050f6",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "# Download the registry file\n",
-                "# This will default to the default registry location at the default base url,\n",
-                "# then output as the default registry file name, but these can be overridden\n",
-                "# with the url and outfile keywords\n",
+                "lephare.data_retrieval.download_registry_from_github()\n",
                 "\n",
-                "lephare.data_retrieval.download_registry_from_github()"
+                "# Or specify:\n",
+                "# lephare.data_retrieval.download_registry_from_github(url=\"my_url\", outfile=\"my_file\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "adc3fbd2",
+            "metadata": {},
+            "source": [
+                "## Download the data files"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f51d15c5-9d0b-480a-947f-8ba727f2f4a4",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "# Download the data files\n",
-                "\n",
-                "# The parameters here are already the default values in the function,\n",
-                "# but we explictly define them for examples' sake\n",
+                "# The parameters here are already the function's default values,\n",
+                "# but we explictly define them for examples' sake:\n",
                 "base_url = lephare.data_retrieval.DEFAULT_BASE_DATA_URL\n",
                 "registry_file = lephare.data_retrieval.DEFAULT_REGISTRY_FILE\n",
-                "data_path = lephare.data_retrieval.DEFAULT_LOCAL_DATA_PATH\n",
+                "data_path = lephare.LEPHAREDIR\n",
                 "\n",
                 "retriever = lephare.data_retrieval.make_retriever(\n",
                 "    base_url=base_url, registry_file=registry_file, data_path=data_path\n",
                 ")\n",
                 "\n",
-                "lephare.data_retrieval.download_all_files(retriever, file_names, ignore_registry=False)"
+                "lephare.data_retrieval.download_all_files(retriever, file_names)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8ba1d5c5-09ea-48b8-b9f0-85019728466c",
+            "id": "65ce83b2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "base_url = lephare.data_retrieval.DEFAULT_BASE_DATA_URL\n",
-                "registry_file = lephare.data_retrieval.DEFAULT_REGISTRY_FILE\n",
-                "data_path = lephare.LEPHAREDIR\n",
-                "base_url, registry_file, data_path"
+                "# If you run into problems with the registry, you can disable the requirement\n",
+                "# by setting ignore_registry=True:\n",
+                "\n",
+                "# lephare.data_retrieval.download_all_files(retriever, file_names, ignore_registry=True)\n",
+                "\n",
+                "# (Note that this is not recommended, as pooch will be unable to verify whether\n",
+                "# or not your local files are up-to-date, and each will be re-downloaded.)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "c228e762",
+            "metadata": {},
+            "source": [
+                "## If you don't know what subset you need and want to get all the data at once"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fb792b02-ec35-4dbd-b7b5-b8ea74fdd721",
+            "id": "99446731-e9c6-46a5-b7b3-63a683d37df8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "retriever = lephare.data_retrieval.make_retriever(\n",
-                "    base_url=base_url, registry_file=registry_file, data_path=data_path\n",
-                ")\n",
+                "# Run get_auxiliary_data with no keymap set to clone the entire data repository\n",
+                "# to the default local data directory:\n",
                 "\n",
-                "lephare.data_retrieval.download_all_files(retriever, file_names, ignore_registry=False)"
+                "# data_retrieval.get_auxiliary_data()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "66042a05",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Or, grab the zip file from OSF: https://osf.io/mvpks/files/osfstorage"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "f2d481fc",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Or, clone the data repo: https://github.com/lephare-photoz/lephare-data"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -185,13 +234,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.6"
+            "version": "3.10.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lephare-0.1.2/docs/notebooks/Example_SED_manipulation.ipynb` & `lephare-0.1.4/docs/notebooks/Example_SED_manipulation.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/docs/notebooks/Example_cosmo.ipynb` & `lephare-0.1.4/docs/notebooks/Example_cosmo.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/docs/notebooks/Example_full_run.ipynb` & `lephare-0.1.4/docs/notebooks/Example_full_run.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971992924528301%*

 * *Differences: {"'cells'": "{42: {'source': {insert: [(1, 'for i in range(10):\\n')], delete: [1]}}, 44: "*

 * *            "{'source': {insert: [(0, 'photz.run_photoz(photozlist[:10], a0, a1)\\n')], delete: "*

 * *            "[0]}}, 46: {'source': ['t = photz.build_output_tables(photozlist[:10], para_out=None, "*

 * *            'filename="outputpython.fits")\']}, 50: {\'source\': {insert: [(2, '*

 * *            "'photz.write_outputs(photozlist[:10], int(time.time()))')], delete: [2]}}, insert: "*

 * *            "[(48, OrderedDict([('cell_typ […]*

```diff
@@ -462,15 +462,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "23e36e5d-a503-4bc8-bf64-0e808e72d06d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "photozlist = []\n",
-                "for i in range(100):\n",
+                "for i in range(10):\n",
                 "    oneObj = lp.onesource(i, photz.gridz)\n",
                 "    oneObj.readsource(str(id[i]), fluxes[i, :], efluxes[i, :], int(context[i]), zspec[i], \" \")\n",
                 "    photz.prep_data(oneObj)\n",
                 "    photozlist.append(oneObj)\n",
                 "print(\"Number of sources to be analysed: \", len(srclist))"
             ]
         },
@@ -485,15 +485,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cce71934-cc95-4364-9a4a-f87200ba573f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "photz.run_photoz(photozlist[:100], a0, a1)\n",
+                "photz.run_photoz(photozlist[:10], a0, a1)\n",
                 "# If adaption of the zero-points is turned off\n",
                 "# photz.run_photoz(photozlist[:100], [],[] )"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f1b12906-006a-48ae-b6ef-f9cc8bbaac5d",
@@ -505,28 +505,38 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a1ed1d5b-5bd9-4e01-b150-d0b295a929ce",
             "metadata": {},
             "outputs": [],
             "source": [
-                "t = photz.build_output_tables(photozlist[:100], para_out=None, filename=\"outputpython.fits\")"
+                "t = photz.build_output_tables(photozlist[:10], para_out=None, filename=\"outputpython.fits\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6a47dedd-414c-4bfd-ae20-de3b4021badf",
             "metadata": {},
             "outputs": [],
             "source": [
                 "t[:5]"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "d7e7c675",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "t[:5]"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "id": "e8969641-6110-4d8a-88cc-72aebf9e6619",
             "metadata": {},
             "source": [
                 "Create one ascii file per object to produce the best-fit template plot"
             ]
         },
@@ -535,15 +545,15 @@
             "execution_count": null,
             "id": "39ad9dea-b259-41b9-a47e-4d0155b17cd6",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import time\n",
                 "\n",
-                "photz.write_outputs(photozlist[:100], int(time.time()))"
+                "photz.write_outputs(photozlist[:10], int(time.time()))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5192bcfe-a8ee-44b8-a59f-06c90b1e90f3",
             "metadata": {},
             "source": [
```

### Comparing `lephare-0.1.2/docs/notebooks/Example_of_usage_of_magSvc.ipynb` & `lephare-0.1.4/docs/notebooks/Example_of_usage_of_magSvc.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/docs/notebooks/README.md` & `lephare-0.1.4/docs/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb` & `lephare-0.1.4/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/docs/notebooks/data/COSMOS.para` & `lephare-0.1.4/docs/notebooks/data/COSMOS.para`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 #-------------------      From GALAXY LIBRARY            ------------------------------
 GAL_LIB_IN	LIB_CE 	        # Input GALAXY LIBRARY   (in $ZPHOTWORK/lib_bin/*)
 GAL_LIB_OUT	CE_COSMOS	# Output GALAXY LIBRARY  (-> $ZPHOTWORK/lib_mag/*) 
 #
 #------------------   MAG + Z_STEP + COSMO + EXTINCTION   -----------------------------
 MAGTYPE         AB		# Magnitude type (AB or VEGA)
 ZGRID_TYPE      0               # Define the kind of redshift grid (0: linear ; 1: dz*(1+z)) 
-Z_STEP 		0.01,0.,7. 	# dz, zmin, zmax 
+Z_STEP 		0.1,0.,5. 	# dz, zmin, zmax VERY SPARSE FOR EXAMPLE ONLY
 COSMOLOGY	70,0.3,0.7	# H0,om0,lbd0    (if lb0>0->om0+lbd0=1)
 MOD_EXTINC 	0,0		# model range for extinction 
 EXTINC_LAW	SMC_prevot.dat,SB_calzetti.dat,SB_calzetti_bump1.dat,SB_calzetti_bump2.dat	# ext. law (in  $ZPHOTDIR/ext/*)
 EB_V            0.,0.05,0.1,0.15,0.2,0.25,0.3,0.35,0.4,0.5 # E(B-V) (<50 values)
 EM_LINES        EMP_UV          # [NO/EMP_UV/EMP_SFR/PHYS] choice between emission line prescription  
 EM_DISPERSION   0.5,0.75,1.,1.5,2. # Dispersion allowed in the emission line flux factor
 ADD_DUSTEM      NO               # Add the dust emission in templates when missing
```

### Comparing `lephare-0.1.2/docs/notebooks/data/output.para` & `lephare-0.1.4/docs/notebooks/data/output.para`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/docs/notebooks.rst` & `lephare-0.1.4/docs/notebooks.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/examples/color.py` & `lephare-0.1.4/examples/color.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/examples/figuresLPP.py` & `lephare-0.1.4/examples/figuresLPP.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/examples/figuresLPZ.py` & `lephare-0.1.4/examples/figuresLPZ.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/examples/spec.py` & `lephare-0.1.4/examples/spec.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/pyproject.toml` & `lephare-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [project]
 name = "lephare"
 license = {file = "LICENSE"}
 readme = "README.md"
 description = "LEPHARE photometric redshift estimator"
 authors = [
-    { name = "Johann Cohen-Tanugi", email = "johann.cohentanugi@gmail.com" }
+    { name = "Stéphane Arnouts", email = "stephane.arnouts@lam.fr" },
+    { name = "Olivier Ilbert", email = "olivier.ilbert@lam.fr" },
+    { name = "Johann Cohen-Tanugi", email = "johann.cohen-tanugi@in2p3.fr" },
+    { name = "Raphael Shirley", email = "rshirley@mpe.mpg.de" }
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lephare-0.1.2/setup.py` & `lephare-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
         if platform.system() == "Windows":
             cmake_args += [f"-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_{cfg.upper()}={extdir}"]
             if sys.maxsize > 2**32:
                 cmake_args += ["-A", "x64"]
             build_args += ["--", "/m"]
         else:
-            cmake_args += ["-DCMAKE_BUILD_TYPE=" + cfg]
+            cmake_args += ["-DCMAKE_BUILD_TYPE:STRING=" + cfg]
             build_args += ["--", "-j2"]
 
         env = os.environ.copy()
         env["CXXFLAGS"] = '{} -DVERSION_INFO=\\"{}\\"'.format(
             env.get("CXXFLAGS", ""), self.distribution.get_version()
         )
         if not os.path.exists(self.build_temp):
```

### Comparing `lephare-0.1.2/src/lephare/__init__.py` & `lephare-0.1.4/src/lephare/__init__.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lephare/_flt.py` & `lephare-0.1.4/src/lephare/_flt.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lephare/_pdf.py` & `lephare-0.1.4/src/lephare/_pdf.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lephare/_photoz.py` & `lephare-0.1.4/src/lephare/_photoz.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lephare/_spec.py` & `lephare-0.1.4/src/lephare/_spec.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lephare/_utils.py` & `lephare-0.1.4/src/lephare/_utils.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lephare/data_manager.py` & `lephare-0.1.4/src/lephare/data_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,31 +43,37 @@
         self.lephare_work_dir = os.getenv("LEPHAREWORK", None)
 
         # If LEPHAREWORK is not set then set to default and make directories
         if self.lephare_work_dir is None:
             # get <default_cache> locations
             default_os_cache = user_cache_dir("lephare", ensure_exists=True)
 
-            # create a runs directory in the default cache locations
-            os.makedirs(f"{default_os_cache}/runs", exist_ok=True)
-
-            # create a timestamped directory under runs
-            now = datetime.datetime.now().strftime("%Y%m%dT%H%M%S")
-            run_directory = f"{default_os_cache}/runs/{now}"
-            os.makedirs(run_directory, exist_ok=True)
-
-            # create the subdirectories in the new run directory
-            self.create_work_subdirectories(run_directory)
-
-            # create a symlink between <default_cache>/work and the timestamped directory
+            # Location of work linked dir <default_cache>/work and the timestamped directory
             symlink_work_directory = f"{default_os_cache}/work"
+
             # first remove the symlink if it already exists
             if os.path.islink(symlink_work_directory):
-                os.unlink(symlink_work_directory)
-            os.symlink(run_directory, symlink_work_directory)
+                # os.unlink(symlink_work_directory) #We no longer make a new link
+                print(
+                    f"""Default work cache at {symlink_work_directory}
+                    is already linked. This is linked to the run directory:
+                    {os.readlink(symlink_work_directory)}"""
+                )
+            else:
+                # create a runs directory in the default cache locations
+                os.makedirs(f"{default_os_cache}/runs", exist_ok=True)
+
+                # create a timestamped directory under runs
+                now = datetime.datetime.now().strftime("%Y%m%dT%H%M%S")
+                run_directory = f"{default_os_cache}/runs/{now}"
+                os.makedirs(run_directory, exist_ok=True)
+
+                # create the subdirectories in the new run directory
+                self.create_work_subdirectories(run_directory)
+                os.symlink(run_directory, symlink_work_directory)
 
             # set the LEPHAREWORK environment variable to the <default_cache>/work symlink
             os.environ["LEPHAREWORK"] = symlink_work_directory
 
             # set the instance variable to the <default_cache>/work symlink
             self.lephare_work_dir = symlink_work_directory
         else:
```

### Comparing `lephare-0.1.2/src/lephare/data_retrieval.py` & `lephare-0.1.4/src/lephare/data_retrieval.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,18 @@
 import pooch
 import requests
 
 from lephare import LEPHAREDIR
 
 DEFAULT_BASE_DATA_URL = "https://raw.githubusercontent.com/lephare-photoz/lephare-data/main/"
 DEFAULT_REGISTRY_FILE = "data_registry.txt"
+DEFAULT_LOCAL_DATA_PATH = LEPHAREDIR
 
-#! Replace DEFAULT_LOCAL_DATA_PATH with the following:
-# from lephare import data_marshaller
-# DEFAULT_LOCAL_DATA_PATH = data_marshaller.get_data_path()
-#  likely something like: ~/Library/Caches/lephare/data/
-#  Note that we can use pooch.os_cache("lephare") to create a directory in the
-#  default cache location and return its path
-DEFAULT_LOCAL_DATA_PATH = "./data"
-
+# If a file is not downloaded the first time, retry this many times
+MAX_RETRY_ATTEMPTS = 2
 
 __all__ = [
     "download_all_files",
     "download_file",
     "download_registry_from_github",
     "filter_files_by_prefix",
     "make_default_retriever",
@@ -54,42 +49,88 @@
     with open(file_path, "r", encoding="utf-8") as file:
         for line in file:
             if any(line.startswith(prefix) for prefix in target_prefixes):
                 matching_lines.append(line.split(" ")[0].strip())
     return matching_lines
 
 
+def _check_registry_is_latest_version(remote_registry_url, local_registry_file):
+    """Checks whether the local registry file is the latest version compared to a remote registry.
+
+    Parameters
+    ----------
+    remote_registry_url : str
+        The URL to the remote registry file, used to construct the URL to fetch the remote hash.
+    local_registry_file : str
+        The path to the local registry file whose up-to-date status is to be checked.
+
+    Returns
+    -------
+    bool
+        Returns True if the local registry file is up to date, otherwise False.
+
+    Notes
+    -----
+    We make the assumption that the hash file for the registry will be stored in
+    the same directory as the registry file, with the same name (sans extension)
+    plus "_hash.sha256".
+
+    Raises
+    ------
+    Exception
+        If there is any problem fetching the registry hash file, including network issues,
+        server errors, or other HTTP errors.
+    """
+    local_registry_hash = pooch.file_hash(local_registry_file, alg="sha256")
+    remote_hash_url = os.path.splitext(remote_registry_url)[0] + "_hash.sha256"
+
+    remote_hash_response = requests.get(remote_hash_url, timeout=60)
+    remote_hash_response.raise_for_status()  # Raise exceptions for non-200 status codes
+
+    return remote_hash_response.text.strip() == local_registry_hash
+
+
 def download_registry_from_github(url="", outfile=""):
     """Fetch the contents of a file from a GitHub repository.
 
     Parameters
     ----------
     url : str
-        The URL of the registry file. Defaults to a "data-registry.txt" file at
+        The URL of the registry file. Defaults to a "data_registry.txt" file at
         DEFAULT_BASE_DATA_URL.
     outfile : str
         The path where the file will be saved. Defaults to DEFAULT_REGISTRY_FILE.
 
     Raises
     ------
     Exception
-        If the file cannot be fetched from the URL.
+        If there is any problem fetching the registry hash file or full registry file,
+        including network issues, server errors, or other HTTP errors.
     """
+    remote_registry_name = "data_registry.txt"
+
+    # Assign defaults if keywords left blank
     if url == "":
-        url = urljoin(DEFAULT_BASE_DATA_URL, "data-registry.txt")
+        url = urljoin(DEFAULT_BASE_DATA_URL, remote_registry_name)
     if outfile == "":
         outfile = DEFAULT_REGISTRY_FILE
 
-    response = requests.get(url, timeout=60)
-    if response.status_code == 200:
-        with open(outfile, "w", encoding="utf-8") as file:
-            file.write(response.text)
-        print(f"File downloaded and saved as {outfile}")
-    else:
-        raise requests.exceptions.HTTPError(f"Failed to fetch file: {response.status_code}")
+    # If local registry hash matches remote hash, our registry is already up-to-date:
+    if os.path.isfile(outfile) and _check_registry_is_latest_version(url, outfile):
+        print(f"Local registry file is up to date: {outfile}")
+        return
+
+    # Download the registry file
+    response = requests.get(url, timeout=120)
+    response.raise_for_status()  # Raise exceptions for non-200 status codes
+
+    with open(outfile, "w", encoding="utf-8") as file:
+        file.write(response.text)
+
+    print(f"Registry file downloaded and saved as {outfile}.")
 
 
 def read_list_file(list_file, prefix=""):
     """Reads file names from a list file and returns a list of file paths.
 
     Parameters
     ----------
@@ -183,17 +224,15 @@
     """Create directories for the given file names if they do not already exist.
 
     This function is for thread safety when downloading files in parallel.
 
     Parameters
     ----------
     file_names : list of str
-        List of file names with relative paths.
-    base_path : str
-        Path to LEPHAREDIR if not current working directory.
+        List of file names with absolute paths.
     """
     unique_directories = set(
         os.path.dirname(file_name) for file_name in file_names if os.path.dirname(file_name)
     )
     for directory in unique_directories:
         if not os.path.exists(directory):
             os.makedirs(directory)
@@ -225,33 +264,35 @@
             fname=file_name,
             path=retriever.path,
         )
     else:
         return retriever.fetch(file_name)
 
 
-def download_all_files(retriever, file_names, ignore_registry=False):
+def download_all_files(retriever, file_names, ignore_registry=False, retry=MAX_RETRY_ATTEMPTS):
     """Download all files in the given list using the retriever.
 
     Parameters
     ----------
     retriever : pooch.Pooch
         The retriever object for downloading files.
     file_names : list of str
         List of file names to download.
     ignore_registry : bool
         If True, download the files without checking their hashes against the registry.
-
-    Returns
-    -------
-    list of str
-        List of paths to the downloaded files.
+    retry : int
+        Number of times to retry downloading a file if first attempt fails.
     """
+    if len(file_names) == 0:
+        print("Download all files called for list of 0 files; done.")
+        return
+
     # First make directories, for thread safety
-    _create_directories_from_files(file_names)
+    absolute_file_names = [os.path.join(retriever.path, file_name) for file_name in file_names]
+    _create_directories_from_files(absolute_file_names)
 
     # Now the downloading
     print(f"Checking/downloading {len(file_names)} files...")
     with concurrent.futures.ThreadPoolExecutor() as executor:
         download_fn = partial(download_file, retriever, ignore_registry=ignore_registry)
         futures = [executor.submit(download_fn, file_name) for file_name in file_names]
 
@@ -265,16 +306,19 @@
                 print(f"Future completed with a timeout exception: {e}")
             except Exception as e:
                 print(f"Future completed with an exception: {e}")
 
         print(f"{len(completed_futures)} completed.")
 
     # Finish with some checks on our downloaded files
-    absolute_file_names = [os.path.join(retriever.path, file_name) for file_name in file_names]
-    _check_downloaded_files(absolute_file_names, completed_futures)
+    all_files_present = _check_downloaded_files(absolute_file_names, completed_futures)
+
+    if not all_files_present and retry > 0:
+        print("Retrying download for missing files...")
+        download_all_files(retriever, file_names, ignore_registry=ignore_registry, retry=retry - 1)
 
 
 def _check_downloaded_files(file_names, completed_futures):
     """Check if all files have been downloaded successfully and are not empty.
 
     Parameters
     ----------
@@ -326,15 +370,15 @@
     base_url : str
         Url to overwrite default base.
     """
     if base_url is None:
         base_url = DEFAULT_BASE_DATA_URL
     required_files = []
     # We always need alloutputkeys.txt
-    # required_files += ["alloutputkeys.txt"]
+    required_files += ["alloutputkeys.txt"]
     # Opacity always required
     opa_list = ["opa/OPACITY.dat"] + [f"opa/tau{i:02d}.out" for i in np.arange(81)]
     required_files += opa_list
     # vega always required
     vega_list = [
         "vega/BD+17.sed",
         "vega/BD+17o4708.sed",
@@ -381,30 +425,29 @@
         The config dictionary.
     additional_files : list
         Any additional files to be downloaded from the auxiliary file repo.
     """
     # Get the registry file
     download_registry_from_github()
     base_url = DEFAULT_BASE_DATA_URL
+    repo_name = "lephare-data"
+    repo_url = f"https://github.com/lephare-photoz/{repo_name}"
     registry_file = DEFAULT_REGISTRY_FILE
     data_path = lephare_dir
     if keymap is None:
         # Assume if filt is present assume everything is.
         if os.path.isdir(f"{lephare_dir}/filt"):
             warnings.warn(
                 "Some data appears present. Not downloading."
                 "Consider setting a keymap to download a subset."
             )
         else:
             # Get the full repository
-            print("Downloading all auxiliary data (~1.5Gb) to {lephare_dir}.")
-            print(f"Getting data from {base_url}.")
-            os.system(f"git clone {base_url}")
-            os.system(f"mv LEPHARE-data/* {lephare_dir}")
+            print(f"Downloading all auxiliary data (~1.5Gb) to {lephare_dir}.")
+            print(f"Getting data from {repo_url}.")
+            os.system(f"git clone {repo_url} {lephare_dir}")
     else:
         retriever = make_retriever(base_url=base_url, registry_file=registry_file, data_path=data_path)
         file_list = config_to_required_files(keymap)
         download_all_files(retriever, file_list, ignore_registry=False)
-        # TODO! This will be deprecated when alloutputkeys.txt is added to the registry:
-        download_file(retriever, "alloutputkeys.txt", ignore_registry=True)
     if additional_files is not None:
         download_all_files(retriever, additional_files, ignore_registry=False)
```

### Comparing `lephare-0.1.2/src/lephare/filter.py` & `lephare-0.1.4/src/lephare/filter.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lephare/filterSvc.py` & `lephare-0.1.4/src/lephare/filterSvc.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import os
 import xml.dom.minidom
 
 import requests
 import yaml
 
-from . import LEPHAREDIR, flt
+from lephare import LEPHAREDIR
+from lephare._lephare import check_first_char, flt
 
 __all__ = [
     "FilterSvc",
 ]
 
 SVO_URL = "http://svo2.cab.inta-csic.es/theory/fps"
 
@@ -72,15 +73,15 @@
         keywords = ["FILTER_REP", "FILTER_LIST", "TRANS_TYPE", "FILTER_CALIB", "FILTER_FILE"]
         keymap = {}
         with open(config_file) as fstream:
             count = 0
             while count < len(keywords):
                 line = fstream.readline()
                 for key in keywords:
-                    if key in line:
+                    if key in line and check_first_char(line):
                         keymap[key] = line.split()[1]
                         count += 1
         keymap["FILTER_REP"] = keymap["FILTER_REP"].replace("$LEPHAREDIR", LEPHAREDIR)
 
         filter_list = keymap["FILTER_LIST"].split(",")
         filter_calib = keymap["FILTER_CALIB"].split(",")
         filter_trans = keymap["TRANS_TYPE"].split(",")
@@ -162,18 +163,21 @@
         Returns
         -------
         res : `lephare.flt`
             Filter in native lephare format.
         """
         try:
             query = f"{SVO_URL}/fps.php?PhotCalID={filter_id}/{system}"
-            r = requests.get(query)
+            r = requests.get(query, timeout=5)
         except ConnectionRefusedError:
             print(f"request {query} failed due to failure to connect to the server.")
             return None
+        except requests.ConnectTimeout:
+            print("Timeout on SVO server")
+            return None
         try:
             dd = xml.dom.minidom.parseString(r.content)
         except xml.parsers.expat.ExpatError:
             print("SVO server down")
             return None
         # assert query ok
         for info in dd.getElementsByTagName("INFO"):
```

### Comparing `lephare-0.1.2/src/lephare/magSvc.py` & `lephare-0.1.4/src/lephare/magSvc.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lephare/mag_gal.py` & `lephare-0.1.4/src/lephare/mag_gal.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lephare/runner.py` & `lephare-0.1.4/src/lephare/runner.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lephare/sedtolib.py` & `lephare-0.1.4/src/lephare/sedtolib.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lephare/zphota.py` & `lephare-0.1.4/src/lephare/zphota.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lephare.egg-info/PKG-INFO` & `lephare-0.1.4/src/lephare.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lephare
-Version: 0.1.2
+Version: 0.1.4
 Summary: LEPHARE photometric redshift estimator
 Home-page: https://gitlab.lam.fr/Galaxies/LEPHARE
 Author: Johann Cohen-Tanugi
-Author-email: Johann Cohen-Tanugi <johann.cohentanugi@gmail.com>
+Author-email: Stéphane Arnouts <stephane.arnouts@lam.fr>, Olivier Ilbert <olivier.ilbert@lam.fr>, Johann Cohen-Tanugi <johann.cohen-tanugi@in2p3.fr>, Raphael Shirley <rshirley@mpe.mpg.de>
 License: MIT License
         
         Copyright (c) 2023 Johann Cohen-Tanugi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -94,14 +94,15 @@
 >> conda activate <env_name>
 ```
 
 Once you have created a new environment, you can install this project for local
 development using the following commands:
 
 ```
+>> git submodule update --init --recursive
 >> pip install -e .'[dev]'
 >> pre-commit install
 >> conda install pandoc
 ```
 
 Notes:
 1. The single quotes around `'[dev]'` may not be required for your operating system.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lephare-0.1.2/src/lephare.egg-info/SOURCES.txt` & `lephare-0.1.4/src/lephare.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -106,15 +106,19 @@
 tests/data/tau10.out
 tests/data/test_data_registry.txt
 tests/data/test_file_names.list
 tests/data/examples/COSMOS.para
 tests/data/filt/subaru/IB527.pb
 tests/data/sed/WDgd71.sed.ext
 tests/data/sed/o5v.sed.ext
+tests/data/vega/SunLCB.sed
+tests/data/vega/VegaLCB.sed
 tests/lephare/test_cosmology.py
-tests/lephare/test_dataRetrieval.py
 tests/lephare/test_data_manager.py
+tests/lephare/test_data_retrieval.py
+tests/lephare/test_data_retrieval_registry.py
+tests/lephare/test_filter.py
 tests/lephare/test_globals.py
 tests/lephare/test_keyword.py
 tests/lephare/test_oneElLambda.py
 tests/lephare/test_onesource.py
 tests/lephare/test_sed.py
```

### Comparing `lephare-0.1.2/src/lib/Makefile` & `lephare-0.1.4/src/lib/Makefile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/PDF.cpp` & `lephare-0.1.4/src/lib/PDF.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/PDF.h` & `lephare-0.1.4/src/lib/PDF.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/SED.cpp` & `lephare-0.1.4/src/lib/SED.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
   if (!ssed) {
     throw invalid_argument("Can't open SED file " + sedFile);
   }
 
   // Take the stream line by line
   while (getline(ssed, lit)) {
     // If the first character of the line is not #
-    if (test_first_char(lit)) {
+    if (check_first_char(lit)) {
       // put the line into the stream ss again
       stringstream ss(lit);
 
       // fill the lambda/trans values of the SED
       double l, v;
       ss >> l;
       ss >> v;
```

### Comparing `lephare-0.1.2/src/lib/SED.h` & `lephare-0.1.4/src/lib/SED.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/SEDLib.cpp` & `lephare-0.1.4/src/lib/SEDLib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/SEDLib.h` & `lephare-0.1.4/src/lib/SEDLib.h`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
   if (!smod) {
     throw invalid_argument("Can't open mod file " + modList);
   }
 
   // Take the template list line by line
   while (getline(smod, lit)) {
     // If the first character of the line is not #
-    if (test_first_char(lit)) {
+    if (check_first_char(lit)) {
       // put the line into the stream ss again
       stringstream ss(lit);
 
       // Read the name of the SED and the format which need to be used to read
       // it
       ss >> nameSED;
       formatSED = 'A';  // Default: ascii
@@ -293,15 +293,15 @@
       cerr << "Can't open age file " << ageFile << endl;
       cerr << "No selection by age. " << endl;
       // throw "Failing opening ",ageFile.c_str();
     }
 
     while (getline(sage, lit)) {
       // If the first character of the line is not #
-      if (test_first_char(lit)) {
+      if (check_first_char(lit)) {
         // put the line into the stream ss again
         stringstream ss(lit);
         ss >> dage;
 
         // fill the age vector in Gyr.
         ageSel.push_back(dage * 1.e9);
       }
```

### Comparing `lephare-0.1.2/src/lib/_bindings.cc` & `lephare-0.1.4/src/lib/_bindings.cc`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,15 @@
 
   //   ;
 
   //   ;
 
   /******** FUNCTIONS IN GLOBALS.H *********/
   mod.def("get_lephare_env", &get_lephare_env);
-  mod.def("test_first_char", &test_first_char);
+  mod.def("check_first_char", &check_first_char);
   mod.def("blackbody", &blackbody);
   mod.def("CHECK_CONTEXT_BIT", &CHECK_CONTEXT_BIT);
   mod.def("POW10D", &POW10D);
   mod.def("POW10DSLOW", &POW10DSLOW);
   mod.def("LOG10D_SLOW", &LOG10D_SLOW);
   mod.def("LOG10D_FAST", &LOG10D_FAST);
   mod.def("mag2flux", &mag2flux);
```

### Comparing `lephare-0.1.2/src/lib/cosmology.cpp` & `lephare-0.1.4/src/lib/cosmology.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/cosmology.h` & `lephare-0.1.4/src/lib/cosmology.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/ext.cpp` & `lephare-0.1.4/src/lib/ext.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   if (!sext) {
     throw invalid_argument("Can't open file " + extFile);
   }
 
   // Take the stream line by line
   while (getline(sext, lit)) {
     // If the first character of the line is not #
-    if (test_first_char(lit)) {
+    if (check_first_char(lit)) {
       // put the line into the stream ss again
       stringstream ss(lit);
 
       // fill the lambda/trans values of the SED
       double l, v;
       ss >> l;
       ss >> v;
```

### Comparing `lephare-0.1.2/src/lib/ext.h` & `lephare-0.1.4/src/lib/ext.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/ext_curv.cpp` & `lephare-0.1.4/src/lib/ext_curv.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/filter.cpp` & `lephare-0.1.4/src/lib/filter.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/filter_extinc.cpp` & `lephare-0.1.4/src/lib/filter_extinc.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/flt.cpp` & `lephare-0.1.4/src/lib/flt.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 /*
 
   10/11/14
   Implementation of function for the "flt" class
 
 */
 
+#include <unistd.h>  //posix interface, prooviding path access method
+
 #include <algorithm>  // sort
 #include <cmath>      // for the log
 #include <fstream>    // print output file
 #include <iomanip>    // std::setprecision
 #include <iostream>   // print standard file
 #include <sstream>
 #include <string>
@@ -34,15 +36,15 @@
   if (!(sflt)) {
     throw invalid_argument("Can't open file " + fltFile);
   }
 
   // Take the stream line by line
   while (getline(sflt, lit)) {
     // If the first character of the line is not #
-    if (test_first_char(lit)) {
+    if (check_first_char(lit)) {
       // put the line into the stream ss again
       stringstream ss(lit);
 
       // fill the lambda/trans values into one element
       double l, v;
       ss >> l;  // 1 col: lambda
       ss >> v;  // 2 column: transmission
@@ -568,15 +570,15 @@
   string fltfile = lepharework + "/filt/" + filtFile + ".dat";
   ifstream sfltIn;
   sfltIn.open(fltfile.c_str());
 
   // Read each line of the doc file
   while (getline(stfltdoc, line)) {
     // If the first character of the line is not #
-    if (test_first_char(line)) {
+    if (check_first_char(line)) {
       // Transfer the line content to line_stream.
       stringstream line_stream(line);
 
       // Generate one object "flt"
       flt oneFilt;
 
       // read informations on this filter and fill the object flt
```

### Comparing `lephare-0.1.2/src/lib/flt.h` & `lephare-0.1.4/src/lib/flt.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/globals.cpp` & `lephare-0.1.4/src/lib/globals.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 13/12/2013
 Function to test if the first character of a string corresponds to a comment
 String starting with # or ! or - are considered as comment
 If the string has a length of 0, return also false
 input: string to analyse
 output: boolean
 */
-bool test_first_char(string maligne) {
+bool check_first_char(string maligne) {
   for (string::const_iterator it = maligne.begin(); it != maligne.end(); it++) {
     if (*it == ' ' || *it == '\t') {
       continue;
     } else if (*it != '#' && *it != '!') {
       return true;
     } else {
       return false;
```

### Comparing `lephare-0.1.2/src/lib/globals.h` & `lephare-0.1.4/src/lib/globals.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 extern const double pc;
 extern const double pi;
 extern const double hc;
 extern const double f_ga;
 
 void get_lephare_env();
 
-bool test_first_char(string maligne);
+bool check_first_char(string maligne);
 
 double blackbody(double T, double lambda);
 
 int bdincl(int n, long cont, int max);
 
 inline string bool2string(const bool &b) {
   string sb;
```

### Comparing `lephare-0.1.2/src/lib/keyword.cpp` & `lephare-0.1.4/src/lib/keyword.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -244,27 +244,27 @@
     throw invalid_argument("ERROR: can't open config file " + configfile);
   }
 
   // Do that as long as the code can find a new line in the stream
   unsigned int nb_keywords(0);
   while (getline(configst, lit)) {
     // If the first character of the line is not #
-    bool test = test_first_char(lit);
+    bool test = check_first_char(lit);
     if (test) {
       // put the line into the stream ss again
       stringstream ss(lit);
 
       // fill the keyword object
       string name(" "), value(" ");
       ss >> name >> value;
       if (value.back() == ',') {
         string value2;
         while (!ss.eof()) {
           ss >> value2;
-          if (test_first_char(value2)) {
+          if (check_first_char(value2)) {
             value += value2;
           } else {
             break;
           }
         }
       }
       // store all the strings into a vector
```

### Comparing `lephare-0.1.2/src/lib/keyword.h` & `lephare-0.1.4/src/lib/keyword.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/mag.cpp` & `lephare-0.1.4/src/lib/mag.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
   // Create a list of SED with the B12 templates. Need one SED for each redshift
   // of gridz.
   string lit, nameSED, bid;
   double b12z;
   size_t gr = 0;
   while (getline(b12mod, lit)) {
     // If the first character of the line is not #
-    if (test_first_char(lit)) {
+    if (check_first_char(lit)) {
       // Read the SED name + information
       stringstream ss(lit);
       ss >> nameSED >> bid >> b12z;
       string sedpath = lepharedir + "/sed/GAL/" + nameSED;
 
       // Use as template number the value of the redshift x 100
       GalSED oneSEDFIR(sedpath, int(b12z * 100.));
```

### Comparing `lephare-0.1.2/src/lib/mag.h` & `lephare-0.1.4/src/lib/mag.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/mag_gal.cpp` & `lephare-0.1.4/src/lib/mag_gal.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/oneElLambda.cpp` & `lephare-0.1.4/src/lib/oneElLambda.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/oneElLambda.h` & `lephare-0.1.4/src/lib/oneElLambda.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/onesource.cpp` & `lephare-0.1.4/src/lib/onesource.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,16 @@
         chi2loc[il] += inter * inter;
       }
 
       // Upper-limits. Check first if some bands have upper-limits, before
       // applying the condition
       if (nbul > 0) {
         for (size_t k = 0; k < imagm; k++) {
-          if ((dmloc[il] * busul[k] * flux[il][k]) > ab[k]) chi2loc[il] = 1.e9;
+          if ((dmloc[il] * busul[k] * flux[il][k]) > ab[k] && busnorma[k] == 1)
+            chi2loc[il] = 1.e9;
         }
       }
 
       // Model rejection based on prior
       // Abs mag rejection
       double reds;
       int libtype;
```

### Comparing `lephare-0.1.2/src/lib/onesource.h` & `lephare-0.1.4/src/lib/onesource.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/opa.cpp` & `lephare-0.1.4/src/lib/opa.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   // open the ascii file with the extinction law into a stream
   string name = lepharedir + "/opa/" + opaFile;
   sopa.open(name.c_str());
 
   // Take the stream line by line
   while (getline(sopa, lit)) {
     // If the first character of the line is not #
-    if (test_first_char(lit)) {
+    if (check_first_char(lit)) {
       // put the line into the stream ss again
       stringstream ss(lit);
 
       // fill the lambda/trans values of the SED
       double l, v;
       ss >> l;
       ss >> v;
```

### Comparing `lephare-0.1.2/src/lib/opa.h` & `lephare-0.1.4/src/lib/opa.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/photoz_lib.cpp` & `lephare-0.1.4/src/lib/photoz_lib.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -336,14 +336,17 @@
   };
   outputHeader += '\n';
   outputHeader += "# MABS_REF               : ";
   for (int k = 0; k < nbapp; k++) {
     outputHeader += to_string(bapp[k]) + ' ';
   };
   outputHeader += '\n';
+  // AUTO-ADAPT
+  outputHeader += "# AUTO_ADAPT             : " +
+                  bool2string(keys["AUTO_ADAPT"].split_bool("NO", 1)[0]) + '\n';
 
   // ADAPT_BAND selection in one band
   fl_auto = ((key_analysed["ADAPT_BAND"]).split_int("1", 1))[0];
   // Need to substract one because the convention in the .para file start at 1,
   // but 0 in the code
   fl_auto--;
   outputHeader += "# ADAPT_BAND             : " + to_string(fl_auto) + '\n';
@@ -652,15 +655,15 @@
 
     // using a set to find and discard duplicates
     set<string> tmp;
 
     // Take the stream line by line
     while (getline(stoutpara, lit)) {
       // If the first character of the line is not #
-      if (test_first_char(lit)) {
+      if (check_first_char(lit)) {
         // put the line into the stream ss again
         stringstream ss(lit);
 
         // fill the lambda/trans values of the SED
         ss >> fakeString;
 
         if (fakeString == "STRING_INPUT") {
@@ -949,15 +952,15 @@
   // Vector of the objects with a spec-z
   vector<onesource *> adaptSources;
   ifstream sin(cat.c_str());
   // Read all the sources for auto-adapt, store them
   int nobj = 0;
   while (getline(sin, line)) {
     // If the first character of the line is not #
-    if (test_first_char(line)) {
+    if (check_first_char(line)) {
       // Construct one objet
       onesource *oneObj = yield(nobj, line);
 
       // Keep only sources with a spectroscopic redshift
       if (oneObj->zs > adzmin && oneObj->zs < adzmax) {
         // Correct the observed magnitudes and fluxes with the coefficients
         // given in APPLY_SHIFTS
@@ -1364,15 +1367,15 @@
     if (!szex) {
       cout << "External spec-z option, but no file " << externalzfile << endl;
       exit(0);
     }
     string linezex;
     // Ignore the comments
     int nbcomments = 0;
-    while (!(test_first_char(linezex))) {
+    while (!(check_first_char(linezex))) {
       getline(szex, linezex);
       nbcomments++;
     }
     // back to the beginning of the file
     szex.seekg(0, ios::beg);
     ;
     // Go directly to the right lines, skip commented lines
@@ -1398,15 +1401,15 @@
     exit(0);
   }
   // Back to the beginning of the file
   sin.clear();
   sin.seekg(0, sin.beg);
   while (getline(sin, line)) {
     // If the first character of the line is not #
-    if (test_first_char(line)) {
+    if (check_first_char(line)) {
       nobj++;
       if ((nobj < rowmin && rowmin > 0) || (nobj > rowmax && rowmax > 0)) {
         continue;
       }  // CAT_LINES option
 
       // Generate one objet
       onesource *oneObj = yield(nobj, line);
@@ -1557,14 +1560,29 @@
   vector<vector<int>> goodFlt = bestFilter(
       imagm, gridz, fullLib, method, magabscont, bapp, bappOp, zbmin, zbmax);
   vector<vector<double>> maxkcol = maxkcolor(gridz, fullLib, goodFlt);
 
   double funz0 = lcdm.distMod(gridz[1] / 20.);
   vector<opa> opaOut = Mag::read_opa();
 
+  // Specify the offsets in the header
+  string offsets;
+  if (autoadapt) {
+    for (int k = 0; k < imagm; k++) offsets = offsets + to_string(a0[k]) + ",";
+    offsets = "# Offsets from auto-adapt: " + offsets + '\n';
+    outputHeader += offsets;
+  }
+  if (shifts0.size() == (size_t)imagm) {
+    offsets = "";
+    for (int k = 0; k < imagm; k++)
+      offsets = offsets + to_string(shifts0[k]) + ",";
+    offsets = "# Offsets applied directly from keyword: " + offsets + '\n';
+    outputHeader += offsets;
+  }
+
   unsigned int nobj = 0;
   for (auto &oneObj : sources) {
     if (verbose)
       cout << "Fit source " << nobj << " with Id " << oneObj->spec << " \r "
            << flush;
     nobj++;
     // Correct the observed magnitudes and fluxes with the coefficients given in
```

### Comparing `lephare-0.1.2/src/lib/photoz_lib.h` & `lephare-0.1.4/src/lib/photoz_lib.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/sedtolib.cpp` & `lephare-0.1.4/src/lib/sedtolib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/src/lib/zphota.cpp` & `lephare-0.1.4/src/lib/zphota.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -88,19 +88,14 @@
   vector<double> a0, a1;
   if (autoadapt) {
     // Read the sources to be used for auto-adapt
     vector<onesource *> adaptSrcs = photoz.read_autoadapt_sources();
     // Compute the offsets
     std::tie(a0, a1) = photoz.run_autoadapt(adaptSrcs);
     cout << " Done " << endl;
-    string offsets;
-    for (int k = 0; k < photoz.imagm; k++)
-      offsets = offsets + to_string(a0[k]) + ",";
-    offsets = "# Offsets from auto-adapt: " + offsets + '\n';
-    photoz.outputHeader += offsets;
     // Clean the vector
     for (auto &src : adaptSrcs) delete src;
     adaptSrcs.shrink_to_fit();
   } else {
     for (int k = 0; k < photoz.imagm; k++) {
       a0.push_back(0.);
       a1.push_back(0.);
```

### Comparing `lephare-0.1.2/tests/conftest.py` & `lephare-0.1.4/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import pytest
 
 # Set "LEPHAREDIR" locally for tests if it is not already set.
 if "LEPHAREDIR" not in os.environ:
     test_dir = os.path.abspath(os.path.dirname(__file__))
-    os.environ["LEPHAREDIR"] = os.path.join(test_dir, "..")
+    os.environ["LEPHAREDIR"] = os.path.join(test_dir, "data")
 
 # Set "LEPHAREWORK" locally for tests if it is not already set.
 if "LEPHAREWORK" not in os.environ:
     test_dir = os.path.abspath(os.path.dirname(__file__))
     os.environ["LEPHAREWORK"] = os.path.join(test_dir, "tmp")
```

### Comparing `lephare-0.1.2/tests/data/calzetti.dat` & `lephare-0.1.4/tests/data/calzetti.dat`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/tests/data/examples/COSMOS.para` & `lephare-0.1.4/tests/data/examples/COSMOS.para`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,20 @@
 ##############################################################################################
 ###########                          FILTERS                                     #############
 ########### Run : $ZPHOTDIR/source/filter  -c zphot.para                         #############
 ##############################################################################################
 
 # 
 FILTER_REP   $LEPHAREDIR/filt           # Repository in which the filters are stored
-FILTER_LIST   cosmos/u_cfht.lowres,cosmos/u_new.pb,hsc/gHSC.pb,hsc/rHSC.pb,hsc/iHSC.pb,hsc/zHSC.pb,hsc/yHSC.pb,vista/Y.lowres,vista/J.lowres,vista/H.lowres,vista/K.lowres,cosmos/IB427.lowres,cosmos/IB464.lowres,cosmos/IB484.lowres,cosmos/IB505.lowres,cosmos/IB527.lowres,cosmos/IB574.lowres,cosmos/IB624.lowres,cosmos/IB679.lowres,cosmos/IB709.lowres,cosmos/IB738.lowres,cosmos/IB767.lowres,cosmos/IB827.lowres,cosmos/NB711.lowres,cosmos/NB816.lowres,vista/NB118.lowres,cosmos/irac_ch1.lowres,cosmos/irac_ch2.lowres,cosmos/irac_ch3.lowres,cosmos/irac_ch4.lowres 
+FILTER_LIST   subaru/IB527.pb
+# FILTER_LIST   cosmos/u_cfht.lowres,cosmos/u_new.pb,hsc/gHSC.pb,hsc/rHSC.pb,hsc/iHSC.pb,hsc/zHSC.pb,hsc/yHSC.pb,vista/Y.lowres,vista/J.lowres,vista/H.lowres,vista/K.lowres,cosmos/IB427.lowres,cosmos/IB464.lowres,cosmos/IB484.lowres,cosmos/IB505.lowres,cosmos/IB527.lowres,cosmos/IB574.lowres,cosmos/IB624.lowres,cosmos/IB679.lowres,cosmos/IB709.lowres,cosmos/IB738.lowres,cosmos/IB767.lowres,cosmos/IB827.lowres,cosmos/NB711.lowres,cosmos/NB816.lowres,vista/NB118.lowres,cosmos/irac_ch1.lowres,cosmos/irac_ch2.lowres,cosmos/irac_ch3.lowres,cosmos/irac_ch4.lowres 
 TRANS_TYPE	 1			# TRANSMISSION TYPE
                                         # 0[-def]: Energy, 1: Nb of photons
-FILTER_CALIB    0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,1,1,1,1                       # 0[-def]:  fnu=ctt 
+FILTER_CALIB    0
+					# 0[-def]:  fnu=ctt 
                                         # 1      :  nu.fnu=ctt 
                                         # 2      :  fnu=nu 
                                         # 3      :  fnu=Black Body @ T=10000K
                                         # 4      :  for MIPS (leff with nu fnu=ctt and flux with BB @ 10000K  
 FILTER_FILE	filter_cosmos	# name of file with filters (-> $ZPHOTWORK/filt/)
 
 #
```

### Comparing `lephare-0.1.2/tests/data/filt/subaru/IB527.pb` & `lephare-0.1.4/tests/data/filt/subaru/IB527.pb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/tests/data/sed/WDgd71.sed.ext` & `lephare-0.1.4/tests/data/sed/WDgd71.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/tests/data/sed/o5v.sed.ext` & `lephare-0.1.4/tests/data/sed/o5v.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/tests/data/tau10.out` & `lephare-0.1.4/tests/data/tau10.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/tests/lephare/test_cosmology.py` & `lephare-0.1.4/tests/lephare/test_cosmology.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/tests/lephare/test_dataRetrieval.py` & `lephare-0.1.4/tests/lephare/test_data_retrieval.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,34 @@
 import os
-import tempfile
 from pathlib import Path
 from unittest.mock import mock_open, patch
 
 import pytest
-import requests
 from lephare.data_retrieval import (
+    DEFAULT_BASE_DATA_URL,
+    DEFAULT_LOCAL_DATA_PATH,
+    MAX_RETRY_ATTEMPTS,
     _check_downloaded_files,
     _create_directories_from_files,
     download_all_files,
-    download_registry_from_github,
+    download_file,
     filter_files_by_prefix,
     make_default_retriever,
     make_retriever,
     read_list_file,
 )
 
-# TODO: this will be bundled into a module in the future,
-# so replace the hardcoding when that happens
-DEFAULT_BASE_DATA_URL = "https://raw.githubusercontent.com/lephare-photoz/lephare-data/main/"
-DEFAULT_REGISTRY_FILE = "data_registry.txt"
-DEFAULT_LOCAL_DATA_PATH = "./data"
-
 
 def test_filter_file_by_prefix(test_data_dir):
     file_path = os.path.join(test_data_dir, "test_file_names.list")
     target_prefixes = ["prefix1", "prefix2"]
     expected_lines = ["prefix1_file1", "prefix2_file2"]
     assert filter_files_by_prefix(file_path, target_prefixes) == expected_lines
 
 
-@patch("requests.get")
-def test_download_registry_from_github_success(mock_get):
-    mock_get.return_value.status_code = 200
-    mock_get.return_value.text = "file1\nfile2\nfile3"
-
-    with tempfile.TemporaryDirectory() as tmpdir:
-        download_registry_from_github(outfile=os.path.join(tmpdir, "registry.txt"))
-
-        with open(os.path.join(tmpdir, "registry.txt"), "r") as file:
-            assert file.read() == "file1\nfile2\nfile3"
-
-
-@patch("requests.get")
-def test_download_registry_from_github_failure(mock_get):
-    mock_get.return_value.status_code = 404
-    with pytest.raises(requests.exceptions.HTTPError):
-        download_registry_from_github()
-
-
 def test_read_list_file(test_data_dir):
     file_path = os.path.join(test_data_dir, "test_file_names.list")
     expected_files = ["prefix1_file1", "prefix2_file2"]
     assert read_list_file(file_path) == expected_files
 
 
 @patch("requests.get")
@@ -116,17 +92,54 @@
 def test_check_downloaded_files_empty(mock_getsize):
     file_names = ["file1.txt", "file2.txt"]
     downloaded_files = ["/tmp/file1.txt", "/tmp/file2.txt"]
     mock_getsize.side_effect = [10, 0]
     assert not _check_downloaded_files(file_names, downloaded_files)
 
 
+def test_download_single_file(data_registry_file):
+    retriever = make_retriever(registry_file=data_registry_file)
+    file_name = "file1.txt"
+    with patch.object(retriever, "fetch", return_value="/path/to/downloaded/file1.txt") as mock_fetch:
+        download_file(retriever, file_name)
+        mock_fetch.assert_called_once_with(file_name)
+
+
+def test_download_single_file_ignore_registry(data_registry_file):
+    retriever = make_retriever(registry_file=data_registry_file)
+    file_name = "file1.txt"
+    with patch("pooch.retrieve", return_value="/path/to/downloaded/file1.txt") as mock_retrieve:
+        download_file(retriever, file_name, ignore_registry=True)
+        mock_retrieve.assert_any_call(
+            url=f"{retriever.base_url}{file_name}", known_hash=None, fname=file_name, path=retriever.path
+        )
+
+
 @patch("lephare.data_retrieval.download_file")
 def test_download_all_files(mock_download_file, data_registry_file):
+    """This test checks to make sure that we're calling download_file for each file in the list.
+    and also accounts for the fact that we retry downloading each file MAX_RETRY_ATTEMPTS times."""
     retriever = make_retriever(registry_file=data_registry_file)
+
+    # Test with an empty list of files
+    download_all_files(retriever, [])
+    assert mock_download_file.call_count == 0
+
+    # Test with list of 2 files
     file_names = ["file1.txt", "file2.txt"]
     download_all_files(retriever, file_names)
     mock_download_file.assert_any_call(retriever, "file1.txt", ignore_registry=False)
     mock_download_file.assert_any_call(retriever, "file2.txt", ignore_registry=False)
+    # `1 + MAX_RETRY_ATTEMPTS` because we try once, then retry MAX_RETRY_ATTEMPTS more times
+    assert mock_download_file.call_count == len(file_names) * (1 + MAX_RETRY_ATTEMPTS)
+
+
+@patch("lephare.data_retrieval.download_file")
+def test_download_all_files_non_default_retry(mock_download_file, data_registry_file):
+    """This test checks to make sure that we're calling download_file for each file in the list.
+    and sets the retries to 0. This should only try to download each file once."""
+    retriever = make_retriever(registry_file=data_registry_file)
+    file_names = ["file1.txt", "file2.txt"]
+    download_all_files(retriever, file_names, retry=0)
+    mock_download_file.assert_any_call(retriever, "file1.txt", ignore_registry=False)
+    mock_download_file.assert_any_call(retriever, "file2.txt", ignore_registry=False)
     assert mock_download_file.call_count == len(file_names)
-    # TODO could stand to expand this test
-    # Additionally, would be nice to explicitly test single file download
```

### Comparing `lephare-0.1.2/tests/lephare/test_data_manager.py` & `lephare-0.1.4/tests/lephare/test_data_manager.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/tests/lephare/test_keyword.py` & `lephare-0.1.4/tests/lephare/test_keyword.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/tests/lephare/test_oneElLambda.py` & `lephare-0.1.4/tests/lephare/test_oneElLambda.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/tests/lephare/test_onesource.py` & `lephare-0.1.4/tests/lephare/test_onesource.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.2/tests/lephare/test_sed.py` & `lephare-0.1.4/tests/lephare/test_sed.py`

 * *Files identical despite different names*

