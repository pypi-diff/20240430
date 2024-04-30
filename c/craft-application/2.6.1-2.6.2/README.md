# Comparing `tmp/craft_application-2.6.1.tar.gz` & `tmp/craft_application-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft_application-2.6.1.tar", last modified: Mon Apr 29 19:43:26 2024, max compression
+gzip compressed data, was "craft_application-2.6.2.tar", last modified: Tue Apr 30 12:57:14 2024, max compression
```

## Comparing `craft_application-2.6.1.tar` & `craft_application-2.6.2.tar`

### file list

```diff
@@ -1,216 +1,217 @@
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.146244 craft_application-2.6.1/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      723 2023-09-29 14:32:21.000000 craft_application-2.6.1/.editorconfig
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.130244 craft_application-2.6.1/.github/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      518 2024-02-15 23:03:01.000000 craft_application-2.6.1/.github/.jira_sync_config.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.130244 craft_application-2.6.1/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1386 2023-09-29 14:32:21.000000 craft_application-2.6.1/.github/ISSUE_TEMPLATE/bug.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      389 2023-09-29 14:32:21.000000 craft_application-2.6.1/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      788 2023-09-29 14:32:21.000000 craft_application-2.6.1/.github/ISSUE_TEMPLATE/task.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft_application-2.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft_application-2.6.1/.github/release-drafter.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft_application-2.6.1/.github/release-drafter.yml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4699 2024-03-19 19:28:11.000000 craft_application-2.6.1/.github/renovate.json5
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.130244 craft_application-2.6.1/.github/workflows/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft_application-2.6.1/.github/workflows/cla-check.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      919 2024-02-15 23:03:01.000000 craft_application-2.6.1/.github/workflows/docs.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      346 2024-02-15 23:03:01.000000 craft_application-2.6.1/.github/workflows/release-drafter.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4541 2024-02-22 17:50:51.000000 craft_application-2.6.1/.github/workflows/tests.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1949 2023-09-29 14:32:21.000000 craft_application-2.6.1/.gitignore
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      921 2023-09-29 14:32:21.000000 craft_application-2.6.1/.pre-commit-config.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      395 2023-11-10 10:29:35.000000 craft_application-2.6.1/.readthedocs.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      188 2023-09-29 14:32:21.000000 craft_application-2.6.1/.yamllint.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4393 2024-03-12 17:53:13.000000 craft_application-2.6.1/HACKING.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7652 2023-09-29 14:32:21.000000 craft_application-2.6.1/LICENSE
--rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-04-29 19:43:26.146244 craft_application-2.6.1/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      552 2023-09-29 14:32:21.000000 craft_application-2.6.1/README.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.130244 craft_application-2.6.1/craft_application/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1522 2024-03-28 20:33:36.000000 craft_application-2.6.1/craft_application/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      411 2024-04-29 19:43:26.000000 craft_application-2.6.1/craft_application/_version.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    29609 2024-04-29 19:42:20.000000 craft_application-2.6.1/craft_application/application.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/craft_application/commands/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1163 2023-12-06 11:10:45.000000 craft_application-2.6.1/craft_application/commands/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7234 2024-03-12 17:53:13.000000 craft_application-2.6.1/craft_application/commands/base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    12723 2024-03-12 17:53:13.000000 craft_application-2.6.1/craft_application/commands/lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1608 2023-09-29 14:32:21.000000 craft_application-2.6.1/craft_application/commands/other.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7040 2024-03-20 22:10:47.000000 craft_application-2.6.1/craft_application/errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4048 2024-04-29 19:42:27.000000 craft_application-2.6.1/craft_application/grammar.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/craft_application/launchpad/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1135 2024-02-15 23:03:01.000000 craft_application-2.6.1/craft_application/launchpad/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1000 2024-02-15 23:03:01.000000 craft_application-2.6.1/craft_application/launchpad/errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     8564 2024-02-26 17:15:25.000000 craft_application-2.6.1/craft_application/launchpad/launchpad.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/craft_application/launchpad/models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      621 2024-02-26 17:15:16.000000 craft_application-2.6.1/craft_application/launchpad/models/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6820 2024-02-26 17:15:16.000000 craft_application-2.6.1/craft_application/launchpad/models/base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4927 2024-02-26 17:15:25.000000 craft_application-2.6.1/craft_application/launchpad/models/build.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5292 2024-02-26 17:15:16.000000 craft_application-2.6.1/craft_application/launchpad/models/code.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2236 2024-02-26 17:15:16.000000 craft_application-2.6.1/craft_application/launchpad/models/distro.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3496 2024-04-03 17:32:43.000000 craft_application-2.6.1/craft_application/launchpad/models/project.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    16303 2024-03-21 21:55:13.000000 craft_application-2.6.1/craft_application/launchpad/models/recipe.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6039 2024-02-22 17:50:51.000000 craft_application-2.6.1/craft_application/launchpad/util.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/craft_application/misc/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1637 2024-02-15 23:03:01.000000 craft_application-2.6.1/craft_application/misc/instance_bashrc
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/craft_application/models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1421 2024-04-29 19:42:27.000000 craft_application-2.6.1/craft_application/models/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3725 2024-02-15 23:03:01.000000 craft_application-2.6.1/craft_application/models/base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2935 2024-03-12 17:53:13.000000 craft_application-2.6.1/craft_application/models/constraints.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3462 2024-04-29 19:42:27.000000 craft_application-2.6.1/craft_application/models/grammar.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1175 2023-09-29 14:32:21.000000 craft_application-2.6.1/craft_application/models/metadata.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4752 2024-04-29 19:42:27.000000 craft_application-2.6.1/craft_application/models/project.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.1/craft_application/py.typed
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/craft_application/remote/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1337 2024-03-12 17:53:13.000000 craft_application-2.6.1/craft_application/remote/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2329 2024-02-22 17:50:51.000000 craft_application-2.6.1/craft_application/remote/errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    11974 2024-04-16 16:52:34.000000 craft_application-2.6.1/craft_application/remote/git.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4206 2024-04-29 19:42:27.000000 craft_application-2.6.1/craft_application/remote/utils.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2070 2024-02-15 23:03:01.000000 craft_application-2.6.1/craft_application/remote/worktree.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6731 2024-02-22 17:50:51.000000 craft_application-2.6.1/craft_application/secrets.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/craft_application/services/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1444 2024-02-15 23:03:01.000000 craft_application-2.6.1/craft_application/services/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2106 2024-02-15 23:03:01.000000 craft_application-2.6.1/craft_application/services/base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    16549 2024-04-29 17:11:30.000000 craft_application-2.6.1/craft_application/services/lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3128 2024-03-19 19:28:11.000000 craft_application-2.6.1/craft_application/services/package.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    12545 2024-04-29 19:42:27.000000 craft_application-2.6.1/craft_application/services/provider.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    14846 2024-04-16 16:52:34.000000 craft_application-2.6.1/craft_application/services/remotebuild.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4323 2024-02-15 23:03:01.000000 craft_application-2.6.1/craft_application/services/request.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4273 2024-02-15 23:03:01.000000 craft_application-2.6.1/craft_application/services/service_factory.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/craft_application/util/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1701 2024-03-12 17:53:13.000000 craft_application-2.6.1/craft_application/util/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2465 2024-02-22 17:50:51.000000 craft_application-2.6.1/craft_application/util/callbacks.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4170 2024-02-22 17:50:51.000000 craft_application-2.6.1/craft_application/util/error_formatting.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      950 2023-12-06 11:10:45.000000 craft_application-2.6.1/craft_application/util/logging.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1470 2024-02-15 23:03:01.000000 craft_application-2.6.1/craft_application/util/paths.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2494 2024-02-28 16:38:56.000000 craft_application-2.6.1/craft_application/util/platforms.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2507 2024-04-29 17:11:30.000000 craft_application-2.6.1/craft_application/util/repositories.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4110 2024-02-26 17:15:25.000000 craft_application-2.6.1/craft_application/util/snap_config.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2241 2024-03-12 17:53:13.000000 craft_application-2.6.1/craft_application/util/string.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4930 2024-03-19 19:28:11.000000 craft_application-2.6.1/craft_application/util/yaml.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.142244 craft_application-2.6.1/craft_application.egg-info/
--rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-04-29 19:43:26.000000 craft_application-2.6.1/craft_application.egg-info/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6026 2024-04-29 19:43:26.000000 craft_application-2.6.1/craft_application.egg-info/SOURCES.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2024-04-29 19:43:26.000000 craft_application-2.6.1/craft_application.egg-info/dependency_links.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      871 2024-04-29 19:43:26.000000 craft_application-2.6.1/craft_application.egg-info/requires.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-04-29 19:43:26.000000 craft_application-2.6.1/craft_application.egg-info/top_level.txt
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/docs/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.126244 craft_application-2.6.1/docs/_static/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/docs/_static/css/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      481 2024-04-29 19:42:27.000000 craft_application-2.6.1/docs/_static/css/custom.css
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1684 2024-04-29 19:42:27.000000 craft_application-2.6.1/docs/conf.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/docs/explanation/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       72 2023-09-29 14:32:21.000000 craft_application-2.6.1/docs/explanation/index.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/docs/howto/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       70 2023-09-29 14:32:21.000000 craft_application-2.6.1/docs/howto/index.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1201 2023-09-29 14:32:21.000000 craft_application-2.6.1/docs/index.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/docs/reference/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      142 2023-09-29 14:32:21.000000 craft_application-2.6.1/docs/reference/index.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/docs/tutorials/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      238 2023-09-29 14:32:21.000000 craft_application-2.6.1/docs/tutorials/index.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    10638 2024-04-29 19:42:27.000000 craft_application-2.6.1/pyproject.toml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2024-04-29 19:43:26.146244 craft_application-2.6.1/setup.cfg
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/tests/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     9416 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/conftest.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/tests/integration/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/integration/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3149 2024-04-03 17:32:43.000000 craft_application-2.6.1/tests/integration/conftest.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.130244 craft_application-2.6.1/tests/integration/data/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/tests/integration/data/build-secrets/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.134244 craft_application-2.6.1/tests/integration/data/build-secrets/secret-source-folder/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       14 2023-10-19 21:00:44.000000 craft_application-2.6.1/tests/integration/data/build-secrets/secret-source-folder/source-file.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      442 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/integration/data/build-secrets/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.130244 craft_application-2.6.1/tests/integration/data/invalid_projects/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/integration/data/invalid_projects/build-error/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      177 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/integration/data/invalid_projects/build-error/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.130244 craft_application-2.6.1/tests/integration/data/valid_projects/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/integration/data/valid_projects/adoption/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.6.1/tests/integration/data/valid_projects/adoption/stderr
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      209 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/integration/data/valid_projects/adoption/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/integration/data/valid_projects/basic/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.6.1/tests/integration/data/valid_projects/basic/stderr
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      114 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/integration/data/valid_projects/basic/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/integration/data/valid_projects/environment/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.6.1/tests/integration/data/valid_projects/environment/stderr
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      483 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/integration/data/valid_projects/environment/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/integration/data/valid_projects/grammar/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.130244 craft_application-2.6.1/tests/integration/data/valid_projects/grammar/src/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft_application-2.6.1/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/hello.txt
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft_application-2.6.1/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/hello.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-03-20 22:10:47.000000 craft_application-2.6.1/tests/integration/data/valid_projects/grammar/stderr
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      521 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/integration/data/valid_projects/grammar/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/integration/launchpad/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.6.1/tests/integration/launchpad/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1021 2024-02-26 17:15:16.000000 craft_application-2.6.1/tests/integration/launchpad/conftest.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1709 2024-04-29 17:11:30.000000 craft_application-2.6.1/tests/integration/launchpad/test_anonymous_access.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/integration/services/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/integration/services/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5475 2024-02-28 16:38:56.000000 craft_application-2.6.1/tests/integration/services/test_lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4287 2024-03-12 17:53:13.000000 craft_application-2.6.1/tests/integration/services/test_provider.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1886 2024-04-03 17:32:43.000000 craft_application-2.6.1/tests/integration/services/test_remotebuild.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3445 2024-02-15 23:03:01.000000 craft_application-2.6.1/tests/integration/services/test_request.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1909 2024-02-28 16:38:56.000000 craft_application-2.6.1/tests/integration/services/test_service_factory.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    13467 2024-03-21 21:55:13.000000 craft_application-2.6.1/tests/integration/test_application.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2201 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/integration/test_version.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/unit/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/unit/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/unit/commands/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/unit/commands/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6705 2023-12-06 11:10:45.000000 craft_application-2.6.1/tests/unit/commands/test_base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    17375 2024-03-12 17:53:13.000000 craft_application-2.6.1/tests/unit/commands/test_lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1363 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/unit/commands/test_other.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1673 2024-02-15 23:03:01.000000 craft_application-2.6.1/tests/unit/conftest.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/unit/launchpad/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.6.1/tests/unit/launchpad/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1194 2024-02-26 17:15:16.000000 craft_application-2.6.1/tests/unit/launchpad/conftest.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/unit/launchpad/models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.6.1/tests/unit/launchpad/models/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5159 2024-02-26 17:15:16.000000 craft_application-2.6.1/tests/unit/launchpad/models/test_base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2562 2024-02-26 17:15:16.000000 craft_application-2.6.1/tests/unit/launchpad/models/test_code.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     9305 2024-03-21 21:55:13.000000 craft_application-2.6.1/tests/unit/launchpad/test_launchpad.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3500 2024-02-28 16:38:56.000000 craft_application-2.6.1/tests/unit/launchpad/test_util.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/unit/models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/unit/models/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/unit/models/project_models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       68 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/unit/models/project_models/basic_project.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      436 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/unit/models/project_models/full_project.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       24 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/unit/models/project_models/invalid_project.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4489 2024-02-15 23:03:01.000000 craft_application-2.6.1/tests/unit/models/test_constraints.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    10302 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/unit/models/test_project.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.138244 craft_application-2.6.1/tests/unit/remote/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.6.1/tests/unit/remote/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      855 2024-02-15 23:03:01.000000 craft_application-2.6.1/tests/unit/remote/conftest.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2116 2024-02-15 23:03:01.000000 craft_application-2.6.1/tests/unit/remote/test_errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    18388 2024-03-19 19:28:11.000000 craft_application-2.6.1/tests/unit/remote/test_git.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5855 2024-03-12 17:53:13.000000 craft_application-2.6.1/tests/unit/remote/test_utils.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3034 2024-02-15 23:03:01.000000 craft_application-2.6.1/tests/unit/remote/test_worktree.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.142244 craft_application-2.6.1/tests/unit/services/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/unit/services/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3946 2024-04-16 16:52:34.000000 craft_application-2.6.1/tests/unit/services/conftest.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    21815 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/unit/services/test_lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3413 2024-03-12 17:53:13.000000 craft_application-2.6.1/tests/unit/services/test_package.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    19346 2024-04-02 11:30:59.000000 craft_application-2.6.1/tests/unit/services/test_provider.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    11829 2024-04-16 16:52:34.000000 craft_application-2.6.1/tests/unit/services/test_remotebuild.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3867 2024-04-29 17:11:30.000000 craft_application-2.6.1/tests/unit/services/test_repositories.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4000 2024-02-15 23:03:01.000000 craft_application-2.6.1/tests/unit/services/test_request.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5005 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/unit/services/test_service_factory.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    55000 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/unit/test_application.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2968 2024-02-15 23:03:01.000000 craft_application-2.6.1/tests/unit/test_errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7670 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/unit/test_grammar.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       57 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/unit/test_nothing.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5444 2023-10-19 21:00:44.000000 craft_application-2.6.1/tests/unit/test_secrets.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.142244 craft_application-2.6.1/tests/unit/util/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/unit/util/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.142244 craft_application-2.6.1/tests/unit/util/invalid_yaml/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      156 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/unit/util/invalid_yaml/_README
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       46 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/unit/util/invalid_yaml/duplicate_second_level.yaml-invalid
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       40 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/unit/util/invalid_yaml/duplicate_top_level.yaml-invalid
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       30 2024-04-29 19:42:27.000000 craft_application-2.6.1/tests/unit/util/invalid_yaml/unhashable.yaml-invalid
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3189 2023-12-07 17:42:39.000000 craft_application-2.6.1/tests/unit/util/test_error_formatting.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      603 2023-12-06 11:10:45.000000 craft_application-2.6.1/tests/unit/util/test_logging.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1573 2024-02-15 23:03:01.000000 craft_application-2.6.1/tests/unit/util/test_paths.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5221 2024-02-26 17:15:25.000000 craft_application-2.6.1/tests/unit/util/test_snap_config.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3383 2024-03-12 17:53:13.000000 craft_application-2.6.1/tests/unit/util/test_string.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2992 2024-03-19 19:28:11.000000 craft_application-2.6.1/tests/unit/util/test_yaml.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-29 19:43:26.142244 craft_application-2.6.1/tests/unit/util/valid_yaml/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.1/tests/unit/util/valid_yaml/empty.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4900 2024-04-29 19:42:27.000000 craft_application-2.6.1/tox.ini
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.263649 craft_application-2.6.2/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      723 2023-09-29 14:32:21.000000 craft_application-2.6.2/.editorconfig
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.239649 craft_application-2.6.2/.github/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      518 2024-02-15 23:03:01.000000 craft_application-2.6.2/.github/.jira_sync_config.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.239649 craft_application-2.6.2/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1386 2023-09-29 14:32:21.000000 craft_application-2.6.2/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      389 2023-09-29 14:32:21.000000 craft_application-2.6.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      788 2023-09-29 14:32:21.000000 craft_application-2.6.2/.github/ISSUE_TEMPLATE/task.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft_application-2.6.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft_application-2.6.2/.github/release-drafter.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft_application-2.6.2/.github/release-drafter.yml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4699 2024-03-19 19:28:11.000000 craft_application-2.6.2/.github/renovate.json5
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.239649 craft_application-2.6.2/.github/workflows/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft_application-2.6.2/.github/workflows/cla-check.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      919 2024-02-15 23:03:01.000000 craft_application-2.6.2/.github/workflows/docs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      346 2024-02-15 23:03:01.000000 craft_application-2.6.2/.github/workflows/release-drafter.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4541 2024-02-22 17:50:51.000000 craft_application-2.6.2/.github/workflows/tests.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1949 2023-09-29 14:32:21.000000 craft_application-2.6.2/.gitignore
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      921 2023-09-29 14:32:21.000000 craft_application-2.6.2/.pre-commit-config.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      395 2023-11-10 10:29:35.000000 craft_application-2.6.2/.readthedocs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      188 2023-09-29 14:32:21.000000 craft_application-2.6.2/.yamllint.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4393 2024-03-12 17:53:13.000000 craft_application-2.6.2/HACKING.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7652 2023-09-29 14:32:21.000000 craft_application-2.6.2/LICENSE
+-rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-04-30 12:57:14.263649 craft_application-2.6.2/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      552 2023-09-29 14:32:21.000000 craft_application-2.6.2/README.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.243649 craft_application-2.6.2/craft_application/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1522 2024-03-28 20:33:36.000000 craft_application-2.6.2/craft_application/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      411 2024-04-30 12:57:14.000000 craft_application-2.6.2/craft_application/_version.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    29609 2024-04-29 19:42:20.000000 craft_application-2.6.2/craft_application/application.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.243649 craft_application-2.6.2/craft_application/commands/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1163 2023-12-06 11:10:45.000000 craft_application-2.6.2/craft_application/commands/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7234 2024-03-12 17:53:13.000000 craft_application-2.6.2/craft_application/commands/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    12723 2024-03-12 17:53:13.000000 craft_application-2.6.2/craft_application/commands/lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1608 2023-09-29 14:32:21.000000 craft_application-2.6.2/craft_application/commands/other.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7040 2024-03-20 22:10:47.000000 craft_application-2.6.2/craft_application/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4504 2024-04-30 12:51:44.000000 craft_application-2.6.2/craft_application/grammar.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.243649 craft_application-2.6.2/craft_application/launchpad/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1135 2024-02-15 23:03:01.000000 craft_application-2.6.2/craft_application/launchpad/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1000 2024-02-15 23:03:01.000000 craft_application-2.6.2/craft_application/launchpad/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     8564 2024-02-26 17:15:25.000000 craft_application-2.6.2/craft_application/launchpad/launchpad.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.243649 craft_application-2.6.2/craft_application/launchpad/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      621 2024-02-26 17:15:16.000000 craft_application-2.6.2/craft_application/launchpad/models/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6820 2024-02-26 17:15:16.000000 craft_application-2.6.2/craft_application/launchpad/models/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4927 2024-02-26 17:15:25.000000 craft_application-2.6.2/craft_application/launchpad/models/build.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5292 2024-02-26 17:15:16.000000 craft_application-2.6.2/craft_application/launchpad/models/code.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2236 2024-02-26 17:15:16.000000 craft_application-2.6.2/craft_application/launchpad/models/distro.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3496 2024-04-03 17:32:43.000000 craft_application-2.6.2/craft_application/launchpad/models/project.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    16303 2024-03-21 21:55:13.000000 craft_application-2.6.2/craft_application/launchpad/models/recipe.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6039 2024-02-22 17:50:51.000000 craft_application-2.6.2/craft_application/launchpad/util.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.243649 craft_application-2.6.2/craft_application/misc/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1637 2024-02-15 23:03:01.000000 craft_application-2.6.2/craft_application/misc/instance_bashrc
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.247649 craft_application-2.6.2/craft_application/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1506 2024-04-30 12:51:44.000000 craft_application-2.6.2/craft_application/models/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3725 2024-02-15 23:03:01.000000 craft_application-2.6.2/craft_application/models/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2935 2024-03-12 17:53:13.000000 craft_application-2.6.2/craft_application/models/constraints.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3823 2024-04-30 12:51:44.000000 craft_application-2.6.2/craft_application/models/grammar.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1175 2023-09-29 14:32:21.000000 craft_application-2.6.2/craft_application/models/metadata.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4752 2024-04-29 19:42:27.000000 craft_application-2.6.2/craft_application/models/project.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.2/craft_application/py.typed
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.247649 craft_application-2.6.2/craft_application/remote/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1337 2024-03-12 17:53:13.000000 craft_application-2.6.2/craft_application/remote/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2329 2024-02-22 17:50:51.000000 craft_application-2.6.2/craft_application/remote/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    11974 2024-04-16 16:52:34.000000 craft_application-2.6.2/craft_application/remote/git.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4206 2024-04-29 19:42:27.000000 craft_application-2.6.2/craft_application/remote/utils.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2070 2024-02-15 23:03:01.000000 craft_application-2.6.2/craft_application/remote/worktree.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6731 2024-02-22 17:50:51.000000 craft_application-2.6.2/craft_application/secrets.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.247649 craft_application-2.6.2/craft_application/services/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1444 2024-02-15 23:03:01.000000 craft_application-2.6.2/craft_application/services/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2106 2024-02-15 23:03:01.000000 craft_application-2.6.2/craft_application/services/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    16549 2024-04-29 17:11:30.000000 craft_application-2.6.2/craft_application/services/lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3128 2024-03-19 19:28:11.000000 craft_application-2.6.2/craft_application/services/package.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    12545 2024-04-29 19:42:27.000000 craft_application-2.6.2/craft_application/services/provider.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    14846 2024-04-16 16:52:34.000000 craft_application-2.6.2/craft_application/services/remotebuild.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4323 2024-02-15 23:03:01.000000 craft_application-2.6.2/craft_application/services/request.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4273 2024-02-15 23:03:01.000000 craft_application-2.6.2/craft_application/services/service_factory.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.247649 craft_application-2.6.2/craft_application/util/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1701 2024-03-12 17:53:13.000000 craft_application-2.6.2/craft_application/util/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2465 2024-02-22 17:50:51.000000 craft_application-2.6.2/craft_application/util/callbacks.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4170 2024-02-22 17:50:51.000000 craft_application-2.6.2/craft_application/util/error_formatting.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      950 2023-12-06 11:10:45.000000 craft_application-2.6.2/craft_application/util/logging.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1470 2024-02-15 23:03:01.000000 craft_application-2.6.2/craft_application/util/paths.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2494 2024-02-28 16:38:56.000000 craft_application-2.6.2/craft_application/util/platforms.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2507 2024-04-29 17:11:30.000000 craft_application-2.6.2/craft_application/util/repositories.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4110 2024-02-26 17:15:25.000000 craft_application-2.6.2/craft_application/util/snap_config.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2241 2024-03-12 17:53:13.000000 craft_application-2.6.2/craft_application/util/string.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4930 2024-03-19 19:28:11.000000 craft_application-2.6.2/craft_application/util/yaml.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.263649 craft_application-2.6.2/craft_application.egg-info/
+-rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-04-30 12:57:14.000000 craft_application-2.6.2/craft_application.egg-info/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6060 2024-04-30 12:57:14.000000 craft_application-2.6.2/craft_application.egg-info/SOURCES.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2024-04-30 12:57:14.000000 craft_application-2.6.2/craft_application.egg-info/dependency_links.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      871 2024-04-30 12:57:14.000000 craft_application-2.6.2/craft_application.egg-info/requires.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-04-30 12:57:14.000000 craft_application-2.6.2/craft_application.egg-info/top_level.txt
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/docs/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.235649 craft_application-2.6.2/docs/_static/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/docs/_static/css/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      481 2024-04-29 19:42:27.000000 craft_application-2.6.2/docs/_static/css/custom.css
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1684 2024-04-29 19:42:27.000000 craft_application-2.6.2/docs/conf.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/docs/explanation/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       72 2023-09-29 14:32:21.000000 craft_application-2.6.2/docs/explanation/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/docs/howto/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       70 2023-09-29 14:32:21.000000 craft_application-2.6.2/docs/howto/index.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1201 2023-09-29 14:32:21.000000 craft_application-2.6.2/docs/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/docs/reference/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      142 2023-09-29 14:32:21.000000 craft_application-2.6.2/docs/reference/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/docs/tutorials/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      238 2023-09-29 14:32:21.000000 craft_application-2.6.2/docs/tutorials/index.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10638 2024-04-29 19:42:27.000000 craft_application-2.6.2/pyproject.toml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2024-04-30 12:57:14.263649 craft_application-2.6.2/setup.cfg
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/tests/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     9416 2024-04-29 19:42:27.000000 craft_application-2.6.2/tests/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/tests/integration/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/integration/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3149 2024-04-03 17:32:43.000000 craft_application-2.6.2/tests/integration/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.235649 craft_application-2.6.2/tests/integration/data/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/tests/integration/data/build-secrets/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/tests/integration/data/build-secrets/secret-source-folder/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       14 2023-10-19 21:00:44.000000 craft_application-2.6.2/tests/integration/data/build-secrets/secret-source-folder/source-file.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      442 2024-04-29 19:42:27.000000 craft_application-2.6.2/tests/integration/data/build-secrets/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.235649 craft_application-2.6.2/tests/integration/data/invalid_projects/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/tests/integration/data/invalid_projects/build-error/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      177 2024-04-29 19:42:27.000000 craft_application-2.6.2/tests/integration/data/invalid_projects/build-error/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.235649 craft_application-2.6.2/tests/integration/data/valid_projects/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/tests/integration/data/valid_projects/adoption/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.6.2/tests/integration/data/valid_projects/adoption/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      209 2024-04-29 19:42:27.000000 craft_application-2.6.2/tests/integration/data/valid_projects/adoption/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/tests/integration/data/valid_projects/basic/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.6.2/tests/integration/data/valid_projects/basic/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      114 2024-04-29 19:42:27.000000 craft_application-2.6.2/tests/integration/data/valid_projects/basic/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/tests/integration/data/valid_projects/environment/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.6.2/tests/integration/data/valid_projects/environment/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      483 2024-04-29 19:42:27.000000 craft_application-2.6.2/tests/integration/data/valid_projects/environment/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/tests/integration/data/valid_projects/grammar/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.235649 craft_application-2.6.2/tests/integration/data/valid_projects/grammar/src/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft_application-2.6.2/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/hello.txt
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft_application-2.6.2/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/hello.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-03-20 22:10:47.000000 craft_application-2.6.2/tests/integration/data/valid_projects/grammar/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      521 2024-04-29 19:42:27.000000 craft_application-2.6.2/tests/integration/data/valid_projects/grammar/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.251649 craft_application-2.6.2/tests/integration/launchpad/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.6.2/tests/integration/launchpad/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1021 2024-02-26 17:15:16.000000 craft_application-2.6.2/tests/integration/launchpad/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1709 2024-04-29 17:11:30.000000 craft_application-2.6.2/tests/integration/launchpad/test_anonymous_access.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.255649 craft_application-2.6.2/tests/integration/services/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/integration/services/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5475 2024-02-28 16:38:56.000000 craft_application-2.6.2/tests/integration/services/test_lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4287 2024-03-12 17:53:13.000000 craft_application-2.6.2/tests/integration/services/test_provider.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1886 2024-04-03 17:32:43.000000 craft_application-2.6.2/tests/integration/services/test_remotebuild.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3445 2024-02-15 23:03:01.000000 craft_application-2.6.2/tests/integration/services/test_request.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1909 2024-02-28 16:38:56.000000 craft_application-2.6.2/tests/integration/services/test_service_factory.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    13467 2024-03-21 21:55:13.000000 craft_application-2.6.2/tests/integration/test_application.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2201 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/integration/test_version.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.255649 craft_application-2.6.2/tests/unit/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/unit/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.255649 craft_application-2.6.2/tests/unit/commands/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/unit/commands/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6705 2023-12-06 11:10:45.000000 craft_application-2.6.2/tests/unit/commands/test_base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    17375 2024-03-12 17:53:13.000000 craft_application-2.6.2/tests/unit/commands/test_lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1363 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/unit/commands/test_other.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1673 2024-02-15 23:03:01.000000 craft_application-2.6.2/tests/unit/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.255649 craft_application-2.6.2/tests/unit/launchpad/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.6.2/tests/unit/launchpad/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1194 2024-02-26 17:15:16.000000 craft_application-2.6.2/tests/unit/launchpad/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.255649 craft_application-2.6.2/tests/unit/launchpad/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.6.2/tests/unit/launchpad/models/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5159 2024-02-26 17:15:16.000000 craft_application-2.6.2/tests/unit/launchpad/models/test_base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2562 2024-02-26 17:15:16.000000 craft_application-2.6.2/tests/unit/launchpad/models/test_code.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     9305 2024-03-21 21:55:13.000000 craft_application-2.6.2/tests/unit/launchpad/test_launchpad.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3500 2024-02-28 16:38:56.000000 craft_application-2.6.2/tests/unit/launchpad/test_util.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.259649 craft_application-2.6.2/tests/unit/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/unit/models/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.259649 craft_application-2.6.2/tests/unit/models/project_models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       68 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/unit/models/project_models/basic_project.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      436 2024-04-29 19:42:27.000000 craft_application-2.6.2/tests/unit/models/project_models/full_project.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       24 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/unit/models/project_models/invalid_project.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4489 2024-02-15 23:03:01.000000 craft_application-2.6.2/tests/unit/models/test_constraints.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1673 2024-04-30 12:51:44.000000 craft_application-2.6.2/tests/unit/models/test_grammar.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10302 2024-04-29 19:42:27.000000 craft_application-2.6.2/tests/unit/models/test_project.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.259649 craft_application-2.6.2/tests/unit/remote/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.6.2/tests/unit/remote/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      855 2024-02-15 23:03:01.000000 craft_application-2.6.2/tests/unit/remote/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2116 2024-02-15 23:03:01.000000 craft_application-2.6.2/tests/unit/remote/test_errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    18388 2024-03-19 19:28:11.000000 craft_application-2.6.2/tests/unit/remote/test_git.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5855 2024-03-12 17:53:13.000000 craft_application-2.6.2/tests/unit/remote/test_utils.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3034 2024-02-15 23:03:01.000000 craft_application-2.6.2/tests/unit/remote/test_worktree.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.259649 craft_application-2.6.2/tests/unit/services/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/unit/services/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3946 2024-04-16 16:52:34.000000 craft_application-2.6.2/tests/unit/services/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    21815 2024-04-29 19:42:27.000000 craft_application-2.6.2/tests/unit/services/test_lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3413 2024-03-12 17:53:13.000000 craft_application-2.6.2/tests/unit/services/test_package.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    19346 2024-04-02 11:30:59.000000 craft_application-2.6.2/tests/unit/services/test_provider.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    11829 2024-04-16 16:52:34.000000 craft_application-2.6.2/tests/unit/services/test_remotebuild.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3867 2024-04-29 17:11:30.000000 craft_application-2.6.2/tests/unit/services/test_repositories.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4000 2024-02-15 23:03:01.000000 craft_application-2.6.2/tests/unit/services/test_request.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5005 2024-04-29 19:42:27.000000 craft_application-2.6.2/tests/unit/services/test_service_factory.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    55309 2024-04-30 12:51:44.000000 craft_application-2.6.2/tests/unit/test_application.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2968 2024-02-15 23:03:01.000000 craft_application-2.6.2/tests/unit/test_errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7670 2024-04-29 19:42:27.000000 craft_application-2.6.2/tests/unit/test_grammar.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       57 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/unit/test_nothing.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5444 2023-10-19 21:00:44.000000 craft_application-2.6.2/tests/unit/test_secrets.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.263649 craft_application-2.6.2/tests/unit/util/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/unit/util/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.263649 craft_application-2.6.2/tests/unit/util/invalid_yaml/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      156 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/unit/util/invalid_yaml/_README
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       46 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/unit/util/invalid_yaml/duplicate_second_level.yaml-invalid
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       40 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/unit/util/invalid_yaml/duplicate_top_level.yaml-invalid
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       30 2024-04-29 19:42:27.000000 craft_application-2.6.2/tests/unit/util/invalid_yaml/unhashable.yaml-invalid
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3189 2023-12-07 17:42:39.000000 craft_application-2.6.2/tests/unit/util/test_error_formatting.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      603 2023-12-06 11:10:45.000000 craft_application-2.6.2/tests/unit/util/test_logging.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1573 2024-02-15 23:03:01.000000 craft_application-2.6.2/tests/unit/util/test_paths.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5221 2024-02-26 17:15:25.000000 craft_application-2.6.2/tests/unit/util/test_snap_config.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3383 2024-03-12 17:53:13.000000 craft_application-2.6.2/tests/unit/util/test_string.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2992 2024-03-19 19:28:11.000000 craft_application-2.6.2/tests/unit/util/test_yaml.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-30 12:57:14.263649 craft_application-2.6.2/tests/unit/util/valid_yaml/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6.2/tests/unit/util/valid_yaml/empty.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4900 2024-04-29 19:42:27.000000 craft_application-2.6.2/tox.ini
```

### Comparing `craft_application-2.6.1/.editorconfig` & `craft_application-2.6.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/.github/.jira_sync_config.yaml` & `craft_application-2.6.2/.github/.jira_sync_config.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/.github/ISSUE_TEMPLATE/bug.yaml` & `craft_application-2.6.2/.github/ISSUE_TEMPLATE/bug.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/.github/ISSUE_TEMPLATE/task.yaml` & `craft_application-2.6.2/.github/ISSUE_TEMPLATE/task.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/.github/renovate.json5` & `craft_application-2.6.2/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/.github/workflows/docs.yaml` & `craft_application-2.6.2/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/.github/workflows/tests.yaml` & `craft_application-2.6.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/.gitignore` & `craft_application-2.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/.pre-commit-config.yaml` & `craft_application-2.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/HACKING.rst` & `craft_application-2.6.2/HACKING.rst`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/LICENSE` & `craft_application-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/PKG-INFO` & `craft_application-2.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-application
-Version: 2.6.1
+Version: 2.6.2
 Summary: A framework for *craft applications.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `craft_application-2.6.1/README.rst` & `craft_application-2.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/__init__.py` & `craft_application-2.6.2/craft_application/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/application.py` & `craft_application-2.6.2/craft_application/application.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/commands/__init__.py` & `craft_application-2.6.2/craft_application/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/commands/base.py` & `craft_application-2.6.2/craft_application/commands/base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/commands/lifecycle.py` & `craft_application-2.6.2/craft_application/commands/lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/commands/other.py` & `craft_application-2.6.2/craft_application/commands/other.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/errors.py` & `craft_application-2.6.2/craft_application/errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/grammar.py` & `craft_application-2.6.2/craft_application/grammar.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from typing import Any, cast
 
 import craft_cli
 from craft_grammar import GrammarProcessor  # type: ignore[import-untyped]
 from craft_grammar.errors import GrammarSyntaxError  # type: ignore[import-untyped]
 
 from craft_application.errors import CraftValidationError
+from craft_application.models import get_grammar_aware_part_keywords
 
 # Values that should return as a single object / list / dict.
 _NON_SCALAR_VALUES = [
     "source-submodules",
     "after",
     "overlay-packages",
     "build-attributes",
@@ -49,24 +50,36 @@
 
 def process_part(
     *, part_yaml_data: dict[str, Any], processor: GrammarProcessor
 ) -> dict[str, Any]:
     """Process grammar for a given part."""
     for key in part_yaml_data:
         unprocessed_grammar = part_yaml_data[key]
-        craft_cli.emit.debug(f"Processing grammar for {key}: {unprocessed_grammar}")
 
+        # ignore non-grammar keywords
+        if key not in get_grammar_aware_part_keywords():
+            craft_cli.emit.debug(
+                f"Not processing grammar for non-grammar enabled keyword {key}"
+            )
+            continue
+
+        craft_cli.emit.debug(f"Processing grammar for {key}: {unprocessed_grammar}")
         # grammar aware models can be strings or list of dicts and strings
         if isinstance(unprocessed_grammar, list):
             # all items in the list must be a dict or a string
             if any(not isinstance(d, dict | str) for d in unprocessed_grammar):  # type: ignore[reportUnknownVariableType]
                 continue
+
             # all keys in the dictionary must be a string
-            if any(not isinstance(key, str) for d in unprocessed_grammar for key in d):  # type: ignore[reportUnknownVariableType]
-                continue
+            for item in unprocessed_grammar:  # type: ignore[reportUnknownVariableType]
+                if isinstance(item, dict) and any(
+                    not isinstance(key, str) for key in item  # type: ignore[reportUnknownVariableType]
+                ):
+                    continue
+
             unprocessed_grammar = cast(list[dict[str, Any] | str], unprocessed_grammar)
         # grammar aware models can be a string
         elif isinstance(unprocessed_grammar, str):
             unprocessed_grammar = [unprocessed_grammar]
         # skip all other data types
         else:
             continue
@@ -74,17 +87,17 @@
         try:
             processed_grammar = processor.process(grammar=unprocessed_grammar)
         except GrammarSyntaxError as e:
             raise CraftValidationError(
                 f"Invalid grammar syntax while processing '{key}' in '{part_yaml_data}': {e}"
             ) from e
 
-        # special cases
-        # scalar values should return as a single object, not in a list.
-        # dict values should return as a dict, not in a list.
+        # special cases:
+        # - scalar values should return as a single object, not in a list.
+        # - dict values should return as a dict, not in a list.
         if key not in _NON_SCALAR_VALUES or key in _DICT_ONLY_VALUES:
             processed_grammar = processed_grammar[0] if processed_grammar else None
 
         part_yaml_data[key] = processed_grammar
 
     return part_yaml_data
```

### Comparing `craft_application-2.6.1/craft_application/launchpad/__init__.py` & `craft_application-2.6.2/craft_application/launchpad/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/launchpad/errors.py` & `craft_application-2.6.2/craft_application/launchpad/errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/launchpad/launchpad.py` & `craft_application-2.6.2/craft_application/launchpad/launchpad.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/launchpad/models/__init__.py` & `craft_application-2.6.2/craft_application/launchpad/models/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/launchpad/models/base.py` & `craft_application-2.6.2/craft_application/launchpad/models/base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/launchpad/models/build.py` & `craft_application-2.6.2/craft_application/launchpad/models/build.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/launchpad/models/code.py` & `craft_application-2.6.2/craft_application/launchpad/models/code.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/launchpad/models/distro.py` & `craft_application-2.6.2/craft_application/launchpad/models/distro.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/launchpad/models/project.py` & `craft_application-2.6.2/craft_application/launchpad/models/project.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/launchpad/models/recipe.py` & `craft_application-2.6.2/craft_application/launchpad/models/recipe.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/launchpad/util.py` & `craft_application-2.6.2/craft_application/launchpad/util.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/misc/instance_bashrc` & `craft_application-2.6.2/craft_application/misc/instance_bashrc`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/models/__init__.py` & `craft_application-2.6.2/craft_application/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,24 +19,28 @@
 from craft_application.models.constraints import (
     ProjectName,
     ProjectTitle,
     SummaryStr,
     UniqueStrList,
     VersionStr,
 )
-from craft_application.models.grammar import GrammarAwareProject
+from craft_application.models.grammar import (
+    GrammarAwareProject,
+    get_grammar_aware_part_keywords,
+)
 from craft_application.models.metadata import BaseMetadata
 from craft_application.models.project import BuildInfo, BuildPlanner, Project
 
 
 __all__ = [
     "BaseMetadata",
     "BuildInfo",
     "CraftBaseConfig",
     "CraftBaseModel",
+    "get_grammar_aware_part_keywords",
     "GrammarAwareProject",
     "Project",
     "BuildPlanner",
     "ProjectName",
     "ProjectTitle",
     "SummaryStr",
     "UniqueStrList",
```

### Comparing `craft_application-2.6.1/craft_application/models/base.py` & `craft_application-2.6.2/craft_application/models/base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/models/constraints.py` & `craft_application-2.6.2/craft_application/models/constraints.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/models/grammar.py` & `craft_application-2.6.2/craft_application/models/grammar.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of craft_application.
 #
-# Copyright 2023 Canonical Ltd.
+# Copyright 2023-2024 Canonical Ltd.
 #
 # This program is free software: you can redistribute it and/or modify it
 # under the terms of the GNU Lesser General Public License version 3, as
 # published by the Free Software Foundation.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranties of MERCHANTABILITY,
@@ -57,27 +57,33 @@
     overlay_packages: GrammarStrList | None
     stage_snaps: GrammarStrList | None
     stage_packages: GrammarStrList | None
     build_snaps: GrammarStrList | None
     build_packages: GrammarStrList | None
     build_environment: GrammarSingleEntryDictList | None
     build_attributes: GrammarStrList | None
-    organize_files: GrammarDict | None
-    overlay_files: GrammarStrList | None
-    stage_files: GrammarStrList | None
-    prime_files: GrammarStrList | None
+    organize_files: GrammarDict | None = pydantic.Field(alias="organize")
+    overlay_files: GrammarStrList | None = pydantic.Field(alias="overlay")
+    stage_files: GrammarStrList | None = pydantic.Field(alias="stage")
+    prime_files: GrammarStrList | None = pydantic.Field(alias="prime")
     override_pull: GrammarStr | None
     overlay_script: GrammarStr | None
     override_build: GrammarStr | None
     override_stage: GrammarStr | None
     override_prime: GrammarStr | None
     permissions: GrammarDictList | None
     parse_info: GrammarStrList | None
 
 
+def get_grammar_aware_part_keywords() -> list[str]:
+    """Return all supported grammar keywords for a part."""
+    keywords: list[str] = [item.alias for item in _GrammarAwarePart.__fields__.values()]
+    return keywords
+
+
 class GrammarAwareProject(_GrammarAwareModel):
     """Project definition containing grammar-aware components."""
 
     parts: "dict[str, _GrammarAwarePart]"
 
     @pydantic.root_validator(  # pyright: ignore[reportUntypedFunctionDecorator,reportUnknownMemberType]
         pre=True
```

### Comparing `craft_application-2.6.1/craft_application/models/metadata.py` & `craft_application-2.6.2/craft_application/models/metadata.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/models/project.py` & `craft_application-2.6.2/craft_application/models/project.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/remote/__init__.py` & `craft_application-2.6.2/craft_application/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/remote/errors.py` & `craft_application-2.6.2/craft_application/remote/errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/remote/git.py` & `craft_application-2.6.2/craft_application/remote/git.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/remote/utils.py` & `craft_application-2.6.2/craft_application/remote/utils.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/remote/worktree.py` & `craft_application-2.6.2/craft_application/remote/worktree.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/secrets.py` & `craft_application-2.6.2/craft_application/secrets.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/services/__init__.py` & `craft_application-2.6.2/craft_application/services/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/services/base.py` & `craft_application-2.6.2/craft_application/services/base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/services/lifecycle.py` & `craft_application-2.6.2/craft_application/services/lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/services/package.py` & `craft_application-2.6.2/craft_application/services/package.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/services/provider.py` & `craft_application-2.6.2/craft_application/services/provider.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/services/remotebuild.py` & `craft_application-2.6.2/craft_application/services/remotebuild.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/services/request.py` & `craft_application-2.6.2/craft_application/services/request.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/services/service_factory.py` & `craft_application-2.6.2/craft_application/services/service_factory.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/util/__init__.py` & `craft_application-2.6.2/craft_application/util/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/util/callbacks.py` & `craft_application-2.6.2/craft_application/util/callbacks.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/util/error_formatting.py` & `craft_application-2.6.2/craft_application/util/error_formatting.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/util/logging.py` & `craft_application-2.6.2/craft_application/util/logging.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/util/paths.py` & `craft_application-2.6.2/craft_application/util/paths.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/util/platforms.py` & `craft_application-2.6.2/craft_application/util/platforms.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/util/repositories.py` & `craft_application-2.6.2/craft_application/util/repositories.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/util/snap_config.py` & `craft_application-2.6.2/craft_application/util/snap_config.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/util/string.py` & `craft_application-2.6.2/craft_application/util/string.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application/util/yaml.py` & `craft_application-2.6.2/craft_application/util/yaml.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/craft_application.egg-info/PKG-INFO` & `craft_application-2.6.2/craft_application.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-application
-Version: 2.6.1
+Version: 2.6.2
 Summary: A framework for *craft applications.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `craft_application-2.6.1/craft_application.egg-info/SOURCES.txt` & `craft_application-2.6.2/craft_application.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 tests/unit/launchpad/test_launchpad.py
 tests/unit/launchpad/test_util.py
 tests/unit/launchpad/models/__init__.py
 tests/unit/launchpad/models/test_base.py
 tests/unit/launchpad/models/test_code.py
 tests/unit/models/__init__.py
 tests/unit/models/test_constraints.py
+tests/unit/models/test_grammar.py
 tests/unit/models/test_project.py
 tests/unit/models/project_models/basic_project.yaml
 tests/unit/models/project_models/full_project.yaml
 tests/unit/models/project_models/invalid_project.yaml
 tests/unit/remote/__init__.py
 tests/unit/remote/conftest.py
 tests/unit/remote/test_errors.py
```

### Comparing `craft_application-2.6.1/craft_application.egg-info/requires.txt` & `craft_application-2.6.2/craft_application.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/docs/conf.py` & `craft_application-2.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/docs/index.rst` & `craft_application-2.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/pyproject.toml` & `craft_application-2.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/conftest.py` & `craft_application-2.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/integration/conftest.py` & `craft_application-2.6.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/integration/data/valid_projects/grammar/testcraft.yaml` & `craft_application-2.6.2/tests/integration/data/valid_projects/grammar/testcraft.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/integration/launchpad/conftest.py` & `craft_application-2.6.2/tests/integration/launchpad/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/integration/launchpad/test_anonymous_access.py` & `craft_application-2.6.2/tests/integration/launchpad/test_anonymous_access.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/integration/services/test_lifecycle.py` & `craft_application-2.6.2/tests/integration/services/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/integration/services/test_provider.py` & `craft_application-2.6.2/tests/integration/services/test_provider.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/integration/services/test_remotebuild.py` & `craft_application-2.6.2/tests/integration/services/test_remotebuild.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/integration/services/test_request.py` & `craft_application-2.6.2/tests/integration/services/test_request.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/integration/services/test_service_factory.py` & `craft_application-2.6.2/tests/integration/services/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/integration/test_application.py` & `craft_application-2.6.2/tests/integration/test_application.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/integration/test_version.py` & `craft_application-2.6.2/tests/integration/test_version.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/commands/test_base.py` & `craft_application-2.6.2/tests/unit/commands/test_base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/commands/test_lifecycle.py` & `craft_application-2.6.2/tests/unit/commands/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/commands/test_other.py` & `craft_application-2.6.2/tests/unit/commands/test_other.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/conftest.py` & `craft_application-2.6.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/launchpad/conftest.py` & `craft_application-2.6.2/tests/unit/launchpad/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/launchpad/models/test_base.py` & `craft_application-2.6.2/tests/unit/launchpad/models/test_base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/launchpad/models/test_code.py` & `craft_application-2.6.2/tests/unit/launchpad/models/test_code.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/launchpad/test_launchpad.py` & `craft_application-2.6.2/tests/unit/launchpad/test_launchpad.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/launchpad/test_util.py` & `craft_application-2.6.2/tests/unit/launchpad/test_util.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/models/test_constraints.py` & `craft_application-2.6.2/tests/unit/models/test_constraints.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/models/test_project.py` & `craft_application-2.6.2/tests/unit/models/test_project.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/remote/conftest.py` & `craft_application-2.6.2/tests/unit/remote/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/remote/test_errors.py` & `craft_application-2.6.2/tests/unit/remote/test_errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/remote/test_git.py` & `craft_application-2.6.2/tests/unit/remote/test_git.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/remote/test_utils.py` & `craft_application-2.6.2/tests/unit/remote/test_utils.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/remote/test_worktree.py` & `craft_application-2.6.2/tests/unit/remote/test_worktree.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/services/conftest.py` & `craft_application-2.6.2/tests/unit/services/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/services/test_lifecycle.py` & `craft_application-2.6.2/tests/unit/services/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/services/test_package.py` & `craft_application-2.6.2/tests/unit/services/test_package.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/services/test_provider.py` & `craft_application-2.6.2/tests/unit/services/test_provider.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/services/test_remotebuild.py` & `craft_application-2.6.2/tests/unit/services/test_remotebuild.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/services/test_repositories.py` & `craft_application-2.6.2/tests/unit/services/test_repositories.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/services/test_request.py` & `craft_application-2.6.2/tests/unit/services/test_request.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/services/test_service_factory.py` & `craft_application-2.6.2/tests/unit/services/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/test_application.py` & `craft_application-2.6.2/tests/unit/test_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1337,28 +1337,34 @@
     """A project that builds on amd64 to riscv64 and s390x."""
     contents = dedent(
         """\
     name: myproject
     version: 1.0
     parts:
       mypart:
-        plugin: nil
+        plugin: meson
 
         # grammar-only string
         source:
         - on amd64 to riscv64: on-amd64-to-riscv64
         - on amd64 to s390x: on-amd64-to-s390x
+        - else: other
 
         # list of grammar and non-grammar data
         build-packages:
         - test-package
         - on amd64 to riscv64:
           - on-amd64-to-riscv64
         - on amd64 to s390x:
           - on-amd64-to-s390x
+
+        # non-grammar data in a non-grammar keyword
+        meson-parameters:
+        - foo
+        - bar
     """
     )
     project_file = tmp_path / "testcraft.yaml"
     project_file.write_text(contents)
 
 
 @pytest.fixture()
@@ -1468,14 +1474,21 @@
     assert project.parts["mypart"]["source"] == "on-amd64-to-riscv64"
     assert project.parts["mypart"]["build-packages"] == [
         "test-package",
         "on-amd64-to-riscv64",
     ]
 
 
+def test_process_grammar_non_grammar(grammar_app_mini):
+    """Non-grammar keywords should not be modified."""
+    project = grammar_app_mini.get_project(platform="platform-riscv64")
+
+    assert project.parts["mypart"]["meson-parameters"] == ["foo", "bar"]
+
+
 def test_process_grammar_default(grammar_app_mini):
     """Test that if nothing is provided the first BuildInfo is used by the grammar."""
     project = grammar_app_mini.get_project()
     assert project.parts["mypart"]["source"] == "on-amd64-to-riscv64"
     assert project.parts["mypart"]["build-packages"] == [
         "test-package",
         "on-amd64-to-riscv64",
@@ -1483,16 +1496,15 @@
 
 
 def test_process_grammar_no_match(grammar_app_mini, mocker):
     """Test that if the build plan is empty, the grammar uses the host as target arch."""
     mocker.patch("craft_application.util.get_host_architecture", return_value="i386")
     project = grammar_app_mini.get_project()
 
-    # "source" is empty because "i386" doesn't match any of the grammar statements.
-    assert project.parts["mypart"]["source"] is None
+    assert project.parts["mypart"]["source"] == "other"
     assert project.parts["mypart"]["build-packages"] == ["test-package"]
 
 
 class FakeApplicationWithYamlTransform(FakeApplication):
     """Application class that adds advanced grammar in `_extra_yaml_transform`."""
 
     @override
```

### Comparing `craft_application-2.6.1/tests/unit/test_errors.py` & `craft_application-2.6.2/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/test_grammar.py` & `craft_application-2.6.2/tests/unit/test_grammar.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/test_secrets.py` & `craft_application-2.6.2/tests/unit/test_secrets.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/util/test_error_formatting.py` & `craft_application-2.6.2/tests/unit/util/test_error_formatting.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/util/test_logging.py` & `craft_application-2.6.2/tests/unit/util/test_logging.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/util/test_paths.py` & `craft_application-2.6.2/tests/unit/util/test_paths.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/util/test_snap_config.py` & `craft_application-2.6.2/tests/unit/util/test_snap_config.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/util/test_string.py` & `craft_application-2.6.2/tests/unit/util/test_string.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tests/unit/util/test_yaml.py` & `craft_application-2.6.2/tests/unit/util/test_yaml.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.1/tox.ini` & `craft_application-2.6.2/tox.ini`

 * *Files identical despite different names*

