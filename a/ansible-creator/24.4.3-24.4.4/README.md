# Comparing `tmp/ansible_creator-24.4.3.tar.gz` & `tmp/ansible_creator-24.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_creator-24.4.3.tar", last modified: Thu Apr 25 15:24:46 2024, max compression
+gzip compressed data, was "ansible_creator-24.4.4.tar", last modified: Tue Apr 30 14:57:37 2024, max compression
```

## Comparing `ansible_creator-24.4.3.tar` & `ansible_creator-24.4.4.tar`

### file list

```diff
@@ -1,376 +1,376 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.321469 ansible_creator-24.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.269469 ansible_creator-24.4.3/.config/
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.config/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.config/requirements-docs.in
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.config/requirements-test.in
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.269469 ansible_creator-24.4.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.269469 ansible_creator-24.4.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.github/ISSUE_TEMPLATE/documentation_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.269469 ansible_creator-24.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.273469 ansible_creator-24.4.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-25 15:24:46.321469 ansible_creator-24.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.273469 ansible_creator-24.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/docs/collection_creation.md
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/docs/installing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.285469 ansible_creator-24.4.3/docs/media/
--rw-r--r--   0 runner    (1001) docker     (127)  2113880 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/docs/media/log-to-file.gif
--rw-r--r--   0 runner    (1001) docker     (127)  3211387 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/docs/media/open-collection.gif
--rw-r--r--   0 runner    (1001) docker     (127)  2769642 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/docs/media/open-folder.gif
--rw-r--r--   0 runner    (1001) docker     (127)  3250683 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/docs/media/open-log-file.gif
--rw-r--r--   0 runner    (1001) docker     (127)   297010 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/docs/media/refresh.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:24:46.321469 ansible_creator-24.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.253469 ansible_creator-24.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.289469 ansible_creator-24.4.3/src/ansible_creator/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 15:24:46.000000 ansible_creator-24.4.3/src/ansible_creator/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/output.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.253469 ansible_creator-24.4.3/src/ansible_creator/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.289469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/.github/ansible-code-bot.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/.github/workflows/tests.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/README.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/ansible-navigator.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/ansible.cfg.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/collections/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.253469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/collections/ansible_collections/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.253469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.253469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/roles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/roles/run/
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/roles/run/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/roles/run/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/roles/run/tasks/main.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/collections/requirements.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/inventory/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/inventory/group_vars/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/inventory/group_vars/all.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/inventory/group_vars/web_servers.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/inventory/host_vars/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/inventory/host_vars/server1.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/inventory/host_vars/server2.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/inventory/host_vars/server3.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/inventory/host_vars/switch1.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/inventory/host_vars/switch2.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/inventory/hosts.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/linux_playbook.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/network_playbook.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/site.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.253469 ansible_creator-24.4.3/src/ansible_creator/resources/common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.253469 ansible_creator-24.4.3/src/ansible_creator/resources/common/devcontainer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/common/devcontainer/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/common/devcontainer/.devcontainer/devcontainer.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/common/devcontainer/.devcontainer/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/common/devcontainer/.devcontainer/docker/devcontainer.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/common/devcontainer/.devcontainer/podman/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/common/devcontainer/.devcontainer/podman/devcontainer.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/common/devfile/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/common/devfile/devfile.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.293469 ansible_creator-24.4.3/src/ansible_creator/resources/common/gitignore/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/common/gitignore/.gitignore.j2
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/common/gitignore/__meta__.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.297469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.253469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.297469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/.github/workflows/release.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/.github/workflows/tests.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/.isort.cfg.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/.pre-commit-config.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/.prettierignore.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.297469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/CONTRIBUTING
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/LICENSE.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.297469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/changelogs/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/changelogs/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.297469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/docs/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.297469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/docs/docsite/
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/docs/docsite/links.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.253469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.253469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/extensions/eda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.297469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/extensions/eda/rulebooks/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/extensions/eda/rulebooks/rulebook.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.257469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/extensions/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.297469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/extensions/molecule/integration_hello_world/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/extensions/molecule/integration_hello_world/molecule.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.257469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/extensions/molecule/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.297469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/extensions/molecule/utils/playbooks/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/extensions/molecule/utils/playbooks/converge.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/extensions/molecule/utils/playbooks/noop.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/extensions/molecule/utils/vars/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/extensions/molecule/utils/vars/vars.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/galaxy.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/meta/runtime.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.257469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/action/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/cache/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/filter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/filter/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/filter/hello_world.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/inventory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/inventory/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/module_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/module_utils/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/modules/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/plugin_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/plugin_utils/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/sub_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/sub_plugins/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/plugins/test/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.257469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/defaults/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/files/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/handlers/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/meta/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/meta/main.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/templates/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/tests/inventory
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/vars/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/vars/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/tests/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/tests/integration/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.257469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/tests/integration/targets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.257469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/tests/integration/targets/hello_world/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.301469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/tests/integration/targets/hello_world/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/tests/integration/targets/hello_world/tasks/main.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/tests/integration/test_integration.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.305469 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/tests/unit/.keep
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/tox-ansible.ini.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.305469 ansible_creator-24.4.3/src/ansible_creator/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.305469 ansible_creator-24.4.3/src/ansible_creator/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/subcommands/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/templar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/src/ansible_creator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.321469 ansible_creator-24.4.3/src/ansible_creator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-25 15:24:46.000000 ansible_creator-24.4.3/src/ansible_creator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12955 2024-04-25 15:24:46.000000 ansible_creator-24.4.3/src/ansible_creator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:24:46.000000 ansible_creator-24.4.3/src/ansible_creator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 15:24:46.000000 ansible_creator-24.4.3/src/ansible_creator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 15:24:46.000000 ansible_creator-24.4.3/src/ansible_creator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 15:24:46.000000 ansible_creator-24.4.3/src/ansible_creator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.305469 ansible_creator-24.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.265469 ansible_creator-24.4.3/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.257469 ansible_creator-24.4.3/tests/fixtures/collection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.257469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.305469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.305469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.devcontainer/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.devcontainer/docker/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.devcontainer/podman/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.devcontainer/podman/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.261469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.prettierignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/CONTRIBUTING
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/changelogs/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/changelogs/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/devfile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/docs/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/docs/docsite/
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/docs/docsite/links.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.261469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.261469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/extensions/eda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/extensions/eda/rulebooks/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/extensions/eda/rulebooks/rulebook.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.261469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/extensions/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/extensions/molecule/integration_hello_world/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/extensions/molecule/integration_hello_world/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.261469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/playbooks/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/playbooks/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/playbooks/noop.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/vars/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/vars/vars.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/meta/runtime.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.261469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/action/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/filter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/filter/hello_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/inventory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/inventory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/module_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/module_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/plugin_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/plugin_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.309469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/sub_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/sub_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/plugins/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.261469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/defaults/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/files/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/handlers/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/meta/
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/templates/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/tests/inventory
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/vars/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/vars/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/tests/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.261469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/tests/integration/targets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.261469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/tests/integration/targets/hello_world/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/tests/integration/targets/hello_world/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/tests/integration/targets/hello_world/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/tests/integration/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/tests/unit/.keep
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/tox-ansible.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.265469 ansible_creator-24.4.3/tests/fixtures/project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.313469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.devcontainer/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.devcontainer/docker/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.devcontainer/podman/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.devcontainer/podman/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.github/ansible-code-bot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/ansible-navigator.yml
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/ansible.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/collections/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.265469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/collections/ansible_collections/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.265469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.265469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/roles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/roles/run/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/roles/run/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/roles/run/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/roles/run/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/collections/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/devfile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/inventory/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/inventory/group_vars/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/inventory/group_vars/all.yml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/inventory/group_vars/web_servers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/inventory/host_vars/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/inventory/host_vars/server1.yml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/inventory/host_vars/server2.yml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/inventory/host_vars/server3.yml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/inventory/host_vars/switch1.yml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/inventory/host_vars/switch2.yml
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/inventory/hosts.yml
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/linux_playbook.yml
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/network_playbook.yml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/fixtures/project/ansible_project/site.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/integration/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:24:46.317469 ansible_creator-24.4.3/tests/units/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/units/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tests/units/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-25 15:24:34.000000 ansible_creator-24.4.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.941631 ansible_creator-24.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.889631 ansible_creator-24.4.4/.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.config/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.config/requirements-docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.config/requirements-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.889631 ansible_creator-24.4.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.889631 ansible_creator-24.4.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.github/ISSUE_TEMPLATE/documentation_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.889631 ansible_creator-24.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.893631 ansible_creator-24.4.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-30 14:57:37.941631 ansible_creator-24.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.893631 ansible_creator-24.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/docs/collection_creation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/docs/installing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.905631 ansible_creator-24.4.4/docs/media/
+-rw-r--r--   0 runner    (1001) docker     (127)  2113880 2024-04-30 14:57:26.000000 ansible_creator-24.4.4/docs/media/log-to-file.gif
+-rw-r--r--   0 runner    (1001) docker     (127)  3211387 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/docs/media/open-collection.gif
+-rw-r--r--   0 runner    (1001) docker     (127)  2769642 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/docs/media/open-folder.gif
+-rw-r--r--   0 runner    (1001) docker     (127)  3250683 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/docs/media/open-log-file.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   297010 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/docs/media/refresh.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:57:37.941631 ansible_creator-24.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.873631 ansible_creator-24.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.909631 ansible_creator-24.4.4/src/ansible_creator/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-30 14:57:37.000000 ansible_creator-24.4.4/src/ansible_creator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.873631 ansible_creator-24.4.4/src/ansible_creator/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/.github/ansible-code-bot.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/.github/workflows/tests.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/README.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/ansible-navigator.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/ansible.cfg.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/collections/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.873631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/collections/ansible_collections/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.873631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.873631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/roles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/roles/run/
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/roles/run/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/roles/run/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/roles/run/tasks/main.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/collections/requirements.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/inventory/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/inventory/group_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/inventory/group_vars/all.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/inventory/group_vars/web_servers.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/inventory/host_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/inventory/host_vars/server1.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/inventory/host_vars/server2.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/inventory/host_vars/server3.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/inventory/host_vars/switch1.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/inventory/host_vars/switch2.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/inventory/hosts.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/linux_playbook.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/network_playbook.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/site.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.873631 ansible_creator-24.4.4/src/ansible_creator/resources/common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.873631 ansible_creator-24.4.4/src/ansible_creator/resources/common/devcontainer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/common/devcontainer/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/common/devcontainer/.devcontainer/devcontainer.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/common/devcontainer/.devcontainer/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/common/devcontainer/.devcontainer/docker/devcontainer.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/common/devcontainer/.devcontainer/podman/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/common/devcontainer/.devcontainer/podman/devcontainer.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.913631 ansible_creator-24.4.4/src/ansible_creator/resources/common/devfile/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/common/devfile/devfile.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.917631 ansible_creator-24.4.4/src/ansible_creator/resources/common/gitignore/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/common/gitignore/.gitignore.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/common/gitignore/__meta__.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.917631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.873631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.917631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/.github/workflows/release.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/.github/workflows/tests.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/.isort.cfg.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/.pre-commit-config.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/.prettierignore.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.917631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/CONTRIBUTING
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/LICENSE.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.917631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/changelogs/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/changelogs/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.917631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/docs/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.917631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/docs/docsite/
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/docs/docsite/links.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.877631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.873631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/extensions/eda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.917631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/extensions/eda/rulebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/extensions/eda/rulebooks/rulebook.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.877631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/extensions/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.917631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/extensions/molecule/integration_hello_world/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/extensions/molecule/integration_hello_world/molecule.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.877631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/extensions/molecule/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/extensions/molecule/utils/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/extensions/molecule/utils/playbooks/converge.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/extensions/molecule/utils/playbooks/noop.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/extensions/molecule/utils/vars/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/extensions/molecule/utils/vars/vars.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/galaxy.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/meta/runtime.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.877631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/action/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/cache/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/filter/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/filter/hello_world.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/inventory/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/module_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/module_utils/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/modules/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/plugin_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/plugin_utils/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/sub_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/sub_plugins/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/plugins/test/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.877631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/defaults/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/files/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/handlers/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/meta/main.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/templates/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.921631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/tests/inventory
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.925631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/vars/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.925631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/tests/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.925631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/tests/integration/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.877631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/tests/integration/targets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.877631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/tests/integration/targets/hello_world/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.925631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/tests/integration/targets/hello_world/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/tests/integration/targets/hello_world/tasks/main.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/tests/integration/test_integration.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.925631 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/tests/unit/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/tox-ansible.ini.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.925631 ansible_creator-24.4.4/src/ansible_creator/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.925631 ansible_creator-24.4.4/src/ansible_creator/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/subcommands/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/templar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/src/ansible_creator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.941631 ansible_creator-24.4.4/src/ansible_creator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-30 14:57:37.000000 ansible_creator-24.4.4/src/ansible_creator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12955 2024-04-30 14:57:37.000000 ansible_creator-24.4.4/src/ansible_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:57:37.000000 ansible_creator-24.4.4/src/ansible_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-30 14:57:37.000000 ansible_creator-24.4.4/src/ansible_creator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-30 14:57:37.000000 ansible_creator-24.4.4/src/ansible_creator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 14:57:37.000000 ansible_creator-24.4.4/src/ansible_creator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.925631 ansible_creator-24.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.885631 ansible_creator-24.4.4/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.877631 ansible_creator-24.4.4/tests/fixtures/collection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.877631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.devcontainer/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.devcontainer/docker/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.devcontainer/podman/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.devcontainer/podman/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.881631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.prettierignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/CONTRIBUTING
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/changelogs/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/changelogs/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/devfile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/docs/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/docs/docsite/
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/docs/docsite/links.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.881631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.881631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/extensions/eda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/extensions/eda/rulebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/extensions/eda/rulebooks/rulebook.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.881631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/extensions/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/extensions/molecule/integration_hello_world/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/extensions/molecule/integration_hello_world/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.881631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/playbooks/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/playbooks/noop.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/vars/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/extensions/molecule/utils/vars/vars.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/meta/runtime.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.881631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/action/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.929631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/filter/hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/inventory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/module_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/module_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/plugin_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/plugin_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/sub_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/sub_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/plugins/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.881631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/defaults/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/files/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/handlers/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/templates/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/tests/inventory
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/vars/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/tests/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.885631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/tests/integration/targets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.885631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/tests/integration/targets/hello_world/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/tests/integration/targets/hello_world/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/tests/integration/targets/hello_world/tasks/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/tests/integration/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.933631 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/tests/unit/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.885631 ansible_creator-24.4.4/tests/fixtures/project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.937631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.937631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.937631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.devcontainer/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.devcontainer/docker/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.937631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.devcontainer/podman/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.devcontainer/podman/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.937631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.github/ansible-code-bot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.937631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.937631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/ansible-navigator.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/ansible.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.937631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/collections/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.885631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/collections/ansible_collections/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.885631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.937631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.885631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/roles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.937631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/roles/run/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/roles/run/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.937631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/roles/run/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/roles/run/tasks/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/collections/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/devfile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.937631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/inventory/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.937631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/inventory/group_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/inventory/group_vars/all.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/inventory/group_vars/web_servers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.941631 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/inventory/host_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/inventory/host_vars/server1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/inventory/host_vars/server2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/inventory/host_vars/server3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/inventory/host_vars/switch1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/inventory/host_vars/switch2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/inventory/hosts.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/linux_playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/network_playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/fixtures/project/ansible_project/site.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.941631 ansible_creator-24.4.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/integration/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:57:37.941631 ansible_creator-24.4.4/tests/units/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/units/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tests/units/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-30 14:57:27.000000 ansible_creator-24.4.4/tox.ini
```

### Comparing `ansible_creator-24.4.3/.config/constraints.txt` & `ansible_creator-24.4.4/.config/constraints.txt`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/.config/dictionary.txt` & `ansible_creator-24.4.4/.config/dictionary.txt`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/.flake8` & `ansible_creator-24.4.4/.flake8`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/.github/ISSUE_TEMPLATE/bug_report.md` & `ansible_creator-24.4.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/.github/workflows/release.yml` & `ansible_creator-24.4.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/.github/workflows/tox.yml` & `ansible_creator-24.4.4/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/.pre-commit-config.yaml` & `ansible_creator-24.4.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/.vscode/launch.json` & `ansible_creator-24.4.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/LICENSE` & `ansible_creator-24.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/PKG-INFO` & `ansible_creator-24.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-creator
-Version: 24.4.3
+Version: 24.4.4
 Summary: A CLI tool for scaffolding Ansible Content.
 Author-email: Nilashish Chakarborty <nchakrab@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: changelog, https://github.com/ansible-community/ansible-creator/releases
 Project-URL: documentation, https://ansible-creator.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/ansible-community/ansible-creator
```

### Comparing `ansible_creator-24.4.3/README.md` & `ansible_creator-24.4.4/README.md`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/cspell.config.yaml` & `ansible_creator-24.4.4/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/docs/collection_creation.md` & `ansible_creator-24.4.4/docs/collection_creation.md`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/docs/contributing.md` & `ansible_creator-24.4.4/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/docs/index.md` & `ansible_creator-24.4.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/docs/installing.md` & `ansible_creator-24.4.4/docs/installing.md`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/docs/media/log-to-file.gif` & `ansible_creator-24.4.4/docs/media/log-to-file.gif`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/docs/media/open-collection.gif` & `ansible_creator-24.4.4/docs/media/open-collection.gif`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/docs/media/open-folder.gif` & `ansible_creator-24.4.4/docs/media/open-folder.gif`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/docs/media/open-log-file.gif` & `ansible_creator-24.4.4/docs/media/open-log-file.gif`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/docs/media/refresh.gif` & `ansible_creator-24.4.4/docs/media/refresh.gif`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/mkdocs.yml` & `ansible_creator-24.4.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/pyproject.toml` & `ansible_creator-24.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/cli.py` & `ansible_creator-24.4.4/src/ansible_creator/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/config.py` & `ansible_creator-24.4.4/src/ansible_creator/config.py`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/exceptions.py` & `ansible_creator-24.4.4/src/ansible_creator/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/output.py` & `ansible_creator-24.4.4/src/ansible_creator/output.py`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/README.md.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/README.md.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/ansible.cfg.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/ansible.cfg.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/README.md.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/README.md.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/roles/run/README.md.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/collections/ansible_collections/project_org/project_repo/roles/run/README.md.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/linux_playbook.yml.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/linux_playbook.yml.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/ansible_project/network_playbook.yml.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/ansible_project/network_playbook.yml.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/common/devcontainer/.devcontainer/devcontainer.json.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/common/devcontainer/.devcontainer/devcontainer.json.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/common/devcontainer/.devcontainer/docker/devcontainer.json.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/common/devcontainer/.devcontainer/docker/devcontainer.json.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/common/devcontainer/.devcontainer/podman/devcontainer.json.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/common/devcontainer/.devcontainer/podman/devcontainer.json.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/common/gitignore/.gitignore.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/common/gitignore/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/.github/workflows/tests.yml.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/.github/workflows/tests.yml.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/.pre-commit-config.yaml.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/.pre-commit-config.yaml.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/LICENSE.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/README.md.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/README.md.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/changelogs/config.yaml` & `ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/changelogs/config.yaml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/docs/docsite/links.yml` & `ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/docs/docsite/links.yml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/galaxy.yml.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/galaxy.yml.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/README.md.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/README.md.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/resources/new_collection/roles/run/meta/main.yml.j2` & `ansible_creator-24.4.4/src/ansible_creator/resources/new_collection/roles/run/meta/main.yml.j2`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/subcommands/init.py` & `ansible_creator-24.4.4/src/ansible_creator/subcommands/init.py`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/templar.py` & `ansible_creator-24.4.4/src/ansible_creator/templar.py`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator/utils.py` & `ansible_creator-24.4.4/src/ansible_creator/utils.py`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/src/ansible_creator.egg-info/PKG-INFO` & `ansible_creator-24.4.4/src/ansible_creator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-creator
-Version: 24.4.3
+Version: 24.4.4
 Summary: A CLI tool for scaffolding Ansible Content.
 Author-email: Nilashish Chakarborty <nchakrab@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: changelog, https://github.com/ansible-community/ansible-creator/releases
 Project-URL: documentation, https://ansible-creator.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/ansible-community/ansible-creator
```

### Comparing `ansible_creator-24.4.3/src/ansible_creator.egg-info/SOURCES.txt` & `ansible_creator-24.4.4/src/ansible_creator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/conftest.py` & `ansible_creator-24.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.devcontainer/devcontainer.json` & `ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.devcontainer/docker/devcontainer.json` & `ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.devcontainer/docker/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.devcontainer/podman/devcontainer.json` & `ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.devcontainer/podman/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.github/workflows/tests.yml` & `ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.gitignore` & `ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/.pre-commit-config.yaml` & `ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/LICENSE` & `ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/README.md` & `ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/README.md`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/changelogs/config.yaml` & `ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/changelogs/config.yaml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/docs/docsite/links.yml` & `ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/docs/docsite/links.yml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/galaxy.yml` & `ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/galaxy.yml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/README.md` & `ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/README.md`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/collection/testorg/testcol/roles/run/meta/main.yml` & `ansible_creator-24.4.4/tests/fixtures/collection/testorg/testcol/roles/run/meta/main.yml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.devcontainer/devcontainer.json` & `ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.devcontainer/docker/devcontainer.json` & `ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.devcontainer/docker/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.devcontainer/podman/devcontainer.json` & `ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.devcontainer/podman/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/project/ansible_project/.gitignore` & `ansible_creator-24.4.4/tests/fixtures/project/ansible_project/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/project/ansible_project/README.md` & `ansible_creator-24.4.4/tests/fixtures/project/ansible_project/README.md`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/project/ansible_project/ansible.cfg` & `ansible_creator-24.4.4/tests/fixtures/project/ansible_project/ansible.cfg`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/README.md` & `ansible_creator-24.4.4/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/README.md`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/roles/run/README.md` & `ansible_creator-24.4.4/tests/fixtures/project/ansible_project/collections/ansible_collections/weather/demo/roles/run/README.md`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/project/ansible_project/linux_playbook.yml` & `ansible_creator-24.4.4/tests/fixtures/project/ansible_project/linux_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/fixtures/project/ansible_project/network_playbook.yml` & `ansible_creator-24.4.4/tests/fixtures/project/ansible_project/network_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/integration/test_init.py` & `ansible_creator-24.4.4/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/units/test_basic.py` & `ansible_creator-24.4.4/tests/units/test_basic.py`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tests/units/test_init.py` & `ansible_creator-24.4.4/tests/units/test_init.py`

 * *Files identical despite different names*

### Comparing `ansible_creator-24.4.3/tox.ini` & `ansible_creator-24.4.4/tox.ini`

 * *Files identical despite different names*

