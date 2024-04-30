# Comparing `tmp/pypipegraph2-3.0.6.tar.gz` & `tmp/pypipegraph2-3.0.7.tar.gz`

## Comparing `pypipegraph2-3.0.6.tar` & `pypipegraph2-3.0.7.tar`

### file list

```diff
@@ -1,122 +1,124 @@
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 pypipegraph2-3.0.6/Cargo.toml
--rw-r--r--   0     1001      127      595 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/.coveragerc
--rw-r--r--   0     1001      127     1231 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/.github/workflows/pytest.yml
--rw-r--r--   0     1001      127     1876 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/.github/workflows/release.yml
--rw-r--r--   0     1001      127      754 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/.gitignore
--rw-r--r--   0     1001      127      754 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/.gitignore.orig
--rw-r--r--   0     1001      127      106 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/.hgignore
--rw-r--r--   0     1001      127       30 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/.ppg/logs/runtimes.tsv
--rw-r--r--   0     1001      127       95 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/AUTHORS.rst
--rw-r--r--   0     1001      127      128 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/CHANGELOG.rst
--rw-r--r--   0     1001      127    13831 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/Cargo.lock
--rw-r--r--   0     1001      127     9569 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/README.md
--rw-r--r--   0     1001      127     1363 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/Session.vim
--rwxr-xr-x   0     1001      127       55 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/bacon.sh
--rw-r--r--   0     1001      127      700 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/benches/bench1.rs
--rwxr-xr-x   0     1001      127      841 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/benchmarks/bench_disjoint.py
--rwxr-xr-x   0     1001      127      802 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/benchmarks/bench_kilo_jobs.py
--rwxr-xr-x   0     1001      127     1133 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/benchmarks/bench_simple.py
--rwxr-xr-x   0     1001      127      985 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/benchmarks/bench_tall.py
--rwxr-xr-x   0     1001      127      947 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/benchmarks/bench_wide.py
--rw-r--r--   0     1001      127     6315 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/designgoals.md
--rw-r--r--   0     1001      127     7618 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/docs/Makefile
--rw-r--r--   0     1001      127       18 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/docs/_static/.gitignore
--rw-r--r--   0     1001      127       41 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/docs/authors.rst
--rw-r--r--   0     1001      127       43 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/docs/changelog.rst
--rw-r--r--   0     1001      127     9264 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/docs/conf.py
--rw-r--r--   0     1001      127     2241 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/docs/index.rst
--rw-r--r--   0     1001      127       67 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/docs/license.rst
--rwxr-xr-x   0     1001      127       93 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/edit_version.sh
--rw-r--r--   0     1001      127    21307 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/examples/Basic_notebook.ipynb
--rw-r--r--   0     1001      127     1409 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/examples/abort_when_stalled.py
--rw-r--r--   0     1001      127     1120 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/examples/call_externals.py
--rw-r--r--   0     1001      127     1126 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/examples/long_for_interactive.py
--rw-r--r--   0     1001      127      260 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/examples/massive_exception.py
--rw-r--r--   0     1001      127      501 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/examples/nested_exception.py
--rw-r--r--   0     1001      127      563 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/examples/pandas_exception.py
--rw-r--r--   0     1001      127      506 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/examples/runtimes.py
--rw-r--r--   0     1001      127     5790 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/examples/simplest/simplest.py
--rw-r--r--   0     1001      127     1148 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/examples/slow_for_interactive.py
--rw-r--r--   0     1001      127     1241 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/examples/stall.py
--rw-r--r--   0     1001      127     1458 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/examples/stop_then_abort_when_stalled.py
--rw-r--r--   0     1001      127     1554 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/examples/stop_when_stalled.py
--rw-r--r--   0     1001      127     2533 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/flake.lock
--rw-r--r--   0     1001      127     6145 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/flake.nix
--rwxr-xr-x   0     1001      127      121 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/loop_cargo_test.sh
--rwxr-xr-x   0     1001      127      151 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/loop_main.sh
--rwxr-xr-x   0     1001      127      162 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/loop_ppg2_iterations_with_fail.sh
--rwxr-xr-x   0     1001      127      165 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/loop_ppg2_iterations_without_fail.sh
--rwxr-xr-x   0     1001      127       64 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/loop_pytest.sh
--rwxr-xr-x   0     1001      127      271 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/prep_for_tests.sh
--rwxr-xr-x   0     1001      127     1986 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/pyproject.toml
--rwxr-xr-x   0     1001      127     6124 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/__init__.py
--rw-r--r--   0     1001      127     3224 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/entry_points.py
--rw-r--r--   0     1001      127     1831 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/enums.py
--rw-r--r--   0     1001      127     1899 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/exceptions.py
--rwxr-xr-x   0     1001      127    29747 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/graph.py
--rw-r--r--   0     1001      127     1528 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/hashers.py
--rwxr-xr-x   0     1001      127     2257 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/history_comparisons.py
--rw-r--r--   0     1001      127    10730 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/interactive.py
--rwxr-xr-x   0     1001      127      843 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/job_status.py
--rwxr-xr-x   0     1001      127   112816 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/jobs.py
--rw-r--r--   0     1001      127     3408 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/parallel.py
--rw-r--r--   0     1001      127    18439 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/ppg1_compatibility.py
--rw-r--r--   0     1001      127     8513 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/ppg_traceback.py
--rwxr-xr-x   0     1001      127    41496 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/runner.py
--rw-r--r--   0     1001      127     2551 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/testing/__init__.py
--rw-r--r--   0     1001      127     9557 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/testing/fixtures.py
--rw-r--r--   0     1001      127     5217 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/python/pypipegraph2/util.py
--rwxr-xr-x   0     1001      127      167 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/run_pytest.sh
--rwxr-xr-x   0     1001      127     1655 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/setup.cfg
--rw-r--r--   0     1001      127      557 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/setup.py
--rwxr-xr-x   0     1001      127   108325 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/src/engine.rs
--rwxr-xr-x   0     1001      127    20032 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/src/lib.rs
--rw-r--r--   0     1001      127     1009 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/src/main.rs
--rwxr-xr-x   0     1001      127    15752 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/src/main_iterations_with_fail.rs
--rw-r--r--   0     1001      127    10553 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/src/main_iterations_without_fail.rs
--rwxr-xr-x   0     1001      127    94515 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/src/tests.rs
--rw-r--r--   0     1001      127      209 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/t.py
--rw-r--r--   0     1001      127        0 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/__init__.py
--rw-r--r--   0     1001      127      282 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/_import_does_not_hang.py
--rw-r--r--   0     1001      127     4975 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/conftest.py
--rw-r--r--   0     1001      127      677 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/old_history_for_conversion_test.gz
--rw-r--r--   0     1001      127        0 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/__init__.py
--rw-r--r--   0     1001      127      965 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/shared.py
--rw-r--r--   0     1001      127    27757 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_cache_jobs.py
--rw-r--r--   0     1001      127     5840 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_compatibility_layer.py
--rw-r--r--   0     1001      127     3050 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_cycles.py
--rw-r--r--   0     1001      127    75082 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py
--rw-r--r--   0     1001      127    23004 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_job_gen_jobs.py
--rw-r--r--   0     1001      127    17831 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_other.py
--rw-r--r--   0     1001      127    21651 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_plotjobs.py
--rw-r--r--   0     1001      127     4365 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_prune.py
--rw-r--r--   0     1001      127     3196 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_simple.py
--rw-r--r--   0     1001      127     4792 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_util.py
--rw-r--r--   0     1001      127      927 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/shared.py
--rw-r--r--   0     1001      127    69648 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_basics.py
--rw-r--r--   0     1001      127     7374 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_bootstrap.py
--rw-r--r--   0     1001      127    14235 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_cache_jobs.py
--rw-r--r--   0     1001      127     1636 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_cycles.py
--rw-r--r--   0     1001      127      558 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_flake8.py
--rw-r--r--   0     1001      127     3366 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_function_invariants.py
--rw-r--r--   0     1001      127     2499 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_interactive.py
--rw-r--r--   0     1001      127    47281 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_invariants_and_dependencies.py
--rw-r--r--   0     1001      127    11292 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_job_generating_jobs.py
--rwxr-xr-x   0     1001      127    67423 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_jobs.py
--rw-r--r--   0     1001      127    22839 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_other.py
--rw-r--r--   0     1001      127     2616 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_parallel.py
--rw-r--r--   0     1001      127        2 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_parent_termination_kills_children/A
--rw-r--r--   0     1001      127      759 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_parent_termination_kills_children/manual.py
--rwxr-xr-x   0     1001      127       52 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_parent_termination_kills_children/sleeper.sh
--rw-r--r--   0     1001      127      977 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_parent_termination_kills_children/stage2.py
--rw-r--r--   0     1001      127    16239 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_plotjobs.py
--rw-r--r--   0     1001      127     2736 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_prune.py
--rw-r--r--   0     1001      127     1914 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_rust_conversion.py
--rw-r--r--   0     1001      127    23688 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_shared_jobs.py
--rw-r--r--   0     1001      127     1846 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_simple.py
--rw-r--r--   0     1001      127     3691 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_util.py
--rw-r--r--   0     1001      127      507 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/test_version.py
--rw-r--r--   0     1001      127    61338 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tests/tests_from_the_field.py
--rw-r--r--   0     1001      127     5453 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/todo.md
--rw-r--r--   0     1001      127      154 2023-11-23 14:32:30.000000 pypipegraph2-3.0.6/tox.ini
--rw-r--r--   0        0        0    11702 1970-01-01 00:00:00.000000 pypipegraph2-3.0.6/PKG-INFO
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 pypipegraph2-3.0.7/Cargo.toml
+-rw-r--r--   0     1001      127      595 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/.coveragerc
+-rw-r--r--   0     1001      127     1231 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/.github/workflows/pytest.yml
+-rw-r--r--   0     1001      127     1876 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      754 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/.gitignore
+-rw-r--r--   0     1001      127      754 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/.gitignore.orig
+-rw-r--r--   0     1001      127      106 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/.hgignore
+-rw-r--r--   0     1001      127       48 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/.hgtags
+-rw-r--r--   0     1001      127       30 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/.ppg/logs/runtimes.tsv
+-rw-r--r--   0     1001      127       95 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/AUTHORS.rst
+-rw-r--r--   0     1001      127      128 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/CHANGELOG.rst
+-rw-r--r--   0     1001      127    13831 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/Cargo.lock
+-rw-r--r--   0     1001      127     9569 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/README.md
+-rw-r--r--   0     1001      127     1363 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/Session.vim
+-rwxr-xr-x   0     1001      127       55 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/bacon.sh
+-rw-r--r--   0     1001      127      700 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/benches/bench1.rs
+-rwxr-xr-x   0     1001      127      841 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/benchmarks/bench_disjoint.py
+-rwxr-xr-x   0     1001      127      802 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/benchmarks/bench_kilo_jobs.py
+-rwxr-xr-x   0     1001      127     1133 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/benchmarks/bench_simple.py
+-rwxr-xr-x   0     1001      127      985 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/benchmarks/bench_tall.py
+-rwxr-xr-x   0     1001      127      947 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/benchmarks/bench_wide.py
+-rw-r--r--   0     1001      127     6315 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/designgoals.md
+-rw-r--r--   0     1001      127     7618 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/docs/Makefile
+-rw-r--r--   0     1001      127       18 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/docs/_static/.gitignore
+-rw-r--r--   0     1001      127       41 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/docs/authors.rst
+-rw-r--r--   0     1001      127       43 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/docs/changelog.rst
+-rw-r--r--   0     1001      127     9264 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/docs/conf.py
+-rw-r--r--   0     1001      127     2241 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/docs/index.rst
+-rw-r--r--   0     1001      127       67 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/docs/license.rst
+-rwxr-xr-x   0     1001      127       93 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/edit_version.sh
+-rw-r--r--   0     1001      127    21307 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/examples/Basic_notebook.ipynb
+-rw-r--r--   0     1001      127     1409 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/examples/abort_when_stalled.py
+-rw-r--r--   0     1001      127     1120 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/examples/call_externals.py
+-rw-r--r--   0     1001      127     1126 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/examples/long_for_interactive.py
+-rw-r--r--   0     1001      127      260 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/examples/massive_exception.py
+-rw-r--r--   0     1001      127      501 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/examples/nested_exception.py
+-rw-r--r--   0     1001      127      563 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/examples/pandas_exception.py
+-rw-r--r--   0     1001      127      506 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/examples/runtimes.py
+-rw-r--r--   0     1001      127     5790 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/examples/simplest/simplest.py
+-rw-r--r--   0     1001      127     1148 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/examples/slow_for_interactive.py
+-rw-r--r--   0     1001      127     1241 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/examples/stall.py
+-rw-r--r--   0     1001      127     1458 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/examples/stop_then_abort_when_stalled.py
+-rw-r--r--   0     1001      127     1554 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/examples/stop_when_stalled.py
+-rw-r--r--   0     1001      127     2533 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/flake.lock
+-rw-r--r--   0     1001      127     6145 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/flake.nix
+-rwxr-xr-x   0     1001      127      121 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/loop_cargo_test.sh
+-rwxr-xr-x   0     1001      127      151 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/loop_main.sh
+-rwxr-xr-x   0     1001      127      162 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/loop_ppg2_iterations_with_fail.sh
+-rwxr-xr-x   0     1001      127      165 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/loop_ppg2_iterations_without_fail.sh
+-rwxr-xr-x   0     1001      127       64 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/loop_pytest.sh
+-rwxr-xr-x   0     1001      127      271 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/prep_for_tests.sh
+-rwxr-xr-x   0     1001      127     1986 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/pyproject.toml
+-rwxr-xr-x   0     1001      127     6174 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/__init__.py
+-rw-r--r--   0     1001      127     3224 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/entry_points.py
+-rw-r--r--   0     1001      127     1831 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/enums.py
+-rw-r--r--   0     1001      127     1899 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/exceptions.py
+-rwxr-xr-x   0     1001      127    29747 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/graph.py
+-rw-r--r--   0     1001      127     1528 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/hashers.py
+-rwxr-xr-x   0     1001      127     2257 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/history_comparisons.py
+-rwxr-xr-x   0     1001      127     2645 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/history_comparisons.py.orig
+-rw-r--r--   0     1001      127    10742 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/interactive.py
+-rwxr-xr-x   0     1001      127      843 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/job_status.py
+-rwxr-xr-x   0     1001      127   114290 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/jobs.py
+-rw-r--r--   0     1001      127     3408 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/parallel.py
+-rw-r--r--   0     1001      127    18441 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/ppg1_compatibility.py
+-rw-r--r--   0     1001      127     8513 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/ppg_traceback.py
+-rwxr-xr-x   0     1001      127    41640 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/runner.py
+-rw-r--r--   0     1001      127     2551 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/testing/__init__.py
+-rw-r--r--   0     1001      127     9557 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/testing/fixtures.py
+-rwxr-xr-x   0     1001      127     6087 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/python/pypipegraph2/util.py
+-rwxr-xr-x   0     1001      127      167 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/run_pytest.sh
+-rwxr-xr-x   0     1001      127     1655 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/setup.cfg
+-rw-r--r--   0     1001      127      557 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/setup.py
+-rwxr-xr-x   0     1001      127   108279 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/src/engine.rs
+-rwxr-xr-x   0     1001      127    20032 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/src/lib.rs
+-rw-r--r--   0     1001      127     1009 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/src/main.rs
+-rwxr-xr-x   0     1001      127    15752 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/src/main_iterations_with_fail.rs
+-rw-r--r--   0     1001      127    10553 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/src/main_iterations_without_fail.rs
+-rwxr-xr-x   0     1001      127    94515 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/src/tests.rs
+-rw-r--r--   0     1001      127      209 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/t.py
+-rw-r--r--   0     1001      127        0 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/__init__.py
+-rw-r--r--   0     1001      127      282 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/_import_does_not_hang.py
+-rw-r--r--   0     1001      127     4975 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/conftest.py
+-rw-r--r--   0     1001      127      677 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/old_history_for_conversion_test.gz
+-rw-r--r--   0     1001      127        0 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/__init__.py
+-rw-r--r--   0     1001      127      965 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/shared.py
+-rw-r--r--   0     1001      127    27757 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_cache_jobs.py
+-rw-r--r--   0     1001      127     5840 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_compatibility_layer.py
+-rw-r--r--   0     1001      127     3050 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_cycles.py
+-rw-r--r--   0     1001      127    75082 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py
+-rw-r--r--   0     1001      127    23004 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_job_gen_jobs.py
+-rw-r--r--   0     1001      127    17831 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_other.py
+-rw-r--r--   0     1001      127    21651 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_plotjobs.py
+-rw-r--r--   0     1001      127     4365 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_prune.py
+-rw-r--r--   0     1001      127     3196 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_simple.py
+-rw-r--r--   0     1001      127     4792 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_util.py
+-rw-r--r--   0     1001      127      927 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/shared.py
+-rw-r--r--   0     1001      127    69652 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_basics.py
+-rw-r--r--   0     1001      127     7374 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_bootstrap.py
+-rw-r--r--   0     1001      127    14235 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_cache_jobs.py
+-rw-r--r--   0     1001      127     1636 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_cycles.py
+-rw-r--r--   0     1001      127      558 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_flake8.py
+-rw-r--r--   0     1001      127     3366 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_function_invariants.py
+-rw-r--r--   0     1001      127     2499 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_interactive.py
+-rw-r--r--   0     1001      127    47281 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_invariants_and_dependencies.py
+-rw-r--r--   0     1001      127    13779 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_job_generating_jobs.py
+-rwxr-xr-x   0     1001      127    67423 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_jobs.py
+-rwxr-xr-x   0     1001      127    22998 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_other.py
+-rw-r--r--   0     1001      127     2616 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_parallel.py
+-rw-r--r--   0     1001      127        2 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_parent_termination_kills_children/A
+-rw-r--r--   0     1001      127      759 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_parent_termination_kills_children/manual.py
+-rwxr-xr-x   0     1001      127       52 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_parent_termination_kills_children/sleeper.sh
+-rw-r--r--   0     1001      127      977 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_parent_termination_kills_children/stage2.py
+-rw-r--r--   0     1001      127    16239 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_plotjobs.py
+-rw-r--r--   0     1001      127     2736 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_prune.py
+-rw-r--r--   0     1001      127     1914 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_rust_conversion.py
+-rw-r--r--   0     1001      127    23688 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_shared_jobs.py
+-rw-r--r--   0     1001      127     1846 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_simple.py
+-rw-r--r--   0     1001      127     4657 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_util.py
+-rw-r--r--   0     1001      127      507 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/test_version.py
+-rwxr-xr-x   0     1001      127    62028 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tests/tests_from_the_field.py
+-rw-r--r--   0     1001      127     5616 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/todo.md
+-rw-r--r--   0     1001      127      154 2024-04-30 12:14:34.000000 pypipegraph2-3.0.7/tox.ini
+-rw-r--r--   0        0        0    11702 1970-01-01 00:00:00.000000 pypipegraph2-3.0.7/PKG-INFO
```

### Comparing `pypipegraph2-3.0.6/Cargo.toml` & `pypipegraph2-3.0.7/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pypipegraph2"
-version = "3.0.6"
+version = "3.0.7"
 edition = "2018"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pypipegraph2"
 crate-type = ["cdylib", "rlib"]
```

### Comparing `pypipegraph2-3.0.6/.coveragerc` & `pypipegraph2-3.0.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/.github/workflows/pytest.yml` & `pypipegraph2-3.0.7/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/.github/workflows/release.yml` & `pypipegraph2-3.0.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/.gitignore` & `pypipegraph2-3.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/.gitignore.orig` & `pypipegraph2-3.0.7/.gitignore.orig`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/Cargo.lock` & `pypipegraph2-3.0.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pypipegraph2"
-version = "3.0.6"
+version = "3.0.7"
 dependencies = [
  "backtrace",
  "colored",
  "env_logger",
  "itertools",
  "log",
  "num_cpus",
```

### Comparing `pypipegraph2-3.0.6/README.md` & `pypipegraph2-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/Session.vim` & `pypipegraph2-3.0.7/Session.vim`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/benches/bench1.rs` & `pypipegraph2-3.0.7/benches/bench1.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/benchmarks/bench_disjoint.py` & `pypipegraph2-3.0.7/benchmarks/bench_disjoint.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/benchmarks/bench_kilo_jobs.py` & `pypipegraph2-3.0.7/benchmarks/bench_kilo_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/benchmarks/bench_simple.py` & `pypipegraph2-3.0.7/benchmarks/bench_simple.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/benchmarks/bench_tall.py` & `pypipegraph2-3.0.7/benchmarks/bench_tall.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/benchmarks/bench_wide.py` & `pypipegraph2-3.0.7/benchmarks/bench_wide.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/designgoals.md` & `pypipegraph2-3.0.7/designgoals.md`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/docs/Makefile` & `pypipegraph2-3.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/docs/conf.py` & `pypipegraph2-3.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/docs/index.rst` & `pypipegraph2-3.0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/examples/Basic_notebook.ipynb` & `pypipegraph2-3.0.7/examples/Basic_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/examples/abort_when_stalled.py` & `pypipegraph2-3.0.7/examples/abort_when_stalled.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/examples/call_externals.py` & `pypipegraph2-3.0.7/examples/call_externals.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/examples/long_for_interactive.py` & `pypipegraph2-3.0.7/examples/long_for_interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/examples/pandas_exception.py` & `pypipegraph2-3.0.7/examples/pandas_exception.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/examples/simplest/simplest.py` & `pypipegraph2-3.0.7/examples/simplest/simplest.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/examples/slow_for_interactive.py` & `pypipegraph2-3.0.7/examples/slow_for_interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/examples/stall.py` & `pypipegraph2-3.0.7/examples/stall.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/examples/stop_then_abort_when_stalled.py` & `pypipegraph2-3.0.7/examples/stop_then_abort_when_stalled.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/examples/stop_when_stalled.py` & `pypipegraph2-3.0.7/examples/stop_when_stalled.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/flake.lock` & `pypipegraph2-3.0.7/flake.lock`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/flake.nix` & `pypipegraph2-3.0.7/flake.nix`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/pyproject.toml` & `pypipegraph2-3.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.12,<0.13"]
 build-backend = "maturin"
 
 [project]
 name = "pypipegraph2"
-version = "3.0.6"
+version = "3.0.7"
 description = "Advanced python 'what changed and what do we need to do' tracking"
 # long-description = "README.md"
 authors = [
  {"name" = "Florian Finkernagel", "email" = "finkernagel@imt.uni-marburg.de"}
 ]
 classifiers = [
 	"Development Status :: 4 - Beta",
```

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/__init__.py` & `pypipegraph2-3.0.7/python/pypipegraph2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "3.0.6"
+__version__ = "3.0.7"
 
 from pathlib import Path
 import logging
 import contextlib
 from .graph import PyPipeGraph, ALL_CORES
 from .jobs import (
     FileGeneratingJob,
@@ -13,14 +13,15 @@
     DataLoadingJob,
     ValuePlusHash,
     AttributeLoadingJob,
     CachedDataLoadingJob,
     CachedAttributeLoadingJob,
     PlotJob,
     FunctionInvariant,
+    _FunctionInvariant,
     FileInvariant,
     ParameterInvariant,
     JobGeneratingJob,
     Job,
     JobList,
     SharedMultiFileGeneratingJob,
     NotebookInvariant,
@@ -206,14 +207,15 @@
     "DataLoadingJob",
     "ValuePlusHash",
     "AttributeLoadingJob",
     "CachedDataLoadingJob",
     "CachedAttributeLoadingJob",
     "PlotJob",
     "FunctionInvariant",
+    "_FunctionInvariant",
     "FileInvariant",
     "ParameterInvariant",
     "NotebookInvariant",
     "NotebookJob",
     "JobGeneratingJob",
     "SharedMultiFileGeneratingJob",
     "PPGException",
```

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/entry_points.py` & `pypipegraph2-3.0.7/python/pypipegraph2/entry_points.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/enums.py` & `pypipegraph2-3.0.7/python/pypipegraph2/enums.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/exceptions.py` & `pypipegraph2-3.0.7/python/pypipegraph2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/graph.py` & `pypipegraph2-3.0.7/python/pypipegraph2/graph.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/hashers.py` & `pypipegraph2-3.0.7/python/pypipegraph2/hashers.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/history_comparisons.py` & `pypipegraph2-3.0.7/python/pypipegraph2/history_comparisons.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/interactive.py` & `pypipegraph2-3.0.7/python/pypipegraph2/interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                     else:  # must have been stdin.
                         value = sys.stdin.read(1)
                         # log_info(f"received {repr(value)}")
                         if value == "\x03":  # ctrl-c:
                             self.cmd = ""
                         elif value == "\x1a":  # ctrl-z
                             os.kill(os.getpid(), signal.SIGTSTP)
-                        elif ord("0") <= ord(value) <= ord("z") or value == " ":
+                        elif value and (ord("0") <= ord(value) <= ord("z") or value == " "):
                             self.cmd += value
                         elif value == "\x7f":  # backspace
                             self.cmd = self.cmd[:-1]
                         elif value == "\n" or value == "\r":
                             try:
                                 if self.cmd:
                                     command = self.cmd
@@ -259,15 +259,15 @@
             print("Job is not running in an external process - can't kill")
             return
         print("ok, killing job", job.job_id)
         log_info(f"Command kill {job.job_id} ")
         job.kill_if_running()
 
     def _cmd_debug(self, args):
-        """Write the debug status from teh evaluator to debug.txt"""
+        """Write the debug status from the evaluator to debug.txt"""
         from pathlib import Path
 
         # import pypipegraph2
 
         # pypipegraph2.pypipegraph2.enable_logging()
         filename = Path("debug.txt").absolute()
         print(f"Writing to {filename}")
```

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/job_status.py` & `pypipegraph2-3.0.7/python/pypipegraph2/job_status.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/jobs.py` & `pypipegraph2-3.0.7/python/pypipegraph2/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             ) and (str(type(j)) == "<class 'pypipegraph2.jobs.FileInvariant'>"):
                 # going this way should be save, the compat. class
                 # can do everything the regular one can.
                 # but the other way around is not necessarily safe
                 pass  #
             else:
                 raise exceptions.JobRedefinitionError(
-                    f"Redefining job {job_id} with different type - prohibited by RunMode. Was {type(j)}, wants to be {cls}"
+                    f"Redefining job {job_id} with different type - prohibited by RunMode. Was {type(j)}, wants to be {cls}. If the job ids make no sense, check for symlinks"
                 )
         return global_pipegraph.jobs[job_id]
     else:
         return object.__new__(cls)
 
 
 def _mark_function_wrapped(outer, inner, desc="callback"):
@@ -262,16 +262,22 @@
         *other_jobs: Union[Union[str, Job], List[Union[str, Job]]],
     ):
         """Depend on another Job, which must be done before this one can run.
         If the other job changes it's output, this job will be invalidated (and rerun).
 
         You may pass in one ore more Jobs, a list of such,
         ore a callable that will return such. The callable will
-        be called when the ppg is run the first time
-        (todo: when is the later useful)
+        be called when the ppg is run the first time.
+        (This is usefull if you need to finalize e.g. a tree structure
+         and design the actual dependencies on that tree structure).
+
+        This method will also take a filename, in which case we'll look
+        up the job producing the filename.
+        Bonus: Dependency is the nonly on the contens of that file,
+        not on all files of the (MultiFileGenerating) Job.
         """
 
         from . import global_pipegraph
 
         if other_job is False and not other_jobs:
             # raise ValueError("You have to pass in at least one job")
             return self  # this is how ppg1 did it
@@ -340,15 +346,15 @@
         """Create a function invariant.
         Return a NamedTumple (invariant, self)
         (so you can change with job.depends_on_func(func)[1].depends_on(...))
         """
         if isinstance(function, str):
             function, name = name, function
         if not name:
-            name = FunctionInvariant.func_to_name(function)
+            name = _FunctionInvariant.func_to_name(function)
 
         upstream = FunctionInvariant(function, self.job_id + "_" + name)
         self.depends_on(upstream)
         return DependsOnInvariant(upstream, self)
 
     def depends_on_file(self, filename):
         job = FileInvariant(filename)
@@ -569,16 +575,16 @@
             op.write("\n".join(["        "] + [ll for ll in lines]))
 
 
 class MultiFileGeneratingJob(Job):
     eval_job_kind = "Output"
 
     def __new__(cls, files, *args, **kwargs):
-        files = cls._validate_files_argument(files)[0]
-        return Job.__new__(cls, [str(x) for x in files])
+        valid_files = cls._validate_files_argument(files)[0]
+        return Job.__new__(cls, [str(x) for x in valid_files])
 
     def __init__(
         self,
         files: List[Path],  # todo: extend type attribute to allow mapping
         generating_function: Callable[List[Path]],
         resources: Resources = Resources.SingleCore,
         depend_on_function: bool = True,
@@ -1161,25 +1167,25 @@
                 h = hashers.hash_file(file)
                 runner._hash_file_cache[file] = h
                 return h
         else:
             return hashers.hash_file(file)
 
 
-class FunctionInvariant(_InvariantMixin, Job, _FileInvariantMixin):
+class _FunctionInvariant(_InvariantMixin, Job, _FileInvariantMixin):
     def __new__(cls, function, name=None):
         name, function = cls._parse_args(function, name)
         return super().__new__(cls, [name])
 
     @classmethod
     def _parse_args(cls, function, name):
+        # duplicated from FunctionInvariant for the compatibility layer
         if isinstance(function, (str, Path)):
             name, function = function, name
-
-        name = "FI" + (str(name) if name else FunctionInvariant.func_to_name(function))
+        name = "FI" + (str(name) if name else _FunctionInvariant.func_to_name(function))
         return name, function
 
     def __init__(
         self, function, name=None
     ):  # must support the inverse calling with name, function, for compatibility to pypipegraph
         name, function = self._parse_args(function, name)
         self.verify_arguments(name, function)
@@ -1617,28 +1623,31 @@
             filename = found.__file__.replace(".so", ".pyx").replace(
                 ".pyc", ".py"
             )  # pyc replacement is for mock testing
         return filename, line_no
 
     def verify_arguments(self, job_id, function):
         if not callable(function) and function is not None:
-            raise TypeError("%s function was not a callable (or None)" % job_id)
-        if hasattr(self, "function") and not FunctionInvariant.functions_equal(
+            raise TypeError(
+                "%s function was not a callable (or None), function: %s"
+                % (job_id, repr(function))
+            )
+        if hasattr(self, "function") and not _FunctionInvariant.functions_equal(
             function, self.function
         ):
             from . import global_pipegraph
 
             if global_pipegraph.run_mode.is_strict():
                 raise exceptions.JobRedefinitionError(
                     "FunctionInvariant %s created twice with different functions: \n%s\n%s\n%s"
                     % (
                         job_id,
-                        FunctionInvariant.function_to_str(function),
-                        FunctionInvariant.function_to_str(self.function),
-                        FunctionInvariant.debug_function_differences(
+                        _FunctionInvariant.function_to_str(function),
+                        _FunctionInvariant.function_to_str(self.function),
+                        _FunctionInvariant.debug_function_differences(
                             self.function, function
                         ),
                     )
                 )
 
     @staticmethod
     def func_to_name(function):
@@ -1681,14 +1690,37 @@
             return "%s (job_id=%s,id=%s, Function: None)" % (
                 self.__class__.__name__,
                 self.job_id,
                 id(self),
             )
 
 
+def FunctionInvariant(function, name=None):
+    if isinstance(function, (str, Path)):
+        name, function = function, name
+    if hasattr(function, "wrapped_function"):
+        f1 = _FunctionInvariant(function, name)
+        f2 = _FunctionInvariant(function.wrapped_function, name + "_inner")
+        return [f1, f2]
+    else:
+        return _FunctionInvariant(function, name)
+
+
+FunctionInvariant.compare_hashes = _FunctionInvariant.compare_hashes
+FunctionInvariant.debug_function_differences = (
+    _FunctionInvariant.debug_function_differences
+)
+FunctionInvariant.functions_equal = _FunctionInvariant.functions_equal
+FunctionInvariant.function_to_str = _FunctionInvariant.function_to_str
+FunctionInvariant.get_cython_filename_and_line_no = (
+    _FunctionInvariant.get_cython_filename_and_line_no
+)
+FunctionInvariant.get_cython_source = _FunctionInvariant.get_cython_source
+
+
 class FileInvariant(_InvariantMixin, Job, _FileInvariantMixin):
     def __new__(cls, file):
         return super().__new__(cls, [str(_normalize_path(file))])
 
     def __init__(self, file):
         from . import global_pipegraph
 
@@ -1976,14 +2008,15 @@
 
         if not isinstance(attribute_name, str):
             raise ValueError("attribute_name was not a string")
         self.depend_on_function = depend_on_function
         self.object = object
         self.attribute_name = attribute_name
         self.callback = data_function
+        self.do_cleanup = True
         super().__init__([job_id], resources=resources)
 
     def cleanup(self):
         delattr(self.object, self.attribute_name)
 
     def readd(self):  # Todo: refactor
         super().readd()
```

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/parallel.py` & `pypipegraph2-3.0.7/python/pypipegraph2/parallel.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/ppg1_compatibility.py` & `pypipegraph2-3.0.7/python/pypipegraph2/ppg1_compatibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 
 class Job:
     _InvariantJob = ppg2.jobs._InvariantMixin
     pass
 
 
 job = Job()
-job.function_to_str = ppg2.FunctionInvariant.function_to_str
+job.function_to_str = ppg2._FunctionInvariant.function_to_str
 
 
 class FakeRC:
     @property
     def cores_available(self):
         return ppg2.global_pipegraph.cores
 
@@ -385,15 +385,15 @@
     pass
 
 
 class FileInvariant(PPG1AdaptorBase, ppg2.FileInvariant):
     pass
 
 
-class FunctionInvariant(PPG1AdaptorBase, ppg2.FunctionInvariant):
+class FunctionInvariant(PPG1AdaptorBase, ppg2._FunctionInvariant):
     pass
 
 
 class ParameterInvariant(PPG1AdaptorBase, ppg2.ParameterInvariant):
     pass
```

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/ppg_traceback.py` & `pypipegraph2-3.0.7/python/pypipegraph2/ppg_traceback.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/runner.py` & `pypipegraph2-3.0.7/python/pypipegraph2/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,17 @@
                 run_id  # to allow jobgenerating jobs to run just once per graph.run()
             )
 
             if not networkx.algorithms.is_directed_acyclic_graph(
                 self.job_graph.job_dag
             ):  # pragma: no cover - defensive
                 error_fn = self.job_graph.log_dir / "debug_edges_with_cycles.txt"
-                networkx.write_edgelist(self.job_graph.job_dag, error_fn)
+                networkx.write_edgelist(
+                    self.job_graph.job_dag, error_fn, delimiter="\t"
+                )
                 cycles = list(networkx.simple_cycles(self.job_graph.job_dag))
                 raise exceptions.NotADag(
                     f"Not a directed *acyclic* graph. See {error_fn}. Cycles between {cycles}"
                 )
             assert len(self.jobs) == len(job_graph.job_dag)
 
             log_job_trace(f"Focus on these jobs: {focus_on_these_jobs}")
@@ -222,15 +224,15 @@
                 ),
             )
 
             if not networkx.algorithms.is_directed_acyclic_graph(
                 self.dag
             ):  # pragma: no cover - defensive
                 error_fn = self.job_graph.log_dir / "debug_edges_with_cycles.txt"
-                networkx.write_edgelist(self.dag, error_fn)
+                networkx.write_edgelist(self.dag, error_fn, delimiter="\t")
                 cycles = list(networkx.simple_cycles(self.dag))
                 raise exceptions.NotADag(
                     f"Not a directed *acyclic* graph after modification. See {error_fn}. Cycles between {cycles}"
                 )
 
             self.event_lock = threading.Lock()
             self.jobs_to_run_que = queue.PriorityQueue()
@@ -321,15 +323,17 @@
         dag = job_graph.job_dag.copy()
         if dump_graphml:
             for node in dag.nodes():
                 dag.nodes[node]["label"] = node
                 dag.nodes[node]["shape"] = self.jobs[node].__class__.__name__
             networkx.readwrite.graphml.write_graphml(
                 dag,
-                self.job_graph.log_dir / "graph_pre_mod.graphml",
+                self.job_graph.log_file.with_name(
+                    self.job_graph.log_file.stem + "pre_prune.graphml"
+                ),
                 named_key_ids=True,
             )
 
         pruned = self._apply_pruning(
             dag, focus_on_these_jobs, jobs_already_run_previously
         )
         return dag, pruned
@@ -664,15 +668,15 @@
                     try:
                         do_sleep = False
                         with self.evaluator_lock:
                             cleanups = self.evaluator.jobs_ready_for_cleanup()
 
                             for cleanup_job_id in cleanups:
                                 try:
-                                    log_error(f"Cleanup for {cleanup_job_id}")
+                                    log_info(f"Cleanup for {cleanup_job_id}")
                                     self.jobs[cleanup_job_id].cleanup()
                                 except Exception as e:
                                     log_error(f"Cleanup had an exception {repr(e)}")
                                 self.evaluator.event_job_cleanup_done(cleanup_job_id)
 
                             rr = self.evaluator.jobs_ready_to_run()
                             if not rr:
```

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/testing/__init__.py` & `pypipegraph2-3.0.7/python/pypipegraph2/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/testing/fixtures.py` & `pypipegraph2-3.0.7/python/pypipegraph2/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/python/pypipegraph2/util.py` & `pypipegraph2-3.0.7/python/pypipegraph2/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,25 +42,34 @@
     return cpu_count
 
 
 def job_or_filename(job_or_filename, invariant_class=None):
     """Take a filename, or a job. Return Path(filename), dependency-for-that-file
     ie. either the job, or a invariant_class (default: FileInvariant)"""
     from .jobs import Job, FileInvariant
+    from . import global_pipegraph
     from pathlib import Path
 
+    if global_pipegraph is None:
+        return Path(job_or_filename), []
+
     if invariant_class is None:  # pragma: no cover
         invariant_class = FileInvariant
 
     if isinstance(job_or_filename, Job):
         filename = job_or_filename.files[0]
         deps = [job_or_filename]
     elif job_or_filename is not None:
-        filename = Path(job_or_filename)
-        deps = [invariant_class(filename)]
+        try:
+            global_pipegraph.find_job_from_file(str(job_or_filename))
+            deps = [str(job_or_filename)]
+            filename = job_or_filename
+        except KeyError:
+            filename = Path(job_or_filename)
+            deps = [invariant_class(filename)]
     else:
         filename = None
         deps = []
     return filename, deps
 
 
 def assert_uniqueness_of_object(
@@ -155,23 +164,41 @@
     else:
         return job_id
 
 
 def pretty_log_errors(func):
     """capture exceptions (on a function outside of ppg)
     and format it with our fancy local logging exception logger
+
+    This is a decorator!
     """
 
     def inner(*args, **kwargs):
         try:
-            func(*args, **kwargs)
+            return func(*args, **kwargs)
         except Exception as e:
             exception_type, exception_value, tb = sys.exc_info()
             captured_tb = ppg_traceback.Trace(exception_type, exception_value, tb)
             logger.error(
                 captured_tb._format_rich_traceback_fallback(
                     include_locals=True, include_formating=True
                 )
             )
             raise
 
     return inner
+
+
+def wrap_for_function_invariant(function, *args, **kwargs):
+    """When you need to pass a function + parameters which ends up in a FunctionInvariant.
+    Think lambda: some_func(filename).
+
+    This marks it so that the FunctionInvariant tracks 'somefunc',
+    not the lambda."""
+    from .jobs import _mark_function_wrapped
+
+    def wrapper(function=function, args=args, kwargs=kwargs):
+        return function(*args, **kwargs)
+
+    _mark_function_wrapped(wrapper, function, "wrap_for_function_invariant")
+
+    return wrapper
```

### Comparing `pypipegraph2-3.0.6/setup.cfg` & `pypipegraph2-3.0.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 [metadata]
 name = pypipegraph2
 description = Advanced python 'what changed and what do we need to do' tracking
-version = 3.0.6
+version = 3.0.7
 author = Florian Finkernagel
 author-email = finkernagel@imt.uni-marburg.de
 license = mit
 long-description = file: README.md
 long-description-content-type = text/markdown; charset=UTF-8
 url = https://github.com/pyscaffold/pyscaffold/
 project-urls =
```

### Comparing `pypipegraph2-3.0.6/setup.py` & `pypipegraph2-3.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/src/engine.rs` & `pypipegraph2-3.0.7/src/engine.rs`

 * *Files 2% similar despite different names*

```diff
@@ -651,93 +651,96 @@
         for ds_id in downstreams {
             if !Self::_job_and_downstreams_are_ephemeral(dag, jobs, ds_id) {
                 return false;
             }
         }
         true
     }
+    ///
+    /// Retrieve the 'new history' after a ppg run
     pub fn new_history(&self) -> Result<HashMap<String, String>, PPGEvaluatorError> {
         match self.already_started {
             StartStatus::Finished => {}
             _ => {
                 debug!("{}", Self::debug(&self.dag, &self.jobs));
                 panic!("Graph wasn't finished, not handing out history..."); // todo: actually, why not, we could save history occasionally?
             }
         }
         //our history 'keys'
-        //(we can't do tuple indices because of json dumping)
+        //(we can't do tuple indices because of json history-save-format.)
         //no !!! -> job output.
         //ends with !!! -> the list of named inputs
         //x!!!y -> input x for job y.
+
         //todo: consider splitting into multiple functions?
-        let mut multi_output_job_filtered_outputs = HashSet::new();
+
+        // when a multi-file-generating-job get's renamed, we need to remove the old history.
+        // but only then.
+        let mut multi_parts_to_jobs = HashMap::new();
         for j in self.jobs.iter() {
             if j.job_id.contains(":::") {
-                for output_name in j.job_id.split(":::") {
-                    multi_output_job_filtered_outputs.insert(output_name.to_string());
+                for part in j.job_id.split(":::") {
+                    multi_parts_to_jobs.insert(part, j.job_id.clone());
                 }
+            } else {
+                multi_parts_to_jobs.insert(&j.job_id, j.job_id.clone());
             }
         }
-        // let failed: HashSet<String> = self.query_failed();
-        // dbg!(&failed);
+
+        let filter_if_renamed = |job_id: &str| -> bool {
+            if job_id.contains(":::") {
+                let last_time = multi_parts_to_jobs.get(job_id);
+                match last_time {
+                    Some(last_time) => last_time == job_id,
+                    None => true, //not present.
+                }
+            } else {
+                return true;
+            }
+        };
+
         let mut out = self.history.clone();
         let mut out: HashMap<_, _> = out
             .drain()
             .filter(|(k, _v)| {
                 if k.contains("!!!") {
                     let (job_id_a, job_id_b) = k.split_once("!!!").unwrap();
                     if !job_id_b.is_empty() {
                         let node_idx_a = self.job_id_to_node_idx.get(job_id_a);
                         let node_idx_b = self.job_id_to_node_idx.get(job_id_b);
                         match (node_idx_a, node_idx_b) {
                             (Some(node_idx_a), Some(node_idx_b)) => {
                                 self.dag.edge_weight(*node_idx_a, *node_idx_b).is_some()
                             }
                             _ => {
-                                for output_name in job_id_a.split(":::") {
-                                    if multi_output_job_filtered_outputs.contains(output_name) {
-                                        return false;
-                                    }
-                                }
-
-                                true
+                                //if it's from a multi-output job that was producing different
+                                //stuff before,
+                                filter_if_renamed(job_id_a)
                             }
                         }
                     } else {
                         // a node uplink entry.
-                        for output_name in job_id_a.split(":::") {
-                            if multi_output_job_filtered_outputs.contains(output_name) {
-                                return false;
-                            }
-                        }
-
-                        true
+                        filter_if_renamed(job_id_a)
                     }
                 } else {
                     // when MultiFileGeneratingJobs
                     // get renamed, we need to make sure we don't keep
                     // old history around
-                    for output_name in k.split(":::") {
-                        if multi_output_job_filtered_outputs.contains(output_name) {
-                            return false;
-                        }
-                    }
-                    /* if failed.contains(k) { that's  being taken care of down in the next loop.
-                        return false;
-                    }; */
-                    true // a node entry
+                    filter_if_renamed(k)
                 }
             })
             .collect();
 
         for (idx, job) in self.jobs.iter().enumerate() {
             //step 1: record what jobs when into this one
 
             //step 2: record the actual output of this job
             // (are we using this anywhere?)
+            // (todo: I think there's a potential to reuse it for ephemeral jobs that are needed
+            // again, because their downstream failed)
             // We're not for checking-the-ephemeral-invariant-upholding,
             // for that we use the ones stored on the downstream jobs.
 
             let key = job.job_id.to_string();
             let job_was_success = job.history_output.is_some();
             let input_name_key = format!("{}!!!", job.job_id);
             if job_was_success {
```

### Comparing `pypipegraph2-3.0.6/src/lib.rs` & `pypipegraph2-3.0.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/src/main.rs` & `pypipegraph2-3.0.7/src/main.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/src/main_iterations_with_fail.rs` & `pypipegraph2-3.0.7/src/main_iterations_with_fail.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/src/main_iterations_without_fail.rs` & `pypipegraph2-3.0.7/src/main_iterations_without_fail.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/src/tests.rs` & `pypipegraph2-3.0.7/src/tests.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/conftest.py` & `pypipegraph2-3.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/old_history_for_conversion_test.gz` & `pypipegraph2-3.0.7/tests/old_history_for_conversion_test.gz`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/shared.py` & `pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/shared.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_cache_jobs.py` & `pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_cache_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_compatibility_layer.py` & `pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_compatibility_layer.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_cycles.py` & `pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_cycles.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py` & `pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_job_gen_jobs.py` & `pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_job_gen_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_other.py` & `pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_other.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_plotjobs.py` & `pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_plotjobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_prune.py` & `pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_prune.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_simple.py` & `pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_simple.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/ppg1_compatibility_layer/test_util.py` & `pypipegraph2-3.0.7/tests/ppg1_compatibility_layer/test_util.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/shared.py` & `pypipegraph2-3.0.7/tests/shared.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_basics.py` & `pypipegraph2-3.0.7/tests/test_basics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1446,18 +1446,18 @@
         def inner():
             return 55
 
         f1 = a.depends_on_func("mylambda1", lambda: 55)
         f2 = a.depends_on_func("inner", inner)
         f3 = a.depends_on_func(inner)
         f4 = a.depends_on_func(open)  # built in
-        assert isinstance(f1.invariant, ppg.FunctionInvariant)
-        assert isinstance(f2.invariant, ppg.FunctionInvariant)
-        assert isinstance(f3.invariant, ppg.FunctionInvariant)
-        assert isinstance(f4.invariant, ppg.FunctionInvariant)
+        assert isinstance(f1.invariant, ppg._FunctionInvariant)
+        assert isinstance(f2.invariant, ppg._FunctionInvariant)
+        assert isinstance(f3.invariant, ppg._FunctionInvariant)
+        assert isinstance(f4.invariant, ppg._FunctionInvariant)
         assert f1.self is a
         assert f2.self is a
         assert f3.self is a
         assert f4.self is a
         assert ppg.global_pipegraph.has_edge(f1.invariant, a)
         assert ppg.global_pipegraph.has_edge(f2.invariant, a)
         assert ppg.global_pipegraph.has_edge(f3.invariant, a)
```

### Comparing `pypipegraph2-3.0.6/tests/test_bootstrap.py` & `pypipegraph2-3.0.7/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_cache_jobs.py` & `pypipegraph2-3.0.7/tests/test_cache_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_cycles.py` & `pypipegraph2-3.0.7/tests/test_cycles.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_flake8.py` & `pypipegraph2-3.0.7/tests/test_flake8.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_function_invariants.py` & `pypipegraph2-3.0.7/tests/test_function_invariants.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_interactive.py` & `pypipegraph2-3.0.7/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_invariants_and_dependencies.py` & `pypipegraph2-3.0.7/tests/test_invariants_and_dependencies.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_jobs.py` & `pypipegraph2-3.0.7/tests/test_jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1887,54 +1887,54 @@
         jobC = ppg.FileGeneratingJob(
             "C", lambda of: counter("c") and of.write_text(of.name)
         )
         jobC.depends_on("A")
         ppg.run()
         assert Path("D").read_text() == "D"
         assert Path("C").read_text() == "C"
-        assert Path("a").read_text() == "3"
+        assert Path("a").read_text() == "2"
         assert Path("c").read_text() == "1"
 
         # take one out & put one in *at the same time*
         ppg.new()
         jobA = ppg.MultiFileGeneratingJob(["A", "B", "E"], do_a)
         jobC = ppg.FileGeneratingJob(
             "C", lambda of: counter("c") and of.write_text(of.name)
         )
         jobC.depends_on("A")
         ppg.run()
         assert Path("D").read_text() == "D"
         assert Path("C").read_text() == "C"
-        assert Path("a").read_text() == "4"
+        assert Path("a").read_text() == "3"
         assert Path("c").read_text() == "1"
 
         # now turn it into a FG
         ppg.new()
         jobA = ppg.FileGeneratingJob("A", do_a)
         jobC = ppg.FileGeneratingJob(
             "C", lambda of: counter("c") and of.write_text(of.name)
         )
         jobC.depends_on("A")
         ppg.run()
         assert Path("D").read_text() == "D"
         assert Path("C").read_text() == "C"
-        assert Path("a").read_text() == "5"
+        assert Path("a").read_text() == "4"
         assert Path("c").read_text() == "1"
 
         # now turn it into back into a MFG
         ppg.new()
         ppg.MultiFileGeneratingJob(["A", "B"], do_a)
         jobC = ppg.FileGeneratingJob(
             "C", lambda of: counter("c") and of.write_text(of.name)
         )
         jobC.depends_on("A")
         ppg.run()
         assert Path("D").read_text() == "D"
         assert Path("C").read_text() == "C"
-        assert Path("a").read_text() == "6"
+        assert Path("a").read_text() == "4"
         assert Path("c").read_text() == "1"
 
 
 @pytest.mark.usefixtures("create_out_dir")
 @pytest.mark.usefixtures("ppg2_per_test")
 class TestMultiTempFileGeneratingJob:
     def test_basic(self):
```

### Comparing `pypipegraph2-3.0.6/tests/test_other.py` & `pypipegraph2-3.0.7/tests/test_other.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,14 +291,18 @@
     assert dep_b[0] is j
     assert len(dep_b) == 1
 
     c, dep_c = ppg.util.job_or_filename(None)
     assert c is None
     assert not dep_c
 
+    b2, dep_b2 = ppg.util.job_or_filename("out/B")
+    assert b2 == ("out/B")
+    assert dep_b2 == ["out/B"]  # still not a job, but it's findable downstream
+
 
 @pytest.mark.xfail()  # todo
 def test_interactive_import(ppg2_per_test):
     # just so at least the import part of interactive is under coverage
     import pypipegraph2.interactive  # noqa:F401
```

### Comparing `pypipegraph2-3.0.6/tests/test_parallel.py` & `pypipegraph2-3.0.7/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_parent_termination_kills_children/manual.py` & `pypipegraph2-3.0.7/tests/test_parent_termination_kills_children/manual.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_parent_termination_kills_children/stage2.py` & `pypipegraph2-3.0.7/tests/test_parent_termination_kills_children/stage2.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_plotjobs.py` & `pypipegraph2-3.0.7/tests/test_plotjobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_prune.py` & `pypipegraph2-3.0.7/tests/test_prune.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_rust_conversion.py` & `pypipegraph2-3.0.7/tests/test_rust_conversion.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_shared_jobs.py` & `pypipegraph2-3.0.7/tests/test_shared_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/test_simple.py` & `pypipegraph2-3.0.7/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.6/tests/tests_from_the_field.py` & `pypipegraph2-3.0.7/tests/tests_from_the_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
         edges = []
         edges.append(("J0", "J2"))
         edges.append(("J2", "J3"))
         edges.append(("J2", "J76"))
         edges.append(("J76", "J3"))
 
-        for (a, b) in edges:
+        for a, b in edges:
             if a in ppg.global_pipegraph.jobs and b in ppg.global_pipegraph.jobs:
                 ppg.global_pipegraph.jobs[a].depends_on(ppg.global_pipegraph.jobs[b])
             else:
                 print("unused edge", a, b)
 
         ppg.run()
         ppg.run(event_timeout=1)
@@ -1393,15 +1393,15 @@
         edges.append(("81", "102"))
         edges.append(("103", "104"))
         edges.append(("80", "105"))
         edges.append(("79", "106"))
         edges.append(("76", "107"))
         edges.append(("76", "108"))
         edges.append(("2", "109"))
-        for (a, b) in edges:
+        for a, b in edges:
             if a in ppg.global_pipegraph.jobs and b in ppg.global_pipegraph.jobs:
                 ppg.global_pipegraph.jobs[a].depends_on(ppg.global_pipegraph.jobs[b])
 
         ppg.run()
         ppg.run()
         edges.append(("8", "5"))
         edges.append(("5", "6"))
@@ -1455,15 +1455,15 @@
         edges.append(("81", "102"))
         edges.append(("103", "104"))
         edges.append(("80", "105"))
         edges.append(("79", "106"))
         edges.append(("76", "107"))
         edges.append(("76", "108"))
         edges.append(("2", "109"))
-        for (a, b) in edges:
+        for a, b in edges:
             if a in ppg.global_pipegraph.jobs and b in ppg.global_pipegraph.jobs:
                 ppg.global_pipegraph.jobs[a].depends_on(ppg.global_pipegraph.jobs[b])
 
         ppg.run()
         ppg.run()
 
     def test_20210729(self, job_trace_log):
@@ -1491,15 +1491,15 @@
                 ("542", "530"),
                 ("542", "1"),
                 ("541", "1"),
                 ("541", "542"),
             ]
 
             ok_edges = []
-            for (a, b) in edges:
+            for a, b in edges:
                 if a in jobs_by_no and b in jobs_by_no:
                     jobs_by_no[a].depends_on(jobs_by_no[b])
                     ok_edges.append((a, b))
 
         ppg.new(allow_short_filenames=True)
         build()
         ppg.run()
@@ -1573,15 +1573,15 @@
 
         edges = []
 
         edges.append(("61", "48"))
         edges.append(("67", "48"))
         edges.append(("61", "3"))
 
-        for (a, b) in edges:
+        for a, b in edges:
             if a in ppg.global_pipegraph.jobs and b in ppg.global_pipegraph.jobs:
                 ppg.global_pipegraph.jobs[a].depends_on(ppg.global_pipegraph.jobs[b])
 
         ppg.run()
         ppg.run()
         do_fail = True
         with pytest.raises(ppg.JobsFailed):
@@ -1651,15 +1651,15 @@
                 no = k[k.find("_") + 1 :]
                 cjobs_by_no[no] = v
         edges = []
         ea = edges.append
         ea(("1", "2"))
         ea(("8", "11"))
         ea(("8", "2"))
-        for (a, b) in edges:
+        for a, b in edges:
             if a in cjobs_by_no and b in cjobs_by_no:
                 cjobs_by_no[a].depends_on(cjobs_by_no[b])
                 # print(f"ea(('{a}', '{b}'))")
 
         ppg.run()
 
         # now make it fail
@@ -1667,15 +1667,15 @@
         # as above
         job_1 = ppg.FileGeneratingJob("1", dummy_fg, depend_on_function=False)
         job_2 = ppg.TempFileGeneratingJob("2", dummy_fg, depend_on_function=False)
         job_8 = ppg.FileGeneratingJob("8", dummy_fg, depend_on_function=False)
 
         # make this one fail.
         job_11 = ppg.FileGeneratingJob("11", dummy_fg_raising, depend_on_function=True)
-        for (a, b) in edges:
+        for a, b in edges:
             if a in cjobs_by_no and b in cjobs_by_no:
                 cjobs_by_no[a].depends_on(cjobs_by_no[b])
 
         with pytest.raises(ppg.JobsFailed):
             ppg.run()
         assert (
             ppg.global_pipegraph.last_run_result["11"].outcome
@@ -1688,17 +1688,34 @@
         assert (
             ppg.global_pipegraph.last_run_result["CleanUp:2"].outcome
             == ppg.enums.JobOutcome.UpstreamFailed  # 11 fails, which fails 8, which fails this cleanup
         )
 
         # and boom, job was marked done & skipped, but we now inform it it's upstream failed.
 
+    def test_depends_on_mfg_by_str_job_id_does_not_work(self):
+        """Verify that you can't depend_on(job_id) off a multi file generating job,
+        but you can depend on the individual files.
 
-def gen_20211221(func):
+        """
+        a = ppg.FileGeneratingJob("a", lambda of: of.write_text("a"))
+
+        def do_b(ofs):
+            for fn in ofs:
+                fn.write_text(fn.name)
+
+        b = ppg.MultiFileGeneratingJob(["b", "c"], do_b)
+        # aassert ppg.global_pipegraph.find_job_from_file(b.job_id) is b
+        with pytest.raises(KeyError):
+            a.depends_on(b.job_id)
+        assert ppg.global_pipegraph.find_job_from_file("b") is b
+        assert ppg.global_pipegraph.find_job_from_file("c") is b
 
+
+def gen_20211221(func):
     global do_fail
 
     def dummy_fg_fail(of):
         global do_fail
         if do_fail[0]:
             raise ValueError()
         of.parent.mkdir(exist_ok=True, parents=True)
@@ -1722,11 +1739,11 @@
             cjobs_by_no[no] = v
     edges = []
     ea = edges.append
     ea(("1079", "1096"))
     ea(("1096", "650"))
     ea(("1096", "661"))
     ea(("650", "651"))
-    for (a, b) in edges:
+    for a, b in edges:
         if a in cjobs_by_no and b in cjobs_by_no:
             cjobs_by_no[a].depends_on(cjobs_by_no[b])
             # print(f"ea(('{a}', '{b}'))")
```

### Comparing `pypipegraph2-3.0.6/todo.md` & `pypipegraph2-3.0.7/todo.md`

 * *Files 5% similar despite different names*

```diff
@@ -126,7 +126,12 @@
 	- 
 	
 	- - test case for running
 	- does adding an *output* file correctly triggere a rebuild? how about removing one?
 
 
    - stop when having jobGeneratingJobs not working
+
+
+- recheck everything above
+   - sort interactive jobs by 'status' (running, waiting)
+   - much better default log output... tell me what jobs spawned & finished
```

### Comparing `pypipegraph2-3.0.6/PKG-INFO` & `pypipegraph2-3.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypipegraph2
-Version: 3.0.6
+Version: 3.0.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Requires-Dist: loguru
 Requires-Dist: rich
 Requires-Dist: xxhash
 Requires-Dist: wrapt
```

