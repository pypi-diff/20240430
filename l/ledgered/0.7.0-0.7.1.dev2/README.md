# Comparing `tmp/ledgered-0.7.0.tar.gz` & `tmp/ledgered-0.7.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledgered-0.7.0.tar", last modified: Fri Apr 12 15:08:34 2024, max compression
+gzip compressed data, was "ledgered-0.7.1.dev2.tar", last modified: Tue Apr 30 10:09:56 2024, max compression
```

## Comparing `ledgered-0.7.0.tar` & `ledgered-0.7.1.dev2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.058695 ledgered-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.050695 ledgered-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.054695 ledgered-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-12 15:08:25.000000 ledgered-0.7.0/.github/workflows/build_and_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-12 15:08:25.000000 ledgered-0.7.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-12 15:08:25.000000 ledgered-0.7.0/.github/workflows/fast-checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-12 15:08:25.000000 ledgered-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-12 15:08:25.000000 ledgered-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 15:08:25.000000 ledgered-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-12 15:08:34.058695 ledgered-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-12 15:08:25.000000 ledgered-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.054695 ledgered-0.7.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-12 15:08:25.000000 ledgered-0.7.0/doc/binary.md
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-12 15:08:25.000000 ledgered-0.7.0/doc/manifest.md
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-12 15:08:25.000000 ledgered-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:08:34.058695 ledgered-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.050695 ledgered-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.054695 ledgered-0.7.0/src/ledgered/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 15:08:33.000000 ledgered-0.7.0/src/ledgered/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/github.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.054695 ledgered-0.7.0/src/ledgered/manifest/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/manifest/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/manifest/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/manifest/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/manifest/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/manifest/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/manifest/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/manifest/use_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/manifest/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.054695 ledgered-0.7.0/src/ledgered/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:25.000000 ledgered-0.7.0/src/ledgered/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.058695 ledgered-0.7.0/src/ledgered.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-12 15:08:34.000000 ledgered-0.7.0/src/ledgered.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-12 15:08:34.000000 ledgered-0.7.0/src/ledgered.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:08:34.000000 ledgered-0.7.0/src/ledgered.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-12 15:08:34.000000 ledgered-0.7.0/src/ledgered.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 15:08:34.000000 ledgered-0.7.0/src/ledgered.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 15:08:34.000000 ledgered-0.7.0/src/ledgered.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.050695 ledgered-0.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.058695 ledgered-0.7.0/tests/_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/_data/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/_data/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/_data/full_correct.toml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/_data/ledger_app.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/_data/minimal.toml
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/_data/one_leaf.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.058695 ledgered-0.7.0/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/functional/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.058695 ledgered-0.7.0/tests/functional/manifest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/functional/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/functional/manifest/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/functional/test_github.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.058695 ledgered-0.7.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:34.058695 ledgered-0.7.0/tests/unit/manifest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/unit/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/unit/manifest/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/unit/manifest/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/unit/manifest/test_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/unit/manifest/test_use_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/unit/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/unit/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-12 15:08:25.000000 ledgered-0.7.0/tests/unit/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.677004 ledgered-0.7.1.dev2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.669004 ledgered-0.7.1.dev2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.669004 ledgered-0.7.1.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/.github/workflows/build_and_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/.github/workflows/fast-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-30 10:09:56.677004 ledgered-0.7.1.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.669004 ledgered-0.7.1.dev2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/doc/binary.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/doc/manifest.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 10:09:56.677004 ledgered-0.7.1.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.669004 ledgered-0.7.1.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.673004 ledgered-0.7.1.dev2/src/ledgered/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 10:09:56.000000 ledgered-0.7.1.dev2/src/ledgered/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.673004 ledgered-0.7.1.dev2/src/ledgered/manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/manifest/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/manifest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/manifest/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/manifest/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/manifest/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/manifest/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/manifest/use_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/manifest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.673004 ledgered-0.7.1.dev2/src/ledgered/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/src/ledgered/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.677004 ledgered-0.7.1.dev2/src/ledgered.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-30 10:09:56.000000 ledgered-0.7.1.dev2/src/ledgered.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-30 10:09:56.000000 ledgered-0.7.1.dev2/src/ledgered.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:09:56.000000 ledgered-0.7.1.dev2/src/ledgered.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 10:09:56.000000 ledgered-0.7.1.dev2/src/ledgered.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 10:09:56.000000 ledgered-0.7.1.dev2/src/ledgered.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 10:09:56.000000 ledgered-0.7.1.dev2/src/ledgered.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.669004 ledgered-0.7.1.dev2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.677004 ledgered-0.7.1.dev2/tests/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/_data/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/_data/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/_data/full_correct.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/_data/ledger_app.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/_data/minimal.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/_data/one_leaf.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.677004 ledgered-0.7.1.dev2/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/functional/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.677004 ledgered-0.7.1.dev2/tests/functional/manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/functional/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/functional/manifest/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/functional/test_github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.677004 ledgered-0.7.1.dev2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:56.677004 ledgered-0.7.1.dev2/tests/unit/manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/unit/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/unit/manifest/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/unit/manifest/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/unit/manifest/test_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/unit/manifest/test_use_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/unit/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/unit/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-30 10:09:50.000000 ledgered-0.7.1.dev2/tests/unit/test_serializers.py
```

### Comparing `ledgered-0.7.0/.github/workflows/build_and_tests.yml` & `ledgered-0.7.1.dev2/.github/workflows/build_and_tests.yml`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/.github/workflows/codeql-analysis.yml` & `ledgered-0.7.1.dev2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/.github/workflows/fast-checks.yml` & `ledgered-0.7.1.dev2/.github/workflows/fast-checks.yml`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/CHANGELOG.md` & `ledgered-0.7.1.dev2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.7.1] - 2024-04-30
+
+### Fixed
+
+- Clean error management when there is not `ledger_app.toml` manifest to access to on a given
+  repository/branch
 
 ## [0.7.0] - 2024-04-12
 
 ### Added
 
 - Added wrapper around GitHub API to ease manipulating Ledger application repositories
```

### Comparing `ledgered-0.7.0/LICENSE` & `ledgered-0.7.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/PKG-INFO` & `ledgered-0.7.1.dev2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledgered
-Version: 0.7.0
+Version: 0.7.1.dev2
 Summary: Python tools, utils, libraries, to be used with Ledger cryptodevices
 Author-email: Ledger <hello@ledger.fr>
 License: MIT License
         
         Copyright (c) 2023 Ledger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,8 +57,8 @@
 
 
 It will also contain libraries, utilitaries and other snippets useful when interfacing with Ledger
 devices (NanoS, S+, X and Stax).
 
 ## Library sections
 
-- [`ledger.utils.manifest` ](doc/manifest.md)
+- [`ledger.manifest` ](doc/manifest.md)
```

### Comparing `ledgered-0.7.0/README.md` & `ledgered-0.7.1.dev2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 
 
 It will also contain libraries, utilitaries and other snippets useful when interfacing with Ledger
 devices (NanoS, S+, X and Stax).
 
 ## Library sections
 
-- [`ledger.utils.manifest` ](doc/manifest.md)
+- [`ledger.manifest` ](doc/manifest.md)
```

### Comparing `ledgered-0.7.0/doc/binary.md` & `ledgered-0.7.1.dev2/doc/binary.md`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/doc/manifest.md` & `ledgered-0.7.1.dev2/doc/manifest.md`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/pyproject.toml` & `ledgered-0.7.1.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/src/ledgered/binary.py` & `ledgered-0.7.1.dev2/src/ledgered/binary.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/src/ledgered/github.py` & `ledgered-0.7.1.dev2/src/ledgered/github.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import IntEnum, auto
 from github import ContentFile as PyContentFile, Github as PyGithub, Repository as PyRepository
+from github.GithubException import UnknownObjectException
 from pathlib import Path
 from typing import List, Optional
 from unittest.mock import patch
 
 from ledgered.manifest import MANIFEST_FILE_NAME, Manifest
 
 LEDGER_ORG_NAME = "ledgerhq"
@@ -11,26 +12,39 @@
 
 class Condition(IntEnum):
     WITH = auto()
     WITHOUT = auto()
     ONLY = auto()
 
 
+class NoManifestException(FileNotFoundError):
+
+    def __init__(self, repository: "AppRepository"):
+        super().__init__(f"`ledger_app.toml` manifest not found in repository '{repository.url}', "
+                         f"branch '{repository.current_branch}'.")
+
+
 class AppRepository(PyRepository.Repository):
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._manifest: Optional[Manifest] = None
         self._makefile: Optional[str] = None
         self._branch: str = self.default_branch
 
     @property
     def manifest(self) -> Manifest:
         if self._manifest is None:
-            manifest = self.get_contents(MANIFEST_FILE_NAME, ref=self.current_branch)
+            try:
+                manifest = self.get_contents(MANIFEST_FILE_NAME, ref=self.current_branch)
+            except UnknownObjectException as e:
+                if e.status == 404:
+                    raise NoManifestException(self)
+                raise e
+
             # `get_contents` can return a list, but here there can only be one manifest
             assert isinstance(manifest, PyContentFile.ContentFile)
             manifest_content = manifest.decoded_content.decode()
             self._manifest = Manifest.from_string(manifest_content)
         return self._manifest
 
     @property
```

### Comparing `ledgered-0.7.0/src/ledgered/manifest/app.py` & `ledgered-0.7.1.dev2/src/ledgered/manifest/app.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/src/ledgered/manifest/cli.py` & `ledgered-0.7.1.dev2/src/ledgered/manifest/cli.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/src/ledgered/manifest/manifest.py` & `ledgered-0.7.1.dev2/src/ledgered/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/src/ledgered/manifest/tests.py` & `ledgered-0.7.1.dev2/src/ledgered/manifest/tests.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/src/ledgered/manifest/use_cases.py` & `ledgered-0.7.1.dev2/src/ledgered/manifest/use_cases.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/src/ledgered/serializers.py` & `ledgered-0.7.1.dev2/src/ledgered/serializers.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/src/ledgered.egg-info/PKG-INFO` & `ledgered-0.7.1.dev2/src/ledgered.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledgered
-Version: 0.7.0
+Version: 0.7.1.dev2
 Summary: Python tools, utils, libraries, to be used with Ledger cryptodevices
 Author-email: Ledger <hello@ledger.fr>
 License: MIT License
         
         Copyright (c) 2023 Ledger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,8 +57,8 @@
 
 
 It will also contain libraries, utilitaries and other snippets useful when interfacing with Ledger
 devices (NanoS, S+, X and Stax).
 
 ## Library sections
 
-- [`ledger.utils.manifest` ](doc/manifest.md)
+- [`ledger.manifest` ](doc/manifest.md)
```

### Comparing `ledgered-0.7.0/src/ledgered.egg-info/SOURCES.txt` & `ledgered-0.7.1.dev2/src/ledgered.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/tests/functional/conftest.py` & `ledgered-0.7.1.dev2/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/tests/functional/manifest/test_cli.py` & `ledgered-0.7.1.dev2/tests/functional/manifest/test_cli.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/tests/functional/test_github.py` & `ledgered-0.7.1.dev2/tests/functional/test_github.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/tests/unit/manifest/test_app.py` & `ledgered-0.7.1.dev2/tests/unit/manifest/test_app.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/tests/unit/manifest/test_manifest.py` & `ledgered-0.7.1.dev2/tests/unit/manifest/test_manifest.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/tests/unit/manifest/test_tests.py` & `ledgered-0.7.1.dev2/tests/unit/manifest/test_tests.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/tests/unit/manifest/test_use_cases.py` & `ledgered-0.7.1.dev2/tests/unit/manifest/test_use_cases.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/tests/unit/test_binary.py` & `ledgered-0.7.1.dev2/tests/unit/test_binary.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/tests/unit/test_github.py` & `ledgered-0.7.1.dev2/tests/unit/test_github.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.7.0/tests/unit/test_serializers.py` & `ledgered-0.7.1.dev2/tests/unit/test_serializers.py`

 * *Files identical despite different names*

