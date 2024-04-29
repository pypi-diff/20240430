# Comparing `tmp/ansible_dev_tools-24.4.1.tar.gz` & `tmp/ansible_dev_tools-24.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_dev_tools-24.4.1.tar", last modified: Thu Apr 25 15:52:43 2024, max compression
+gzip compressed data, was "ansible_dev_tools-24.4.2.tar", last modified: Mon Apr 29 15:41:31 2024, max compression
```

## Comparing `ansible_dev_tools-24.4.1.tar` & `ansible_dev_tools-24.4.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.906848 ansible_dev_tools-24.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.894848 ansible_dev_tools-24.4.1/.config/
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.config/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.config/requirements-docs.in
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.config/requirements-server.in
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.config/requirements-test.in
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.config/requirements.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.894848 ansible_dev_tools-24.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.894848 ansible_dev_tools-24.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.894848 ansible_dev_tools-24.4.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-25 15:52:43.906848 ansible_dev_tools-24.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.894848 ansible_dev_tools-24.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/contributor-guide.md
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.898848 ansible_dev_tools-24.4.1/docs/media/
--rw-r--r--   0 runner    (1001) docker     (127)   351712 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/media/ansible-lint.mp4
--rw-r--r--   0 runner    (1001) docker     (127)   185365 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/media/ansible-navigator-run.mp4
--rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/media/compress.sh
--rw-r--r--   0 runner    (1001) docker     (127)   325589 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/media/create-collection.mp4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.898848 ansible_dev_tools-24.4.1/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/building-collection.md
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/ci-setup.md
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/content-best-practices.md
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/content-release.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.898848 ansible_dev_tools-24.4.1/docs/user-guide/images/
--rw-r--r--   0 runner    (1001) docker     (127)    75270 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/images/ci.png
--rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/images/release.png
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/testing.md
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:52:43.906848 ansible_dev_tools-24.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.890848 ansible_dev_tools-24.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.902848 ansible_dev_tools-24.4.1/src/ansible_dev_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.890848 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.902848 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.902848 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/data/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/data/openapi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/server_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.902848 ansible_dev_tools-24.4.1/src/ansible_dev_tools/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/subcommands/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/version_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.906848 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.902848 ansible_dev_tools-24.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.906848 ansible_dev_tools-24.4.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/tests/integration/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/tests/integration/test_server_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.689140 ansible_dev_tools-24.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.677141 ansible_dev_tools-24.4.2/.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.config/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.config/requirements-docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.config/requirements-server.in
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.config/requirements-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.config/requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.677141 ansible_dev_tools-24.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.677141 ansible_dev_tools-24.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.677141 ansible_dev_tools-24.4.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-29 15:41:31.689140 ansible_dev_tools-24.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.681141 ansible_dev_tools-24.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/contributor-guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.681141 ansible_dev_tools-24.4.2/docs/media/
+-rw-r--r--   0 runner    (1001) docker     (127)   351712 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/media/ansible-lint.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)   185365 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/media/ansible-navigator-run.mp4
+-rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/media/compress.sh
+-rw-r--r--   0 runner    (1001) docker     (127)   325589 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/media/create-collection.mp4
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.681141 ansible_dev_tools-24.4.2/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/user-guide/building-collection.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/user-guide/ci-setup.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/user-guide/content-best-practices.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/user-guide/content-release.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.685140 ansible_dev_tools-24.4.2/docs/user-guide/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    75270 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/user-guide/images/ci.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/user-guide/images/release.png
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/user-guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/docs/user-guide/testing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:41:31.689140 ansible_dev_tools-24.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.673141 ansible_dev_tools-24.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.685140 ansible_dev_tools-24.4.2/src/ansible_dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-29 15:41:31.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.673141 ansible_dev_tools-24.4.2/src/ansible_dev_tools/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.685140 ansible_dev_tools-24.4.2/src/ansible_dev_tools/resources/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/resources/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/resources/server/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.685140 ansible_dev_tools-24.4.2/src/ansible_dev_tools/resources/server/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/resources/server/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/resources/server/data/openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/server_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.685140 ansible_dev_tools-24.4.2/src/ansible_dev_tools/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/subcommands/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools/version_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.689140 ansible_dev_tools-24.4.2/src/ansible_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-29 15:41:31.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-29 15:41:31.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:41:31.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 15:41:31.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-29 15:41:31.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 15:41:31.000000 ansible_dev_tools-24.4.2/src/ansible_dev_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.689140 ansible_dev_tools-24.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:41:31.689140 ansible_dev_tools-24.4.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/tests/integration/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/tests/integration/test_server_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-29 15:41:19.000000 ansible_dev_tools-24.4.2/tox.ini
```

### Comparing `ansible_dev_tools-24.4.1/.config/constraints.txt` & `ansible_dev_tools-24.4.2/.config/constraints.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 ansible-builder==3.0.1
 ansible-compat==4.1.11
 ansible-core==2.16.6
 ansible-creator==24.4.3
 ansible-dev-environment==24.4.0
 ansible-lint==24.2.2
-ansible-navigator==24.2.0
+ansible-navigator==24.3.2
 ansible-runner==2.3.6
 ansible-sign==0.1.1
 asgiref==3.8.1
 attrs==23.2.0
 babel==2.14.0
 beautifulsoup4==4.12.3
 bindep==2.11.0
```

### Comparing `ansible_dev_tools-24.4.1/.github/dependabot.yml` & `ansible_dev_tools-24.4.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/.github/workflows/release.yml` & `ansible_dev_tools-24.4.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/.github/workflows/tox.yml` & `ansible_dev_tools-24.4.2/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/.gitignore` & `ansible_dev_tools-24.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/.pre-commit-config.yaml` & `ansible_dev_tools-24.4.2/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     rev: v1.9.0
     hooks:
       - id: mypy
         additional_dependencies:
           - django-stubs[compatible-mypy]
           - jinja2
           - pytest
+          - ansible-creator
           - tox
           - types-pyyaml
           - types-requests
           - types-setuptools
         args:
           - src
           - tests
```

### Comparing `ansible_dev_tools-24.4.1/LICENSE` & `ansible_dev_tools-24.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/PKG-INFO` & `ansible_dev_tools-24.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-tools
-Version: 24.4.1
+Version: 24.4.2
 Summary: Ansible Developtment Tools kit bundles all tools needed for content creation and testing.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-tools/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-tools/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-tools
```

### Comparing `ansible_dev_tools-24.4.1/README.md` & `ansible_dev_tools-24.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/cspell.config.yaml` & `ansible_dev_tools-24.4.2/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/contributor-guide.md` & `ansible_dev_tools-24.4.2/docs/contributor-guide.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/index.md` & `ansible_dev_tools-24.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/installation.md` & `ansible_dev_tools-24.4.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/media/ansible-lint.mp4` & `ansible_dev_tools-24.4.2/docs/media/ansible-lint.mp4`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/media/ansible-navigator-run.mp4` & `ansible_dev_tools-24.4.2/docs/media/ansible-navigator-run.mp4`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/media/create-collection.mp4` & `ansible_dev_tools-24.4.2/docs/media/create-collection.mp4`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/user-guide/building-collection.md` & `ansible_dev_tools-24.4.2/docs/user-guide/building-collection.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/user-guide/ci-setup.md` & `ansible_dev_tools-24.4.2/docs/user-guide/ci-setup.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/user-guide/content-best-practices.md` & `ansible_dev_tools-24.4.2/docs/user-guide/content-best-practices.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/user-guide/content-release.md` & `ansible_dev_tools-24.4.2/docs/user-guide/content-release.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/user-guide/images/ci.png` & `ansible_dev_tools-24.4.2/docs/user-guide/images/ci.png`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/user-guide/images/release.png` & `ansible_dev_tools-24.4.2/docs/user-guide/images/release.png`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/user-guide/index.md` & `ansible_dev_tools-24.4.2/docs/user-guide/index.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/docs/user-guide/testing.md` & `ansible_dev_tools-24.4.2/docs/user-guide/testing.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/mkdocs.yml` & `ansible_dev_tools-24.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/pyproject.toml` & `ansible_dev_tools-24.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 [tool.mypy]
 files = ["src", "tests"]
 strict = true
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
-module = ["gunicorn.*", "openapi_core.*", "ansible_creator.*"]
+module = ["gunicorn.*", "openapi_core.*"]
 
 [tool.pydoclint]
 allow-init-docstring = true
 arg-type-hints-in-docstring = false
 check-return-types = false
 style = 'google'
```

### Comparing `ansible_dev_tools-24.4.1/src/ansible_dev_tools/arg_parser.py` & `ansible_dev_tools-24.4.2/src/ansible_dev_tools/arg_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/src/ansible_dev_tools/cli.py` & `ansible_dev_tools-24.4.2/src/ansible_dev_tools/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/creator.py` & `ansible_dev_tools-24.4.2/src/ansible_dev_tools/resources/server/creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,16 +92,15 @@
 
         return validate_response(
             request=request,
             response=response,
         )
 
 
-# TO-DO: remove type ignore after creator is released with py.typed
-class CreatorOutput(Output):  # type: ignore[misc]
+class CreatorOutput(Output):
     """The creator output."""
 
     def __init__(self: CreatorOutput, log_file: str) -> None:
         """
         Initialize the creator output.
 
         Convenience class to consistently define output with a changing temporary directory.
```

### Comparing `ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/data/openapi.yaml` & `ansible_dev_tools-24.4.2/src/ansible_dev_tools/resources/server/data/openapi.yaml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/src/ansible_dev_tools/server_utils.py` & `ansible_dev_tools-24.4.2/src/ansible_dev_tools/server_utils.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/src/ansible_dev_tools/subcommands/server.py` & `ansible_dev_tools-24.4.2/src/ansible_dev_tools/subcommands/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,14 @@
             port: The port on which the server would run.
             debug: Enable or disable debug logging.
         """
         self.port: str = port
         self.debug: bool = debug
 
         settings.configure(
-            DEBUG=self.debug,
             SECRET_KEY=os.environ.get("SECRET_KEY", os.urandom(32)),
             ALLOWED_HOSTS=[
                 "*",
             ],
             ROOT_URLCONF=__name__,
             MIDDLEWARE_CLASSES=(
                 "django.middleware.common.CommonMiddleware",
@@ -87,8 +86,12 @@
         self.application = get_wsgi_application()
 
     def run(self: Server) -> None:
         """Start the server."""
         options = {
             "bind": f"0.0.0.0:{self.port}",
         }
+        if self.debug:
+            # set log level to debug and write access logs to stdout
+            options.update({"loglevel": "debug", "accesslog": "-"})
+
         AdtServerApp(self.application, options).run()
```

### Comparing `ansible_dev_tools-24.4.1/src/ansible_dev_tools/utils.py` & `ansible_dev_tools-24.4.2/src/ansible_dev_tools/utils.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/src/ansible_dev_tools/version_builder.py` & `ansible_dev_tools-24.4.2/src/ansible_dev_tools/version_builder.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/PKG-INFO` & `ansible_dev_tools-24.4.2/src/ansible_dev_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-tools
-Version: 24.4.1
+Version: 24.4.2
 Summary: Ansible Developtment Tools kit bundles all tools needed for content creation and testing.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-tools/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-tools/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-tools
```

### Comparing `ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/SOURCES.txt` & `ansible_dev_tools-24.4.2/src/ansible_dev_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/tests/integration/conftest.py` & `ansible_dev_tools-24.4.2/tests/integration/conftest.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,11 +10,13 @@
 import pytest
 
 
 @pytest.fixture(scope="session")
 def dev_tools_server() -> Generator[str, None, None]:
     """Run the server."""
     bin_path = Path(sys.executable).parent / "adt"
-    with subprocess.Popen([bin_path, "server", "-p", "8000"]) as proc:  # noqa: S603
+    with subprocess.Popen(
+        [bin_path, "server", "-p", "8000", "--debug"],  # noqa: S603
+    ) as proc:
         time.sleep(1)  # allow the server to start
         yield "http://localhost:8000"
         proc.terminate()
```

### Comparing `ansible_dev_tools-24.4.1/tests/integration/test_cli.py` & `ansible_dev_tools-24.4.2/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/tests/integration/test_server_creator.py` & `ansible_dev_tools-24.4.2/tests/integration/test_server_creator.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.1/tox.ini` & `ansible_dev_tools-24.4.2/tox.ini`

 * *Files identical despite different names*

