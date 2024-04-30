# Comparing `tmp/timeseriesflattener-2.1.2.tar.gz` & `tmp/timeseriesflattener-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-2.1.2.tar", last modified: Thu Apr 18 11:02:06 2024, max compression
+gzip compressed data, was "timeseriesflattener-2.2.0.tar", last modified: Tue Apr 30 09:05:45 2024, max compression
```

## Comparing `timeseriesflattener-2.1.2.tar` & `timeseriesflattener-2.2.0.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.203967 timeseriesflattener-2.1.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.139966 timeseriesflattener-2.1.2/.devcontainer/
--rw-r--r--   0 root         (0) root         (0)     1639 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.devcontainer/devcontainer.json
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.devcontainer/post-start.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.143966 timeseriesflattener-2.1.2/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.131966 timeseriesflattener-2.1.2/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.143966 timeseriesflattener-2.1.2/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      901 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.143966 timeseriesflattener-2.1.2/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      885 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.143966 timeseriesflattener-2.1.2/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      636 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/workflows/benchmark.yml
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)      849 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      898 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     1939 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)      788 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2885 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)      697 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.python-version
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.143966 timeseriesflattener-2.1.2/.vscode/
--rw-r--r--   0 root         (0) root         (0)      346 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.vscode/extensions.json
--rw-r--r--   0 root         (0) root         (0)      249 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.vscode/settings.json
--rw-r--r--   0 root         (0) root         (0)     1373 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.vscode/tasks.json
--rw-r--r--   0 root         (0) root         (0)     1286 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    73523 2024-04-18 11:02:00.000000 timeseriesflattener-2.1.2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1031 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1087 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/Makefile
--rw-r--r--   0 root         (0) root         (0)    11505 2024-04-18 11:02:06.203967 timeseriesflattener-2.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7629 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1763 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.147966 timeseriesflattener-2.1.2/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.147966 timeseriesflattener-2.1.2/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   424821 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)      291 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/aggregators.rst
--rw-r--r--   0 root         (0) root         (0)     4115 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     1013 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)      295 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/flattener.rst
--rw-r--r--   0 root         (0) root         (0)     5165 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/installation.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.147966 timeseriesflattener-2.1.2/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   128585 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    40071 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    24394 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/tutorials/03_text.ipynb
--rw-r--r--   0 root         (0) root         (0)     5314 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/tutorials/04_from_legacy.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.151966 timeseriesflattener-2.1.2/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)     1833 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/example.py
--rw-r--r--   0 root         (0) root         (0)    49714 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/icon.png
--rw-r--r--   0 root         (0) root         (0)      426 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/lefthook.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.151966 timeseriesflattener-2.1.2/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4633 2024-04-18 11:02:00.000000 timeseriesflattener-2.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2520 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/requirements-dev.lock
--rw-r--r--   0 root         (0) root         (0)     1474 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/requirements.lock
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 11:02:06.203967 timeseriesflattener-2.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.151966 timeseriesflattener-2.1.2/src/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5207 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/test_benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.155966 timeseriesflattener-2.1.2/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      721 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1467 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/_frame_validator.py
--rw-r--r--   0 root         (0) root         (0)     3852 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/_intermediary_frames.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/aggregators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.155966 timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      215 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/default_column_names.py
--rw-r--r--   0 root         (0) root         (0)     3708 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/from_legacy.py
--rw-r--r--   0 root         (0) root         (0)     2825 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/meta.py
--rw-r--r--   0 root         (0) root         (0)     2498 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/outcome.py
--rw-r--r--   0 root         (0) root         (0)     1723 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1389 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/predictor.py
--rw-r--r--   0 root         (0) root         (0)     1434 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/static.py
--rw-r--r--   0 root         (0) root         (0)     1349 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/test_from_legacy.py
--rw-r--r--   0 root         (0) root         (0)     1917 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/test_specs.py
--rw-r--r--   0 root         (0) root         (0)     2144 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/timedelta.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/timestamp_frame.py
--rw-r--r--   0 root         (0) root         (0)     5993 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/flattener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.159966 timeseriesflattener-2.1.2/src/timeseriesflattener/frame_utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/frame_utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/frame_utilities/_horisontally_concat.py
--rw-r--r--   0 root         (0) root         (0)      644 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py
--rw-r--r--   0 root         (0) root         (0)      937 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/process_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.159966 timeseriesflattener-2.1.2/src/timeseriesflattener/spec_processors/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/spec_processors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/spec_processors/static.py
--rw-r--r--   0 root         (0) root         (0)     6595 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/spec_processors/temporal.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/spec_processors/test_static.py
--rw-r--r--   0 root         (0) root         (0)     8576 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/spec_processors/test_temporal.py
--rw-r--r--   0 root         (0) root         (0)     1524 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/spec_processors/timedelta.py
--rw-r--r--   0 root         (0) root         (0)     4997 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/test_aggregators.py
--rw-r--r--   0 root         (0) root         (0)     9793 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/test_flattener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.159966 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     1519 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.159966 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5619 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2746 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     1958 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.135966 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.131966 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.159966 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1494 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.175967 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      754 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)      830 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      807 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   200734 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv
--rw-r--r--   0 root         (0) root         (0)   248865 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     5511 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.179967 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/
--rw-r--r--   0 root         (0) root         (0)      264 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2855 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1070 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/df_transforms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.179967 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1980 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6112 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.179967 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/feature_specs/
--rw-r--r--   0 root         (0) root         (0)     5535 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/feature_specs/group_specs.py
--rw-r--r--   0 root         (0) root         (0)     7823 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/feature_specs/single_specs.py
--rw-r--r--   0 root         (0) root         (0)    35049 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/logger.py
--rw-r--r--   0 root         (0) root         (0)     7524 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/misc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.179967 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/
--rw-r--r--   0 root         (0) root         (0)     2981 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.179967 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5527 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2697 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     1962 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.135966 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.135966 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.183967 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1461 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.183967 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1877 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.199967 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)      795 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      772 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      696 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   200734 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv
--rw-r--r--   0 root         (0) root         (0)   248865 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     5446 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.199967 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.199967 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3232 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.199967 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13595 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1295 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py
--rw-r--r--   0 root         (0) root         (0)     3399 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.199967 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23392 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2663 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2308 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2321 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     5796 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.203967 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/utils/
--rw-r--r--   0 root         (0) root         (0)      984 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/src/timeseriesflattener/v1/utils/pydantic_basemodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 11:02:06.203967 timeseriesflattener-2.1.2/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11505 2024-04-18 11:02:06.000000 timeseriesflattener-2.1.2/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8537 2024-04-18 11:02:06.000000 timeseriesflattener-2.1.2/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 11:02:06.000000 timeseriesflattener-2.1.2/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      650 2024-04-18 11:02:06.000000 timeseriesflattener-2.1.2/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-04-18 11:02:06.000000 timeseriesflattener-2.1.2/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     8330 2024-04-18 11:01:59.000000 timeseriesflattener-2.1.2/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.674690 timeseriesflattener-2.2.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.610690 timeseriesflattener-2.2.0/.devcontainer/
+-rw-r--r--   0 root         (0) root         (0)     1639 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.devcontainer/post-start.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.610690 timeseriesflattener-2.2.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.602690 timeseriesflattener-2.2.0/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.614690 timeseriesflattener-2.2.0/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      901 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.614690 timeseriesflattener-2.2.0/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.614690 timeseriesflattener-2.2.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      636 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/benchmark.yml
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      898 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     1939 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)      788 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      697 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.python-version
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.614690 timeseriesflattener-2.2.0/.vscode/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.vscode/extensions.json
+-rw-r--r--   0 root         (0) root         (0)      249 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.vscode/settings.json
+-rw-r--r--   0 root         (0) root         (0)     1373 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.vscode/tasks.json
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    73705 2024-04-30 09:05:40.000000 timeseriesflattener-2.2.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11507 2024-04-30 09:05:45.674690 timeseriesflattener-2.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7631 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.618690 timeseriesflattener-2.2.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.618690 timeseriesflattener-2.2.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   424821 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)      291 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/aggregators.rst
+-rw-r--r--   0 root         (0) root         (0)     4115 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     1013 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)      295 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/flattener.rst
+-rw-r--r--   0 root         (0) root         (0)     5165 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/installation.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.618690 timeseriesflattener-2.2.0/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   128585 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    40071 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)    24394 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/03_text.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5314 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/04_from_legacy.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.622690 timeseriesflattener-2.2.0/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/example.py
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/icon.png
+-rw-r--r--   0 root         (0) root         (0)      426 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/lefthook.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.622690 timeseriesflattener-2.2.0/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4633 2024-04-30 09:05:40.000000 timeseriesflattener-2.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/requirements-dev.lock
+-rw-r--r--   0 root         (0) root         (0)     1474 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/requirements.lock
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 09:05:45.674690 timeseriesflattener-2.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.622690 timeseriesflattener-2.2.0/src/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/test_benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.622690 timeseriesflattener-2.2.0/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      721 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/_frame_validator.py
+-rw-r--r--   0 root         (0) root         (0)     3852 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/_intermediary_frames.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/aggregators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.626690 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      215 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/default_column_names.py
+-rw-r--r--   0 root         (0) root         (0)     3708 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/from_legacy.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/meta.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/predictor.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/static.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/test_from_legacy.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/test_specs.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/timedelta.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/timestamp_frame.py
+-rw-r--r--   0 root         (0) root         (0)     6278 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/flattener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.626690 timeseriesflattener-2.2.0/src/timeseriesflattener/frame_utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/frame_utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/frame_utilities/_horisontally_concat.py
+-rw-r--r--   0 root         (0) root         (0)      644 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/process_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.630690 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/static.py
+-rw-r--r--   0 root         (0) root         (0)    10222 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/temporal.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/test_static.py
+-rw-r--r--   0 root         (0) root         (0)    10508 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/test_temporal.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/timedelta.py
+-rw-r--r--   0 root         (0) root         (0)     4997 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/test_aggregators.py
+-rw-r--r--   0 root         (0) root         (0)    11028 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/test_flattener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.630690 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     1519 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.630690 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.602690 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.602690 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.630690 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1494 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.646690 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      754 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)      830 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      807 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   200734 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv
+-rw-r--r--   0 root         (0) root         (0)   248865 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5511 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.650690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/
+-rw-r--r--   0 root         (0) root         (0)      264 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/df_transforms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.650690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6112 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.650690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)     5535 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_specs/group_specs.py
+-rw-r--r--   0 root         (0) root         (0)     7823 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_specs/single_specs.py
+-rw-r--r--   0 root         (0) root         (0)    35049 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7524 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/misc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.650690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/
+-rw-r--r--   0 root         (0) root         (0)     2981 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.650690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5527 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.606690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.606690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.650690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.654690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.666690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)      795 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      772 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      696 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   200734 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv
+-rw-r--r--   0 root         (0) root         (0)   248865 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5446 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.670690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.670690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3232 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.670690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13595 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.670690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23392 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     5796 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.670690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/utils/
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/utils/pydantic_basemodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.670690 timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11507 2024-04-30 09:05:45.000000 timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8537 2024-04-30 09:05:45.000000 timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 09:05:45.000000 timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      650 2024-04-30 09:05:45.000000 timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-04-30 09:05:45.000000 timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     8330 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/tasks.py
```

### Comparing `timeseriesflattener-2.1.2/.devcontainer/devcontainer.json` & `timeseriesflattener-2.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.github/actions/test/action.yml` & `timeseriesflattener-2.2.0/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-2.2.0/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.github/dependabot.yml` & `timeseriesflattener-2.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.github/recommended_repo_setup.md` & `timeseriesflattener-2.2.0/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.github/workflows/benchmark.yml` & `timeseriesflattener-2.2.0/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.github/workflows/check_for_rej.yml` & `timeseriesflattener-2.2.0/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-2.2.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.github/workflows/documentation.yml` & `timeseriesflattener-2.2.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-2.2.0/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-2.2.0/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.github/workflows/pre-commit.yml` & `timeseriesflattener-2.2.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.github/workflows/stalebot.yml` & `timeseriesflattener-2.2.0/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.github/workflows/static_type_checks.yml` & `timeseriesflattener-2.2.0/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.gitignore` & `timeseriesflattener-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.pre-commit-config.yaml` & `timeseriesflattener-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.vscode/tasks.json` & `timeseriesflattener-2.2.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/.zenodo.json` & `timeseriesflattener-2.2.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/CHANGELOG.md` & `timeseriesflattener-2.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.2.0 (2024-04-30)
+
+### Feature
+
+* Bump release ([`879e752`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/879e752928808f8c3927808cab6a2f9a80a85610))
+
 ## v2.1.2 (2024-04-18)
 
 ### Fix
 
 * Ensure entity col name is passed to the valueframe in legacy spec ([`6702cb9`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/6702cb9b03c857a864100b7552540f3f60fe8968))
 
 ## v2.1.1 (2024-04-18)
```

### Comparing `timeseriesflattener-2.1.2/CODE_OF_CONDUCT.md` & `timeseriesflattener-2.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/CONTRIBUTING.md` & `timeseriesflattener-2.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/Dockerfile` & `timeseriesflattener-2.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/LICENSE` & `timeseriesflattener-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/PKG-INFO` & `timeseriesflattener-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 2.1.2
+Version: 2.2.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
         
@@ -85,19 +85,19 @@
 [![github actions pytest](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/actions/workflows/main_test_and_release.yml/badge.svg)](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/actions)
 [![python versions](https://img.shields.io/pypi/pyversions/timeseriesflattener)](https://pypi.org/project/timeseriesflattener/)
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 
 [![PyPI version](https://badge.fury.io/py/timeseriesflattener.svg)](https://pypi.org/project/timeseriesflattener/)
 [![status](https://joss.theoj.org/papers/3bbea8745668d1aa40ff796c6fd3db87/status.svg)](https://joss.theoj.org/papers/3bbea8745668d1aa40ff796c6fd3db87)
 
-Time series from e.g. electronic health records often have a large number of variables, are sampled at irregular intervals and tend to have a large number of missing values. Before this type of data can be used for prediction modelling with machine learning methods such as logistic regression or XGBoost, the data needs to be reshaped. 
+Time series from e.g. electronic health records often have a large number of variables, are sampled at irregular intervals and tend to have a large number of missing values. Before this type of data can be used for prediction modelling with machine learning methods such as logistic regression or XGBoost, the data needs to be reshaped.  
 
 In essence, the time series need to be *flattened* so that each prediction time is represented by a set of predictor values and an outcome value. These predictor values can be constructed by aggregating the preceding values in the time series within a certain time window. 
 
-`timeseriesflattener` aims to simplify this process by providing an easy-to-use and fully-specified pipeline for flattening complex time series. 
+`timeseriesflattener` aims to simplify this process by providing an easy-to-use and fully-specified pipeline for flattening complex time series.  
 
 ## 🔧 Installation
 To get started using timeseriesflattener simply install it using pip by running the following line in your terminal:
 
 ```
 pip install timeseriesflattener
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.1.2 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-2.1.2/README.md` & `timeseriesflattener-2.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 [![github actions pytest](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/actions/workflows/main_test_and_release.yml/badge.svg)](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/actions)
 [![python versions](https://img.shields.io/pypi/pyversions/timeseriesflattener)](https://pypi.org/project/timeseriesflattener/)
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 
 [![PyPI version](https://badge.fury.io/py/timeseriesflattener.svg)](https://pypi.org/project/timeseriesflattener/)
 [![status](https://joss.theoj.org/papers/3bbea8745668d1aa40ff796c6fd3db87/status.svg)](https://joss.theoj.org/papers/3bbea8745668d1aa40ff796c6fd3db87)
 
-Time series from e.g. electronic health records often have a large number of variables, are sampled at irregular intervals and tend to have a large number of missing values. Before this type of data can be used for prediction modelling with machine learning methods such as logistic regression or XGBoost, the data needs to be reshaped. 
+Time series from e.g. electronic health records often have a large number of variables, are sampled at irregular intervals and tend to have a large number of missing values. Before this type of data can be used for prediction modelling with machine learning methods such as logistic regression or XGBoost, the data needs to be reshaped.  
 
 In essence, the time series need to be *flattened* so that each prediction time is represented by a set of predictor values and an outcome value. These predictor values can be constructed by aggregating the preceding values in the time series within a certain time window. 
 
-`timeseriesflattener` aims to simplify this process by providing an easy-to-use and fully-specified pipeline for flattening complex time series. 
+`timeseriesflattener` aims to simplify this process by providing an easy-to-use and fully-specified pipeline for flattening complex time series.  
 
 ## 🔧 Installation
 To get started using timeseriesflattener simply install it using pip by running the following line in your terminal:
 
 ```
 pip install timeseriesflattener
 ```
```

### Comparing `timeseriesflattener-2.1.2/citation.cff` & `timeseriesflattener-2.2.0/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/Makefile` & `timeseriesflattener-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/_static/favicon.ico` & `timeseriesflattener-2.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/_static/icon.png` & `timeseriesflattener-2.2.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/_static/icon_dark.png` & `timeseriesflattener-2.2.0/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/_static/terminology_figure.png` & `timeseriesflattener-2.2.0/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/conf.py` & `timeseriesflattener-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/faq.rst` & `timeseriesflattener-2.2.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/feature_specifications.rst` & `timeseriesflattener-2.2.0/docs/feature_specifications.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/index.rst` & `timeseriesflattener-2.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-2.2.0/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-2.2.0/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/tutorials/03_text.ipynb` & `timeseriesflattener-2.2.0/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/tutorials/04_from_legacy.ipynb` & `timeseriesflattener-2.2.0/docs/tutorials/04_from_legacy.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/tutorials/img/term_a.png` & `timeseriesflattener-2.2.0/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/tutorials/img/term_b.png` & `timeseriesflattener-2.2.0/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/tutorials/img/term_c.png` & `timeseriesflattener-2.2.0/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/docs/tutorials/img/term_d.png` & `timeseriesflattener-2.2.0/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/example.py` & `timeseriesflattener-2.2.0/example.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/icon.png` & `timeseriesflattener-2.2.0/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/paper/paper.bib` & `timeseriesflattener-2.2.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/paper/paper.md` & `timeseriesflattener-2.2.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/pyproject.toml` & `timeseriesflattener-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "2.1.2"
+version = "2.2.0"
 authors = [
   { name = "Lasse Hansen", email = "lasseh0310@gmail.com" },
   { name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com" },
   { name = "Kenneth Enevoldsen" },
   { name = "Martin Bernstorff", email = "martinbernstorff@gmail.com" },
 ]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
```

### Comparing `timeseriesflattener-2.1.2/requirements-dev.lock` & `timeseriesflattener-2.2.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/requirements.lock` & `timeseriesflattener-2.2.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/conftest.py` & `timeseriesflattener-2.2.0/src/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/test_benchmark.py` & `timeseriesflattener-2.2.0/src/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/__init__.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/__init__.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/_frame_validator.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/_frame_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/_intermediary_frames.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/_intermediary_frames.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/aggregators.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/aggregators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/from_legacy.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/from_legacy.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/meta.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,17 +36,22 @@
         value_timestamp_col_name: The name of the column containing the timestamps. Must be a string, and the column's values must be datetimes.
         Additional columns containing the values of the time series. The name of the columns will be used for feature naming.
     """
 
     init_df: InitVar[InitDF_T]
     entity_id_col_name: str = default_entity_id_col_name
     value_timestamp_col_name: str = "timestamp"
+    coerce_to_lazy: InitVar[bool] = True
+
+    def __post_init__(self, init_df: InitDF_T, coerce_to_lazy: bool):
+        if coerce_to_lazy:
+            self.df = _anyframe_to_lazyframe(init_df)
+        else:
+            self.df: pl.LazyFrame = init_df
 
-    def __post_init__(self, init_df: InitDF_T):
-        self.df = _anyframe_to_lazyframe(init_df)
         _validate_col_name_columns_exist(obj=self)
         self.value_col_names = [
             col
             for col in self.df.columns
             if col not in [self.entity_id_col_name, self.value_timestamp_col_name]
         ]
```

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/outcome.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/prediction_times.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/prediction_times.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,17 +28,21 @@
         timestamp_col_name: The name of the column containing the timestamps for when to make a prediction.
     """
 
     init_df: InitVar[InitDF_T]
     entity_id_col_name: str = default_entity_id_col_name
     timestamp_col_name: str = default_pred_time_col_name
     pred_time_uuid_col_name: str = default_pred_time_uuid_col_name
+    coerce_to_lazy: InitVar[bool] = True
 
-    def __post_init__(self, init_df: InitDF_T):
-        self.df = _anyframe_to_lazyframe(init_df)
+    def __post_init__(self, init_df: InitDF_T, coerce_to_lazy: bool):
+        if coerce_to_lazy:
+            self.df = _anyframe_to_lazyframe(init_df)
+        else:
+            self.df: pl.LazyFrame = init_df
 
         self.df = self.df.with_columns(
             pl.concat_str(
                 pl.col(self.entity_id_col_name), pl.lit("-"), pl.col(self.timestamp_col_name)
             ).alias(self.pred_time_uuid_col_name)
         )
```

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/predictor.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/predictor.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/static.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/test_from_legacy.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/test_from_legacy.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/test_specs.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/test_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/timedelta.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/timedelta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/feature_specs/timestamp_frame.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/timestamp_frame.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/flattener.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/flattener.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from functools import partial
 from multiprocessing import Pool
 from typing import TYPE_CHECKING, Union
+import datetime as dt
 
 import polars as pl
 import tqdm
 from iterpy.iter import Iter
 from rich.progress import track
 
 from timeseriesflattener.frame_utilities._horisontally_concat import horizontally_concatenate_dfs
@@ -93,15 +94,17 @@
 
 @dataclass
 class Flattener:
     predictiontime_frame: PredictionTimeFrame
     compute_lazily: bool = False
     n_workers: int | None = None
 
-    def aggregate_timeseries(self, specs: Sequence[ValueSpecification]) -> AggregatedFrame:
+    def aggregate_timeseries(
+        self, specs: Sequence[ValueSpecification], step_size: dt.timedelta | None = None
+    ) -> AggregatedFrame:
         if self.compute_lazily:
             print(
                 "We have encountered performance issues on Windows when using lazy evaluation. If you encounter performance issues, try setting lazy=False."
             )
 
         # Check for conflicts in the specs
         conflicting_specs = _get_spec_conflicts(specs)
@@ -116,22 +119,26 @@
                 + "".join(errors.map(lambda error: f"  \n - {error.description}").to_list())
             )
 
         if not self.compute_lazily:
             self.predictiontime_frame.df = self.predictiontime_frame.collect()  # type: ignore
             for spec in specs:
                 spec.value_frame.df = spec.value_frame.collect()  # type: ignore
+        else:
+            self.predictiontime_frame.df = self.predictiontime_frame.df.lazy()
+            for spec in specs:
+                spec.value_frame.df = spec.value_frame.df.lazy()
 
         # Process and collect the specs. One-by-one, to get feedback on progress.
         dfs: Sequence[pl.LazyFrame] = []
         if self.n_workers is None:
             for spec in track(specs, description="Processing specs..."):
                 print(f"Processing spec: {spec.value_frame.value_col_names}")
                 processed_spec = process_spec(
-                    predictiontime_frame=self.predictiontime_frame, spec=spec
+                    predictiontime_frame=self.predictiontime_frame, spec=spec, step_size=step_size
                 )
 
                 if isinstance(processed_spec.df, pl.LazyFrame):
                     dfs.append(processed_spec.collect().lazy())
                 else:
                     dfs.append(processed_spec.df)
         else:
```

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/process_spec.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/process_spec.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
+import datetime as dt
 
 from .feature_specs.static import StaticSpec
 from .feature_specs.timedelta import TimeDeltaSpec
 from .spec_processors.static import process_static_spec
 from .spec_processors.temporal import process_temporal_spec
 from .spec_processors.timedelta import process_timedelta_spec
 
 if TYPE_CHECKING:
     from ._intermediary_frames import ProcessedFrame
     from .feature_specs.prediction_times import PredictionTimeFrame
     from .flattener import ValueSpecification
 
 
 def process_spec(
-    spec: ValueSpecification, predictiontime_frame: PredictionTimeFrame
+    spec: ValueSpecification,
+    predictiontime_frame: PredictionTimeFrame,
+    step_size: dt.timedelta | None = None,
 ) -> ProcessedFrame:
     if isinstance(spec, TimeDeltaSpec):
         return process_timedelta_spec(spec, predictiontime_frame)
     if isinstance(spec, StaticSpec):
         return process_static_spec(spec, predictiontime_frame)
 
-    return process_temporal_spec(spec=spec, predictiontime_frame=predictiontime_frame)
+    return process_temporal_spec(
+        spec=spec, predictiontime_frame=predictiontime_frame, step_size=step_size
+    )
```

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/spec_processors/static.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/spec_processors/test_static.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/test_static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/spec_processors/test_temporal.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/test_temporal.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import datetime as dt
 
+import numpy as np
 import polars as pl
 from timeseriesflattener.testing.utils_for_testing import str_to_pl_df
 
 import timeseriesflattener.spec_processors.temporal as process_spec
 import timeseriesflattener.spec_processors.timedelta
 from timeseriesflattener.feature_specs.predictor import PredictorSpec
 
@@ -284,7 +285,58 @@
     )
 
     expected = str_to_pl_df(
         """pred_time_uuid,pred_value_1_within_0_to_1_days_mean_fallback_0,pred_value_2_within_0_to_1_days_mean_fallback_0
 1-2021-01-01 00:00:00.000000,1,2"""
     )
     assert_frame_equal(result.collect(), expected)
+
+
+def test_sliding_window():
+    pred_frame = str_to_pl_df(
+        """entity_id,pred_timestamp
+                              1,2011-01-01,
+                              1,2014-01-01,
+                              1,2016-01-01,
+                              1,2018-01-01,
+                              1,2020-01-01,
+                              1,2022-01-01,"""  # 2012 year without prediction times
+    )
+
+    value_frame = str_to_pl_df(
+        """entity_id,timestamp,value
+                                1,2011-01-01,1
+                                1,2012-01-01,2
+                                1,2013-01-01,3
+                                1,2014-01-01,4
+                                1,2015-01-01,5
+                                1,2016-01-01,6
+                                1,2019-01-01,9
+                                1,2021-01-01,11 
+                                1,2021-01-01,12"""  # 2021 year with multiple values
+    )  # 2022 year with no values
+
+    result = process_spec.process_temporal_spec(
+        spec=PredictorSpec(
+            value_frame=ValueFrame(init_df=value_frame.lazy()),
+            lookbehind_distances=[
+                dt.timedelta(days=10),
+                dt.timedelta(days=365),
+            ],  # test multiple lookperiods
+            aggregators=[MeanAggregator()],
+            fallback=0,
+        ),
+        predictiontime_frame=PredictionTimeFrame(init_df=pred_frame.lazy()),
+        step_size=dt.timedelta(days=365),
+    )
+
+    expected = str_to_pl_df(
+        """pred_time_uuid,pred_value_within_0_to_10_days_mean_fallback_0,pred_value_within_0_to_365_days_mean_fallback_0
+1-2011-01-01 00:00:00.000000,1.0,1.0
+1-2014-01-01 00:00:00.000000,4.0,3.5
+1-2016-01-01 00:00:00.000000,6.0,5.5
+1-2018-01-01 00:00:00.000000,0.0,0.0
+1-2020-01-01 00:00:00.000000,0.0,9.0
+1-2022-01-01 00:00:00.000000,0.0,11.5"""
+    )
+
+    assert_frame_equal(result.collect(), expected)
```

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/spec_processors/timedelta.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/timedelta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/test_aggregators.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/test_aggregators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/test_flattener.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/test_flattener.py`

 * *Files 12% similar despite different names*

```diff
@@ -280,7 +280,38 @@
         ]
     )
     expected = str_to_pl_df(
         """pred_time_uuid,outc_value_within_5_to_30_days_mean_fallback_nan
 1-2022-01-01 00:00:00.000000,1"""
     )
     assert_frame_equal(result.collect(), expected, ignore_colums=["entity_id", "pred_timestamp"])
+
+
+def test_add_features_with_non_default_entity_id_col_name():
+    prediction_times_df_str = """dw_ek_borger,pred_timestamp,
+                            1,2022-01-01 00:00:00
+                            """
+    outcome_df_str = """dw_ek_borger,timestamp,value,
+                        1,2022-01-02 00:00:01, 2
+                        1,2022-01-15 00:00:00, 1
+                        """
+    result = flattener.Flattener(
+        predictiontime_frame=PredictionTimeFrame(
+            init_df=str_to_pl_df(prediction_times_df_str), entity_id_col_name="dw_ek_borger"
+        )
+    ).aggregate_timeseries(
+        specs=[
+            OutcomeSpec(
+                value_frame=ValueFrame(
+                    init_df=str_to_pl_df(outcome_df_str), entity_id_col_name="dw_ek_borger"
+                ),
+                lookahead_distances=[(dt.timedelta(days=5), dt.timedelta(days=30))],
+                fallback=np.NaN,
+                aggregators=[MeanAggregator()],
+            )
+        ]
+    )
+    expected = str_to_pl_df(
+        """pred_time_uuid,outc_value_within_5_to_30_days_mean_fallback_nan
+1-2022-01-01 00:00:00.000000,1"""
+    )
+    assert_frame_equal(result.collect(), expected, ignore_colums=["dw_ek_borger", "pred_timestamp"])
```

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/synth_data_generator/utils.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/aggregation_fns.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/df_transforms.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/feature_specs/group_specs.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_specs/group_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/feature_specs/single_specs.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_specs/single_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/flattened_dataset.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/flattened_ds_validator.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/logger.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/misc_utils.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/misc_utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/load_synth_data.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/testing/utils_for_testing.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener/v1/utils/pydantic_basemodel.py` & `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/utils/pydantic_basemodel.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 2.1.2
+Version: 2.2.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
         
@@ -85,19 +85,19 @@
 [![github actions pytest](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/actions/workflows/main_test_and_release.yml/badge.svg)](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/actions)
 [![python versions](https://img.shields.io/pypi/pyversions/timeseriesflattener)](https://pypi.org/project/timeseriesflattener/)
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 
 [![PyPI version](https://badge.fury.io/py/timeseriesflattener.svg)](https://pypi.org/project/timeseriesflattener/)
 [![status](https://joss.theoj.org/papers/3bbea8745668d1aa40ff796c6fd3db87/status.svg)](https://joss.theoj.org/papers/3bbea8745668d1aa40ff796c6fd3db87)
 
-Time series from e.g. electronic health records often have a large number of variables, are sampled at irregular intervals and tend to have a large number of missing values. Before this type of data can be used for prediction modelling with machine learning methods such as logistic regression or XGBoost, the data needs to be reshaped. 
+Time series from e.g. electronic health records often have a large number of variables, are sampled at irregular intervals and tend to have a large number of missing values. Before this type of data can be used for prediction modelling with machine learning methods such as logistic regression or XGBoost, the data needs to be reshaped.  
 
 In essence, the time series need to be *flattened* so that each prediction time is represented by a set of predictor values and an outcome value. These predictor values can be constructed by aggregating the preceding values in the time series within a certain time window. 
 
-`timeseriesflattener` aims to simplify this process by providing an easy-to-use and fully-specified pipeline for flattening complex time series. 
+`timeseriesflattener` aims to simplify this process by providing an easy-to-use and fully-specified pipeline for flattening complex time series.  
 
 ## 🔧 Installation
 To get started using timeseriesflattener simply install it using pip by running the following line in your terminal:
 
 ```
 pip install timeseriesflattener
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.1.2 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.1.2/tasks.py` & `timeseriesflattener-2.2.0/tasks.py`

 * *Files identical despite different names*

