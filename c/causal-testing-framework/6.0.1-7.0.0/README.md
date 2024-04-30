# Comparing `tmp/causal_testing_framework-6.0.1.tar.gz` & `tmp/causal_testing_framework-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causal_testing_framework-6.0.1.tar", last modified: Mon Mar 18 14:33:15 2024, max compression
+gzip compressed data, was "causal_testing_framework-7.0.0.tar", last modified: Tue Apr 30 15:43:49 2024, max compression
```

## Comparing `causal_testing_framework-6.0.1.tar` & `causal_testing_framework-7.0.0.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.484004 causal_testing_framework-6.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.448004 causal_testing_framework-6.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.452004 causal_testing_framework-6.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.452004 causal_testing_framework-6.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/.github/workflows/ci-tests-drafts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/.github/workflows/ci-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/.github/workflows/figshare.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/.github/workflows/lint-format.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/.github/workflows/publish-to-dafni.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/.mega-linter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    20375 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-03-18 14:33:15.484004 causal_testing_framework-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.452004 causal_testing_framework-6.0.1/causal_testing/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.452004 causal_testing_framework-6.0.1/causal_testing/data_collection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/data_collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/data_collection/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.452004 causal_testing_framework-6.0.1/causal_testing/generation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/generation/abstract_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/generation/enum_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.452004 causal_testing_framework-6.0.1/causal_testing/json_front/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/json_front/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20805 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/json_front/json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.456004 causal_testing_framework-6.0.1/causal_testing/specification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28137 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/specification/causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/specification/causal_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/specification/metamorphic_relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/specification/scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/specification/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.456004 causal_testing_framework-6.0.1/causal_testing/surrogate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/surrogate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/surrogate/causal_surrogate_assisted.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/surrogate/surrogate_search_algorithms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.456004 causal_testing_framework-6.0.1/causal_testing/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/testing/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/testing/causal_test_adequacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/testing/causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/testing/causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/testing/causal_test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/testing/causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/testing/effect.py
--rw-r--r--   0 runner    (1001) docker     (127)    31651 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/testing/estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/testing/intervention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.456004 causal_testing_framework-6.0.1/causal_testing/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/causal_testing/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.480004 causal_testing_framework-6.0.1/causal_testing_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-03-18 14:33:15.000000 causal_testing_framework-6.0.1/causal_testing_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-03-18 14:33:15.000000 causal_testing_framework-6.0.1/causal_testing_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 14:33:15.000000 causal_testing_framework-6.0.1/causal_testing_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-18 14:33:15.000000 causal_testing_framework-6.0.1/causal_testing_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-18 14:33:15.000000 causal_testing_framework-6.0.1/causal_testing_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.460004 causal_testing_framework-6.0.1/dafni/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/dafni/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/dafni/.env
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/dafni/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/dafni/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.444004 causal_testing_framework-6.0.1/dafni/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.460004 causal_testing_framework-6.0.1/dafni/data/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/dafni/data/inputs/causal_tests.json
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/dafni/data/inputs/dag.dot
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/dafni/data/inputs/runtime_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/dafni/data/inputs/variables.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.460004 causal_testing_framework-6.0.1/dafni/data/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/dafni/data/outputs/causal_tests_results.json
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/dafni/docker-compose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6958 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/dafni/main_dafni.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/dafni/model_definition.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.460004 causal_testing_framework-6.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.464004 causal_testing_framework-6.0.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.444004 causal_testing_framework-6.0.1/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.464004 causal_testing_framework-6.0.1/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.464004 causal_testing_framework-6.0.1/docs/source/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    20244 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/_static/images/CITCOM-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/credits.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/description.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.464004 causal_testing_framework-6.0.1/docs/source/dev/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/dev/actions_and_webhooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/dev/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/dev/version_release.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.464004 causal_testing_framework-6.0.1/docs/source/frontends/
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/frontends/json_front_end.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/frontends/test_suite.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/glossary.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.464004 causal_testing_framework-6.0.1/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (127)   184134 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.464004 causal_testing_framework-6.0.1/docs/source/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/modules/causal_specification.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/modules/causal_tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/modules/data_collector.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.464004 causal_testing_framework-6.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.444004 causal_testing_framework-6.0.1/examples/covasim_/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.468004 causal_testing_framework-6.0.1/examples/covasim_/doubling_beta/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/covasim_/doubling_beta/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/covasim_/doubling_beta/dag.dot
--rw-r--r--   0 runner    (1001) docker     (127)    24596 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/covasim_/doubling_beta/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.468004 causal_testing_framework-6.0.1/examples/covasim_/doubling_beta/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1355776 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/covasim_/doubling_beta/data/10k_observational_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)    15579 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/covasim_/doubling_beta/example_beta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.468004 causal_testing_framework-6.0.1/examples/covasim_/vaccinating_elderly/
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/covasim_/vaccinating_elderly/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/covasim_/vaccinating_elderly/dag.dot
--rw-r--r--   0 runner    (1001) docker     (127)    23290 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/covasim_/vaccinating_elderly/dag.png
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/covasim_/vaccinating_elderly/example_vaccine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/covasim_/vaccinating_elderly/simulated_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.472004 causal_testing_framework-6.0.1/examples/lr91/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/lr91/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/lr91/dag.dot
--rw-r--r--   0 runner    (1001) docker     (127)    73886 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/lr91/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.472004 causal_testing_framework-6.0.1/examples/lr91/data/
--rw-r--r--   0 runner    (1001) docker     (127)    40715 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/lr91/data/normalised_results.csv
--rw-r--r--   0 runner    (1001) docker     (127)    40686 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/lr91/data/results.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/lr91/example_max_conductances.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/lr91/example_max_conductances_test_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.472004 causal_testing_framework-6.0.1/examples/poisson/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson/causal_tests.json
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson/dag.dot
--rw-r--r--   0 runner    (1001) docker     (127)    61017 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson/data.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson/example_run_causal_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.472004 causal_testing_framework-6.0.1/examples/poisson-line-process/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/dag.dot
--rw-r--r--   0 runner    (1001) docker     (127)    53765 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.448004 causal_testing_framework-6.0.1/examples/poisson-line-process/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.472004 causal_testing_framework-6.0.1/examples/poisson-line-process/data/random/
--rw-r--r--   0 runner    (1001) docker     (127)   102007 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/data/random/data_random_1000.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.476004 causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/
--rw-r--r--   0 runner    (1001) docker     (127)    15080 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
--rw-r--r--   0 runner    (1001) docker     (127)    24851 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
--rw-r--r--   0 runner    (1001) docker     (127)    14925 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
--rw-r--r--   0 runner    (1001) docker     (127)    13682 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
--rw-r--r--   0 runner    (1001) docker     (127)    25451 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
--rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
--rw-r--r--   0 runner    (1001) docker     (127)    26889 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/examples/poisson-line-process/example_poisson_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.476004 causal_testing_framework-6.0.1/images/
--rw-r--r--   0 runner    (1001) docker     (127)   184134 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 14:33:15.484004 causal_testing_framework-6.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.476004 causal_testing_framework-6.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.476004 causal_testing_framework-6.0.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   374288 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/data/nhefs.csv
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/data/scarf_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.476004 causal_testing_framework-6.0.1/tests/data_collection_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/data_collection_tests/test_observational_data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.476004 causal_testing_framework-6.0.1/tests/generation_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/generation_tests/test_abstract_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.476004 causal_testing_framework-6.0.1/tests/json_front_tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/json_front_tests/test_json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.448004 causal_testing_framework-6.0.1/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.480004 causal_testing_framework-6.0.1/tests/resources/data/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/resources/data/dag.dot
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/resources/data/data.csv
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/resources/data/data_with_categorical.csv
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/resources/data/data_with_meta.csv
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/resources/data/tests.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.480004 causal_testing_framework-6.0.1/tests/specification_tests/
--rw-r--r--   0 runner    (1001) docker     (127)    19329 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/specification_tests/test_causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/specification_tests/test_metamorphic_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/specification_tests/test_variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.480004 causal_testing_framework-6.0.1/tests/surrogate_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8710 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/surrogate_tests/test_causal_surrogate_assisted.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:33:15.480004 causal_testing_framework-6.0.1/tests/testing_tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/testing_tests/test_causal_test_adequacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/testing_tests/test_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/testing_tests/test_causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/testing_tests/test_causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-03-18 14:32:07.000000 causal_testing_framework-6.0.1/tests/testing_tests/test_estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.468982 causal_testing_framework-7.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.436982 causal_testing_framework-7.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.436982 causal_testing_framework-7.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.440982 causal_testing_framework-7.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/.github/workflows/ci-tests-drafts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/.github/workflows/ci-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/.github/workflows/figshare.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/.github/workflows/lint-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/.github/workflows/publish-to-dafni.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/.mega-linter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    20375 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-04-30 15:43:49.464982 causal_testing_framework-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.440982 causal_testing_framework-7.0.0/causal_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.440982 causal_testing_framework-7.0.0/causal_testing/data_collection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/data_collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/data_collection/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.440982 causal_testing_framework-7.0.0/causal_testing/generation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/generation/abstract_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/generation/enum_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.440982 causal_testing_framework-7.0.0/causal_testing/json_front/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/json_front/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/json_front/json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.440982 causal_testing_framework-7.0.0/causal_testing/specification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28137 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/specification/causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/specification/causal_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/specification/metamorphic_relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/specification/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/specification/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.440982 causal_testing_framework-7.0.0/causal_testing/surrogate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/surrogate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/surrogate/causal_surrogate_assisted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/surrogate/surrogate_search_algorithms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.444982 causal_testing_framework-7.0.0/causal_testing/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/testing/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/testing/causal_test_adequacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/testing/causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/testing/causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/testing/causal_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/testing/causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/testing/effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26390 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/testing/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/testing/intervention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.444982 causal_testing_framework-7.0.0/causal_testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/causal_testing/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.464982 causal_testing_framework-7.0.0/causal_testing_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-04-30 15:43:49.000000 causal_testing_framework-7.0.0/causal_testing_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-30 15:43:49.000000 causal_testing_framework-7.0.0/causal_testing_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:43:49.000000 causal_testing_framework-7.0.0/causal_testing_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-30 15:43:49.000000 causal_testing_framework-7.0.0/causal_testing_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 15:43:49.000000 causal_testing_framework-7.0.0/causal_testing_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.444982 causal_testing_framework-7.0.0/dafni/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/dafni/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/dafni/.env
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/dafni/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/dafni/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.432983 causal_testing_framework-7.0.0/dafni/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.448982 causal_testing_framework-7.0.0/dafni/data/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/dafni/data/inputs/causal_tests.json
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/dafni/data/inputs/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/dafni/data/inputs/runtime_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/dafni/data/inputs/variables.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.448982 causal_testing_framework-7.0.0/dafni/data/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/dafni/data/outputs/causal_tests_results.json
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/dafni/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6958 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/dafni/main_dafni.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/dafni/model_definition.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.448982 causal_testing_framework-7.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.448982 causal_testing_framework-7.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.432983 causal_testing_framework-7.0.0/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.448982 causal_testing_framework-7.0.0/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.448982 causal_testing_framework-7.0.0/docs/source/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20244 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/_static/images/CITCOM-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/description.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.448982 causal_testing_framework-7.0.0/docs/source/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/dev/actions_and_webhooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/dev/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/dev/version_release.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.448982 causal_testing_framework-7.0.0/docs/source/frontends/
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/frontends/json_front_end.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/frontends/test_suite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.452982 causal_testing_framework-7.0.0/docs/source/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/modules/causal_specification.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/modules/causal_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/modules/data_collector.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.452982 causal_testing_framework-7.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.432983 causal_testing_framework-7.0.0/examples/covasim_/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.452982 causal_testing_framework-7.0.0/examples/covasim_/doubling_beta/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/covasim_/doubling_beta/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/covasim_/doubling_beta/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (127)    24596 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/covasim_/doubling_beta/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.452982 causal_testing_framework-7.0.0/examples/covasim_/doubling_beta/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1355776 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15579 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/covasim_/doubling_beta/example_beta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.452982 causal_testing_framework-7.0.0/examples/covasim_/vaccinating_elderly/
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/covasim_/vaccinating_elderly/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/covasim_/vaccinating_elderly/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (127)    23290 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/covasim_/vaccinating_elderly/dag.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/covasim_/vaccinating_elderly/example_vaccine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/covasim_/vaccinating_elderly/simulated_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.456982 causal_testing_framework-7.0.0/examples/lr91/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/lr91/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/lr91/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (127)    73886 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/lr91/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.456982 causal_testing_framework-7.0.0/examples/lr91/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    40715 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/lr91/data/normalised_results.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    40686 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/lr91/data/results.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/lr91/example_max_conductances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/lr91/example_max_conductances_test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.456982 causal_testing_framework-7.0.0/examples/poisson/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson/causal_tests.json
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (127)    61017 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson/data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson/example_run_causal_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.456982 causal_testing_framework-7.0.0/examples/poisson-line-process/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (127)    53765 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.436982 causal_testing_framework-7.0.0/examples/poisson-line-process/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.456982 causal_testing_framework-7.0.0/examples/poisson-line-process/data/random/
+-rw-r--r--   0 runner    (1001) docker     (127)   102007 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/data/random/data_random_1000.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.460982 causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/
+-rw-r--r--   0 runner    (1001) docker     (127)    15080 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    24851 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14925 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13682 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    25451 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    26889 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/examples/poisson-line-process/example_poisson_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.460982 causal_testing_framework-7.0.0/images/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/images/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    59744 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/images/schematic-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55989 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/images/schematic.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/images/schematic.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:43:49.468982 causal_testing_framework-7.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.460982 causal_testing_framework-7.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.460982 causal_testing_framework-7.0.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   374288 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/data/nhefs.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/data/scarf_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.460982 causal_testing_framework-7.0.0/tests/data_collection_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/data_collection_tests/test_observational_data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.460982 causal_testing_framework-7.0.0/tests/generation_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/generation_tests/test_abstract_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.460982 causal_testing_framework-7.0.0/tests/json_front_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14101 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/json_front_tests/test_json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.436982 causal_testing_framework-7.0.0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.464982 causal_testing_framework-7.0.0/tests/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/resources/data/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/resources/data/data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/resources/data/data_with_categorical.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/resources/data/data_with_meta.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/resources/data/tests.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.464982 causal_testing_framework-7.0.0/tests/specification_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19331 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/specification_tests/test_causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13891 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/specification_tests/test_metamorphic_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/specification_tests/test_variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.464982 causal_testing_framework-7.0.0/tests/surrogate_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/surrogate_tests/test_causal_surrogate_assisted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:43:49.464982 causal_testing_framework-7.0.0/tests/testing_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/testing_tests/test_causal_test_adequacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/testing_tests/test_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/testing_tests/test_causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/testing_tests/test_causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18701 2024-04-30 15:43:09.000000 causal_testing_framework-7.0.0/tests/testing_tests/test_estimators.py
```

### Comparing `causal_testing_framework-6.0.1/.github/CONTRIBUTING.md` & `causal_testing_framework-7.0.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `causal_testing_framework-7.0.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `causal_testing_framework-7.0.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/.github/workflows/ci-tests-drafts.yaml` & `causal_testing_framework-7.0.0/.github/workflows/ci-tests-drafts.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   build:
     if: github.event.pull_request.draft == true
     name: Ex1 (${{ matrix.python-version }}, ${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: ["ubuntu-latest", "windows-latest", "macos-latest"]
-        python-version: ["3.9"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python using Miniconda
         uses: conda-incubator/setup-miniconda@v2
         with:
           auto-update-conda: true
           python-version: ${{ matrix.python-version }}
```

### Comparing `causal_testing_framework-6.0.1/.github/workflows/ci-tests.yaml` & `causal_testing_framework-7.0.0/.github/workflows/ci-tests.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   build:
     if: github.event.pull_request.draft == false # Filter out draft PRs
     name: Ex1 (${{ matrix.python-version }}, ${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: ["ubuntu-latest", "windows-latest", "macos-latest"]
-        python-version: ["3.9"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python using Miniconda
         uses: conda-incubator/setup-miniconda@v2
         with:
           auto-update-conda: true
           python-version: ${{ matrix.python-version }}
```

### Comparing `causal_testing_framework-6.0.1/.github/workflows/figshare.yaml` & `causal_testing_framework-7.0.0/.github/workflows/figshare.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/.github/workflows/lint-format.yaml` & `causal_testing_framework-7.0.0/.github/workflows/lint-format.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/.github/workflows/publish-to-pypi.yaml` & `causal_testing_framework-7.0.0/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/.gitignore` & `causal_testing_framework-7.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/.pylintrc` & `causal_testing_framework-7.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/.readthedocs.yaml` & `causal_testing_framework-7.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/LICENSE` & `causal_testing_framework-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/causal_testing/data_collection/data_collector.py` & `causal_testing_framework-7.0.0/causal_testing/data_collection/data_collector.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/causal_testing/generation/abstract_causal_test_case.py` & `causal_testing_framework-7.0.0/causal_testing/generation/abstract_causal_test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module contains the class AbstractCausalTestCase, which generates concrete test cases"""
+
 import itertools
 import logging
 from enum import Enum
 from typing import Iterable
 
 import lhsmdu
 import pandas as pd
```

### Comparing `causal_testing_framework-6.0.1/causal_testing/generation/enum_gen.py` & `causal_testing_framework-7.0.0/causal_testing/generation/enum_gen.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/causal_testing/json_front/json_class.py` & `causal_testing_framework-7.0.0/causal_testing/json_front/json_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,17 +104,17 @@
             scenario=self.scenario,
             intervention_constraints=[mutates[v](k) for k, v in test["mutations"].items()],
             treatment_variable=treatment_var,
             expected_causal_effect={
                 self.scenario.variables[variable]: effects[effect]
                 for variable, effect in test["expected_effect"].items()
             },
-            effect_modifiers={self.scenario.variables[v] for v in test["effect_modifiers"]}
-            if "effect_modifiers" in test
-            else {},
+            effect_modifiers=(
+                {self.scenario.variables[v] for v in test["effect_modifiers"]} if "effect_modifiers" in test else {}
+            ),
             estimate_type=test["estimate_type"],
             effect=test.get("effect", "total"),
         )
         return abstract_test
 
     def run_json_tests(self, effects: dict, estimators: dict, f_flag: bool = False, mutates: dict = None):
         """Runs and evaluates each test case specified in the JSON input
```

### Comparing `causal_testing_framework-6.0.1/causal_testing/specification/causal_dag.py` & `causal_testing_framework-7.0.0/causal_testing/specification/causal_dag.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/causal_testing/specification/causal_specification.py` & `causal_testing_framework-7.0.0/causal_testing/specification/causal_specification.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/causal_testing/specification/metamorphic_relation.py` & `causal_testing_framework-7.0.0/causal_testing/specification/metamorphic_relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,17 +69,19 @@
                 str(self),
             )
             for source_inputs, follow_up_inputs, other_inputs in zip(
                 source_follow_up_test_inputs[[self.treatment_var]].to_dict(orient="records"),
                 source_follow_up_test_inputs[[follow_up_input]]
                 .rename(columns={follow_up_input: self.treatment_var})
                 .to_dict(orient="records"),
-                test_inputs.to_dict(orient="records")
-                if not test_inputs.empty
-                else [{}] * len(source_follow_up_test_inputs),
+                (
+                    test_inputs.to_dict(orient="records")
+                    if not test_inputs.empty
+                    else [{}] * len(source_follow_up_test_inputs)
+                ),
             )
         ]
 
     def execute_tests(self, data_collector: ExperimentalDataCollector):
         """Execute the generated list of metamorphic tests, returning a dictionary of tests that pass and fail.
 
         :param data_collector: An experimental data collector for the system-under-test.
```

### Comparing `causal_testing_framework-6.0.1/causal_testing/specification/scenario.py` & `causal_testing_framework-7.0.0/causal_testing/specification/scenario.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module holds the Scenario Class"""
+
 from collections.abc import Iterable, Mapping
 
 from tabulate import tabulate
 from z3 import ExprRef, substitute
 
 from .variable import Input, Meta, Output, Variable
```

### Comparing `causal_testing_framework-6.0.1/causal_testing/specification/variable.py` & `causal_testing_framework-7.0.0/causal_testing/specification/variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/causal_testing/surrogate/causal_surrogate_assisted.py` & `causal_testing_framework-7.0.0/causal_testing/surrogate/causal_surrogate_assisted.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/causal_testing/surrogate/surrogate_search_algorithms.py` & `causal_testing_framework-7.0.0/causal_testing/surrogate/surrogate_search_algorithms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing implementation of search algorithm for surrogate search """
+
 # Fitness functions are required to be iteratively defined, including all variables within.
 
 from operator import itemgetter
 from pygad import GA
 
 from causal_testing.specification.causal_specification import CausalSpecification
 from causal_testing.testing.estimators import CubicSplineRegressionEstimator
```

### Comparing `causal_testing_framework-6.0.1/causal_testing/testing/base_test_case.py` & `causal_testing_framework-7.0.0/causal_testing/testing/base_test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module contains the BaseTestCase dataclass, which stores the information required for identification"""
+
 from dataclasses import dataclass
 from causal_testing.specification.variable import Variable
 from causal_testing.testing.effect import Effect
 
 
 @dataclass(frozen=True)
 class BaseTestCase:
```

### Comparing `causal_testing_framework-6.0.1/causal_testing/testing/causal_test_adequacy.py` & `causal_testing_framework-7.0.0/causal_testing/testing/causal_test_adequacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This module contains code to measure various aspects of causal test adequacy.
 """
+
 from itertools import combinations
 from copy import deepcopy
 import pandas as pd
 
 from causal_testing.testing.causal_test_suite import CausalTestSuite
 from causal_testing.data_collection.data_collector import DataCollector
 from causal_testing.specification.causal_dag import CausalDAG
```

### Comparing `causal_testing_framework-6.0.1/causal_testing/testing/causal_test_case.py` & `causal_testing_framework-7.0.0/causal_testing/testing/causal_test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module contains the CausalTestCase class, a class that holds the information required for a causal test"""
+
 import logging
 from typing import Any
 import numpy as np
 
 from causal_testing.specification.variable import Variable
 from causal_testing.testing.causal_test_outcome import CausalTestOutcome
 from causal_testing.testing.base_test_case import BaseTestCase
```

### Comparing `causal_testing_framework-6.0.1/causal_testing/testing/causal_test_outcome.py` & `causal_testing_framework-7.0.0/causal_testing/testing/causal_test_outcome.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/causal_testing/testing/causal_test_result.py` & `causal_testing_framework-7.0.0/causal_testing/testing/causal_test_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module contains the CausalTestResult class, which is a container for the results of a causal test, and the
 TestValue dataclass.
 """
+
 from typing import Any
 from dataclasses import dataclass
 import pandas as pd
 
 from causal_testing.testing.estimators import Estimator
 from causal_testing.specification.variable import Variable
 
@@ -82,17 +83,19 @@
         base_dict = {
             "treatment": self.estimator.treatment,
             "control_value": self.estimator.control_value,
             "treatment_value": self.estimator.treatment_value,
             "outcome": self.estimator.outcome,
             "adjustment_set": list(self.adjustment_set) if json else self.adjustment_set,
             "effect_measure": self.test_value.type,
-            "effect_estimate": self.test_value.value.to_dict()
-            if json and hasattr(self.test_value.value, "to_dict")
-            else self.test_value.value,
+            "effect_estimate": (
+                self.test_value.value.to_dict()
+                if json and hasattr(self.test_value.value, "to_dict")
+                else self.test_value.value
+            ),
             "ci_low": self.ci_low().to_dict() if json and hasattr(self.ci_low(), "to_dict") else self.ci_low(),
             "ci_high": self.ci_high().to_dict() if json and hasattr(self.ci_high(), "to_dict") else self.ci_high(),
         }
         if self.adequacy:
             base_dict["adequacy"] = self.adequacy.to_dict()
         return base_dict
```

### Comparing `causal_testing_framework-6.0.1/causal_testing/testing/causal_test_suite.py` & `causal_testing_framework-7.0.0/causal_testing/testing/causal_test_suite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """This module contains the CausalTestSuite class, for details on using it:
 https://causal-testing-framework.readthedocs.io/en/latest/test_suite.html"""
+
 import logging
 
 from collections import UserDict
 from typing import Type, Iterable
 from causal_testing.testing.base_test_case import BaseTestCase
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.estimators import Estimator
```

### Comparing `causal_testing_framework-6.0.1/causal_testing/testing/estimators.py` & `causal_testing_framework-7.0.0/causal_testing/testing/estimators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """This module contains the Estimator abstract class, as well as its concrete extensions: LogisticRegressionEstimator,
-LinearRegressionEstimator and CausalForestEstimator"""
+LinearRegressionEstimator"""
+
 import logging
 from abc import ABC, abstractmethod
 from typing import Any
 from math import ceil
 
 import numpy as np
 import pandas as pd
 import statsmodels.api as sm
 import statsmodels.formula.api as smf
-from econml.dml import CausalForestDML
 from patsy import dmatrix  # pylint: disable = no-name-in-module
 from patsy import ModelDesc
-from sklearn.ensemble import GradientBoostingRegressor
 from statsmodels.regression.linear_model import RegressionResultsWrapper
 from statsmodels.tools.sm_exceptions import PerfectSeparationError
 
 from causal_testing.specification.variable import Variable
 
 logger = logging.getLogger(__name__)
 
@@ -348,22 +347,24 @@
         caused by a unit change in treatment.
 
         :return: The unit average treatment effect and the 95% Wald confidence intervals.
         """
         model = self._run_linear_regression()
         newline = "\n"
         patsy_md = ModelDesc.from_formula(self.treatment)
+
         if any(
             (
                 self.df.dtypes[factor.name()] == "object"
                 for factor in patsy_md.rhs_termlist[1].factors
                 # We want to remove this long term as it prevents us from discovering categoricals within I(...) blocks
                 if factor.name() in self.df.dtypes
             )
         ):
+
             design_info = dmatrix(self.formula.split("~")[1], self.df).design_info
             treatment = design_info.column_names[design_info.term_name_slices[self.treatment]]
         else:
             treatment = [self.treatment]
         assert set(treatment).issubset(
             model.params.index.tolist()
         ), f"{treatment} not in\n{'  ' + str(model.params.index).replace(newline, newline + '  ')}"
@@ -594,105 +595,7 @@
             [self.estimate_iv_coefficient(self.df.sample(len(self.df), replace=True)) for _ in range(bootstrap_size)]
         )
         bound = ceil((bootstrap_size * self.alpha) / 2)
         ci_low = pd.Series(bootstraps[bound])
         ci_high = pd.Series(bootstraps[bootstrap_size - bound])
 
         return pd.Series(self.estimate_iv_coefficient(self.df)), [ci_low, ci_high]
-
-
-class CausalForestEstimator(Estimator):
-    """A causal random forest estimator is a non-parametric estimator which recursively partitions the covariate space
-    to learn a low-dimensional representation of treatment effect heterogeneity. This form of estimator is best suited
-    to the estimation of heterogeneous treatment effects i.e. the estimated effect for every sample rather than the
-    population average.
-    """
-
-    def add_modelling_assumptions(self):
-        """Add any modelling assumptions to the estimator.
-
-        :return self: Update self.modelling_assumptions
-        """
-        self.modelling_assumptions.append("Non-parametric estimator: no restrictions imposed on the data.")
-
-    def estimate_ate(self) -> tuple[pd.Series, list[pd.Series, pd.Series]]:
-        """Estimate the average treatment effect.
-
-        :return ate, confidence_intervals: The average treatment effect and 95% confidence intervals.
-        """
-        # Remove any NA containing rows
-        reduced_df = self.df.copy()
-        necessary_cols = [self.treatment] + list(self.adjustment_set) + [self.outcome]
-        missing_rows = reduced_df[necessary_cols].isnull().any(axis=1)
-        reduced_df = reduced_df[~missing_rows]
-
-        # Split data into effect modifiers (X), confounders (W), treatments (T), and outcome (Y)
-        if self.effect_modifiers:
-            effect_modifier_df = reduced_df[list(self.effect_modifiers)]
-        else:
-            effect_modifier_df = reduced_df[list(self.adjustment_set)]
-        confounders_df = reduced_df[list(self.adjustment_set)]
-        treatment_df = np.ravel(reduced_df[[self.treatment]])
-        outcome_df = np.ravel(reduced_df[[self.outcome]])
-
-        # Fit the model to the data using a gradient boosting regressor for both the treatment and outcome model
-        model = CausalForestDML(
-            model_y=GradientBoostingRegressor(),
-            model_t=GradientBoostingRegressor(),
-        )
-        model.fit(outcome_df, treatment_df, X=effect_modifier_df, W=confounders_df)
-
-        # Obtain the ATE and 95% confidence intervals
-        ate = pd.Series(model.ate(effect_modifier_df, T0=self.control_value, T1=self.treatment_value))
-        ate_interval = model.ate_interval(effect_modifier_df, T0=self.control_value, T1=self.treatment_value)
-        ci_low, ci_high = pd.Series(ate_interval[0]), pd.Series(ate_interval[1])
-        return ate, [ci_low, ci_high]
-
-    def estimate_cates(self) -> pd.DataFrame:
-        """Estimate the conditional average treatment effect for each sample in the data as a function of a set of
-        covariates (X) i.e. effect modifiers. That is, the predicted change in outcome caused by the intervention
-        (change in treatment from control to treatment value) for every execution of the system-under-test, taking into
-        account the value of each effect modifier X. As a result, for every unique setting of the set of covariates X,
-        we expect a different CATE.
-
-        :return results_df: A dataframe containing a conditional average treatment effect, 95% confidence intervals, and
-        the covariate (effect modifier) values for each sample.
-        """
-
-        # Remove any NA containing rows
-        reduced_df = self.df.copy()
-        necessary_cols = [self.treatment] + list(self.adjustment_set) + [self.outcome]
-        missing_rows = reduced_df[necessary_cols].isnull().any(axis=1)
-        reduced_df = reduced_df[~missing_rows]
-
-        # Split data into effect modifiers (X), confounders (W), treatments (T), and outcome (Y)
-        if self.effect_modifiers:
-            effect_modifier_df = reduced_df[list(self.effect_modifiers)]
-        else:
-            raise ValueError("CATE requires the user to define a set of effect modifiers.")
-
-        if self.adjustment_set:
-            confounders_df = reduced_df[list(self.adjustment_set)]
-        else:
-            confounders_df = None
-        treatment_df = reduced_df[[self.treatment]]
-        outcome_df = reduced_df[[self.outcome]]
-
-        # Fit a model to the data
-        model = CausalForestDML(model_y=GradientBoostingRegressor(), model_t=GradientBoostingRegressor())
-        model.fit(outcome_df, treatment_df, X=effect_modifier_df, W=confounders_df)
-
-        # Obtain CATES and confidence intervals
-        conditional_ates = model.effect(effect_modifier_df, T0=self.control_value, T1=self.treatment_value).flatten()
-        [ci_low, ci_high] = model.effect_interval(
-            effect_modifier_df, T0=self.control_value, T1=self.treatment_value, alpha=self.alpha
-        )
-
-        # Merge results into a dataframe (CATE, confidence intervals, and effect modifier values)
-        results_df = pd.DataFrame(columns=["cate", "ci_low", "ci_high"])
-        results_df["cate"] = list(conditional_ates)
-        results_df["ci_low"] = list(ci_low.flatten())
-        results_df["ci_high"] = list(ci_high.flatten())
-        effect_modifier_df.reset_index(drop=True, inplace=True)
-        results_df[list(self.effect_modifiers)] = effect_modifier_df
-        results_df.sort_values(by=list(self.effect_modifiers), inplace=True)
-        return results_df, None
```

### Comparing `causal_testing_framework-6.0.1/causal_testing/testing/intervention.py` & `causal_testing_framework-7.0.0/causal_testing/testing/intervention.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/causal_testing/utils/validation.py` & `causal_testing_framework-7.0.0/causal_testing/utils/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module contains the CausalValidator class for performing Quantitive Bias Analysis techniques"""
+
 import math
 import numpy as np
 from scipy.stats import t
 from statsmodels.regression.linear_model import RegressionResultsWrapper
 
 
 class CausalValidator:
```

### Comparing `causal_testing_framework-6.0.1/causal_testing_framework.egg-info/SOURCES.txt` & `causal_testing_framework-7.0.0/causal_testing_framework.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 docs/source/_static/css/custom.css
 docs/source/_static/images/CITCOM-logo.png
 docs/source/dev/actions_and_webhooks.rst
 docs/source/dev/documentation.rst
 docs/source/dev/version_release.rst
 docs/source/frontends/json_front_end.rst
 docs/source/frontends/test_suite.rst
-docs/source/images/workflow.png
 docs/source/modules/causal_specification.rst
 docs/source/modules/causal_tests.rst
 docs/source/modules/data_collector.rst
 examples/.gitignore
 examples/covasim_/doubling_beta/README.md
 examples/covasim_/doubling_beta/dag.dot
 examples/covasim_/doubling_beta/dag.png
@@ -118,17 +117,19 @@
 examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
 examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
 examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
 examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
 examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
 examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
 examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
-images/workflow.png
+images/.gitignore
+images/schematic-dark.png
+images/schematic.png
+images/schematic.tex
 tests/__init__.py
-tests/test_helpers.py
 tests/data/nhefs.csv
 tests/data/scarf_data.csv
 tests/data_collection_tests/test_observational_data_collector.py
 tests/generation_tests/test_abstract_test_case.py
 tests/json_front_tests/test_json_class.py
 tests/resources/data/dag.dot
 tests/resources/data/data.csv
```

### Comparing `causal_testing_framework-6.0.1/dafni/Dockerfile` & `causal_testing_framework-7.0.0/dafni/Dockerfile`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/dafni/README.md` & `causal_testing_framework-7.0.0/dafni/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/dafni/data/inputs/causal_tests.json` & `causal_testing_framework-7.0.0/dafni/data/inputs/causal_tests.json`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/dafni/data/inputs/runtime_data.csv` & `causal_testing_framework-7.0.0/dafni/data/inputs/runtime_data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/dafni/data/inputs/variables.json` & `causal_testing_framework-7.0.0/dafni/data/inputs/variables.json`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/dafni/data/outputs/causal_tests_results.json` & `causal_testing_framework-7.0.0/dafni/data/outputs/causal_tests_results.json`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/dafni/main_dafni.py` & `causal_testing_framework-7.0.0/dafni/main_dafni.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/dafni/model_definition.yaml` & `causal_testing_framework-7.0.0/dafni/model_definition.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/Makefile` & `causal_testing_framework-7.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/README.md` & `causal_testing_framework-7.0.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/make.bat` & `causal_testing_framework-7.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/_static/css/custom.css` & `causal_testing_framework-7.0.0/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/_static/images/CITCOM-logo.png` & `causal_testing_framework-7.0.0/docs/source/_static/images/CITCOM-logo.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/conf.py` & `causal_testing_framework-7.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/credits.rst` & `causal_testing_framework-7.0.0/docs/source/credits.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/description.rst` & `causal_testing_framework-7.0.0/docs/source/description.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/dev/actions_and_webhooks.rst` & `causal_testing_framework-7.0.0/docs/source/dev/actions_and_webhooks.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Github Actions and Webhooks
 ===========================
 
 Actions
 --------------
 
-Currently, this project makes use of 3 `Github Actions <https://github.com/features/actions>`_,
+Currently, this project makes use of 4 `Github Actions <https://github.com/features/actions>`_,
 which can be found in the
 `.github/workflows <https://github.com/CITCOM-project/CausalTestingFramework/tree/main/.github/workflows>`_ directory.
 
 They are:
 
 #.  ``ci-tests.yaml``, which runs continuous integration (CI) tests on each on each pull request.
 
 #.  ``lint-format.yaml``, which runs linting on each pull request.
 
 #.  ``publish-to-pypi.yaml``, runs when a new version tag is pushed and publishes that tag version to PyPI.
 
+#. ``figshare.yaml``, releases new versions to `Figshare <https://orda.shef.ac.uk/articles/software/CITCOM_Software_Release/24427516?file=43686015>`_.
+
+#. ``publish-to-dafni.yaml``, which containerises and uploads every major release to `DAFNI <https://www.dafni.ac.uk/>`_.
+
+
 Webhooks
 ---------------
 
-The project also uses 3 `Webhooks <https://docs.github.com/en/webhooks-and-events/webhooks/about-webhooks>`_, which can
+The project also uses 2 `Webhooks <https://docs.github.com/en/webhooks-and-events/webhooks/about-webhooks>`_, which can
 be found in the `project settings <https://github.com/CITCOM-project/CausalTestingFramework/settings>`_ on Github. These
 include:
 
-#.  `Codacy <https://github.com/codacy>`_
 
 #.  `Codecov <https://github.com/codecov>`_
 
 #.  `Read the Docs <https://github.com/readthedocs>`_
```

### Comparing `causal_testing_framework-6.0.1/docs/source/dev/documentation.rst` & `causal_testing_framework-7.0.0/docs/source/dev/documentation.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/dev/version_release.rst` & `causal_testing_framework-7.0.0/docs/source/dev/version_release.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/frontends/json_front_end.rst` & `causal_testing_framework-7.0.0/docs/source/frontends/json_front_end.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/frontends/test_suite.rst` & `causal_testing_framework-7.0.0/docs/source/frontends/test_suite.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/glossary.rst` & `causal_testing_framework-7.0.0/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/index.rst` & `causal_testing_framework-7.0.0/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 Overview
 **********
 
 Causal testing is a :term:`causal inference`-driven framework for functional black-box testing. This framework utilises
 graphical causal inference (CI) techniques for the specification and functional testing of software from a black-box
 perspective. In this framework, we use causal directed acyclic graphs (DAGs) to express the anticipated cause-effect
 relationships amongst the inputs and outputs of the system-under-test and the supporting mathematical framework to
-relationships amongst the inputs and outputs of the system-under-test and the supporting mathematical framework to
 design statistical procedures capable of making causal inferences. Each causal test case focuses on the causal effect
 of an intervention made to the system-under test. That is, a prescribed change to the input configuration of the
 system-under-test that is expected to cause a change to some output(s).
 
 .. raw:: html
 
    <style>
@@ -33,15 +32,15 @@
 
    .zoom-container {
        cursor: zoom-in;
        transition: transform 1s ease-in-out;
    }
 
    .zoom-container.zoomed {
-       transform: scale(2);
+       transform: scale(4);
        cursor: zoom-out;
    }
 
    .zoomable-image {
        max-width: 100%;
        max-height: 100%;
        margin: auto;
@@ -80,25 +79,23 @@
    });
    </script>
 
 
 
 .. container:: zoom-container
 
-   .. image:: /images/workflow.png
+   .. image:: /images/schematic.png
       :class: zoomable-image
       :alt: Zoomable Image
 
 
 .. toctree::
    :hidden:
    :caption: Home
 
-   self
-
 .. toctree::
    :hidden:
    :maxdepth: 1
    :caption: Introduction
 
    description
    installation
```

#### html2text {}

```diff
@@ -2,24 +2,22 @@
 ========================================== |status| |ci-tests| |code-cov|
 |docs| |python| |pypi| |doi| |license| Overview ********** Causal testing is a
 :term:`causal inference`-driven framework for functional black-box testing.
 This framework utilises graphical causal inference (CI) techniques for the
 specification and functional testing of software from a black-box perspective.
 In this framework, we use causal directed acyclic graphs (DAGs) to express the
 anticipated cause-effect relationships amongst the inputs and outputs of the
-system-under-test and the supporting mathematical framework to relationships
-amongst the inputs and outputs of the system-under-test and the supporting
-mathematical framework to design statistical procedures capable of making
-causal inferences. Each causal test case focuses on the causal effect of an
-intervention made to the system-under test. That is, a prescribed change to the
-input configuration of the system-under-test that is expected to cause a change
-to some output(s). .. raw:: html
+system-under-test and the supporting mathematical framework to design
+statistical procedures capable of making causal inferences. Each causal test
+case focuses on the causal effect of an intervention made to the system-under
+test. That is, a prescribed change to the input configuration of the system-
+under-test that is expected to cause a change to some output(s). .. raw:: html
 .. raw:: html
-.. container:: zoom-container .. image:: /images/workflow.png :class: zoomable-
-image :alt: Zoomable Image .. toctree:: :hidden: :caption: Home self ..
+.. container:: zoom-container .. image:: /images/schematic.png :class:
+zoomable-image :alt: Zoomable Image .. toctree:: :hidden: :caption: Home ..
 toctree:: :hidden: :maxdepth: 1 :caption: Introduction description installation
 usage .. toctree:: :hidden: :maxdepth: 1 :caption: Module Descriptions /
 modules/data_collector /modules/causal_specification /modules/causal_tests ..
 toctree:: :maxdepth: 2 :caption: API :hidden: :titlesonly: /autoapi/index ..
 toctree:: :hidden: :maxdepth: 1 :caption: Front Ends frontends/json_front_end
 frontends/test_suite .. toctree:: :hidden: :maxdepth: 1 :caption: Glossary
 glossary .. toctree:: :hidden: :maxdepth: 1 :caption: Development /dev/
```

### Comparing `causal_testing_framework-6.0.1/docs/source/installation.rst` & `causal_testing_framework-7.0.0/docs/source/installation.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Getting started
 ================
 
 Requirements
 ---------------
-* Python >= 3.9.
+* Python 3.9 and 3.10 only.
 * `Microsoft Visual C++ <https://docs.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist>`_ 14.0+ (Windows only).
 
 
 Installation
 -----------------
 The Causal Testing Framework can be installed through either the `Python Package Index (PyPI)`_ (recommended), or directly from source.
```

### Comparing `causal_testing_framework-6.0.1/docs/source/modules/causal_specification.rst` & `causal_testing_framework-7.0.0/docs/source/modules/causal_specification.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/modules/causal_tests.rst` & `causal_testing_framework-7.0.0/docs/source/modules/causal_tests.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/modules/data_collector.rst` & `causal_testing_framework-7.0.0/docs/source/modules/data_collector.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/docs/source/usage.rst` & `causal_testing_framework-7.0.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/covasim_/doubling_beta/README.md` & `causal_testing_framework-7.0.0/examples/covasim_/doubling_beta/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/covasim_/doubling_beta/dag.png` & `causal_testing_framework-7.0.0/examples/covasim_/doubling_beta/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/covasim_/doubling_beta/data/10k_observational_data.csv` & `causal_testing_framework-7.0.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/covasim_/doubling_beta/example_beta.py` & `causal_testing_framework-7.0.0/examples/covasim_/doubling_beta/example_beta.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/covasim_/vaccinating_elderly/README.md` & `causal_testing_framework-7.0.0/examples/covasim_/vaccinating_elderly/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/covasim_/vaccinating_elderly/dag.png` & `causal_testing_framework-7.0.0/examples/covasim_/vaccinating_elderly/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/covasim_/vaccinating_elderly/example_vaccine.py` & `causal_testing_framework-7.0.0/examples/covasim_/vaccinating_elderly/example_vaccine.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/lr91/README.md` & `causal_testing_framework-7.0.0/examples/lr91/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/lr91/dag.dot` & `causal_testing_framework-7.0.0/examples/lr91/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/lr91/dag.png` & `causal_testing_framework-7.0.0/examples/lr91/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/lr91/data/normalised_results.csv` & `causal_testing_framework-7.0.0/examples/lr91/data/normalised_results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/lr91/data/results.csv` & `causal_testing_framework-7.0.0/examples/lr91/data/results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/lr91/example_max_conductances.py` & `causal_testing_framework-7.0.0/examples/lr91/example_max_conductances.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/lr91/example_max_conductances_test_suite.py` & `causal_testing_framework-7.0.0/examples/lr91/example_max_conductances_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson/README.md` & `causal_testing_framework-7.0.0/examples/poisson/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson/causal_tests.json` & `causal_testing_framework-7.0.0/examples/poisson/causal_tests.json`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson/dag.dot` & `causal_testing_framework-7.0.0/examples/poisson/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson/data.csv` & `causal_testing_framework-7.0.0/examples/poisson/data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson/example_run_causal_tests.py` & `causal_testing_framework-7.0.0/examples/poisson/example_run_causal_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import pandas as pd
 import scipy
 import os
 
-from causal_testing.testing.estimators import LinearRegressionEstimator, CausalForestEstimator
+from causal_testing.testing.estimators import LinearRegressionEstimator
 from causal_testing.testing.causal_test_outcome import ExactValue, Positive, Negative, NoEffect, CausalTestOutcome
 from causal_testing.testing.causal_test_result import CausalTestResult
 from causal_testing.json_front.json_class import JsonUtility
 from causal_testing.testing.estimators import Estimator
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.variable import Input, Output, Meta
 
@@ -123,15 +123,14 @@
     "Negative": Negative(),
     "ExactValue4_05": ExactValue(4, atol=0.5),
     "NoEffect": NoEffect(),
 }
 
 estimators = {
     "WidthHeightEstimator": WidthHeightEstimator,
-    "CausalForestEstimator": CausalForestEstimator,
     "LinearRegressionEstimator": LinearRegressionEstimator,
 }
 
 # Create input structure required to create a modelling scenario
 modelling_inputs = (
     [Input(i["name"], i["datatype"], i["distribution"]) for i in inputs]
     + [Output(i["name"], i["datatype"]) for i in outputs]
```

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/README.md` & `causal_testing_framework-7.0.0/examples/poisson-line-process/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 In this case study, we demonstrate how causal testing can be used to implement statistical metamorphic testing as per Guderlei & Mayer 2007. As described in section 5.1 of the paper, this involves running a series of causal test cases that incrementally change the width and height of the sampling window. We then show how statistical estimation can produce similar results using only a fraction of the data.
 
 ## How to run
 To run this case study:
 1. Ensure all project dependencies are installed by running `pip install .` in the top level directory
    (instructions are provided in the project README).
 2. Change directory to `causal_testing/examples/poisson-line-process`.
-3. Run the command `python test_poisson_process.py`
+3. Run the command `python example_poisson_process.py`
 
 This should print a series of causal test results and produce two CSV files. `intensity_num_shapes_results_random_1000.csv` corresponds to table 1, and `width_num_shapes_results_random_1000.csv` relates to our findings regarding the relationship of width and `P_u`.
```

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/dag.png` & `causal_testing_framework-7.0.0/examples/poisson-line-process/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/data/random/data_random_1000.csv` & `causal_testing_framework-7.0.0/examples/poisson-line-process/data/random/data_random_1000.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv` & `causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv` & `causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv` & `causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv` & `causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv` & `causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv` & `causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv` & `causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv` & `causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv` & `causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv` & `causal_testing_framework-7.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/examples/poisson-line-process/example_poisson_process.py` & `causal_testing_framework-7.0.0/examples/poisson-line-process/example_poisson_process.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/pyproject.toml` & `causal_testing_framework-7.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,25 @@
 description = "A framework for causal testing using causal directed acyclic graphs."
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "MIT" }
 keywords = ["causal inference", "verification"]
 dependencies = [
     "z3_solver~=4.11.2", # z3_solver does not follow semantic versioning and tying to 4.11 introduces problems
-    "econml~=0.12",
-    "fitter~=1.4",
+    "fitter~=1.7",
     "lhsmdu~=1.1",
     "networkx~=2.6",
-    "numpy~=1.23",
-    "pandas~=1.3",
-    "scikit_learn~=1.1",
+    "numpy~=1.26",
+    "pandas~=1.5",
+    "scikit_learn~=1.4",
     "scipy~=1.7",
-    "statsmodels~=0.13",
-    "tabulate~=0.8",
-    "pydot~=1.4",
-    "pygad~=3.2"
+    "statsmodels~=0.14",
+    "tabulate~=0.9",
+    "pydot~=2.0",
+    "pygad~=3.3"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "autopep8",
     "isort",
```

### Comparing `causal_testing_framework-6.0.1/tests/data/nhefs.csv` & `causal_testing_framework-7.0.0/tests/data/nhefs.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/tests/data_collection_tests/test_observational_data_collector.py` & `causal_testing_framework-7.0.0/tests/data_collection_tests/test_observational_data_collector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import unittest
 import os
+import shutil, tempfile
 import pandas as pd
 from causal_testing.data_collection.data_collector import ObservationalDataCollector
 from causal_testing.specification.causal_specification import Scenario
 from causal_testing.specification.variable import Input, Output, Meta
 from scipy.stats import uniform, rv_discrete
 from enum import Enum
 import random
-from tests.test_helpers import create_temp_dir_if_non_existent, remove_temp_dir_if_existent
 
 
 class TestObservationalDataCollector(unittest.TestCase):
     def setUp(self) -> None:
         class Color(Enum):
             RED = "RED"
             GREEN = "GREEN"
             BLUE = "BLUE"
 
-        temp_dir_path = create_temp_dir_if_non_existent()
-        self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
-        self.observational_df_path = os.path.join(temp_dir_path, "observational_data.csv")
+        self.temp_dir_path = tempfile.mkdtemp()
+        self.dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
+        self.observational_df_path = os.path.join(self.temp_dir_path, "observational_data.csv")
         # Y = 3*X1 + X2*X3 + 10
         self.observational_df = pd.DataFrame(
             {"X1": [1, 2, 3, 4], "X2": [5, 6, 7, 8], "X3": [10, 20, 30, 40], "Y2": ["RED", "GREEN", "BLUE", "BLUE"]}
         )
         self.observational_df["Y1"] = self.observational_df.apply(
             lambda row: (3 * row.X1) + (row.X2 * row.X3) + 10, axis=1
         )
@@ -62,12 +62,12 @@
         scenario = Scenario({self.X1, meta})
         observational_data_collector = ObservationalDataCollector(scenario, self.observational_df)
         observational_data_collector.collect_data()
         data = observational_data_collector.collect_data()
         assert all((m == 2 * x1 for x1, m in zip(data["X1"], data["M"])))
 
     def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
+        shutil.rmtree(self.temp_dir_path)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `causal_testing_framework-6.0.1/tests/generation_tests/test_abstract_test_case.py` & `causal_testing_framework-7.0.0/tests/generation_tests/test_abstract_test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import unittest
 import os
+import shutil, tempfile
 import pandas as pd
 import numpy as np
 from causal_testing.generation.abstract_causal_test_case import AbstractCausalTestCase
 from causal_testing.generation.enum_gen import EnumGen
 from causal_testing.specification.causal_specification import Scenario
 from causal_testing.specification.variable import Input, Output
 from scipy.stats import uniform, rv_discrete
-from tests.test_helpers import create_temp_dir_if_non_existent, remove_temp_dir_if_existent
 from causal_testing.testing.causal_test_outcome import Positive
 from z3 import And
 from enum import Enum
 
 
 class Car(Enum):
     isetta = "vehicle.bmw.isetta"
@@ -25,17 +25,17 @@
 
 class TestAbstractTestCase(unittest.TestCase):
     """
     Class to test abstract test cases.
     """
 
     def setUp(self) -> None:
-        temp_dir_path = create_temp_dir_if_non_existent()
-        self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
-        self.observational_df_path = os.path.join(temp_dir_path, "observational_data.csv")
+        self.temp_dir_path = tempfile.mkdtemp()
+        self.dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
+        self.observational_df_path = os.path.join(self.temp_dir_path, "observational_data.csv")
         # Y = 3*X1 + X2*X3 + 10
         self.observational_df = pd.DataFrame({"X1": [1, 2, 3, 4], "X2": [5, 6, 7, 8], "X3": [10, 20, 30, 40]})
         self.observational_df["Y"] = self.observational_df.apply(
             lambda row: (3 * row.X1) + (row.X2 * row.X3) + 10, axis=1
         )
         self.observational_df.to_csv(self.observational_df_path)
         self.X1 = Input("X1", float, uniform(1, 4))
@@ -188,12 +188,12 @@
             expected_causal_effect={self.Y: Positive()},
             effect_modifiers=None,
         )
         concrete_tests, _ = abstract.generate_concrete_tests(4, rct=True, target_ks_score=0.1, hard_max=1000)
         assert len(concrete_tests) < 1000
 
     def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
+        shutil.rmtree(self.temp_dir_path)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `causal_testing_framework-6.0.1/tests/json_front_tests/test_json_class.py` & `causal_testing_framework-7.0.0/tests/json_front_tests/test_json_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import unittest
 from pathlib import Path
 from statistics import StatisticsError
 import scipy
 import os
 
-from causal_testing.testing.estimators import LinearRegressionEstimator, CausalForestEstimator
+from causal_testing.testing.estimators import LinearRegressionEstimator, Estimator
 from causal_testing.testing.causal_test_outcome import NoEffect, Positive
-from tests.test_helpers import remove_temp_dir_if_existent
 from causal_testing.json_front.json_class import JsonUtility, CausalVariables
 from causal_testing.specification.variable import Input, Output, Meta
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.causal_specification import CausalSpecification
 
 
 class TestJsonClass(unittest.TestCase):
@@ -288,39 +287,42 @@
         json_class = JsonUtility("temp_out.txt", True)
         json_class.set_paths(self.json_path, self.dag_path)
 
         with self.assertRaises(ValueError):
             json_class.setup(self.scenario)
 
     def test_estimator_formula_type_check(self):
+        class ExampleEstimator(Estimator):
+            def add_modelling_assumptions(self):
+                pass
+
         example_test = {
             "tests": [
                 {
                     "name": "test1",
                     "mutations": {"test_input": "Increase"},
-                    "estimator": "CausalForestEstimator",
+                    "estimator": "ExampleEstimator",
                     "estimate_type": "ate",
                     "effect_modifiers": [],
                     "expected_effect": {"test_output": "Positive"},
                     "skip": False,
                     "formula": "test_output ~ test_input",
                 }
             ]
         }
         self.json_class.test_plan = example_test
         effects = {"Positive": Positive()}
         mutates = {
             "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
                                   > self.json_class.scenario.variables[x].z3
         }
-        estimators = {"CausalForestEstimator": CausalForestEstimator}
+        estimators = {"ExampleEstimator": ExampleEstimator}
         with self.assertRaises(TypeError):
             self.json_class.run_json_tests(effects=effects, mutates=mutates, estimators=estimators, f_flag=False)
 
     def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
         if os.path.exists("temp_out.txt"):
             os.remove("temp_out.txt")
 
 
 def populate_example(*args, **kwargs):
     pass
```

### Comparing `causal_testing_framework-6.0.1/tests/specification_tests/test_causal_dag.py` & `causal_testing_framework-7.0.0/tests/specification_tests/test_causal_dag.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 import unittest
 import os
+import shutil, tempfile
 import networkx as nx
 from causal_testing.specification.causal_dag import CausalDAG, close_separator, list_all_min_sep
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.variable import Input, Output
 from causal_testing.testing.base_test_case import BaseTestCase
-from tests.test_helpers import create_temp_dir_if_non_existent, remove_temp_dir_if_existent
+
+
 
 
 class TestCausalDAGIssue90(unittest.TestCase):
     """
     Test the CausalDAG class for the resolution of Issue 90.
     """
 
     def setUp(self) -> None:
-        temp_dir_path = create_temp_dir_if_non_existent()
-        self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
+        self.temp_dir_path = tempfile.mkdtemp()
+        self.dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
         dag_dot = """digraph DAG { rankdir=LR; Z -> X; X -> M; M -> Y; Z -> M; }"""
         with open(self.dag_dot_path, "w") as f:
             f.write(dag_dot)
 
     def test_enumerate_minimal_adjustment_sets(self):
         """Test whether enumerate_minimal_adjustment_sets lists all possible minimum sized adjustment sets."""
         causal_dag = CausalDAG(self.dag_dot_path)
         xs, ys = ["X"], ["Y"]
         adjustment_sets = causal_dag.enumerate_minimal_adjustment_sets(xs, ys)
         self.assertEqual([{"Z"}], adjustment_sets)
 
     def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
+        shutil.rmtree(self.temp_dir_path)
 
 
 class TestIVAssumptions(unittest.TestCase):
     def setUp(self) -> None:
-        temp_dir_path = create_temp_dir_if_non_existent()
-        self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
+        self.temp_dir_path = tempfile.mkdtemp()
+        self.dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
         dag_dot = """digraph G { I -> X; X -> Y; U -> X; U -> Y;}"""
         f = open(self.dag_dot_path, "w")
         f.write(dag_dot)
         f.close()
 
     def test_valid_iv(self):
         causal_dag = CausalDAG(self.dag_dot_path)
@@ -57,27 +59,29 @@
             causal_dag.check_iv_assumptions("X", "Y", "I")
 
     def test_common_cause(self):
         causal_dag = CausalDAG(self.dag_dot_path)
         causal_dag.graph.add_edge("U", "I")
         with self.assertRaises(ValueError):
             causal_dag.check_iv_assumptions("X", "Y", "I")
-
+    
+    def tearDown(self) -> None:
+        shutil.rmtree(self.temp_dir_path)
 
 class TestCausalDAG(unittest.TestCase):
     """
     Test the CausalDAG class for creation of Causal Directed Acyclic Graphs (DAGs).
 
     In particular, confirm whether the Causal DAG class creates valid causal directed acyclic graphs (empty and directed
     graphs without cycles) and refuses to create invalid (cycle-containing) graphs.
     """
 
     def setUp(self) -> None:
-        temp_dir_path = create_temp_dir_if_non_existent()
-        self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
+        self.temp_dir_path = tempfile.mkdtemp()
+        self.dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
         dag_dot = """digraph G { A -> B; B -> C; D -> A; D -> C;}"""
         f = open(self.dag_dot_path, "w")
         f.write(dag_dot)
         f.close()
 
     def test_valid_causal_dag(self):
         """Test whether the Causal DAG is valid."""
@@ -101,69 +105,71 @@
         assert list(causal_dag.graph.nodes) == [] and list(causal_dag.graph.edges) == []
 
     def test_to_dot_string(self):
         causal_dag = CausalDAG(self.dag_dot_path)
         self.assertEqual(causal_dag.to_dot_string(), """digraph G {\nA -> B;\nB -> C;\nD -> A;\nD -> C;\n}""")
 
     def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
+        shutil.rmtree(self.temp_dir_path)
 
 
 class TestCyclicCausalDAG(unittest.TestCase):
     """
     Test the creation of a cyclic causal graph.
     """
 
     def setUp(self) -> None:
-        temp_dir_path = create_temp_dir_if_non_existent()
-        self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
+        self.temp_dir_path = tempfile.mkdtemp()
+        self.dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
         dag_dot = """digraph G { A -> B; B -> C; D -> A; D -> C; C -> A;}"""
         f = open(self.dag_dot_path, "w")
         f.write(dag_dot)
         f.close()
 
     def test_invalid_causal_dag(self):
         self.assertRaises(nx.HasACycle, CausalDAG, self.dag_dot_path)
 
     def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
+        shutil.rmtree(self.temp_dir_path)
 
 
 class TestDAGDirectEffectIdentification(unittest.TestCase):
     """
     Test the Causal DAG identification algorithms and supporting algorithms.
     """
 
     def setUp(self) -> None:
-        temp_dir_path = create_temp_dir_if_non_existent()
-        self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
+        self.temp_dir_path = tempfile.mkdtemp()
+        self.dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
         dag_dot = """digraph G { X1->X2;X2->V;X2->D1;X2->D2;D1->Y;D1->D2;Y->D3;Z->X2;Z->Y;}"""
         f = open(self.dag_dot_path, "w")
         f.write(dag_dot)
         f.close()
 
     def test_direct_effect_adjustment_sets(self):
         causal_dag = CausalDAG(self.dag_dot_path)
         adjustment_sets = causal_dag.direct_effect_adjustment_sets(["X1"], ["Y"])
         self.assertEqual(list(adjustment_sets), [{"D1", "Z"}, {"X2", "Z"}])
 
     def test_direct_effect_adjustment_sets_no_adjustment(self):
         causal_dag = CausalDAG(self.dag_dot_path)
         adjustment_sets = causal_dag.direct_effect_adjustment_sets(["X2"], ["D1"])
         self.assertEqual(list(adjustment_sets), [set()])
-
+    
+    def tearDown(self) -> None:
+        shutil.rmtree(self.temp_dir_path)
 
 class TestDAGIdentification(unittest.TestCase):
     """
     Test the Causal DAG identification algorithms and supporting algorithms.
     """
 
     def setUp(self) -> None:
-        temp_dir_path = create_temp_dir_if_non_existent()
-        self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
+        self.temp_dir_path = tempfile.mkdtemp()
+        self.dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
         dag_dot = """digraph G { X1->X2;X2->V;X2->D1;X2->D2;D1->Y;D1->D2;Y->D3;Z->X2;Z->Y;}"""
         f = open(self.dag_dot_path, "w")
         f.write(dag_dot)
         f.close()
 
     def test_get_indirect_graph(self):
         causal_dag = CausalDAG(self.dag_dot_path)
@@ -333,29 +339,28 @@
             ]
         )
         xs, ys = ["ba"], ["da"]
         adjustment_sets = causal_dag.enumerate_minimal_adjustment_sets(xs, ys)
         self.assertEqual(adjustment_sets, [{"aa"}, {"la"}, {"va"}])
 
     def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
-
+        shutil.rmtree(self.temp_dir_path)
 
 class TestDependsOnOutputs(unittest.TestCase):
     """
     Test the depends_on_outputs method.
     """
 
     def setUp(self) -> None:
         from scipy.stats import uniform
         from causal_testing.specification.variable import Input, Output, Meta
         from causal_testing.specification.scenario import Scenario
 
-        temp_dir_path = create_temp_dir_if_non_existent()
-        self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
+        self.temp_dir_path = tempfile.mkdtemp()
+        self.dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
         dag_dot = """digraph G { A -> B; B -> C; D -> A; D -> C}"""
         f = open(self.dag_dot_path, "w")
         f.write(dag_dot)
         f.close()
 
         D = Input("D", float, uniform(0, 1))
         A = Meta("A", float, uniform(0, 1))
@@ -385,15 +390,15 @@
     def test_depends_on_outputs_input(self):
         causal_dag = CausalDAG(self.dag_dot_path)
         print("nodes:", causal_dag.nodes())
         print("graph:", causal_dag)
         self.assertFalse(causal_dag.depends_on_outputs("D", self.scenario))
 
     def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
+        shutil.rmtree(self.temp_dir_path)
 
 
 class TestUndirectedGraphAlgorithms(unittest.TestCase):
     """
     Test the graph algorithms designed for the undirected graph variants of a Causal DAG.
     During the identification process, a Causal DAG is converted into several forms of undirected graph which allow for
     more efficient computation of minimal separators. This suite of tests covers the two main algorithms applied to
@@ -425,26 +430,23 @@
             )
         )
 
         # Convert list of sets to set of frozen sets for comparison
         min_separators = set(frozenset(min_separator) for min_separator in min_separators)
         self.assertEqual({frozenset({2, 3}), frozenset({3, 4}), frozenset({4, 5})}, min_separators)
 
-    def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
-
 
 class TestHiddenVariableDAG(unittest.TestCase):
     """
     Test the CausalDAG identification for the exclusion of hidden variables.
     """
 
     def setUp(self) -> None:
-        temp_dir_path = create_temp_dir_if_non_existent()
-        self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
+        self.temp_dir_path = tempfile.mkdtemp()
+        self.dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
         dag_dot = """digraph DAG { rankdir=LR; Z -> X; X -> M; M -> Y; Z -> M; }"""
         with open(self.dag_dot_path, "w") as f:
             f.write(dag_dot)
 
     def test_hidden_varaible_adjustment_sets(self):
         """Test whether identification produces different adjustment sets depending on if a variable is hidden."""
         causal_dag = CausalDAG(self.dag_dot_path)
@@ -457,8 +459,8 @@
 
         z.hidden = True
         adjustment_sets_with_hidden = causal_dag.identification(BaseTestCase(x, m), scenario)
 
         self.assertNotEqual(adjustment_sets, adjustment_sets_with_hidden)
 
     def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
+        shutil.rmtree(self.temp_dir_path)
```

### Comparing `causal_testing_framework-6.0.1/tests/specification_tests/test_metamorphic_relations.py` & `causal_testing_framework-7.0.0/tests/specification_tests/test_metamorphic_relations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import unittest
 import os
-
+import shutil, tempfile
 import pandas as pd
 from itertools import combinations
 
-from tests.test_helpers import create_temp_dir_if_non_existent
 from causal_testing.specification.causal_dag import CausalDAG
 from causal_testing.specification.causal_specification import Scenario
 from causal_testing.specification.metamorphic_relation import (
     ShouldCause,
     ShouldNotCause,
     generate_metamorphic_relations,
 )
@@ -65,16 +64,16 @@
         results_dict = buggy_program_under_test(**input_configuration)
         results_df = pd.DataFrame(results_dict, index=[0])
         return results_df
 
 
 class TestMetamorphicRelation(unittest.TestCase):
     def setUp(self) -> None:
-        temp_dir_path = create_temp_dir_if_non_existent()
-        self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
+        self.temp_dir_path = tempfile.mkdtemp()
+        self.dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
         dag_dot = """digraph DAG { rankdir=LR; X1 -> Z; Z -> M; M -> Y; X2 -> Z; X3 -> M;}"""
         with open(self.dag_dot_path, "w") as f:
             f.write(dag_dot)
 
         X1 = Input("X1", float)
         X2 = Input("X2", float)
         X3 = Input("X3", float)
@@ -84,14 +83,17 @@
         self.scenario = Scenario(variables={X1, X2, X3, Z, M, Y})
         self.default_control_input_config = {"X1": 1, "X2": 2, "X3": 3}
         self.default_treatment_input_config = {"X1": 2, "X2": 3, "X3": 3}
         self.data_collector = ProgramUnderTestEDC(
             self.scenario, self.default_control_input_config, self.default_treatment_input_config
         )
 
+    def tearDown(self) -> None:
+        shutil.rmtree(self.temp_dir_path)
+
     def test_should_cause_metamorphic_relations_correct_spec(self):
         """Test if the ShouldCause MR passes all metamorphic tests where the DAG perfectly represents the program."""
         causal_dag = CausalDAG(self.dag_dot_path)
         for edge in causal_dag.graph.edges:
             (u, v) = edge
             adj_set = list(causal_dag.direct_effect_adjustment_sets([u], [v])[0])
             should_cause_MR = ShouldCause(u, v, adj_set, causal_dag)
```

### Comparing `causal_testing_framework-6.0.1/tests/specification_tests/test_variable.py` & `causal_testing_framework-7.0.0/tests/specification_tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/tests/surrogate_tests/test_causal_surrogate_assisted.py` & `causal_testing_framework-7.0.0/tests/surrogate_tests/test_causal_surrogate_assisted.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from causal_testing.specification.causal_dag import CausalDAG
 from causal_testing.specification.causal_specification import CausalSpecification
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.variable import Input, Output
 from causal_testing.surrogate.causal_surrogate_assisted import SimulationResult, CausalSurrogateAssistedTestCase, Simulator
 from causal_testing.surrogate.surrogate_search_algorithms import GeneticSearchAlgorithm
 from causal_testing.testing.estimators import CubicSplineRegressionEstimator
-from tests.test_helpers import create_temp_dir_if_non_existent, remove_temp_dir_if_existent
+
 import os
+import shutil, tempfile
 import pandas as pd
 import numpy as np
 
 class TestSimulationResult(unittest.TestCase):
 
     def setUp(self):
 
@@ -39,16 +40,16 @@
 class TestCausalSurrogate(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls) -> None:
         cls.class_df = load_class_df()
 
     def setUp(self):
-        temp_dir_path = create_temp_dir_if_non_existent()
-        self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
+        self.temp_dir_path = tempfile.mkdtemp()
+        self.dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
         dag_dot = """digraph DAG { rankdir=LR; Z -> X; X -> M [included=1, expected=positive]; M -> Y [included=1, expected=negative]; Z -> M; }"""
         with open(self.dag_dot_path, "w") as f:
             f.write(dag_dot)
 
     def test_surrogate_model_generation(self):
         c_s_a_test_case = CausalSurrogateAssistedTestCase(None, None, None)
 
@@ -195,15 +196,15 @@
         c_s_a_test_case = CausalSurrogateAssistedTestCase(specification, search_algorithm, simulator)
 
         self.assertRaises(ValueError, c_s_a_test_case.execute, 
                           data_collector=ObservationalDataCollector(scenario, df),
                           custom_data_aggregator=data_double_aggregator)
 
     def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
+        shutil.rmtree(self.temp_dir_path)
 
 def load_class_df():
     """Get the testing data and put into a dataframe."""
 
     class_df = pd.DataFrame({"Z": np.arange(16), "X": np.arange(16), "M": np.arange(16, 32), "Y": np.arange(32,16,-1)})
     return class_df
```

### Comparing `causal_testing_framework-6.0.1/tests/testing_tests/test_causal_test_adequacy.py` & `causal_testing_framework-7.0.0/tests/testing_tests/test_causal_test_adequacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from causal_testing.testing.estimators import LinearRegressionEstimator
 from causal_testing.testing.base_test_case import BaseTestCase
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.causal_test_suite import CausalTestSuite
 from causal_testing.testing.causal_test_adequacy import DAGAdequacy
 from causal_testing.testing.causal_test_outcome import NoEffect, Positive
-from tests.test_helpers import remove_temp_dir_if_existent
 from causal_testing.json_front.json_class import JsonUtility, CausalVariables
 from causal_testing.specification.variable import Input, Output, Meta
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.causal_specification import CausalSpecification
 
 
 class TestCausalTestAdequacy(unittest.TestCase):
@@ -251,10 +250,9 @@
                     ("test_input_no_dist", "C"),
                 },
                 "dag_adequacy": 0.1,
             },
         )
 
     def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
         if os.path.exists("temp_out.txt"):
             os.remove("temp_out.txt")
```

### Comparing `causal_testing_framework-6.0.1/tests/testing_tests/test_causal_test_case.py` & `causal_testing_framework-7.0.0/tests/testing_tests/test_causal_test_case.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import unittest
 import os
+import tempfile
+import shutil
 import pandas as pd
 import numpy as np
 
-from tests.test_helpers import create_temp_dir_if_non_existent, remove_temp_dir_if_existent
 from causal_testing.specification.causal_specification import CausalSpecification, Scenario
 from causal_testing.specification.variable import Input, Output
 from causal_testing.specification.causal_dag import CausalDAG
 from causal_testing.data_collection.data_collector import ObservationalDataCollector
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.causal_test_outcome import ExactValue
-from causal_testing.testing.estimators import CausalForestEstimator, LinearRegressionEstimator
+from causal_testing.testing.estimators import LinearRegressionEstimator
 from causal_testing.testing.base_test_case import BaseTestCase
 
 
 class TestCausalTestCase(unittest.TestCase):
     """Test the CausalTestCase class.
 
     The base test case is a data class which contains the minimum information
@@ -40,29 +41,26 @@
     def test_str(self):
         self.assertEqual(
             str(self.causal_test_case),
             "Running {'A': 1} instead of {'A': 0} should cause the following changes to"
             " {Output: C::float}: ExactValue: 4±0.2.",
         )
 
-    def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
-
 
 class TestCausalTestExecution(unittest.TestCase):
     """Test the causal test execution workflow using observational data.
 
     The causal test engine (CTE) is the main workflow for the causal testing framework. The CTE takes a causal test case
     and a causal specification and computes the causal effect of the intervention on the outcome of interest.
     """
 
     def setUp(self) -> None:
         # 1. Create Causal DAG
-        temp_dir_path = create_temp_dir_if_non_existent()
-        dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
+        self.temp_dir_path = tempfile.mkdtemp()
+        dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
         dag_dot = """digraph G { A -> C; D -> A; D -> C}"""
         with open(dag_dot_path, "w") as file:
             file.write(dag_dot)
         self.causal_dag = CausalDAG(dag_dot_path)
 
         # 2. Create Scenario and Causal Specification
         A = Input("A", float)
@@ -84,45 +82,35 @@
         )
 
         # 4. Create dummy test data and write to csv
         np.random.seed(1)
         df = pd.DataFrame({"D": list(np.random.normal(60, 10, 1000))})  # D = exogenous
         df["A"] = [1 if d > 50 else 0 for d in df["D"]]
         df["C"] = df["D"] + (4 * (df["A"] + 2))  # C = (4*(A+2)) + D
-        self.observational_data_csv_path = os.path.join(temp_dir_path, "observational_data.csv")
+        self.observational_data_csv_path = os.path.join(self.temp_dir_path, "observational_data.csv")
         df.to_csv(self.observational_data_csv_path, index=False)
 
         # 5. Create observational data collector
         # Obsolete?
         self.data_collector = ObservationalDataCollector(self.scenario, df)
         self.data_collector.collect_data()
         self.df = self.data_collector.collect_data()
         self.minimal_adjustment_set = self.causal_dag.identification(self.base_test_case)
         # 6. Easier to access treatment and outcome values
         self.treatment_value = 1
         self.control_value = 0
 
+    def tearDown(self) -> None:
+        shutil.rmtree(self.temp_dir_path)
+
     def test_check_minimum_adjustment_set(self):
         """Check that the minimum adjustment set is correctly made"""
         minimal_adjustment_set = self.causal_dag.identification(self.base_test_case)
         self.assertEqual(minimal_adjustment_set, {"D"})
 
-    def test_execute_test_observational_causal_forest_estimator(self):
-        """Check that executing the causal test case returns the correct results for the dummy data using a causal
-        forest estimator."""
-        estimation_model = CausalForestEstimator(
-            "A",
-            self.treatment_value,
-            self.control_value,
-            self.minimal_adjustment_set,
-            "C",
-            self.df,
-        )
-        causal_test_result = self.causal_test_case.execute_test(estimation_model, self.data_collector)
-        pd.testing.assert_series_equal(causal_test_result.test_value.value, pd.Series(4.0), atol=1)
 
     def test_invalid_causal_effect(self):
         """Check that executing the causal test case returns the correct results for dummy data using a linear
         regression estimator."""
         base_test_case = BaseTestCase(treatment_variable=self.A, outcome_variable=self.C, effect="error")
 
         with self.assertRaises(Exception):
@@ -224,37 +212,7 @@
             self.minimal_adjustment_set,
             "C",
             self.df,
             formula=f"C ~ A + {'+'.join(self.minimal_adjustment_set)} + (D ** 2)",
         )
         causal_test_result = self.causal_test_case.execute_test(estimation_model, self.data_collector)
         pd.testing.assert_series_equal(causal_test_result.test_value.value, pd.Series(4.0), atol=1)
-
-    def test_execute_observational_causal_forest_estimator_cates(self):
-        """Check that executing the causal test case returns the correct conditional average treatment effects for
-        dummy data with effect multiplicative effect modification. C ~ (4*(A+2) + D)*M"""
-        # Add some effect modifier M that has a multiplicative effect on C
-        self.df["M"] = np.random.randint(1, 5, len(self.df))
-        self.df["C"] *= self.df["M"]
-        estimation_model = CausalForestEstimator(
-            "A",
-            self.treatment_value,
-            self.control_value,
-            self.minimal_adjustment_set,
-            "C",
-            self.df,
-            effect_modifiers={"M": None},
-        )
-        self.causal_test_case.estimate_type = "cates"
-        causal_test_result = self.causal_test_case.execute_test(estimation_model, self.data_collector)
-        causal_test_result = causal_test_result.test_value.value
-        # Check that each effect modifier's strata has a greater ATE than the last (ascending order)
-        causal_test_result_m1 = causal_test_result.loc[causal_test_result["M"] == 1]
-        causal_test_result_m2 = causal_test_result.loc[causal_test_result["M"] == 2]
-        causal_test_result_m3 = causal_test_result.loc[causal_test_result["M"] == 3]
-        causal_test_result_m4 = causal_test_result.loc[causal_test_result["M"] == 4]
-        self.assertLess(causal_test_result_m1["cate"].mean(), causal_test_result_m2["cate"].mean())
-        self.assertLess(causal_test_result_m2["cate"].mean(), causal_test_result_m3["cate"].mean())
-        self.assertLess(causal_test_result_m3["cate"].mean(), causal_test_result_m4["cate"].mean())
-
-    def tearDown(self) -> None:
-        remove_temp_dir_if_existent()
```

### Comparing `causal_testing_framework-6.0.1/tests/testing_tests/test_causal_test_outcome.py` & `causal_testing_framework-7.0.0/tests/testing_tests/test_causal_test_outcome.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-6.0.1/tests/testing_tests/test_causal_test_suite.py` & `causal_testing_framework-7.0.0/tests/testing_tests/test_causal_test_suite.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import unittest
 import os
+import tempfile
 import numpy as np
+import shutil
 import pandas as pd
 from causal_testing.testing.causal_test_suite import CausalTestSuite
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.base_test_case import BaseTestCase
 from causal_testing.specification.variable import Input, Output
 from causal_testing.testing.causal_test_outcome import ExactValue
-from causal_testing.testing.estimators import CausalForestEstimator, LinearRegressionEstimator
+from causal_testing.testing.estimators import LinearRegressionEstimator, LogisticRegressionEstimator
 from causal_testing.specification.causal_specification import CausalSpecification, Scenario
 from causal_testing.data_collection.data_collector import ObservationalDataCollector
-from tests.test_helpers import create_temp_dir_if_non_existent, remove_temp_dir_if_existent
 from causal_testing.specification.causal_dag import CausalDAG
 
 
 class TestCausalTestSuite(unittest.TestCase):
     """Test the Test Suite object and it's implementation in the test engine using dummy data."""
 
     def setUp(self) -> None:
@@ -25,16 +26,16 @@
         self.C = C
         D = Output("D", float)
         self.D = D
         self.base_test_case = BaseTestCase(A, C)
         self.scenario = Scenario({A, C, D})
 
         # 2. Create DAG and dummy data and write to csvs
-        temp_dir_path = create_temp_dir_if_non_existent()
-        dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
+        self.temp_dir_path = tempfile.mkdtemp()
+        dag_dot_path = os.path.join(self.temp_dir_path, "dag.dot")
         dag_dot = """digraph G { A -> C; D -> A; D -> C}"""
         with open(dag_dot_path, "w") as file:
             file.write(dag_dot)
 
         np.random.seed(1)
         df = pd.DataFrame({"D": list(np.random.normal(60, 10, 1000))})  # D = exogenous
         df["A"] = [1 if d > 50 else 0 for d in df["D"]]
@@ -60,14 +61,17 @@
         self.test_suite.add_test_object(
             base_test_case=self.base_test_case, causal_test_case_list=test_list, estimators_classes=self.estimators
         )
         self.causal_specification = CausalSpecification(self.scenario, self.causal_dag)
 
         self.data_collector = ObservationalDataCollector(self.scenario, self.df)
 
+    def tearDown(self) -> None:
+        shutil.rmtree(self.temp_dir_path)
+
     def test_adding_test_object(self):
         "test an object can be added to the test_suite using the add_test_object function"
         test_suite = CausalTestSuite()
         test_list = [CausalTestCase(self.base_test_case, self.expected_causal_effect, 0, 1)]
         estimators = [LinearRegressionEstimator]
         test_suite.add_test_object(
             base_test_case=self.base_test_case, causal_test_case_list=test_list, estimators_classes=estimators
@@ -96,23 +100,26 @@
     def test_execute_test_suite_single_base_test_case(self):
         """Check that the test suite can return the correct results from dummy data for a single base_test-case"""
 
         causal_test_results = self.test_suite.execute_test_suite(self.data_collector, self.causal_specification)
         causal_test_case_result = causal_test_results[self.base_test_case]
         self.assertAlmostEqual(causal_test_case_result["LinearRegressionEstimator"][0].test_value.value[0], 4, delta=1e-10)
 
-    def test_execute_test_suite_multiple_estimators(self):
-        """Check that executing a test suite with multiple estimators returns correct results for the dummy data
-        for each estimator
-        """
-        estimators = [LinearRegressionEstimator, CausalForestEstimator]
-        test_suite_2_estimators = CausalTestSuite()
-        test_list = [CausalTestCase(self.base_test_case, self.expected_causal_effect, 0, 1)]
-        test_suite_2_estimators.add_test_object(
-            base_test_case=self.base_test_case, causal_test_case_list=test_list, estimators_classes=estimators
-        )
-        causal_test_results = test_suite_2_estimators.execute_test_suite(self.data_collector, self.causal_specification)
-        causal_test_case_result = causal_test_results[self.base_test_case]
-        linear_regression_result = causal_test_case_result["LinearRegressionEstimator"][0]
-        causal_forrest_result = causal_test_case_result["CausalForestEstimator"][0]
-        self.assertAlmostEqual(linear_regression_result.test_value.value[0], 4, delta=1e-1)
-        self.assertAlmostEqual(causal_forrest_result.test_value.value[0], 4, delta=1e-1)
+    # Without CausalForestEstimator we now only have 2 estimators. Unfortunately LogicisticRegressionEstimator does not
+    # currently work with TestSuite. So for now removed test
+
+    # def test_execute_test_suite_multiple_estimators(self):
+    #     """Check that executing a test suite with multiple estimators returns correct results for the dummy data
+    #     for each estimator
+    #     """
+    #     estimators = [LinearRegressionEstimator, LogisticRegressionEstimator]
+    #     test_suite_2_estimators = CausalTestSuite()
+    #     test_list = [CausalTestCase(self.base_test_case, self.expected_causal_effect, 0, 1)]
+    #     test_suite_2_estimators.add_test_object(
+    #         base_test_case=self.base_test_case, causal_test_case_list=test_list, estimators_classes=estimators
+    #     )
+    #     causal_test_results = test_suite_2_estimators.execute_test_suite(self.data_collector, self.causal_specification)
+    #     causal_test_case_result = causal_test_results[self.base_test_case]
+    #     linear_regression_result = causal_test_case_result["LinearRegressionEstimator"][0]
+    #     logistic_regression_estimator = causal_test_case_result["LogisticRegressionEstimator"][0]
+    #     self.assertAlmostEqual(linear_regression_result.test_value.value, 4, delta=1e-1)
+    #     self.assertAlmostEqual(logistic_regression_estimator.test_value.value, 4, delta=1e-1)
```

### Comparing `causal_testing_framework-6.0.1/tests/testing_tests/test_estimators.py` & `causal_testing_framework-7.0.0/tests/testing_tests/test_estimators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import unittest
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from causal_testing.testing.estimators import (
     LinearRegressionEstimator,
-    CausalForestEstimator,
     LogisticRegressionEstimator,
     InstrumentalVariableEstimator,
     CubicSplineRegressionEstimator,
 )
 from causal_testing.specification.variable import Input
 from causal_testing.utils.validation import CausalValidator
 
@@ -434,77 +433,14 @@
         ate_2 = cublic_spline_estimator.estimate_ate_calculated()
 
         # Doubling the treatemebnt value should roughly but not exactly double the ATE
         self.assertNotEqual(ate_1[0] * 2, ate_2[0])
         self.assertAlmostEqual(ate_1[0] * 2, ate_2[0])
 
 
-class TestCausalForestEstimator(unittest.TestCase):
-    """Test the linear regression estimator against the programming exercises in Section 2 of Hernán and Robins [1].
-
-    Reference: Hernán MA, Robins JM (2020). Causal Inference: What If. Boca Raton: Chapman & Hall/CRC.
-    Link: https://www.hsph.harvard.edu/miguel-hernan/causal-inference-book/
-    """
-
-    @classmethod
-    def setUpClass(cls) -> None:
-        cls.nhefs_df = load_nhefs_df()
-        cls.chapter_11_df = load_chapter_11_df()
-
-    def test_program_15_ate(self):
-        """Test whether our causal forest implementation produces the similar ATE to program 15.1 (p. 163, 184)."""
-        df = self.nhefs_df
-        covariates = {
-            "sex",
-            "race",
-            "age",
-            "edu_2",
-            "edu_3",
-            "edu_4",
-            "edu_5",
-            "exercise_1",
-            "exercise_2",
-            "active_1",
-            "active_2",
-            "wt71",
-            "smokeintensity",
-            "smokeyrs",
-        }
-        causal_forest = CausalForestEstimator("qsmk", 1, 0, covariates, "wt82_71", df, {"smokeintensity": 40})
-        ate, _ = causal_forest.estimate_ate()
-        self.assertGreater(round(ate[0], 1), 2.5)
-        self.assertLess(round(ate[0], 1), 4.5)
-
-    def test_program_15_cate(self):
-        """Test whether our causal forest implementation produces the similar CATE to program 15.1 (p. 163, 184)."""
-        df = self.nhefs_df
-        smoking_intensity_5_and_40_df = df.loc[(df["smokeintensity"] == 5) | (df["smokeintensity"] == 40)]
-        covariates = {
-            "sex",
-            "race",
-            "age",
-            "edu_2",
-            "edu_3",
-            "edu_4",
-            "edu_5",
-            "exercise_1",
-            "exercise_2",
-            "active_1",
-            "active_2",
-            "wt71",
-            "smokeintensity",
-            "smokeyrs",
-        }
-        causal_forest = CausalForestEstimator(
-            "qsmk", 1, 0, covariates, "wt82_71", smoking_intensity_5_and_40_df, {"smokeintensity": 40}
-        )
-        cates_df, _ = causal_forest.estimate_cates()
-        self.assertGreater(cates_df["cate"].mean(), 0)
-
-
 class TestLinearRegressionInteraction(unittest.TestCase):
     """Test linear regression for estimating effects involving interaction."""
 
     @classmethod
     def setUpClass(cls) -> None:
         # Y = 2X1 - 3X2 + 2*X1*X2 + 10
         df = pd.DataFrame({"X1": np.random.uniform(-1000, 1000, 1000), "X2": np.random.uniform(-1000, 1000, 1000)})
```

