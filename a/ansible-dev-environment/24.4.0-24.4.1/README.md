# Comparing `tmp/ansible_dev_environment-24.4.0.tar.gz` & `tmp/ansible_dev_environment-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_dev_environment-24.4.0.tar", last modified: Thu Apr 25 15:20:14 2024, max compression
+gzip compressed data, was "ansible_dev_environment-24.4.1.tar", last modified: Mon Apr 29 23:03:54 2024, max compression
```

## Comparing `ansible_dev_environment-24.4.0.tar` & `ansible_dev_environment-24.4.1.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.656499 ansible_dev_environment-24.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.644500 ansible_dev_environment-24.4.0/.config/
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.config/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.config/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.config/requirements-docs.in
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.config/requirements-test.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.config/requirements.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.644500 ansible_dev_environment-24.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.648500 ansible_dev_environment-24.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.648500 ansible_dev_environment-24.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-25 15:20:14.656499 ansible_dev_environment-24.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.648500 ansible_dev_environment-24.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:20:14.656499 ansible_dev_environment-24.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.640500 ansible_dev_environment-24.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.648500 ansible_dev_environment-24.4.0/src/ansible_dev_environment/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.652500 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)    18224 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/lister.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/treemaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/uninstaller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.656499 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.652500 ansible_dev_environment-24.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.652500 ansible_dev_environment-24.4.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/fixtures/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/fixtures/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.652500 ansible_dev_environment-24.4.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/integration/test_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.652500 ansible_dev_environment-24.4.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/unit/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.177497 ansible_dev_environment-24.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.165497 ansible_dev_environment-24.4.1/.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.config/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.config/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.config/requirements-docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.config/requirements-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.config/requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.169497 ansible_dev_environment-24.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.169497 ansible_dev_environment-24.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.169497 ansible_dev_environment-24.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-29 23:03:54.177497 ansible_dev_environment-24.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.169497 ansible_dev_environment-24.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 23:03:54.177497 ansible_dev_environment-24.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.161497 ansible_dev_environment-24.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.169497 ansible_dev_environment-24.4.1/src/ansible_dev_environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.173497 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/lister.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/treemaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/uninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.177497 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 23:03:54.000000 ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.173497 ansible_dev_environment-24.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.173497 ansible_dev_environment-24.4.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/fixtures/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/fixtures/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.173497 ansible_dev_environment-24.4.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/integration/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:03:54.177497 ansible_dev_environment-24.4.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/unit/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/unit/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-29 23:03:43.000000 ansible_dev_environment-24.4.1/tox.ini
```

### Comparing `ansible_dev_environment-24.4.0/.config/constraints.txt` & `ansible_dev_environment-24.4.1/.config/constraints.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,105 +5,105 @@
 #    pip-compile --all-extras --no-annotate --output-file=.config/constraints.txt --strip-extras .config/requirements.in pyproject.toml
 #
 ansible-builder==3.0.1
 attrs==23.2.0
 babel==2.14.0
 beautifulsoup4==4.12.3
 bindep==2.11.0
-black==24.3.0
+black==24.4.2
 cachetools==5.3.3
-cairocffi==1.6.1
+cairocffi==1.7.0
 cairosvg==2.7.1
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
-coverage==7.4.4
+coverage==7.5.0
 csscompressor==0.9.5
 cssselect2==0.7.0
 defusedxml==0.7.1
 distlib==0.3.8
 distro==1.9.0
 dnspython==2.6.1
 docstring-parser-fork==0.0.5
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
 execnet==2.1.1
-filelock==3.13.3
+filelock==3.14.0
 ghp-import==2.1.0
-griffe==0.42.1
+griffe==0.44.0
 htmlmin2==0.1.13
-identify==2.5.35
-idna==3.6
+identify==2.5.36
+idna==3.7
 iniconfig==2.0.0
 jinja2==3.1.3
 jsmin==3.0.1
 jsonschema==4.21.1
 jsonschema-specifications==2023.12.1
 linkchecker==10.4.0
 markdown==3.6
-markdown-exec==1.8.0
+markdown-exec==1.8.1
 markdown-include==0.8.1
 markupsafe==2.1.5
 mergedeep==1.3.4
-mkdocs==1.5.3
+mkdocs==1.6.0
 mkdocs-ansible==24.3.0
 mkdocs-autorefs==1.0.1
 mkdocs-gen-files==0.5.0
-mkdocs-htmlproofer-plugin==1.2.0
-mkdocs-material==9.5.17
+mkdocs-htmlproofer-plugin==1.2.1
+mkdocs-material==9.5.20
 mkdocs-material-extensions==1.3.1
 mkdocs-minify-plugin==0.8.0
 mkdocs-monorepo-plugin==1.1.0
-mkdocstrings==0.24.3
-mkdocstrings-python==1.9.2
-mypy==1.9.0
+mkdocstrings==0.25.0
+mkdocstrings-python==1.10.0
+mypy==1.10.0
 mypy-extensions==1.0.0
 nodeenv==1.8.0
 packaging==24.0
 paginate==0.5.6
 parsley==1.3
 pathspec==0.12.1
 pbr==6.0.0
 pillow==10.3.0
-pipdeptree==2.17.0
-platformdirs==4.2.0
-pluggy==1.4.0
+pipdeptree==2.19.1
+platformdirs==4.2.1
+pluggy==1.5.0
 pre-commit==3.7.0
 pycparser==2.22
 pydoclint==0.4.1
 pygments==2.17.2
-pymdown-extensions==10.7.1
+pymdown-extensions==10.8.1
 pyproject-api==1.6.1
-pytest==8.1.1
-pytest-xdist==3.5.0
+pytest==8.2.0
+pytest-xdist==3.6.1
 python-dateutil==2.9.0.post0
 python-slugify==8.0.4
 pyyaml==6.0.1
 pyyaml-env-tag==0.1
-referencing==0.34.0
-regex==2023.12.25
+referencing==0.35.0
+regex==2024.4.28
 requests==2.31.0
 requirements-parser==0.9.0
 rpds-py==0.18.0
-ruff==0.3.5
+ruff==0.4.2
 six==1.16.0
 soupsieve==2.5
 subprocess-tee==0.4.1
 text-unidecode==1.3
-tinycss2==1.2.1
+tinycss2==1.3.0
 toml-sort==0.23.1
 tomli==2.0.1
 tomlkit==0.12.4
-tox==4.14.2
+tox==4.15.0
 types-pyyaml==6.0.12.20240311
-types-setuptools==69.2.0.20240317
+types-setuptools==69.5.0.20240423
 typing-extensions==4.11.0
 urllib3==2.2.1
-virtualenv==20.25.1
+virtualenv==20.26.1
 watchdog==4.0.0
 webencodings==0.5.1
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `ansible_dev_environment-24.4.0/.github/workflows/ack.yml` & `ansible_dev_environment-24.4.1/.github/workflows/ack.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/.github/workflows/release.yml` & `ansible_dev_environment-24.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/.github/workflows/tox.yml` & `ansible_dev_environment-24.4.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/.gitignore` & `ansible_dev_environment-24.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/.pre-commit-config.yaml` & `ansible_dev_environment-24.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/.vscode/launch.json` & `ansible_dev_environment-24.4.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/.vscode/settings.json` & `ansible_dev_environment-24.4.1/.vscode/settings.json`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   // Override the pyproject.toml and disable xdist to enable test debugging
   "python.testing.pytestArgs": ["-n0", "--dist", "no"],
   "[python]": {
     "editor.formatOnSave": true,
     "editor.codeActionsOnSave": {
       "source.fixAll": "explicit"
     },
-    "editor.defaultFormatter": "ms-python.black-formatter"
+    "editor.defaultFormatter": "charliermarsh.ruff"
   },
   "mypy.runUsingActiveInterpreter": true,
   "mypy.targets": ["src", "tests"],
   "[jsonc]": {
     "editor.defaultFormatter": "esbenp.prettier-vscode"
   }
 }
```

### Comparing `ansible_dev_environment-24.4.0/LICENSE` & `ansible_dev_environment-24.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/PKG-INFO` & `ansible_dev_environment-24.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-environment
-Version: 24.4.0
+Version: 24.4.1
 Summary: A pip-like ansible collection installer.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Bradley Thornton <bthornto@redhat.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-environment/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-environment/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-environment
```

### Comparing `ansible_dev_environment-24.4.0/README.md` & `ansible_dev_environment-24.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/cspell.config.yaml` & `ansible_dev_environment-24.4.1/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/docs/index.md` & `ansible_dev_environment-24.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/mkdocs.yml` & `ansible_dev_environment-24.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/pyproject.toml` & `ansible_dev_environment-24.4.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -80,174 +80,229 @@
   "_version.py" # built by setuptools_scm
 ]
 jobs = 0
 no-docstring-rgx = "__.*__"
 
 [tool.pylint.messages_control]
 disable = [
+  "unknown-option-value",
   # https://gist.github.com/cidrblock/ec3412bacfeb34dbc2d334c1d53bef83
   "C0103", # invalid-name / ruff N815
   "C0105", # typevar-name-incorrect-variance / ruff PLC0105
   "C0112", # empty-docstring / ruff D419
   "C0113", # unneeded-not / ruff SIM208
   "C0114", # missing-module-docstring / ruff D100
   "C0115", # missing-class-docstring / ruff D101
   "C0116", # missing-function-docstring / ruff D103
   "C0121", # singleton-comparison / ruff PLC0121
   "C0123", # unidiomatic-typecheck / ruff E721
   "C0131", # typevar-double-variance / ruff PLC0131
   "C0132", # typevar-name-mismatch / ruff PLC0132
-  # "C0198", # bad-docstring-quotes / ruff Q002
-  # "C0199", # docstring-first-line-empty / ruff D210
+  "C0198", # bad-docstring-quotes / ruff Q002
+  "C0199", # docstring-first-line-empty / ruff D210
   "C0201", # consider-iterating-dictionary / ruff SIM118
   "C0202", # bad-classmethod-argument / ruff PLC0202
   "C0205", # single-string-used-for-slots / ruff PLC0205
   "C0208", # use-sequence-for-iteration / ruff PLC0208
   "C0301", # line-too-long / ruff E501
+  "C0303", # trailing-whitespace / ruff W291
   "C0304", # missing-final-newline / ruff W292
   "C0321", # multiple-statements / ruff PLC0321
-  "C0325", # superfluous-parens / ruff UP034
   "C0410", # multiple-imports / ruff E401
   "C0411", # wrong-import-order / ruff I001
   "C0412", # ungrouped-imports / ruff I001
   "C0413", # wrong-import-position / ruff E402
   "C0414", # useless-import-alias / ruff PLC0414
-  # "C0501", # consider-using-any-or-all / ruff PLC0501
-  # "C1901", # compare-to-empty-string / ruff PLC1901
-  # "C2201", # misplaced-comparison-constant / ruff SIM300
-  "C3001", # unnecessary-lambda-assignment / ruff PLC3001
+  "C0415", # import-outside-toplevel / ruff PLC0415
+  "C0501", # consider-using-any-or-all / ruff PLC0501
+  "C1901", # compare-to-empty-string / ruff PLC1901
+  "C2201", # misplaced-comparison-constant / ruff SIM300
+  "C2401", # non-ascii-name / ruff PLC2401
+  "C2403", # non-ascii-module-import / ruff PLC2403
+  "C2701", # import-private-name / ruff PLC2701
+  "C2801", # unnecessary-dunder-call / ruff PLC2801
+  "C3001", # unnecessary-lambda-assignment / ruff E731
   "C3002", # unnecessary-direct-lambda-call / ruff PLC3002
   "E0001", # syntax-error / ruff E999
+  "E0100", # init-is-generator / ruff PLE0100
   "E0101", # return-in-init / ruff PLE0101
   "E0102", # function-redefined / ruff F811
   "E0103", # not-in-loop / ruff PLE0103
   "E0104", # return-outside-function / ruff F706
   "E0105", # yield-outside-function / ruff F704
   "E0107", # nonexistent-operator / ruff B002
   "E0112", # too-many-star-expressions / ruff F622
+  "E0115", # nonlocal-and-global / ruff PLE0115
   "E0116", # continue-in-finally / ruff PLE0116
   "E0117", # nonlocal-without-binding / ruff PLE0117
   "E0118", # used-prior-global-declaration / ruff PLE0118
   "E0211", # no-method-argument / ruff N805
   "E0213", # no-self-argument / ruff N805
+  "E0237", # assigning-non-slot / ruff PLE0237
   "E0241", # duplicate-bases / ruff PLE0241
   "E0302", # unexpected-special-method-signature / ruff PLE0302
+  "E0303", # invalid-length-returned / ruff PLE0303
+  "E0304", # invalid-bool-returned / ruff PLE0304
+  "E0305", # invalid-index-returned / ruff PLE0305
+  "E0308", # invalid-bytes-returned / ruff PLE0308
+  "E0309", # invalid-hash-returned / ruff PLE0309
+  "E0402", # relative-beyond-top-level / ruff TID252
   "E0602", # undefined-variable / ruff F821
   "E0603", # undefined-all-variable / ruff F822
   "E0604", # invalid-all-object / ruff PLE0604
   "E0605", # invalid-all-format / ruff PLE0605
+  "E0643", # potential-index-error / ruff PLE0643
+  "E0704", # misplaced-bare-raise / ruff PLE0704
   "E0711", # notimplemented-raised / ruff F901
+  "E1132", # repeated-keyword / ruff PLE1132
   "E1142", # await-outside-async / ruff PLE1142
   "E1205", # logging-too-many-args / ruff PLE1205
   "E1206", # logging-too-few-args / ruff PLE1206
+  "E1300", # bad-format-character / ruff PLE1300
   "E1301", # truncated-format-string / ruff F501
   "E1302", # mixed-format-string / ruff F506
   "E1303", # format-needs-mapping / ruff F502
   "E1304", # missing-format-string-key / ruff F524
   "E1305", # too-many-format-args / ruff F522
   "E1306", # too-few-format-args / ruff F524
   "E1307", # bad-string-format-type / ruff PLE1307
   "E1310", # bad-str-strip-call / ruff PLE1310
+  "E1519", # singledispatch-method / ruff PLE1519
+  "E1520", # singledispatchmethod-function / ruff PLE5120
   "E1700", # yield-inside-async-function / ruff PLE1700
   "E2502", # bidirectional-unicode / ruff PLE2502
   "E2510", # invalid-character-backspace / ruff PLE2510
   "E2512", # invalid-character-sub / ruff PLE2512
   "E2513", # invalid-character-esc / ruff PLE2513
   "E2514", # invalid-character-nul / ruff PLE2514
   "E2515", # invalid-character-zero-width-space / ruff PLE2515
+  "E4703", # modified-iterating-set / ruff PLE4703
   "R0123", # literal-comparison / ruff F632
   "R0124", # comparison-with-itself / ruff PLR0124
   "R0133", # comparison-of-constants / ruff PLR0133
+  "R0202", # no-classmethod-decorator / ruff PLR0202
+  "R0203", # no-staticmethod-decorator / ruff PLR0203
   "R0205", # useless-object-inheritance / ruff UP004
   "R0206", # property-with-parameters / ruff PLR0206
+  "R0904", # too-many-public-methods / ruff PLR0904
   "R0911", # too-many-return-statements / ruff PLR0911
   "R0912", # too-many-branches / ruff PLR0912
   "R0913", # too-many-arguments / ruff PLR0913
+  "R0914", # too-many-locals / ruff PLR0914
   "R0915", # too-many-statements / ruff PLR0915
-  # "R1260", # too-complex / ruff C901
+  "R0916", # too-many-boolean-expressions / ruff PLR0916
+  "R1260", # too-complex / ruff C901
   "R1701", # consider-merging-isinstance / ruff PLR1701
+  "R1702", # too-many-nested-blocks / ruff PLR1702
+  "R1703", # simplifiable-if-statement / ruff SIM108
+  "R1704", # redefined-argument-from-local / ruff PLR1704
   "R1705", # no-else-return / ruff RET505
-  "R1706", # consider-using-ternary / ruff SIM108
+  "R1706", # consider-using-ternary / ruff PLR1706
   "R1707", # trailing-comma-tuple / ruff COM818
   "R1710", # inconsistent-return-statements / ruff PLR1710
   "R1711", # useless-return / ruff PLR1711
   "R1714", # consider-using-in / ruff PLR1714
   "R1715", # consider-using-get / ruff SIM401
   "R1717", # consider-using-dict-comprehension / ruff C402
   "R1718", # consider-using-set-comprehension / ruff C401
+  "R1719", # simplifiable-if-expression / ruff PLR1719
   "R1720", # no-else-raise / ruff RET506
-  "R1721", # unnecessary-comprehension / ruff PLR1721
+  "R1721", # unnecessary-comprehension / ruff C416
   "R1722", # consider-using-sys-exit / ruff PLR1722
   "R1723", # no-else-break / ruff RET508
   "R1724", # no-else-continue / ruff RET507
   "R1725", # super-with-arguments / ruff UP008
   "R1728", # consider-using-generator / ruff C417
-  "R1729", # use-a-generator / ruff C417
+  "R1729", # use-a-generator / ruff C419
+  "R1730", # consider-using-min-builtin / ruff PLR1730
+  "R1731", # consider-using-max-builtin / ruff PLR1730
+  "R1732", # consider-using-with / ruff SIM115
+  "R1733", # unnecessary-dict-index-lookup / ruff PLR1733
   "R1734", # use-list-literal / ruff C405
   "R1735", # use-dict-literal / ruff C406
-  # "R2004", # magic-value-comparison / ruff PLR2004
-  # "R5501", # else-if-used / ruff PLR5501
-  # "R6002", # consider-using-alias / ruff UP006
-  # "R6003", # consider-alternative-union-syntax / ruff UP007
+  "R1736", # unnecessary-list-index-lookup / ruff PLR1736
+  "R2004", # magic-value-comparison / ruff PLR2004
+  "R2044", # empty-comment / ruff PLR2044
+  "R5501", # else-if-used / ruff PLR5501
+  "R6002", # consider-using-alias / ruff UP006
+  "R6003", # consider-alternative-union-syntax / ruff UP007
+  "R6104", # consider-using-augmented-assign / ruff PLR6104
+  "R6201", # use-set-for-membership / ruff PLR6201
+  "R6301", # no-self-use / ruff PLR6301
   "W0102", # dangerous-default-value / ruff B006
   "W0104", # pointless-statement / ruff B018
   "W0106", # expression-not-assigned / ruff B018
-  "W0107", # unnecessary-pass / ruff PLW0107
+  "W0107", # unnecessary-pass / ruff PIE790
+  "W0108", # unnecessary-lambda / ruff PLW0108
   "W0109", # duplicate-key / ruff F601
   "W0120", # useless-else-on-loop / ruff PLW0120
   "W0122", # exec-used / ruff S102
   "W0123", # eval-used / ruff PGH001
   "W0127", # self-assigning-variable / ruff PLW0127
   "W0129", # assert-on-string-literal / ruff PLW0129
-  "W0130", # duplicate-value / ruff PLW0130
+  "W0130", # duplicate-value / ruff B033
   "W0131", # named-expr-without-context / ruff PLW0131
+  "W0133", # pointless-exception-statement / ruff PLW0133
   "W0150", # lost-exception / ruff B012
-  # "W0160", # consider-ternary-expression / ruff SIM108
+  "W0160", # consider-ternary-expression / ruff SIM108
+  "W0177", # nan-comparison / ruff PLW0117
   "W0199", # assert-on-tuple / ruff F631
+  "W0211", # bad-staticmethod-argument / ruff PLW0211
+  "W0212", # protected-access / ruff SLF001
+  "W0245", # super-without-brackets / ruff PLW0245
   "W0301", # unnecessary-semicolon / ruff E703
   "W0401", # wildcard-import / ruff F403
+  "W0404", # reimported / ruff F811
   "W0406", # import-self / ruff PLW0406
   "W0410", # misplaced-future / ruff F404
   "W0511", # fixme / ruff PLW0511
   "W0602", # global-variable-not-assigned / ruff PLW0602
   "W0603", # global-statement / ruff PLW0603
+  "W0604", # global-at-module-level / ruff PLW0604
   "W0611", # unused-import / ruff F401
   "W0612", # unused-variable / ruff F841
   "W0613", # unused-argument / ruff ARG001
   "W0622", # redefined-builtin / ruff A001
   "W0640", # cell-var-from-loop / ruff B023
   "W0702", # bare-except / ruff E722
   "W0705", # duplicate-except / ruff B014
   "W0706", # try-except-raise / ruff TRY302
   "W0707", # raise-missing-from / ruff TRY200
   "W0711", # binary-op-exception / ruff PLW0711
   "W0718", # broad-exception-caught / ruff PLW0718
+  "W0719", # broad-exception-raised / ruff TRY002
   "W1113", # keyword-arg-before-vararg / ruff B026
   "W1201", # logging-not-lazy / ruff G
   "W1202", # logging-format-interpolation / ruff G
   "W1203", # logging-fstring-interpolation / ruff G
   "W1300", # bad-format-string-key / ruff PLW1300
   "W1301", # unused-format-string-key / ruff F504
   "W1302", # bad-format-string / ruff PLW1302
   "W1303", # missing-format-argument-key / ruff F524
   "W1304", # unused-format-string-argument / ruff F507
   "W1305", # format-combined-specification / ruff F525
   "W1308", # duplicate-string-formatting-argument / ruff PLW1308
   "W1309", # f-string-without-interpolation / ruff F541
-  "W1310", # format-string-without-interpolation / ruff PLW1310
+  "W1310", # format-string-without-interpolation / ruff F541
   "W1401", # anomalous-backslash-in-string / ruff W605
   "W1404", # implicit-str-concat / ruff ISC001
   "W1405", # inconsistent-quotes / ruff Q000
+  "W1406", # redundant-u-string-prefix / ruff UP025
+  "W1501", # bad-open-mode / ruff PLW1501
   "W1508", # invalid-envvar-default / ruff PLW1508
   "W1509", # subprocess-popen-preexec-fn / ruff PLW1509
   "W1510", # subprocess-run-check / ruff PLW1510
+  "W1514", # unspecified-encoding / ruff PLW1514
   "W1515", # forgotten-debug-statement / ruff T100
-  # "W1641", # eq-without-hash / ruff PLW1641
-  # "W2901", # redefined-loop-name / ruff PLW2901
-  # "W3201", # bad-dunder-name / ruff PLW3201
+  "W1518", # method-cache-max-size-none / ruff B019
+  "W1641", # eq-without-hash / ruff PLW1641
+  "W2101", # useless-with-lock / ruff PLW2101
+  "W2402", # non-ascii-file-name / ruff N999
+  "W2901", # redefined-loop-name / ruff PLW2901
+  "W3201", # bad-dunder-name / ruff PLW3201
   "W3301", # nested-min-max / ruff PLW3301
   "duplicate-code",
   "fixme",
   "too-few-public-methods",
   "unsubscriptable-object"
 ]
 
@@ -262,18 +317,19 @@
 parametrize-values-type = "tuple"
 
 [tool.ruff.isort]
 lines-after-imports = 2 # Ensures consistency for cases when there's variable vs function/class definitions after imports
 lines-between-types = 1 # Separate import/from with 1 line
 
 [tool.ruff.per-file-ignores]
+# SLF001: Allow private member access in tests
 # S101 Allow assert in tests
 # S602 Allow shell in test
 # T201 Allow print in tests
-"tests/**" = ["S101", "S602", "T201"]
+"tests/**" = ["SLF001", "S101", "S602", "T201"]
 
 [tool.ruff.pydocstyle]
 convention = "pep257"
 
 [tool.setuptools.dynamic]
 dependencies = {file = [".config/requirements.in"]}
 optional-dependencies.dev = {file = [".config/requirements-dev.in"]}
```

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment/arg_parser.py` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment/arg_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment/cli.py` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment/collection.py` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment/collection.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment/config.py` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment/config.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment/output.py` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment/output.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/checker.py` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/checker.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/inspector.py` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/inspector.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/installer.py` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/installer.py`

 * *Files 8% similar despite different names*

```diff
@@ -211,23 +211,24 @@
         installed = re.findall(r"(\w+\.\w+):.*installed", proc.stdout)
         if not self._config.args.cpi:
             msg = f"Installed collections include: {oxford_join(installed)}"
         else:
             msg = f"Source installed collections include: {oxford_join(installed)}"
         self._output.note(msg)
 
-    def _copy_files_using_git_ls_files(
+    def _find_files_using_git_ls_files(
         self: Installer,
         local_repo_path: Path | None,
-    ) -> str | None:
+    ) -> tuple[str | None, str | None]:
         """Copy collection files tracked using git ls-files to the build directory.
 
         Args:
             local_repo_path: The collection local path.
         Returns:
+            string with the command used to list files or None
             string containing a list of files or nothing
         """
         msg = "List collection files using git ls-files."
         self._output.debug(msg)
 
         try:
             # Get the list of tracked files in the repository
@@ -236,27 +237,29 @@
                 cwd=local_repo_path,
                 verbose=self._config.args.verbose,
                 msg=msg,
                 output=self._output,
             )
         except subprocess.CalledProcessError as exc:
             err = f"Failed to list collection using git ls-files: {exc} {exc.stderr}"
-            self._output.critical(err)
+            self._output.info(err)
+            return None, None
 
-        return tracked_files_output.stdout
+        return "git ls-files", tracked_files_output.stdout
 
-    def _copy_files_using_ls(
+    def _find_files_using_ls(
         self: Installer,
         local_repo_path: Path | None,
-    ) -> str | None:
+    ) -> tuple[str | None, str | None]:
         """Copy collection files tracked using ls to the build directory.
 
         Args:
             local_repo_path: The collection local path.
         Returns:
+            string with the command used to list files or None
             string containing a list of files or nothing
         """
         msg = "List collection files using ls."
         self._output.debug(msg)
 
         try:
             # Get the list of tracked files in the repository
@@ -265,17 +268,18 @@
                 cwd=local_repo_path,
                 verbose=self._config.args.verbose,
                 msg=msg,
                 output=self._output,
             )
         except subprocess.CalledProcessError as exc:
             err = f"Failed to list collection using ls: {exc} {exc.stderr}"
-            self._output.critical(err)
+            self._output.debug(err)
+            return None, None
 
-        return tracked_files_output.stdout
+        return "ls", tracked_files_output.stdout
 
     def _copy_repo_files(
         self: Installer,
         local_repo_path: Path | None,
         destination_path: Path,
     ) -> None:
         """Copy collection files tracked in git to the build directory.
@@ -283,43 +287,42 @@
         Args:
             local_repo_path: The collection local path.
             destination_path: The build destination path.
 
         """
         if local_repo_path is None:
             msg = "Invalid repo path, no files to copy"
-            self._output.info(msg)
+            self._output.debug(msg)
             return
 
         # Get tracked files from git ls-files command
-        tracked_files_output = self._copy_files_using_git_ls_files(
+        found_using, files_stdout = self._find_files_using_git_ls_files(
             local_repo_path=local_repo_path,
         )
 
-        if tracked_files_output is None:
-            msg = "No tracked files found using git ls-files"
-            self._output.info(msg)
-
-            # If no tracked files found, get files using ls command
-            tracked_files_output = self._copy_files_using_ls(
+        if not files_stdout:
+            found_using, files_stdout = self._find_files_using_ls(
                 local_repo_path=local_repo_path,
             )
 
-        if tracked_files_output is None:
-            msg = "No files found"
-            self._output.info(msg)
+        if not files_stdout:
+            msg = "No files found with either 'git ls-files' or 'ls"
+            self._output.critical(msg)
             return
 
+        msg = f"File list generated with '{found_using}'"
+        self._output.info(msg)
+
         # Parse tracked files output
-        tracked_files = tracked_files_output.split("\n")
+        files_list = files_stdout.split("\n")
 
         # Create the destination folder if it doesn't exist
         Path(destination_path).mkdir(parents=True, exist_ok=True)
 
-        for file in tracked_files:
+        for file in files_list:
             src_file_path = Path(local_repo_path) / file
             dest_file_path = Path(destination_path) / file
 
             # Ensure the destination directory for the file exists
             dest_file_path.parent.mkdir(parents=True, exist_ok=True)
 
             if src_file_path.is_dir():
```

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/lister.py` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/lister.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/treemaker.py` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/treemaker.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/uninstaller.py` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment/subcommands/uninstaller.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment/tree.py` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment/tree.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment/utils.py` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment/utils.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/PKG-INFO` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-environment
-Version: 24.4.0
+Version: 24.4.1
 Summary: A pip-like ansible collection installer.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Bradley Thornton <bthornto@redhat.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-environment/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-environment/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-environment
```

### Comparing `ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/SOURCES.txt` & `ansible_dev_environment-24.4.1/src/ansible_dev_environment.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -51,10 +51,12 @@
 src/ansible_dev_environment/subcommands/uninstaller.py
 tests/__init__.py
 tests/fixtures/galaxy.yml
 tests/fixtures/requirements.yml
 tests/integration/__init__.py
 tests/integration/test_basic.py
 tests/unit/__init__.py
+tests/unit/conftest.py
 tests/unit/test_config.py
+tests/unit/test_installer.py
 tests/unit/test_tree.py
 tests/unit/test_utils.py
```

### Comparing `ansible_dev_environment-24.4.0/tests/integration/test_basic.py` & `ansible_dev_environment-24.4.1/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/tests/unit/test_config.py` & `ansible_dev_environment-24.4.1/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/tests/unit/test_tree.py` & `ansible_dev_environment-24.4.1/tests/unit/test_tree.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/tests/unit/test_utils.py` & `ansible_dev_environment-24.4.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_environment-24.4.0/tox.ini` & `ansible_dev_environment-24.4.1/tox.ini`

 * *Files identical despite different names*

