# Comparing `tmp/lf-tape-0.4.0.tar.gz` & `tmp/lf_tape-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lf-tape-0.4.0.tar", last modified: Wed Mar 27 20:36:57 2024, max compression
+gzip compressed data, was "lf_tape-0.4.1.tar", last modified: Tue Apr 30 17:31:08 2024, max compression
```

## Comparing `lf-tape-0.4.0.tar` & `lf_tape-0.4.1.tar`

### file list

```diff
@@ -1,177 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.147379 lf-tape-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.119380 lf-tape-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.119380 lf-tape-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.119380 lf-tape-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/workflows/asv-main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/workflows/asv-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/workflows/asv-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/workflows/publish-benchmarks-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-27 20:36:51.000000 lf-tape-0.4.0/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-27 20:36:51.000000 lf-tape-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-03-27 20:36:57.147379 lf-tape-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-03-27 20:36:51.000000 lf-tape-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.119380 lf-tape-0.4.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:51.000000 lf-tape-0.4.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-03-27 20:36:51.000000 lf-tape-0.4.0/benchmarks/asv.conf.json
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-27 20:36:51.000000 lf-tape-0.4.0/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.123380 lf-tape-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)   145263 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/DARK_Combo_sm.png
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.123380 lf-tape-0.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.123380 lf-tape-0.4.0/docs/_static/tutorial_images/
--rw-r--r--   0 runner    (1001) docker     (127)    84193 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/_static/tutorial_images/ensemble_api_structure.png
--rw-r--r--   0 runner    (1001) docker     (127)    69579 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/_static/tutorial_images/ensemble_frame_hierarchy.png
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.123380 lf-tape-0.4.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/examples/rrlyr-period.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.123380 lf-tape-0.4.0/docs/gettingstarted/
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/gettingstarted/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/gettingstarted/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/gettingstarted.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.127380 lf-tape-0.4.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/tutorials/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    18463 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/tutorials/batch_showcase.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/tutorials/binning_slowly_changing_sources.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/tutorials/common_data_operations.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20366 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/tutorials/structure_function_showcase.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/tutorials/tape_datasets.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/tutorials/using_ray_with_the_ensemble.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/tutorials/working_with_hipscat_and_lsdb.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    30266 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/tutorials/working_with_structure_function.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14235 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/tutorials/working_with_the_ensemble.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/tutorials/working_with_the_timeseries.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-27 20:36:51.000000 lf-tape-0.4.0/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-03-27 20:36:51.000000 lf-tape-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 20:36:57.147379 lf-tape-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.111379 lf-tape-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.147379 lf-tape-0.4.0/src/lf_tape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-03-27 20:36:57.000000 lf-tape-0.4.0/src/lf_tape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-03-27 20:36:57.000000 lf-tape-0.4.0/src/lf_tape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 20:36:57.000000 lf-tape-0.4.0/src/lf_tape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-27 20:36:57.000000 lf-tape-0.4.0/src/lf_tape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-27 20:36:57.000000 lf-tape-0.4.0/src/lf_tape.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.127380 lf-tape-0.4.0/src/tape/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-27 20:36:56.000000 lf-tape-0.4.0/src/tape/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.131379 lf-tape-0.4.0/src/tape/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/light_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/stetsonj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.131379 lf-tape-0.4.0/src/tape/analysis/structure_function/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/base_argument_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/base_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.131379 lf-tape-0.4.0/src/tape/analysis/structure_function/basic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/basic/calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.131379 lf-tape-0.4.0/src/tape/analysis/structure_function/bauer_2009a/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/bauer_2009a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/bauer_2009a/calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.131379 lf-tape-0.4.0/src/tape/analysis/structure_function/bauer_2009b/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/bauer_2009b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/bauer_2009b/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/calculator_registrar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.131379 lf-tape-0.4.0/src/tape/analysis/structure_function/macleod_2012/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/macleod_2012/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/macleod_2012/calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.131379 lf-tape-0.4.0/src/tape/analysis/structure_function/schmidt_2010/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/schmidt_2010/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/schmidt_2010/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structure_function/sf_light_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    17647 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/analysis/structurefunction2.py
--rw-r--r--   0 runner    (1001) docker     (127)    99464 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    57343 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/ensemble_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)    15967 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/ensemble_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.131379 lf-tape-0.4.0/src/tape/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.131379 lf-tape-0.4.0/src/tape/utils/column_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/utils/column_mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/utils/column_mapper/column_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-27 20:36:51.000000 lf-tape-0.4.0/src/tape/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.115379 lf-tape-0.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.135380 lf-tape-0.4.0/tests/tape_tests/
--rw-r--r--   0 runner    (1001) docker     (127)    19236 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.115379 lf-tape-0.4.0/tests/tape_tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.135380 lf-tape-0.4.0/tests/tape_tests/data/object/
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/object/test_object.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.115379 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.139380 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.115379 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.139380 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.139380 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.115379 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.139380 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.115379 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.139380 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)   133704 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.115379 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.143380 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    28379 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86295 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    92667 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    99907 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    42210 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    54775 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    72993 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67804 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    80298 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   162097 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31794 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    43738 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)    29241 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.143380 lf-tape-0.4.0/tests/tape_tests/data/source/
--rw-r--r--   0 runner    (1001) docker     (127)    29887 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/data/source/test_source.parquet
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:36:57.147379 lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_base_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_bauer_2009a_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_bauer_2009b_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_calculator_registrar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_light_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_macleod_2012_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_schmidt_2010_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_sf_light_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    37444 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    89256 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    18157 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/test_ensemble_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/test_feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/test_packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-03-27 20:36:51.000000 lf-tape-0.4.0/tests/tape_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.097476 lf_tape-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.073476 lf_tape-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.073476 lf_tape-0.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.073476 lf_tape-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/workflows/asv-main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/workflows/asv-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/workflows/asv-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/workflows/publish-benchmarks-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-30 17:30:59.000000 lf_tape-0.4.1/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 17:30:59.000000 lf_tape-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-30 17:31:08.097476 lf_tape-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-30 17:30:59.000000 lf_tape-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.073476 lf_tape-0.4.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:30:59.000000 lf_tape-0.4.1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-30 17:30:59.000000 lf_tape-0.4.1/benchmarks/asv.conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-30 17:30:59.000000 lf_tape-0.4.1/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.077476 lf_tape-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)   145263 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/DARK_Combo_sm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.077476 lf_tape-0.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.077476 lf_tape-0.4.1/docs/_static/tutorial_images/
+-rw-r--r--   0 runner    (1001) docker     (127)    84193 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/_static/tutorial_images/ensemble_api_structure.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69579 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/_static/tutorial_images/ensemble_frame_hierarchy.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.077476 lf_tape-0.4.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/examples/rrlyr-period.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.077476 lf_tape-0.4.1/docs/gettingstarted/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/gettingstarted/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/gettingstarted/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/gettingstarted/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/gettingstarted.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.077476 lf_tape-0.4.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/tutorials/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18499 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/tutorials/batch_showcase.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/tutorials/binning_slowly_changing_sources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18617 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/tutorials/common_data_operations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20280 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/tutorials/structure_function_showcase.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/tutorials/tape_datasets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/tutorials/using_ray_with_the_ensemble.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/tutorials/working_with_hipscat_and_lsdb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30266 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/tutorials/working_with_structure_function.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14239 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/tutorials/working_with_the_ensemble.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/tutorials/working_with_the_timeseries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-30 17:30:59.000000 lf_tape-0.4.1/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-30 17:30:59.000000 lf_tape-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 17:31:08.097476 lf_tape-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.069476 lf_tape-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.097476 lf_tape-0.4.1/src/lf_tape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-30 17:31:08.000000 lf_tape-0.4.1/src/lf_tape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-30 17:31:08.000000 lf_tape-0.4.1/src/lf_tape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 17:31:08.000000 lf_tape-0.4.1/src/lf_tape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 17:31:08.000000 lf_tape-0.4.1/src/lf_tape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 17:31:08.000000 lf_tape-0.4.1/src/lf_tape.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.081476 lf_tape-0.4.1/src/tape/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 17:31:07.000000 lf_tape-0.4.1/src/tape/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.081476 lf_tape-0.4.1/src/tape/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/light_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/stetsonj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.081476 lf_tape-0.4.1/src/tape/analysis/structure_function/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/base_argument_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/base_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.081476 lf_tape-0.4.1/src/tape/analysis/structure_function/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/basic/calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.081476 lf_tape-0.4.1/src/tape/analysis/structure_function/bauer_2009a/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/bauer_2009a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/bauer_2009a/calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.085476 lf_tape-0.4.1/src/tape/analysis/structure_function/bauer_2009b/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/bauer_2009b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/bauer_2009b/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/calculator_registrar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.085476 lf_tape-0.4.1/src/tape/analysis/structure_function/macleod_2012/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/macleod_2012/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/macleod_2012/calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.085476 lf_tape-0.4.1/src/tape/analysis/structure_function/schmidt_2010/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/schmidt_2010/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/schmidt_2010/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structure_function/sf_light_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17647 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/analysis/structurefunction2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99923 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58797 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/ensemble_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15967 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/ensemble_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.085476 lf_tape-0.4.1/src/tape/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.085476 lf_tape-0.4.1/src/tape/utils/column_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/utils/column_mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/utils/column_mapper/column_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-30 17:30:59.000000 lf_tape-0.4.1/src/tape/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.069476 lf_tape-0.4.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.085476 lf_tape-0.4.1/tests/tape_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19236 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.069476 lf_tape-0.4.1/tests/tape_tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.085476 lf_tape-0.4.1/tests/tape_tests/data/object/
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/object/test_object.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/object/test_object2.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.069476 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.089476 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.069476 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.089476 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.089476 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.069476 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.089476 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.069476 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.089476 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)   133704 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.069476 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.093476 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    28379 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86295 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    92667 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    99907 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    42210 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54775 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    72993 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67804 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    80298 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   162097 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31794 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    43738 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)    29241 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.093476 lf_tape-0.4.1/tests/tape_tests/data/source/
+-rw-r--r--   0 runner    (1001) docker     (127)    29887 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/source/test_source.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    29887 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/data/source/test_source2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:31:08.097476 lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_base_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_bauer_2009a_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_bauer_2009b_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_calculator_registrar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_light_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_macleod_2012_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_schmidt_2010_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_sf_light_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37444 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89873 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20054 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/test_ensemble_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/test_feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-30 17:30:59.000000 lf_tape-0.4.1/tests/tape_tests/test_utils.py
```

### Comparing `lf-tape-0.4.0/.gitattributes` & `lf_tape-0.4.1/.gitattributes`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.github/ISSUE_TEMPLATE/1-bug_report.md` & `lf_tape-0.4.1/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.github/ISSUE_TEMPLATE/2-feature_request.md` & `lf_tape-0.4.1/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.github/pull_request_template.md` & `lf_tape-0.4.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.github/workflows/asv-main.yml` & `lf_tape-0.4.1/.github/workflows/asv-main.yml`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.github/workflows/asv-nightly.yml` & `lf_tape-0.4.1/.github/workflows/asv-nightly.yml`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.github/workflows/asv-pr.yml` & `lf_tape-0.4.1/.github/workflows/asv-pr.yml`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.github/workflows/build-documentation.yml` & `lf_tape-0.4.1/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.github/workflows/pre-commit-ci.yml` & `lf_tape-0.4.1/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.github/workflows/publish-benchmarks-pr.yml` & `lf_tape-0.4.1/.github/workflows/publish-benchmarks-pr.yml`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.github/workflows/publish-to-pypi.yml` & `lf_tape-0.4.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.github/workflows/smoke-test.yml` & `lf_tape-0.4.1/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.github/workflows/testing-and-coverage.yml` & `lf_tape-0.4.1/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.gitignore` & `lf_tape-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.pre-commit-config.yaml` & `lf_tape-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/.setup_dev.sh` & `lf_tape-0.4.1/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/LICENSE` & `lf_tape-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/PKG-INFO` & `lf_tape-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lf-tape
-Version: 0.4.0
+Version: 0.4.1
 Author-email: LINCC Frameworks Team <Lincc-frameworks-team@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2019 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -34,14 +34,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: dask>=2024.3.0
+Requires-Dist: dask-expr<1.0.11
 Requires-Dist: dask[distributed]>=2024.3.0
 Requires-Dist: pyarrow
 Requires-Dist: pyvo
 Requires-Dist: scipy
 Requires-Dist: requests
 Requires-Dist: aiohttp
 Requires-Dist: coverage
@@ -83,27 +84,16 @@
 
 ## Installation
 TAPE is available to install with pip, using the "lf-tape" package name:
 ``` 
 pip install lf-tape
 ```
 
-## Getting started - for developers
+## Contributing
 
-Download code and install dependencies in a conda environment. Run unit tests at the end as a verification that the packages are properly installed.
+[![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/lincc-frameworks/tape?color=purple&label=Good%20first%20issues&query=is%3Aopen%20label%3A%22good%20first%20issue%22)](https://github.com/lincc-frameworks/tape/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
 
-```
-$ conda create -n seriesenv python=3.11
-$ conda activate seriesenv
-
-$ git clone https://github.com/lincc-frameworks/tape
-$ cd tape/
-$ pip install .
-$ pip install .[dev]  # it may be necessary to use `pip install .'[dev]'` (with single quotes) depending on your machine.
-
-$ pip install pytest
-$ pytest
-```
+See the [Contribution Guide](https://tape.readthedocs.io/en/latest/gettingstarted/contributing.html) for complete installation instructions and contribution best practices.
 
 ## Acknowledgements
 
-LINCC Frameworks is supported by Schmidt Futures, a philanthropic initiative founded by Eric and Wendy Schmidt, as part of the Virtual Institute of Astrophysics (VIA).
+This project is supported by Schmidt Sciences.
```

### Comparing `lf-tape-0.4.0/README.md` & `lf_tape-0.4.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -25,27 +25,16 @@
 
 ## Installation
 TAPE is available to install with pip, using the "lf-tape" package name:
 ``` 
 pip install lf-tape
 ```
 
-## Getting started - for developers
+## Contributing
 
-Download code and install dependencies in a conda environment. Run unit tests at the end as a verification that the packages are properly installed.
+[![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/lincc-frameworks/tape?color=purple&label=Good%20first%20issues&query=is%3Aopen%20label%3A%22good%20first%20issue%22)](https://github.com/lincc-frameworks/tape/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
 
-```
-$ conda create -n seriesenv python=3.11
-$ conda activate seriesenv
-
-$ git clone https://github.com/lincc-frameworks/tape
-$ cd tape/
-$ pip install .
-$ pip install .[dev]  # it may be necessary to use `pip install .'[dev]'` (with single quotes) depending on your machine.
-
-$ pip install pytest
-$ pytest
-```
+See the [Contribution Guide](https://tape.readthedocs.io/en/latest/gettingstarted/contributing.html) for complete installation instructions and contribution best practices.
 
 ## Acknowledgements
 
-LINCC Frameworks is supported by Schmidt Futures, a philanthropic initiative founded by Eric and Wendy Schmidt, as part of the Virtual Institute of Astrophysics (VIA).
+This project is supported by Schmidt Sciences.
```

### Comparing `lf-tape-0.4.0/benchmarks/asv.conf.json` & `lf_tape-0.4.1/benchmarks/asv.conf.json`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/benchmarks/benchmarks.py` & `lf_tape-0.4.1/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/docs/DARK_Combo_sm.png` & `lf_tape-0.4.1/docs/DARK_Combo_sm.png`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/docs/Makefile` & `lf_tape-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/docs/_static/tutorial_images/ensemble_api_structure.png` & `lf_tape-0.4.1/docs/_static/tutorial_images/ensemble_api_structure.png`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/docs/_static/tutorial_images/ensemble_frame_hierarchy.png` & `lf_tape-0.4.1/docs/_static/tutorial_images/ensemble_frame_hierarchy.png`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/docs/conf.py` & `lf_tape-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/docs/examples/rrlyr-period.ipynb` & `lf_tape-0.4.1/docs/examples/rrlyr-period.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988425925925926%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(1, 'ens = "*

 * *            'Ensemble(client=False).from_dataset("s82_rrlyrae", sorted=True)\')], delete: [1]}}}'}*

```diff
@@ -38,15 +38,15 @@
                     "end_time": "2023-09-20T13:16:53.703300Z",
                     "start_time": "2023-09-20T13:16:49.340873Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# Load SDSS Stripe 82 RR Lyrae catalog\n",
-                "ens = Ensemble(client=False).from_dataset(\"s82_rrlyrae\")"
+                "ens = Ensemble(client=False).from_dataset(\"s82_rrlyrae\", sorted=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "5c2dd5a5fd58ce00",
             "metadata": {
```

### Comparing `lf-tape-0.4.0/docs/gettingstarted/installation.rst` & `lf_tape-0.4.1/docs/gettingstarted/installation.rst`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/docs/gettingstarted/quickstart.ipynb` & `lf_tape-0.4.1/docs/gettingstarted/quickstart.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9842684837092732%*

 * *Differences: {"'cells'": "{1: {'source': ['The latest release of TAPE is installable via pip, using the "*

 * *            'following command:\']}, 5: {\'source\': {insert: [(3, \'ens.from_dataset("s82_qso", '*

 * *            "sorted=True)')], delete: [3]}}, insert: [(2, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', None), ('metadata', OrderedDict()), ('outputs', []), ('source', "*

 * *            "['\\n', '%pip install lf-tape --quiet\\n'])])), (3, OrderedDict([('cell_type', "*

 * *            "'markdown'), ('met […]*

```diff
@@ -8,20 +8,31 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The latest release of TAPE is installable via pip, using the following command:\n",
-                "\n",
-                "```\n",
-                "pip install lf-tape\n",
-                "```\n",
+                "The latest release of TAPE is installable via pip, using the following command:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "\n",
+                "%pip install lf-tape --quiet\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "For more detailed installation instructions, see the [Installation Guide](installation.html)."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -34,15 +45,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from tape import Ensemble\n",
                 "\n",
                 "ens = Ensemble()  # Initialize a TAPE Ensemble\n",
-                "ens.from_dataset(\"s82_qso\")"
+                "ens.from_dataset(\"s82_qso\", sorted=True)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -196,15 +207,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.13"
+            "version": "3.10.11"
         },
         "vscode": {
             "interpreter": {
                 "hash": "83afbb17b435d9bf8b0d0042367da76f26510da1c5781f0ff6e6c518eab621ec"
             }
         }
     },
```

### Comparing `lf-tape-0.4.0/docs/tutorials/batch_showcase.ipynb` & `lf_tape-0.4.1/docs/tutorials/batch_showcase.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999582047325103%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(9, '\\n')]}}, 4: {'source': {insert: [(6, '    "*

 * *            "sorted=True,\\n')]}}}"}*

```diff
@@ -41,14 +41,15 @@
                 "np.random.seed(1)\n",
                 "\n",
                 "obj_ids = []\n",
                 "mjds = []\n",
                 "for i in range(10, 110):\n",
                 "    obj_ids.append(np.array([i] * 1250))\n",
                 "    mjds.append(np.arange(0.0, 1250.0, 1.0))\n",
+                "\n",
                 "obj_ids = np.concatenate(obj_ids)\n",
                 "mjds = np.concatenate(mjds)\n",
                 "\n",
                 "flux = 10 * np.random.random(125000)\n",
                 "err = flux / 10\n",
                 "band = np.random.choice([\"g\", \"r\"], 125000)\n",
                 "\n",
@@ -63,14 +64,15 @@
             "source": [
                 "# Load the data into an Ensemble\n",
                 "ens = Ensemble()\n",
                 "\n",
                 "ens.from_source_dict(\n",
                 "    source_dict,\n",
                 "    column_mapper=ColumnMapper(id_col=\"id\", time_col=\"mjd\", flux_col=\"flux\", err_col=\"err\", band_col=\"band\"),\n",
+                "    sorted=True,\n",
                 ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `lf-tape-0.4.0/docs/tutorials/binning_slowly_changing_sources.ipynb` & `lf_tape-0.4.1/docs/tutorials/binning_slowly_changing_sources.ipynb`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/docs/tutorials/common_data_operations.ipynb` & `lf_tape-0.4.1/docs/tutorials/common_data_operations.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9888883667502089%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(4, \'ens.from_dataset("s82_rrlyrae", sorted=True)\')], '*

 * *            "delete: [4]}}, 10: {'source': {insert: [(5, 'some partitions may be empty and `head` "*

 * *            'will have to traverse these empty partitions to find enough rows for your result. An '*

 * *            'empty table with many partitions (O(100)k) might be costly even for an ultimately '*

 * *            "empty result. ')], delete: [5]}}, 11: {'source': {insert: [(0, 'ens.source.head(5)  # "*

 * *            'gra […]*

```diff
@@ -33,15 +33,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from tape import Ensemble\n",
                 "\n",
                 "ens = Ensemble()\n",
                 "\n",
-                "ens.from_dataset(\"s82_rrlyrae\", sort=True)"
+                "ens.from_dataset(\"s82_rrlyrae\", sorted=True)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -106,24 +106,24 @@
             "metadata": {},
             "source": [
                 "### Grab small in-memory views with `head()`\n",
                 "\n",
                 "Often, you'll want to peek at your data even though the full-size is too large for memory.\n",
                 "\n",
                 "> **_Note:_**\n",
-                "By default this only looks at the first partition of data, so any operations that remove all data from the first partition will produce an empty head result. Specify `npartitions=-1` to grab from all partitions.\n"
+                "some partitions may be empty and `head` will have to traverse these empty partitions to find enough rows for your result. An empty table with many partitions (O(100)k) might be costly even for an ultimately empty result. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ens.source.head(5, npartitions=-1)  # grabs the first 5 rows\n",
+                "ens.source.head(5)  # grabs the first 5 rows\n",
                 "\n",
                 "# can also use tail to grab the last 5 rows"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -137,15 +137,18 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Access using a known ID\n",
                 "\n",
-                "If you'd like to access a particular lightcurve given an ID, you can use the `to_timeseries()` function. This allows you to supply a given object ID, and returns a `TimeSeries` object (see [working_with_the_timeseries](working_with_the_timeseries.ipynb))."
+                "If you'd like to access a particular lightcurve given an ID, you can use the `to_timeseries()` function. This allows you to supply a given object ID, and returns a `TimeSeries` object (see [working_with_the_timeseries](working_with_the_timeseries.ipynb)).\n",
+                "\n",
+                "> **_Note:_**\n",
+                "that this loads data from all available bands."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -245,17 +248,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ens.calc_nobs(by_band=True)\n",
+                "ens.calc_nobs(by_band=True, temporary=False)\n",
                 "\n",
-                "ens.object[[\"nobs_u\", \"nobs_g\", \"nobs_r\", \"nobs_i\", \"nobs_z\", \"nobs_total\"]].head(5)"
+                "ens.object.head(5)[[\"nobs_u\", \"nobs_g\", \"nobs_r\", \"nobs_i\", \"nobs_z\", \"nobs_total\"]]"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -460,16 +463,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ens.source.repartition(partition_size=\"100MB\").update_ensemble()  # 100MBs is generally recommended\n",
-                "ens.source  # In this case, we have a small set of data that easily fits into one partition"
+                "ens.source.repartition(partition_size=\"100MB\")  # 100MBs is generally recommended\n",
+                "# In this case, we have a small set of data that easily fits into one partition"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -489,14 +492,36 @@
                 "subset_ens = ens.sample(frac=0.5)  # select ~half of the objects\n",
                 "\n",
                 "print(\"Number of pre-sampled objects: \", len(ens.object))\n",
                 "print(\"Number of post-sampled objects: \", len(subset_ens.object))"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "For reproducible results, you can also specify a random seed via the `random_state` parameter. By re-using the same seed in your `random_state`, you can ensure that a given `Ensemble` will always be sampled the same way."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "subset_ens = ens.sample(\n",
+                "    frac=0.2,  # select a ~fifth of the objects\n",
+                "    random_state=53783594,  # set a random seed for reproducibility\n",
+                ")\n",
+                "\n",
+                "print(\"Number of pre-sampled objects: \", len(ens.object))\n",
+                "print(\"Number of post-sampled objects: \", len(subset_ens.object))"
+            ]
+        },
+        {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> **_Note:_**\n",
                 "Using `Ensemble.sample` to filter large datasets is not recommended, as it does not handle repartitioning. Instead, using partition slicing, shown below."
             ]
@@ -525,14 +550,23 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "ens.object.head(5)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "ens.save_ensemble(\".\", \"ensemble\", additional_frames=False)  # Saves to disk"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -547,14 +581,21 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "new_ens = Ensemble()\n",
                 "new_ens.from_ensemble(\"./ensemble\")"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
@@ -565,15 +606,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.10.14"
         },
         "vscode": {
             "interpreter": {
                 "hash": "83afbb17b435d9bf8b0d0042367da76f26510da1c5781f0ff6e6c518eab621ec"
             }
         }
     },
```

### Comparing `lf-tape-0.4.0/docs/tutorials/structure_function_showcase.ipynb` & `lf_tape-0.4.1/docs/tutorials/structure_function_showcase.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895048701298701%*

 * *Differences: {"'cells'": "{13: {'source': {insert: [(33, '    sorted=True,\\n')]}}, delete: [11]}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.11'}, 'vscode': {'interpreter': {'hash': "*

 * *               "'83afbb17b435d9bf8b0d0042367da76f26510da1c5781f0ff6e6c518eab621ec'}}}"}*

```diff
@@ -159,21 +159,14 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
             "source": [
                 "id_ens, t_ens, y_ens, yerr_ens, filter_ens = (\n",
                 "    np.array([]),\n",
                 "    np.array([]),\n",
                 "    np.array([]),\n",
                 "    np.array([]),\n",
                 "    np.array([]),\n",
@@ -245,14 +238,15 @@
                 "    id_col=\"id_ens\", time_col=\"t_ens\", flux_col=\"y_ens\", err_col=\"yerr_ens\", band_col=\"filter_ens\"\n",
                 ")\n",
                 "\n",
                 "ens = Ensemble()\n",
                 "ens.from_source_dict(\n",
                 "    {\"id_ens\": id_ens, \"t_ens\": t_ens, \"y_ens\": y_ens, \"yerr_ens\": yerr_ens, \"filter_ens\": filter_ens},\n",
                 "    column_mapper=manual_colmap,\n",
+                "    sorted=True,\n",
                 ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -560,18 +554,18 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.9"
+            "version": "3.10.11"
         },
         "vscode": {
             "interpreter": {
-                "hash": "31f2aee4e71d21fbe5cf8b01ff0e069b9275f58929596ceb00d14d90e3e16cd6"
+                "hash": "83afbb17b435d9bf8b0d0042367da76f26510da1c5781f0ff6e6c518eab621ec"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `lf-tape-0.4.0/docs/tutorials/tape_datasets.ipynb` & `lf_tape-0.4.1/docs/tutorials/tape_datasets.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9923477095516569%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(11, "*

 * *            '\'ens.from_parquet(source_file=f"{rel_path}/source/test_source.parquet", '*

 * *            "column_mapper=col_map, sorted=True)\\n')], delete: [11]}}, 5: {'source': {insert: "*

 * *            "[(15, '    sorted=True,\\n')]}}, 12: {'source': {insert: [(0, "*

 * *            '\'ens.from_dataset("s82_rrlyrae", sorted=True)  # Let\\\'s grab the Stripe 82 RR '*

 * *            "Lyrae\\n')], delete: [0]}}, 16: {'source': {insert: [(2, "*

 * *            "'ens.from_source_dict(so […]*

```diff
@@ -42,15 +42,15 @@
                 "\n",
                 "# A ColumnMapper is created to map columns of the parquet file to timeseries quantities, such as flux, time, etc.\n",
                 "col_map = ColumnMapper(\n",
                 "    id_col=\"ps1_objid\", time_col=\"midPointTai\", flux_col=\"psFlux\", err_col=\"psFluxErr\", band_col=\"filterName\"\n",
                 ")\n",
                 "\n",
                 "# Read in data from a parquet file that contains source (timeseries) data\n",
-                "ens.from_parquet(source_file=f\"{rel_path}/source/test_source.parquet\", column_mapper=col_map)\n",
+                "ens.from_parquet(source_file=f\"{rel_path}/source/test_source.parquet\", column_mapper=col_map, sorted=True)\n",
                 "\n",
                 "ens.source.head(5)  # View the first 5 entries of the source table"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -76,14 +76,15 @@
                 ")\n",
                 "\n",
                 "# Read in data from a parquet file that contains source (timeseries) data\n",
                 "ens.from_parquet(\n",
                 "    source_file=f\"{rel_path}/source/test_source.parquet\",\n",
                 "    object_file=f\"{rel_path}/object/test_object.parquet\",\n",
                 "    column_mapper=col_map,\n",
+                "    sorted=True,\n",
                 ")\n",
                 "\n",
                 "ens.object.head(5)  # View the first 5 entries of the object table"
             ]
         },
         {
             "attachments": {},
@@ -143,15 +144,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ens.from_dataset(\"s82_rrlyrae\")  # Let's grab the Stripe 82 RR Lyrae\n",
+                "ens.from_dataset(\"s82_rrlyrae\", sorted=True)  # Let's grab the Stripe 82 RR Lyrae\n",
                 "\n",
                 "ens.object.head(5)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -205,18 +206,25 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "colmap = ColumnMapper(id_col=\"id\", time_col=\"time\", flux_col=\"flux\", err_col=\"error\", band_col=\"band\")\n",
                 "ens = Ensemble()\n",
-                "ens.from_source_dict(source_dict, column_mapper=colmap)\n",
+                "ens.from_source_dict(source_dict, column_mapper=colmap, sorted=True)\n",
                 "\n",
                 "ens.info()"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `lf-tape-0.4.0/docs/tutorials/working_with_hipscat_and_lsdb.ipynb` & `lf_tape-0.4.1/docs/tutorials/working_with_hipscat_and_lsdb.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998538011695907%*

 * *Differences: {"'cells'": "{15: {'source': {insert: [(3, '    radius_arcsec=100000.0,\\n')], delete: [3]}}}"}*

```diff
@@ -171,15 +171,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "object_cat_cone = object_cat.cone_search(\n",
                 "    ra=315.0,\n",
                 "    dec=-69.5,\n",
-                "    radius_arcsec=10.0,\n",
+                "    radius_arcsec=100000.0,\n",
                 ")\n",
                 "\n",
                 "print(f\"Original Number of Objects: {len(object_cat._ddf)}\")\n",
                 "print(f\"New Number of Objects: {len(object_cat_cone._ddf)}\")"
             ]
         },
         {
```

### Comparing `lf-tape-0.4.0/docs/tutorials/working_with_structure_function.ipynb` & `lf_tape-0.4.1/docs/tutorials/working_with_structure_function.ipynb`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/docs/tutorials/working_with_the_ensemble.ipynb` & `lf_tape-0.4.1/docs/tutorials/working_with_the_ensemble.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979715749936338%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(2, \'ens = Ensemble().from_dataset("s82_rrlyrae", '*

 * *            "sorted=True)')], delete: [2]}}, 17: {'source': {insert: [(0, '## Storing and "*

 * *            "Accessing Result Frames\\n')], delete: [0]}}, 29: {'source': {insert: [(0, '## "*

 * *            "Keeping the Object and Source Tables in Sync\\n')], delete: [0]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.11'}}"}*

```diff
@@ -22,15 +22,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from tape.ensemble import Ensemble\n",
                 "\n",
-                "ens = Ensemble().from_dataset(\"s82_rrlyrae\", sort=True)"
+                "ens = Ensemble().from_dataset(\"s82_rrlyrae\", sorted=True)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -193,15 +193,15 @@
                 "Note that the above is still a series of lazy operations that will not be fully evaluated until an operation such as `compute()`. So a call to `update_ensemble()` will not yet alter or move any underlying data."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Storing and Accessing Result Frames\n",
+                "## Storing and Accessing Result Frames\n",
                 "The `Ensemble` provides a powerful batching interface, `Ensemble.batch()`, to perform analysis functions in parallel across your lightcurves.\n",
                 "\n",
                 "For the below example, we use the included suite of analysis functions to apply `tape.analysis.calc_stetson_J` on our dataset. (For more info on `Ensemble.batch()`, including providing your own custom functions, see the [Ensemble Batch Showcase](https://tape.readthedocs.io/en/latest/tutorials/batch_showcase.html#) )"
             ]
         },
         {
             "cell_type": "code",
@@ -315,15 +315,15 @@
                 "    print(\"As expected, the frame 'new_res' was dropped.\\n\", str(e))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Keeping the Object and Source Tables in Sync\n",
+                "## Keeping the Object and Source Tables in Sync\n",
                 "\n",
                 "The `TAPE` `Ensemble` attempts to lazily \"sync\" the Object and Source tables such that:\n",
                 "\n",
                 "* If a series of operations removes all lightcurves for a particular object from the Source table, we will lazily remove that object from the Object table.\n",
                 "* If a series of operations removes an object from the Object table, we will lazily remove all light curves for that object from the Source table.\n",
                 "\n",
                 "As an example, let's filter the Object table only for objects of type 'ab'. This operation marks the result table as `dirty` indicating to the `Ensemble` that if used as part of a result computation, it should check if the Object and Source tables are synced. \n",
@@ -393,15 +393,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.13"
+            "version": "3.10.11"
         },
         "vscode": {
             "interpreter": {
                 "hash": "83afbb17b435d9bf8b0d0042367da76f26510da1c5781f0ff6e6c518eab621ec"
             }
         }
     },
```

### Comparing `lf-tape-0.4.0/docs/tutorials/working_with_the_timeseries.ipynb` & `lf_tape-0.4.1/docs/tutorials/working_with_the_timeseries.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9854758089133089%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(12, '    sorted=True,\\n')]}}, 4: {'source': ['As a result, "*

 * *            'we get a multi-indexed `Pandas` DataFrame with data from a single lightcurve. The '*

 * *            'multi-index contains a band index as well as a integer index. We can operate on this '*

 * *            "as we normally would a `Pandas` DataFrame.\\n', '\\n', 'Below we plot out the g-band "*

 * *            "of the lightcurve.']}, 5: {'source': {insert: [(3, 'ts_g = ts.data[ts.band == "*

 * *            '"g"]\\n\ […]*

```diff
@@ -36,14 +36,15 @@
                 "ens.from_parquet(\n",
                 "    \"../../tests/tape_tests/data/source/test_source.parquet\",\n",
                 "    id_col=\"ps1_objid\",\n",
                 "    time_col=\"midPointTai\",\n",
                 "    flux_col=\"psFlux\",\n",
                 "    err_col=\"psFluxErr\",\n",
                 "    band_col=\"filterName\",\n",
+                "    sorted=True,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -54,51 +55,59 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "As a result, we get a multi-indexed `Pandas` DataFrame with data from a single lightcurve. The multi-index contains a band index as well as a integer index. We can operate on this as we normally would a `Pandas` DataFrame."
+                "As a result, we get a multi-indexed `Pandas` DataFrame with data from a single lightcurve. The multi-index contains a band index as well as a integer index. We can operate on this as we normally would a `Pandas` DataFrame.\n",
+                "\n",
+                "Below we plot out the g-band of the lightcurve."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "ts_r = ts.data[ts.band == \"r\"]\n",
                 "\n",
-                "plt.plot(ts_r[\"midPointTai\"], ts_r[\"psFlux\"])"
+                "ts_g = ts.data[ts.band == \"g\"]\n",
+                "\n",
+                "plt.figure(figsize=(8, 5))\n",
+                "plt.errorbar(ts_g.midPointTai, ts_g.psFlux, ts_g.psFluxErr, fmt=\"o\", color=\"green\", alpha=0.8, label=\"g\")\n",
+                "plt.xlabel(\"Time (MJD)\")\n",
+                "plt.ylabel(\"Flux (mJy)\")\n",
+                "plt.minorticks_on()\n",
+                "plt.legend(title=\"Band\", loc=\"upper left\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "py310",
+            "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.10.14"
         },
         "vscode": {
             "interpreter": {
-                "hash": "08968836a6367873274ed1d5e98a07391f42fc3a62bd5aba54afbd7b11ba8673"
+                "hash": "83afbb17b435d9bf8b0d0042367da76f26510da1c5781f0ff6e6c518eab621ec"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `lf-tape-0.4.0/docs/tutorials.rst` & `lf_tape-0.4.1/docs/tutorials.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Tutorials
 ========================================================================================
 
 These pages contain a set of tutorial notebooks for working through core and more advanced TAPE
 functionality.
 
 .. toctree::
+    :maxdepth: 1
 
     Loading Data into TAPE <tutorials/tape_datasets>
     Working with the TAPE Ensemble object <tutorials/working_with_the_ensemble>
     Working with HiPSCat and LSDB data <tutorials/working_with_hipscat_and_lsdb>
     Working with the TAPE Timeseries object <tutorials/working_with_the_timeseries>
     Common Data Operations with TAPE <tutorials/common_data_operations>
     Working with Structure Function <tutorials/working_with_structure_function>
```

### Comparing `lf-tape-0.4.0/pyproject.toml` & `lf_tape-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ]
 dynamic=["version"]
 requires-python = ">=3.9"
 dependencies = [
     'pandas',
     'numpy',
     'dask>=2024.3.0',
+    'dask-expr<1.0.11', # Temporary pin due to compatibility bug
     'dask[distributed]>=2024.3.0',
     'pyarrow',
     'pyvo',
     'scipy',
     'requests',
     'aiohttp',
     'coverage',
```

### Comparing `lf-tape-0.4.0/src/lf_tape.egg-info/PKG-INFO` & `lf_tape-0.4.1/src/lf_tape.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lf-tape
-Version: 0.4.0
+Version: 0.4.1
 Author-email: LINCC Frameworks Team <Lincc-frameworks-team@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2019 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -34,14 +34,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: dask>=2024.3.0
+Requires-Dist: dask-expr<1.0.11
 Requires-Dist: dask[distributed]>=2024.3.0
 Requires-Dist: pyarrow
 Requires-Dist: pyvo
 Requires-Dist: scipy
 Requires-Dist: requests
 Requires-Dist: aiohttp
 Requires-Dist: coverage
@@ -83,27 +84,16 @@
 
 ## Installation
 TAPE is available to install with pip, using the "lf-tape" package name:
 ``` 
 pip install lf-tape
 ```
 
-## Getting started - for developers
+## Contributing
 
-Download code and install dependencies in a conda environment. Run unit tests at the end as a verification that the packages are properly installed.
+[![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/lincc-frameworks/tape?color=purple&label=Good%20first%20issues&query=is%3Aopen%20label%3A%22good%20first%20issue%22)](https://github.com/lincc-frameworks/tape/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
 
-```
-$ conda create -n seriesenv python=3.11
-$ conda activate seriesenv
-
-$ git clone https://github.com/lincc-frameworks/tape
-$ cd tape/
-$ pip install .
-$ pip install .[dev]  # it may be necessary to use `pip install .'[dev]'` (with single quotes) depending on your machine.
-
-$ pip install pytest
-$ pytest
-```
+See the [Contribution Guide](https://tape.readthedocs.io/en/latest/gettingstarted/contributing.html) for complete installation instructions and contribution best practices.
 
 ## Acknowledgements
 
-LINCC Frameworks is supported by Schmidt Futures, a philanthropic initiative founded by Eric and Wendy Schmidt, as part of the Virtual Institute of Astrophysics (VIA).
+This project is supported by Schmidt Sciences.
```

### Comparing `lf-tape-0.4.0/src/lf_tape.egg-info/SOURCES.txt` & `lf_tape-0.4.1/src/lf_tape.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 docs/index.rst
 docs/requirements.txt
 docs/tutorials.rst
 docs/_static/custom.css
 docs/_static/tutorial_images/ensemble_api_structure.png
 docs/_static/tutorial_images/ensemble_frame_hierarchy.png
 docs/examples/rrlyr-period.ipynb
+docs/gettingstarted/contributing.rst
 docs/gettingstarted/installation.rst
 docs/gettingstarted/quickstart.ipynb
 docs/tutorials/README.md
 docs/tutorials/batch_showcase.ipynb
 docs/tutorials/binning_slowly_changing_sources.ipynb
 docs/tutorials/common_data_operations.ipynb
 docs/tutorials/structure_function_showcase.ipynb
@@ -93,14 +94,15 @@
 tests/tape_tests/test_ensemble_frame.py
 tests/tape_tests/test_feature_extraction.py
 tests/tape_tests/test_init.py
 tests/tape_tests/test_packaging.py
 tests/tape_tests/test_timeseries.py
 tests/tape_tests/test_utils.py
 tests/tape_tests/data/object/test_object.parquet
+tests/tape_tests/data/object/test_object2.parquet
 tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/_common_metadata
 tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/_metadata
 tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/catalog_info.json
 tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/partition_info.csv
 tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/point_map.fits
 tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/provenance_info.json
 tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
@@ -121,14 +123,15 @@
 tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
 tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
 tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
 tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
 tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
 tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
 tests/tape_tests/data/source/test_source.parquet
+tests/tape_tests/data/source/test_source2.parquet
 tests/tape_tests/structure_function_calculators/test_base_calculator.py
 tests/tape_tests/structure_function_calculators/test_bauer_2009a_calculator.py
 tests/tape_tests/structure_function_calculators/test_bauer_2009b_calculator.py
 tests/tape_tests/structure_function_calculators/test_calculator_registrar.py
 tests/tape_tests/structure_function_calculators/test_light_curve.py
 tests/tape_tests/structure_function_calculators/test_macleod_2012_calculator.py
 tests/tape_tests/structure_function_calculators/test_schmidt_2010_calculator.py
```

### Comparing `lf-tape-0.4.0/src/tape/__init__.py` & `lf_tape-0.4.1/src/tape/__init__.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/base.py` & `lf_tape-0.4.1/src/tape/analysis/base.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/feature_extractor.py` & `lf_tape-0.4.1/src/tape/analysis/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/light_curve.py` & `lf_tape-0.4.1/src/tape/analysis/light_curve.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/stetsonj.py` & `lf_tape-0.4.1/src/tape/analysis/stetsonj.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/structure_function/__init__.py` & `lf_tape-0.4.1/src/tape/analysis/structure_function/__init__.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/structure_function/base_argument_container.py` & `lf_tape-0.4.1/src/tape/analysis/structure_function/base_argument_container.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/structure_function/base_calculator.py` & `lf_tape-0.4.1/src/tape/analysis/structure_function/base_calculator.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/structure_function/basic/calculator.py` & `lf_tape-0.4.1/src/tape/analysis/structure_function/basic/calculator.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/structure_function/bauer_2009a/calculator.py` & `lf_tape-0.4.1/src/tape/analysis/structure_function/bauer_2009a/calculator.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/structure_function/bauer_2009b/calculator.py` & `lf_tape-0.4.1/src/tape/analysis/structure_function/bauer_2009b/calculator.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/structure_function/calculator_registrar.py` & `lf_tape-0.4.1/src/tape/analysis/structure_function/calculator_registrar.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/structure_function/macleod_2012/calculator.py` & `lf_tape-0.4.1/src/tape/analysis/structure_function/macleod_2012/calculator.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/structure_function/schmidt_2010/calculator.py` & `lf_tape-0.4.1/src/tape/analysis/structure_function/schmidt_2010/calculator.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/structure_function/sf_light_curve.py` & `lf_tape-0.4.1/src/tape/analysis/structure_function/sf_light_curve.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/analysis/structurefunction2.py` & `lf_tape-0.4.1/src/tape/analysis/structurefunction2.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/ensemble.py` & `lf_tape-0.4.1/src/tape/ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import json
 import shutil
 import warnings
 import requests
 import lsdb
 import dask
+from dask_expr import from_legacy_dataframe
 
 import dask.dataframe as dd
 import numpy as np
 import pandas as pd
 
 from dask.distributed import Client
 from dask import config
@@ -812,15 +813,15 @@
                 band_counts = self.source.map_partitions(
                     lambda x: x.groupby(id_col)[[band_col]]
                     .value_counts()
                     .to_frame()
                     .reset_index()
                     .pivot_table(values=band_col, index=id_col, columns=band_col, aggfunc="sum"),
                     meta=meta,
-                ).repartition(divisions=self.object.divisions)
+                ).repartition(divisions=self.object.divisions, force=True)
             else:
                 band_counts = (
                     self.source.groupby([self._id_col])[self._band_col]  # group by each object
                     .value_counts()  # count occurence of each band
                     .to_frame()  # convert series to dataframe
                     .rename(columns={self._band_col: "counts"})  # rename column
                     .reset_index()  # break up the multiindex
@@ -848,15 +849,15 @@
                 # Grab these up front to help out the task graph
                 id_col = self._id_col
                 band_col = self._band_col
 
                 # Map the groupby to each partition
                 counts = self.source.map_partitions(
                     lambda x: x.groupby([id_col])[[band_col]].aggregate("count")
-                ).repartition(divisions=self.object.divisions)
+                ).repartition(divisions=self.object.divisions, force=True)
             else:
                 # Just do a groupby on all source
                 counts = (
                     self.source.groupby([self._id_col])[[self._band_col]]
                     .aggregate("count")
                     .repartition(npartitions=self.object.npartitions)
                 )
@@ -1717,15 +1718,15 @@
                     warnings.warn(
                         f" The sorted flag was set true with a non _hipscat_index id column ({column_mapper.map['id_col']}). This dataset is sorted by _hipscat_index, so the sorted flag has been turned off and sort has been turned on."
                     )
                     sorted = False
                     sort = True
 
             self.from_dask_dataframe(
-                source_catalog._ddf,
+                from_legacy_dataframe(source_catalog._ddf),
                 None,
                 column_mapper=column_mapper,
                 sync_tables=sync_tables,
                 sorted=sorted,
                 sort=sort,
                 npartitions=None,
                 partition_size=None,
@@ -1740,16 +1741,16 @@
                     f"With hipscat data, it's advised to use the _hipscat_index as the id_col (instead of {column_mapper.map['id_col']}), as the data is sorted using this column. If you'd like to use your chosen id column, make sure it's in both catalogs and use sort=True and sorted=False (these have been auto-set for this call)",
                     UserWarning,
                 )
                 sorted = False
                 sort = True
 
             self.from_dask_dataframe(
-                source_catalog._ddf,
-                object_catalog._ddf,
+                from_legacy_dataframe(source_catalog._ddf),
+                from_legacy_dataframe(object_catalog._ddf),
                 column_mapper=column_mapper,
                 sync_tables=sync_tables,
                 sorted=sorted,
                 sort=sort,
                 npartitions=None,
                 partition_size=None,
             )
@@ -2030,17 +2031,24 @@
             id_col=dataset_map["id"],
             time_col=dataset_map["time"],
             flux_col=dataset_map["flux"],
             err_col=dataset_map["error"],
             band_col=dataset_map["band"],
         )
 
-        return self.from_parquet(
-            source_file=dataset_info["source_file"],
-            object_file=dataset_info["object_file"],
+        # repartition and sort these demo datasets
+        src = dd.read_parquet(dataset_info["source_file"]).repartition(npartitions=4).persist()
+        obj = dd.read_parquet(dataset_info["object_file"]).repartition(npartitions=2).persist()
+
+        src = src.set_index(dataset_map["id"], sort=True)
+        obj = obj.set_index(dataset_map["id"], sort=True)
+
+        return self.from_dask_dataframe(
+            source_frame=src,
+            object_frame=obj,
             column_mapper=col_map,
             **kwargs,
         )
 
     def available_datasets(self):
         """Retrieve descriptions of available TAPE datasets.
```

### Comparing `lf-tape-0.4.0/src/tape/ensemble_frame.py` & `lf_tape-0.4.1/src/tape/ensemble_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -841,14 +841,54 @@
             npartitions=npartitions,
             partition_size=partition_size,
             freq=freq,
             force=force,
         )
         return self._propagate_metadata(result)
 
+    def head(self, n=5, compute=True, npartitions=None):
+        """Returns `n` rows of data for previewing purposes.
+
+        Parameters
+        ----------
+        n : int, optional
+            The number of desired rows. Default is 5.
+        compute : bool, optional
+            Whether to compute the result immediately. Default is True.
+        npartitions : int, optional
+            `npartitions` is not supported and if provided will be ignored. Instead all partitions may be used.
+
+        Returns:
+            A pandas DataFrame with up to `n` rows of data.
+        """
+        if npartitions is not None:
+            warnings.warn(
+                "The 'npartitions' parameter is not supported for TAPE dataframes. All partitions may be used."
+            )
+
+        if not compute:
+            # Just use the Dask head method
+            return super().head(n, compute=False)
+
+        if n <= 0:
+            return super().head(0)
+
+        # Iterate over the partitions until we have enough rows
+        dfs = []
+        remaining_rows = n
+        for partition in self.partitions:
+            if remaining_rows == 0:
+                break
+            # Note that partition is itself a _Frame object, so we need to compute to avoid infinite recursion
+            partition_head = partition.compute().head(remaining_rows)
+            dfs.append(partition_head)
+            remaining_rows -= len(partition_head)
+
+        return pd.concat(dfs)
+
 
 class EnsembleSeries(_Frame, dd.Series):
     """A barebones extension of a Dask Series for Ensemble data."""
 
     _partition_type = TapeSeries  # Tracks the underlying data type
```

### Comparing `lf-tape-0.4.0/src/tape/ensemble_readers.py` & `lf_tape-0.4.1/src/tape/ensemble_readers.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/timeseries.py` & `lf_tape-0.4.1/src/tape/timeseries.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/utils/column_mapper/column_mapper.py` & `lf_tape-0.4.1/src/tape/utils/column_mapper/column_mapper.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/src/tape/utils/utils.py` & `lf_tape-0.4.1/src/tape/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/conftest.py` & `lf_tape-0.4.1/tests/tape_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/object/test_object.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/object/test_object.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/_common_metadata` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/_metadata` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/point_map.fits` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/provenance_info.json` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_object_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/_common_metadata` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/_metadata` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/point_map.fits` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/provenance_info.json` & `lf_tape-0.4.1/tests/tape_tests/data/small_sky_hipscat/small_sky_source_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/data/source/test_source.parquet` & `lf_tape-0.4.1/tests/tape_tests/data/source/test_source.parquet`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_base_calculator.py` & `lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_base_calculator.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_bauer_2009a_calculator.py` & `lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_bauer_2009a_calculator.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_bauer_2009b_calculator.py` & `lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_bauer_2009b_calculator.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_calculator_registrar.py` & `lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_calculator_registrar.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_light_curve.py` & `lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_light_curve.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_macleod_2012_calculator.py` & `lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_macleod_2012_calculator.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_schmidt_2010_calculator.py` & `lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_schmidt_2010_calculator.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/structure_function_calculators/test_sf_light_curve.py` & `lf_tape-0.4.1/tests/tape_tests/structure_function_calculators/test_sf_light_curve.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/test_analysis.py` & `lf_tape-0.4.1/tests/tape_tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/test_ensemble.py` & `lf_tape-0.4.1/tests/tape_tests/test_ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -2050,19 +2050,32 @@
 
     # Verify that we preserved lightcurve cohesion
     assert parquet_ensemble.check_lightcurve_cohesion()
 
 
 @pytest.mark.parametrize("on", [None, ["ps1_objid", "filterName"], ["filterName", "ps1_objid"]])
 @pytest.mark.parametrize("func_label", ["mean", "bounds"])
-def test_batch_by_band(parquet_ensemble, func_label, on):
+def test_batch_by_band(func_label, on):
     """
     Test that ensemble.batch(by_band=True) works as intended.
     """
 
+    # TODO(wbeebe): This is a temporary workaround for https://github.com/lincc-frameworks/tape/issues/434 to avoid contention when reading data
+    # from the test files in parallel. This is the same as `parquet_ensemble` but uses copies of the parquet files referenced there.
+    parquet_ensemble = Ensemble(client=False)
+    parquet_ensemble.from_parquet(
+        "tests/tape_tests/data/source/test_source2.parquet",
+        "tests/tape_tests/data/object/test_object2.parquet",
+        id_col="ps1_objid",
+        time_col="midPointTai",
+        band_col="filterName",
+        flux_col="psFlux",
+        err_col="psFluxErr",
+    )
+
     if func_label == "mean":
 
         def my_mean(flux):
             """returns a single value"""
             return np.mean(flux)
 
         res = parquet_ensemble.batch(my_mean, parquet_ensemble._flux_col, on=on, by_band=True)
```

### Comparing `lf-tape-0.4.0/tests/tape_tests/test_ensemble_frame.py` & `lf_tape-0.4.1/tests/tape_tests/test_ensemble_frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Test EnsembleFrame (inherited from Dask.DataFrame) creation and manipulations. """
 
+from math import floor
 import numpy as np
 import pandas as pd
 from tape import (
     Ensemble,
     ColumnMapper,
 )
 
@@ -466,7 +467,65 @@
 
     # slice on source
     ens.source.partitions[0:2].update_ensemble()
     ens._lazy_sync_tables("all")  # sync needed as len() won't trigger one
 
     assert ens.source.npartitions == 2  # should return exactly 2 partitions
     assert len(ens.object) < prior_src_len  # should affect objects
+
+
+@pytest.mark.parametrize(
+    "data_fixture",
+    [
+        "parquet_ensemble",
+        "parquet_ensemble_with_divisions",
+    ],
+)
+def test_head(data_fixture, request):
+    """
+    Tests that head returns the correct number of rows.
+    """
+    ens = request.getfixturevalue(data_fixture)
+
+    # Test witht repartitioning the source frame
+    frame = ens.source
+    frame = frame.repartition(npartitions=10)
+
+    assert frame.npartitions == 10
+
+    # Check that a warning is raised when npartitions are requested.
+    with pytest.warns(UserWarning):
+        frame.head(5, npartitions=5)
+
+    # Test inputs that should return an empty frame
+    assert len(frame.head(-100)) == 0
+    assert len(frame.head(0)) == 0
+    assert len(frame.head(-1)) == 0
+
+    assert len(frame.head(100, compute=False).compute()) == 100
+
+    one_res = frame.head(1)
+    assert len(one_res) == 1
+    assert isinstance(one_res, TapeFrame)
+    assert set(one_res.columns) == set(frame.columns)
+
+    def_result = frame.head()
+    assert len(def_result) == 5
+    assert isinstance(one_res, TapeFrame)
+    assert set(one_res.columns) == set(frame.columns)
+
+    def_result = frame.head(24)
+    assert len(def_result) == 24
+    assert isinstance(one_res, TapeFrame)
+    assert set(one_res.columns) == set(frame.columns)
+
+    # Test that we have sane behavior even when the number of rows requested is larger than the number of rows in the frame.
+    assert len(frame.head(2 * len(frame))) == len(frame)
+
+    # Choose a value that will be guaranteed to hit every partition for this data.
+    # Note that with parquet_ensemble_with_divisions some of the partitions are empty
+    # testing that as well.
+    rows = floor(len(frame.compute()) * 0.98)
+    result = frame.head(rows)
+    assert len(result) == rows
+    assert isinstance(result, TapeFrame)
+    assert set(result.columns) == set(frame.columns)
```

### Comparing `lf-tape-0.4.0/tests/tape_tests/test_feature_extraction.py` & `lf_tape-0.4.1/tests/tape_tests/test_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/test_timeseries.py` & `lf_tape-0.4.1/tests/tape_tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `lf-tape-0.4.0/tests/tape_tests/test_utils.py` & `lf_tape-0.4.1/tests/tape_tests/test_utils.py`

 * *Files identical despite different names*

