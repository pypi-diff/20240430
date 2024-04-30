# Comparing `tmp/polaris_lib-0.3.0.tar.gz` & `tmp/polaris_lib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polaris_lib-0.3.0.tar", last modified: Mon Apr 22 19:21:15 2024, max compression
+gzip compressed data, was "polaris_lib-0.4.0.tar", last modified: Tue Apr 30 20:03:12 2024, max compression
```

## Comparing `polaris_lib-0.3.0.tar` & `polaris_lib-0.4.0.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.139940 polaris_lib-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.123940 polaris_lib-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.123940 polaris_lib-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/.github/ISSUE_TEMPLATE/default-template.md
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/.github/changelog_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.127940 polaris_lib-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-04-22 19:21:15.139940 polaris_lib-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.127940 polaris_lib-0.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.127940 polaris_lib-0.3.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/api/adapters.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/api/base.md
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/api/benchmark.md
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/api/converters.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/api/dataset.md
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/api/evaluation.md
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/api/factory.md
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/api/hub.client.md
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/api/hub.polarisfs.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/api/load.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/api/subset.md
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/api/utils.types.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.123940 polaris_lib-0.3.0/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.127940 polaris_lib-0.3.0/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/assets/css/custom-polaris.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.127940 polaris_lib-0.3.0/docs/community/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/community/community.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.127940 polaris_lib-0.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/images/logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.131940 polaris_lib-0.3.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    31902 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/tutorials/basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23556 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/tutorials/custom_dataset_benchmark.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1239792 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/tutorials/data_curation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    97014 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/tutorials/dataset_factory.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/docs/tutorials/dataset_zarr.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/env.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.131940 polaris_lib-0.3.0/polaris/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.131940 polaris_lib-0.3.0/polaris/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21051 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/benchmark/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/benchmark/_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.131940 polaris_lib-0.3.0/polaris/curation/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/curation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/curation/_chemistry_curator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/curation/_curator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9907 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/curation/_data_curator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/curation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/curation/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.135940 polaris_lib-0.3.0/polaris/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/dataset/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/dataset/_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    18938 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/dataset/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/dataset/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/dataset/_subset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.135940 polaris_lib-0.3.0/polaris/dataset/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/dataset/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/dataset/converters/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/dataset/converters/_sdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/dataset/converters/_zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.135940 polaris_lib-0.3.0/polaris/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/evaluate/_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/evaluate/_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.135940 polaris_lib-0.3.0/polaris/hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30057 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/hub/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/hub/polarisfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/hub/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.135940 polaris_lib-0.3.0/polaris/loader/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/loader/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.135940 polaris_lib-0.3.0/polaris/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/utils/dict2html.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/utils/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/polaris/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.139940 polaris_lib-0.3.0/polaris_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-04-22 19:21:15.000000 polaris_lib-0.3.0/polaris_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-22 19:21:15.000000 polaris_lib-0.3.0/polaris_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:21:15.000000 polaris_lib-0.3.0/polaris_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 19:21:15.000000 polaris_lib-0.3.0/polaris_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-22 19:21:15.000000 polaris_lib-0.3.0/polaris_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 19:21:15.000000 polaris_lib-0.3.0/polaris_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:21:15.139940 polaris_lib-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:21:15.139940 polaris_lib-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/tests/test_curation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/tests/test_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-22 19:17:52.000000 polaris_lib-0.3.0/tests/test_type_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:12.010184 polaris_lib-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:11.994184 polaris_lib-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:11.994184 polaris_lib-0.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/.github/ISSUE_TEMPLATE/default-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/.github/changelog_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:11.994184 polaris_lib-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-04-30 20:03:12.010184 polaris_lib-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:11.994184 polaris_lib-0.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:11.994184 polaris_lib-0.4.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/api/adapters.md
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/api/base.md
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/api/benchmark.md
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/api/converters.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/api/dataset.md
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/api/evaluation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/api/factory.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/api/hub.client.md
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/api/hub.polarisfs.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/api/load.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/api/subset.md
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/api/utils.types.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:11.990184 polaris_lib-0.4.0/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:11.994184 polaris_lib-0.4.0/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/assets/css/custom-polaris.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:11.994184 polaris_lib-0.4.0/docs/community/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/community/community.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:11.998184 polaris_lib-0.4.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/images/logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:11.998184 polaris_lib-0.4.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    31902 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/tutorials/basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23556 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/tutorials/custom_dataset_benchmark.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1239792 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/tutorials/data_curation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    97014 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/tutorials/dataset_factory.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/docs/tutorials/dataset_zarr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:11.998184 polaris_lib-0.4.0/polaris/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:11.998184 polaris_lib-0.4.0/polaris/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21796 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/benchmark/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/benchmark/_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:12.002184 polaris_lib-0.4.0/polaris/curation/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/curation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/curation/_chemistry_curator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/curation/_curator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9907 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/curation/_data_curator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/curation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/curation/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:12.002184 polaris_lib-0.4.0/polaris/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/dataset/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/dataset/_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18938 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/dataset/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/dataset/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/dataset/_subset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:12.002184 polaris_lib-0.4.0/polaris/dataset/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/dataset/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/dataset/converters/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/dataset/converters/_sdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/dataset/converters/_zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:12.002184 polaris_lib-0.4.0/polaris/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/evaluate/_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/evaluate/_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:12.002184 polaris_lib-0.4.0/polaris/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30057 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/hub/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/hub/polarisfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/hub/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:12.002184 polaris_lib-0.4.0/polaris/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/loader/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:12.006184 polaris_lib-0.4.0/polaris/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/utils/dict2html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/utils/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/polaris/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:12.006184 polaris_lib-0.4.0/polaris_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-04-30 20:03:11.000000 polaris_lib-0.4.0/polaris_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-30 20:03:11.000000 polaris_lib-0.4.0/polaris_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:03:11.000000 polaris_lib-0.4.0/polaris_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 20:03:11.000000 polaris_lib-0.4.0/polaris_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-30 20:03:11.000000 polaris_lib-0.4.0/polaris_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 20:03:11.000000 polaris_lib-0.4.0/polaris_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:03:12.010184 polaris_lib-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:03:12.006184 polaris_lib-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/tests/test_curation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/tests/test_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-30 19:58:27.000000 polaris_lib-0.4.0/tests/test_type_checks.py
```

### Comparing `polaris_lib-0.3.0/.github/CODE_OF_CONDUCT.md` & `polaris_lib-0.4.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/.github/ISSUE_TEMPLATE/bug-report.yml` & `polaris_lib-0.4.0/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/.github/ISSUE_TEMPLATE/default-template.md` & `polaris_lib-0.4.0/.github/ISSUE_TEMPLATE/default-template.md`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/.github/ISSUE_TEMPLATE/feature-request.md` & `polaris_lib-0.4.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/.github/PULL_REQUEST_TEMPLATE.md` & `polaris_lib-0.4.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/.github/workflows/code-check.yml` & `polaris_lib-0.4.0/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/.github/workflows/doc.yml` & `polaris_lib-0.4.0/.github/workflows/doc.yml`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,19 @@
         with:
           environment-file: env.yml
           environment-name: my_env
           cache-environment: true
           cache-downloads: true
 
       - name: Install library
-        run: python -m pip install --no-deps .
+        run: |
+          python -m pip install --no-deps .
+          # Note: Temporarily upgrade mkdocs-jupyter through PyPi
+          # See https://github.com/conda-forge/mkdocs-jupyter-feedstock/pull/29
+          python -m pip install mkdocs-jupyter -U
 
       - name: Configure git
         run: |
           git config --global user.name "${GITHUB_ACTOR}"
           git config --global user.email "${GITHUB_ACTOR}@users.noreply.github.com"
 
       - name: Deploy the doc
```

### Comparing `polaris_lib-0.3.0/.github/workflows/release.yml` & `polaris_lib-0.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/.github/workflows/test.yml` & `polaris_lib-0.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/.gitignore` & `polaris_lib-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/LICENSE` & `polaris_lib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/PKG-INFO` & `polaris_lib-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polaris-lib
-Version: 0.3.0
+Version: 0.4.0
 Summary: Client for the Polaris Hub.
 Author-email: Lu Zhu <lu@valencediscovery.com>, Hadrien Mary <hadrien@valencediscovery.com>, Julien St-Laurent <julien.stl@valencediscovery.com>, Cas Wognum <cas@valencediscovery.com>
 Project-URL: Website, https://polarishub.io/
 Project-URL: Source Code, https://github.com/polaris-hub/polaris
 Project-URL: Bug Tracker, https://github.com/polaris-hub/polaris/issues
 Project-URL: Documentation, https://polaris-hub.github.io/polaris/
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polaris-lib Version: 0.3.0 Summary: Client for the
+Metadata-Version: 2.1 Name: polaris-lib Version: 0.4.0 Summary: Client for the
 Polaris Hub. Author-email: Lu Zhu
 valencediscovery.com>, Hadrien Mary
 valencediscovery.com>, Julien St-Laurent
 valencediscovery.com>, Cas Wognum
 valencediscovery.com> Project-URL: Website, https://polarishub.io/ Project-URL:
 Source Code, https://github.com/polaris-hub/polaris Project-URL: Bug Tracker,
 https://github.com/polaris-hub/polaris/issues Project-URL: Documentation,
```

### Comparing `polaris_lib-0.3.0/README.md` & `polaris_lib-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/docs/assets/css/custom-polaris.css` & `polaris_lib-0.4.0/docs/assets/css/custom-polaris.css`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/docs/index.md` & `polaris_lib-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/docs/quickstart.md` & `polaris_lib-0.4.0/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/docs/tutorials/basics.ipynb` & `polaris_lib-0.4.0/docs/tutorials/basics.ipynb`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/docs/tutorials/custom_dataset_benchmark.ipynb` & `polaris_lib-0.4.0/docs/tutorials/custom_dataset_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/docs/tutorials/data_curation.ipynb` & `polaris_lib-0.4.0/docs/tutorials/data_curation.ipynb`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/docs/tutorials/dataset_factory.ipynb` & `polaris_lib-0.4.0/docs/tutorials/dataset_factory.ipynb`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/docs/tutorials/dataset_zarr.ipynb` & `polaris_lib-0.4.0/docs/tutorials/dataset_zarr.ipynb`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/env.yml` & `polaris_lib-0.4.0/env.yml`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/mkdocs.yml` & `polaris_lib-0.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/_artifact.py` & `polaris_lib-0.4.0/polaris/_artifact.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/benchmark/_base.py` & `polaris_lib-0.4.0/polaris/benchmark/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,15 +384,17 @@
         if isinstance(self.split[1], dict):
             test = {k: _get_subset(v, hide_targets=True) for k, v in self.split[1].items()}
         else:
             test = _get_subset(self.split[1], hide_targets=True)
 
         return train, test
 
-    def evaluate(self, y_pred: PredictionsType) -> BenchmarkResults:
+    def evaluate(
+        self, y_pred: Optional[PredictionsType] = None, y_prob: Optional[PredictionsType] = None
+    ) -> BenchmarkResults:
         """Execute the evaluation protocol for the benchmark, given a set of predictions.
 
         info: What about `y_true`?
             Contrary to other frameworks that you might be familiar with, we opted for a signature that includes just
             the predictions. This reduces the chance of accidentally using the test targets during training.
 
         For this method, we make the following assumptions:
@@ -404,14 +406,15 @@
         5. There can be metrics which measure across tasks.
 
         Args:
             y_pred: The predictions for the test set, as NumPy arrays.
                 If there are multiple targets, the predictions should be wrapped in a dictionary with the target labels as keys.
                 If there are multiple test sets, the predictions should be further wrapped in a dictionary
                     with the test subset labels as keys.
+            y_prob: The predicted probabilities for the test set, as NumPy arrays.
 
         Returns:
             A `BenchmarkResults` object. This object can be directly submitted to the Polaris Hub.
         """
 
         # Instead of having the user pass the ground truth, we extract it from the benchmark spec ourselves.
         # This simplifies the API, but also was added to make accidental access to the test set targets less likely.
@@ -425,35 +428,42 @@
         for k, test_subset in test.items():
             with tmp_attribute_change(test_subset, "_hide_targets", False):
                 y_true[k] = test_subset.targets
 
         if not isinstance(y_pred, dict) or all(k in self.target_cols for k in y_pred):
             y_pred = {"test": y_pred}
 
-        if any(k not in y_pred for k in test.keys()):
+        if not isinstance(y_prob, dict) or all(k in self.target_cols for k in y_prob):
+            y_prob = {"test": y_prob}
+
+        if any(k not in y_pred for k in test.keys()) and any(k not in y_prob for k in test.keys()):
             raise KeyError(
                 f"Missing keys for at least one of the test sets. Expecting: {sorted(test.keys())}"
             )
 
         # Results are saved in a tabular format. For more info, see the BenchmarkResults docs.
         scores: ResultsType = pd.DataFrame(columns=BenchmarkResults.RESULTS_COLUMNS)
 
         # For every test set...
         for test_label, y_true_subset in y_true.items():
             # For every metric...
             for metric in self.metrics:
                 if metric.is_multitask:
                     # Multi-task but with a metric across targets
-                    score = metric(y_true=y_true_subset, y_pred=y_pred[test_label])
+                    score = metric(
+                        y_true=y_true_subset, y_pred=y_pred.get(test_label), y_prob=y_prob.get(test_label)
+                    )
                     scores.loc[len(scores)] = (test_label, "aggregated", metric, score)
                     continue
 
                 if not isinstance(y_true_subset, dict):
                     # Single task
-                    score = metric(y_true=y_true_subset, y_pred=y_pred[test_label])
+                    score = metric(
+                        y_true=y_true_subset, y_pred=y_pred.get(test_label), y_prob=y_prob.get(test_label)
+                    )
                     scores.loc[len(scores)] = (
                         test_label,
                         self.target_cols[0],
                         metric,
                         score,
                     )
                     continue
@@ -461,15 +471,20 @@
                 # Otherwise, for every target...
                 for target_label, y_true_target in y_true_subset.items():
                     # Single-task metrics for a multi-task benchmark
                     # In such a setting, there can be NaN values, which we thus have to filter out.
                     mask = ~np.isnan(y_true_target)
                     score = metric(
                         y_true=y_true_target[mask],
-                        y_pred=y_pred[test_label][target_label][mask],
+                        y_pred=y_pred[test_label][target_label][mask]
+                        if y_pred[test_label] is not None
+                        else None,
+                        y_prob=y_prob[test_label][target_label][mask]
+                        if y_prob[test_label] is not None
+                        else None,
                     )
                     scores.loc[len(scores)] = (test_label, target_label, metric, score)
 
         return BenchmarkResults(results=scores, benchmark_name=self.name, benchmark_owner=self.owner)
 
     def upload_to_hub(
         self,
```

### Comparing `polaris_lib-0.3.0/polaris/benchmark/_definitions.py` & `polaris_lib-0.4.0/polaris/benchmark/_definitions.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/cli.py` & `polaris_lib-0.4.0/polaris/cli.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/curation/_chemistry_curator.py` & `polaris_lib-0.4.0/polaris/curation/_chemistry_curator.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/curation/_curator.py` & `polaris_lib-0.4.0/polaris/curation/_curator.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/curation/_data_curator.py` & `polaris_lib-0.4.0/polaris/curation/_data_curator.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/curation/utils.py` & `polaris_lib-0.4.0/polaris/curation/utils.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/curation/viz_utils.py` & `polaris_lib-0.4.0/polaris/curation/viz_utils.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/dataset/_adapters.py` & `polaris_lib-0.4.0/polaris/dataset/_adapters.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/dataset/_column.py` & `polaris_lib-0.4.0/polaris/dataset/_column.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/dataset/_dataset.py` & `polaris_lib-0.4.0/polaris/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/dataset/_factory.py` & `polaris_lib-0.4.0/polaris/dataset/_factory.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/dataset/_subset.py` & `polaris_lib-0.4.0/polaris/dataset/_subset.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/dataset/converters/_base.py` & `polaris_lib-0.4.0/polaris/dataset/converters/_base.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/dataset/converters/_sdf.py` & `polaris_lib-0.4.0/polaris/dataset/converters/_sdf.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/dataset/converters/_zarr.py` & `polaris_lib-0.4.0/polaris/dataset/converters/_zarr.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/evaluate/_results.py` & `polaris_lib-0.4.0/polaris/evaluate/_results.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/hub/client.py` & `polaris_lib-0.4.0/polaris/hub/client.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/hub/polarisfs.py` & `polaris_lib-0.4.0/polaris/hub/polarisfs.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/hub/settings.py` & `polaris_lib-0.4.0/polaris/hub/settings.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/loader/load.py` & `polaris_lib-0.4.0/polaris/loader/load.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/utils/dict2html.py` & `polaris_lib-0.4.0/polaris/utils/dict2html.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/utils/errors.py` & `polaris_lib-0.4.0/polaris/utils/errors.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/utils/httpx.py` & `polaris_lib-0.4.0/polaris/utils/httpx.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/utils/misc.py` & `polaris_lib-0.4.0/polaris/utils/misc.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/polaris/utils/types.py` & `polaris_lib-0.4.0/polaris/utils/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 HttpUrlString: TypeAlias = Annotated[HttpUrl, AfterValidator(str)]
 """
 A validated URL that will be turned into a string.
 This is useful for interactions with httpx and authlib, who have their own URL types.
 """
 
-DirectionType: TypeAlias = Literal["min", "max"]
+DirectionType: TypeAlias = float | Literal["min", "max"]
 """
 The direction of any variable to be sorted.
 This can be used to sort the metric score, indicate the optmization direction of endpoint.
 """
 
 AccessType: TypeAlias = Literal["public", "private"]
 """
```

### Comparing `polaris_lib-0.3.0/polaris_lib.egg-info/PKG-INFO` & `polaris_lib-0.4.0/polaris_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polaris-lib
-Version: 0.3.0
+Version: 0.4.0
 Summary: Client for the Polaris Hub.
 Author-email: Lu Zhu <lu@valencediscovery.com>, Hadrien Mary <hadrien@valencediscovery.com>, Julien St-Laurent <julien.stl@valencediscovery.com>, Cas Wognum <cas@valencediscovery.com>
 Project-URL: Website, https://polarishub.io/
 Project-URL: Source Code, https://github.com/polaris-hub/polaris
 Project-URL: Bug Tracker, https://github.com/polaris-hub/polaris/issues
 Project-URL: Documentation, https://polaris-hub.github.io/polaris/
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polaris-lib Version: 0.3.0 Summary: Client for the
+Metadata-Version: 2.1 Name: polaris-lib Version: 0.4.0 Summary: Client for the
 Polaris Hub. Author-email: Lu Zhu
 valencediscovery.com>, Hadrien Mary
 valencediscovery.com>, Julien St-Laurent
 valencediscovery.com>, Cas Wognum
 valencediscovery.com> Project-URL: Website, https://polarishub.io/ Project-URL:
 Source Code, https://github.com/polaris-hub/polaris Project-URL: Bug Tracker,
 https://github.com/polaris-hub/polaris/issues Project-URL: Documentation,
```

### Comparing `polaris_lib-0.3.0/polaris_lib.egg-info/SOURCES.txt` & `polaris_lib-0.4.0/polaris_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/pyproject.toml` & `polaris_lib-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/tests/conftest.py` & `polaris_lib-0.4.0/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 @pytest.fixture(scope="module")
 def test_data():
     data = dm.data.freesolv()[:100]
     # set an abitrary threshold for testing purpose.
     data["CLASS_expt"] = data["expt"].gt(0).astype(int).values
     data["CLASS_calc"] = data["calc"].gt(0).astype(int).values
+    data["MULTICLASS_expt"] = np.random.randint(low=0, high=3, size=data.shape[0])
+    data["MULTICLASS_calc"] = np.random.randint(low=0, high=3, size=data.shape[0])
     return data
 
 
 @pytest.fixture(scope="module")
 def caffeine():
     # Let's generate a toy dataset with a single molecule
     smiles = "Cn1cnc2c1c(=O)n(C)c(=O)n2C"
@@ -95,14 +97,15 @@
         metrics=[
             "mean_absolute_error",
             "mean_squared_error",
             "r2",
             "spearmanr",
             "pearsonr",
             "explained_var",
+            "absolute_average_fold_error",
         ],
         main_metric="mean_absolute_error",
         split=(train_indices, test_indices),
         target_cols="expt",
         input_cols="smiles",
     )
     check_version(benchmark)
@@ -113,48 +116,100 @@
 def test_single_task_benchmark_clf(test_dataset):
     train_indices = list(range(90))
     test_indices = list(range(90, 100))
     benchmark = SingleTaskBenchmarkSpecification(
         name="single-task-benchmark",
         dataset=test_dataset,
         main_metric="accuracy",
-        metrics=["accuracy", "f1", "roc_auc", "pr_auc", "mcc", "cohen_kappa"],
+        metrics=["accuracy", "f1", "roc_auc", "pr_auc", "mcc", "cohen_kappa", "balanced_accuracy"],
         split=(train_indices, test_indices),
         target_cols="CLASS_expt",
         input_cols="smiles",
     )
     check_version(benchmark)
     return benchmark
 
 
 @pytest.fixture(scope="function")
+def test_single_task_benchmark_multi_clf(test_dataset):
+    np.random.seed(111)
+    indices = np.arange(100)
+    np.random.shuffle(indices)
+    train_indices = indices[:80]
+    test_indices = indices[80:]
+
+    benchmark = SingleTaskBenchmarkSpecification(
+        name="single-task-benchmark",
+        dataset=test_dataset,
+        main_metric="accuracy",
+        metrics=[
+            "accuracy",
+            "balanced_accuracy",
+            "mcc",
+            "cohen_kappa",
+            "f1_macro",
+            "f1_micro",
+            "roc_auc_ovr",
+            "roc_auc_ovo",
+            "pr_auc",
+        ],
+        split=(train_indices, test_indices),
+        target_cols="MULTICLASS_expt",
+        input_cols="smiles",
+    )
+    check_version(benchmark)
+    return benchmark
+
+
+@pytest.fixture(scope="function")
 def test_single_task_benchmark_multiple_test_sets(test_dataset):
     train_indices = list(range(90))
     test_indices = {"test_1": list(range(90, 95)), "test_2": list(range(95, 100))}
     benchmark = SingleTaskBenchmarkSpecification(
         name="single-task-benchmark",
         dataset=test_dataset,
         metrics=[
             "mean_absolute_error",
             "mean_squared_error",
             "r2",
             "spearmanr",
             "pearsonr",
             "explained_var",
+            "absolute_average_fold_error",
         ],
         main_metric="r2",
         split=(train_indices, test_indices),
         target_cols="expt",
         input_cols="smiles",
     )
     check_version(benchmark)
     return benchmark
 
 
 @pytest.fixture(scope="function")
+def test_single_task_benchmark_clf_multiple_test_sets(test_dataset):
+    np.random.seed(111)  # make sure two classes in `y_true`
+    indices = np.arange(100)
+    np.random.shuffle(indices)
+    train_indices = indices[:80]
+    test_indices = {"test_1": indices[80:90], "test_2": indices[90:]}
+    benchmark = SingleTaskBenchmarkSpecification(
+        name="single-task-benchmark-clf",
+        dataset=test_dataset,
+        metrics=["accuracy", "f1", "roc_auc", "pr_auc", "mcc", "cohen_kappa"],
+        main_metric="pr_auc",
+        split=(train_indices, test_indices),
+        target_cols="CLASS_calc",
+        input_cols="smiles",
+    )
+    check_version(benchmark)
+    return benchmark
+
+
+@pytest.fixture(scope="function")
 def test_multi_task_benchmark(test_dataset):
     # For the sake of simplicity, just use a small set of indices
     train_indices = list(range(90))
     test_indices = list(range(90, 100))
     benchmark = MultiTaskBenchmarkSpecification(
         name="multi-task-benchmark",
         dataset=test_dataset,
@@ -162,14 +217,15 @@
         metrics=[
             "mean_absolute_error",
             "mean_squared_error",
             "r2",
             "spearmanr",
             "pearsonr",
             "explained_var",
+            "absolute_average_fold_error",
         ],
         split=(train_indices, test_indices),
         target_cols=["expt", "calc"],
         input_cols="smiles",
         target_types={"expt": "regression"},
     )
     check_version(benchmark)
```

### Comparing `polaris_lib-0.3.0/tests/test_benchmark.py` & `polaris_lib-0.4.0/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/tests/test_curation.py` & `polaris_lib-0.4.0/tests/test_curation.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/tests/test_dataset.py` & `polaris_lib-0.4.0/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/tests/test_factory.py` & `polaris_lib-0.4.0/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/tests/test_integration.py` & `polaris_lib-0.4.0/tests/test_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datamol as dm
 import numpy as np
-from sklearn.ensemble import RandomForestRegressor
+from sklearn.ensemble import RandomForestRegressor, RandomForestClassifier
 
 from polaris.evaluate import BenchmarkResults
 
 
 def test_single_task_benchmark_loop(test_single_task_benchmark):
     """Tests the integrated API for a single-task benchmark."""
     train, test = test_single_task_benchmark.get_train_test_split()
@@ -37,14 +37,39 @@
         x_test = np.array([dm.to_fp(dm.to_mol(smi)) for smi in test_subset.inputs])
         y_pred[k] = model.predict(x_test)
 
     scores = test_single_task_benchmark_multiple_test_sets.evaluate(y_pred)
     assert isinstance(scores, BenchmarkResults)
 
 
+def test_single_task_benchmark_clf_loop_with_multiple_test_sets(
+    test_single_task_benchmark_clf_multiple_test_sets,
+):
+    """Tests the integrated API for a single-task benchmark for classification probabilities with multiple test sets."""
+    train, test = test_single_task_benchmark_clf_multiple_test_sets.get_train_test_split()
+
+    smiles, y = train.as_array("xy")
+
+    x_train = np.array([dm.to_fp(dm.to_mol(smi)) for smi in smiles])
+
+    model = RandomForestClassifier()
+    model.fit(X=x_train, y=y)
+
+    y_prob = {}
+    y_pred = {}
+    for k, test_subset in test.items():
+        print(k, test_subset)
+        x_test = np.array([dm.to_fp(dm.to_mol(smi)) for smi in test_subset.inputs])
+        y_prob[k] = model.predict_proba(x_test)[:, :1]  # for binary classification
+        y_pred[k] = model.predict(x_test)
+
+    scores = test_single_task_benchmark_clf_multiple_test_sets.evaluate(y_prob=y_prob, y_pred=y_pred)
+    assert isinstance(scores, BenchmarkResults)
+
+
 def test_multi_task_benchmark_loop(test_multi_task_benchmark):
     """Tests the integrated API for a multi-task benchmark."""
     train, test = test_multi_task_benchmark.get_train_test_split()
 
     smiles, multi_y = train.as_array("xy")
     x_train = np.array([dm.to_fp(dm.to_mol(smi)) for smi in smiles])
     x_test = np.array([dm.to_fp(dm.to_mol(smi)) for smi in test.inputs])
```

### Comparing `polaris_lib-0.3.0/tests/test_subset.py` & `polaris_lib-0.4.0/tests/test_subset.py`

 * *Files identical despite different names*

### Comparing `polaris_lib-0.3.0/tests/test_type_checks.py` & `polaris_lib-0.4.0/tests/test_type_checks.py`

 * *Files identical despite different names*

