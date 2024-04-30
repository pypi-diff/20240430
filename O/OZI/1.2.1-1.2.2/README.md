# Comparing `tmp/OZI-1.2.1.tar.gz` & `tmp/OZI-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI-1.2.1.tar", last modified: Sun Apr 28 20:24:44 2024, max compression
+gzip compressed data, was "OZI-1.2.2.tar", last modified: Tue Apr 30 20:32:23 2024, max compression
```

## Comparing `OZI-1.2.1.tar` & `OZI-1.2.2.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:24:44.565276 OZI-1.2.1/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/CODEOWNERS
--rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/FUNDING.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/SECURITY.md
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/workflows/dev-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/workflows/dist-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-04-28 20:19:07.000000 OZI-1.2.1/.github/workflows/scorecard.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-04-28 20:19:07.000000 OZI-1.2.1/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)   287792 2024-04-28 20:19:07.000000 OZI-1.2.1/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-04-28 20:19:07.000000 OZI-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-04-28 20:24:44.565276 OZI-1.2.1/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-04-28 20:19:07.000000 OZI-1.2.1/README.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    16576 2024-04-28 20:19:07.000000 OZI-1.2.1/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-04-28 20:19:07.000000 OZI-1.2.1/meson.options
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/
--rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/actions.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/comment.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/dist/
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/dist/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/dist/semantic_release/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/dist/semantic_release/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/dist/semantic_release/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/dist/sigstore/
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/dist/sigstore/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/dist/sigstore/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/fix/
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/fix/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/fix/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/fix/build_definition.py
--rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/fix/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6305 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/fix/missing.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/fix/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7877 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/fix/rewrite_command.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/bandit/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/bandit/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/bandit/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/black/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/black/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/black/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/flake8/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/flake8/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/flake8/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/isort/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/isort/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/isort/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/mypy/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/mypy/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/mypy/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/pyright/
--rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/pyright/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/pyright/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/restructuredtext-lint/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/restructuredtext-lint/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/lint/restructuredtext-lint/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/meson.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/new/
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/new/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/new/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/new/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6436 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/new/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/new/validate.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/pkg_extra.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     4749 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/render.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/scripts/
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/scripts/core_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/scripts/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2044 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/scripts/meson_dist_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/scripts/meson_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/scripts/render_requirements.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/scripts/replace_ruff_target_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/scripts/scm_version_snip.py
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/scripts/to_distribution_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/scripts/version_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/spdx.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/spec/
--rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/spec/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/spec/_license.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/spec/_spec.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/spec/base.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6070 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/spec/ci.py
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/spec/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/spec/pkg.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/spec/project.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6347 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/spec/python.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/spec/src.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/tap.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/test/coverage/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/test/coverage/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/test/coverage/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/test/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/test/pytest/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/test/pytest/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/test/pytest/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/trove.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/__init__.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/email_validator/
--rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/email_validator/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/email_validator/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/email_validator/deliverability.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/email_validator/exceptions_types.py
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/email_validator/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/email_validator/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/email_validator/rfc_constants.py
--rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/email_validator/syntax.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/email_validator/validate_email.py
--rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/email_validator/version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-04-28 20:19:07.000000 OZI-1.2.1/ozi/vendor/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10755 2024-04-28 20:19:07.000000 OZI-1.2.1/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      190 2024-04-28 20:19:07.000000 OZI-1.2.1/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/subprojects/
--rw-rw-r--   0 runner    (1001) docker     (127)      342 2024-04-28 20:19:07.000000 OZI-1.2.1/subprojects/blastpipe.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-04-28 20:19:07.000000 OZI-1.2.1/templates/CHANGELOG.md.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:19:07.000000 OZI-1.2.1/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-04-28 20:19:07.000000 OZI-1.2.1/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11072 2024-04-28 20:19:07.000000 OZI-1.2.1/tests/test_ozi_fix.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14164 2024-04-28 20:19:07.000000 OZI-1.2.1/tests/test_ozi_new.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-04-28 20:19:07.000000 OZI-1.2.1/tests/test_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:32:23.695530 OZI-1.2.2/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/FUNDING.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/SECURITY.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/workflows/dev-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/workflows/dist-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/workflows/scorecard.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-04-30 20:26:34.000000 OZI-1.2.2/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)   289498 2024-04-30 20:26:34.000000 OZI-1.2.2/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-04-30 20:26:34.000000 OZI-1.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-04-30 20:32:23.695530 OZI-1.2.2/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-04-30 20:26:34.000000 OZI-1.2.2/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    16576 2024-04-30 20:26:34.000000 OZI-1.2.2/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-04-30 20:26:34.000000 OZI-1.2.2/meson.options
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/actions.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/comment.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/semantic_release/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/semantic_release/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/semantic_release/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/sigstore/
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/sigstore/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/sigstore/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/build_definition.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6305 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/missing.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7877 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/rewrite_command.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/bandit/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/bandit/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/bandit/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/black/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/black/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/black/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/flake8/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/flake8/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/flake8/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/isort/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/isort/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/isort/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/mypy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/mypy/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/mypy/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/pyright/
+-rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/pyright/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/pyright/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/restructuredtext-lint/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/restructuredtext-lint/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/restructuredtext-lint/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/meson.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/new/
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/new/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/new/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/new/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6436 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/new/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/new/validate.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/pkg_extra.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     4854 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/render.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/core_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2044 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/meson_dist_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/meson_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/render_requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/replace_ruff_target_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/scm_version_snip.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/to_distribution_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/version_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spdx.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/_license.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/_spec.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/base.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6070 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/ci.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/pkg.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/project.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6347 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/python.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/src.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/tap.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/coverage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/coverage/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/coverage/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/pytest/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/pytest/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/pytest/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/trove.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/__init__.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/deliverability.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/exceptions_types.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/rfc_constants.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/syntax.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/validate_email.py
+-rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10755 2024-04-30 20:26:34.000000 OZI-1.2.2/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      190 2024-04-30 20:26:34.000000 OZI-1.2.2/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/subprojects/
+-rw-rw-r--   0 runner    (1001) docker     (127)      342 2024-04-30 20:26:34.000000 OZI-1.2.2/subprojects/blastpipe.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-04-30 20:26:34.000000 OZI-1.2.2/templates/CHANGELOG.md.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-04-30 20:26:34.000000 OZI-1.2.2/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11072 2024-04-30 20:26:34.000000 OZI-1.2.2/tests/test_ozi_fix.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14164 2024-04-30 20:26:34.000000 OZI-1.2.2/tests/test_ozi_new.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-04-30 20:26:34.000000 OZI-1.2.2/tests/test_tap.py
```

### Comparing `OZI-1.2.1/.github/CODEOWNERS` & `OZI-1.2.2/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/.github/CODE_OF_CONDUCT.md` & `OZI-1.2.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/.github/CONTRIBUTING.md` & `OZI-1.2.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `OZI-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `OZI-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/.github/SECURITY.md` & `OZI-1.2.2/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/.github/workflows/codeql.yml` & `OZI-1.2.2/.github/workflows/codeql.yml`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
       matrix:
         language: ["python"]
         # CodeQL supports [ $supported-codeql-languages ]
         # Learn more about CodeQL language support at https://aka.ms/codeql-docs/language-support
 
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
           disable-sudo: true
           egress-policy: block
           allowed-endpoints: >
             api.github.com:443
             github.com:443
             objects.githubusercontent.com:443
```

### Comparing `OZI-1.2.1/.github/workflows/dependency-review.yml` & `OZI-1.2.2/.github/workflows/dependency-review.yml`

 * *Files 14% similar despite different names*

```diff
@@ -18,17 +18,17 @@
   contents: read
 
 jobs:
   dependency-review:
     runs-on: ubuntu-latest
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
           egress-policy: audit
 
       - name: 'Checkout Repository'
         uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
       - name: 'Dependency Review'
-        uses: actions/dependency-review-action@5bbc3ba658137598168acb2ab73b21c432dd411b # v4.2.5
+        uses: actions/dependency-review-action@e58c696e52cac8e62d61cc21fda89565d71505d7 # v4.3.1
         with:
           head-ref: main
```

### Comparing `OZI-1.2.1/.github/workflows/dev-workflow.yml` & `OZI-1.2.2/.github/workflows/dev-workflow.yml`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
     permissions:
         id-token: write
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
           disable-sudo: true
           egress-policy: block
           allowed-endpoints: >
             files.pythonhosted.org:443
             github.com:443
             oziproject.dev:443
@@ -45,15 +45,15 @@
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
     permissions:
         id-token: write
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
           disable-sudo: true
           egress-policy: block
           allowed-endpoints: >
             files.pythonhosted.org:443
             github.com:443
             oziproject.dev:443
@@ -73,15 +73,15 @@
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
     permissions:
         id-token: write
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
           disable-sudo: true
           egress-policy: block
           allowed-endpoints: >
             files.pythonhosted.org:443
             github.com:443
             oziproject.dev:443
```

### Comparing `OZI-1.2.1/.github/workflows/dist-workflow.yml` & `OZI-1.2.2/.github/workflows/dist-workflow.yml`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
     permissions:
         id-token: write
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
           disable-sudo: true
           egress-policy: block
           allowed-endpoints: >
             files.pythonhosted.org:443
             github.com:443
             oziproject.dev:443
@@ -47,15 +47,15 @@
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
     permissions:
         id-token: write
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
           disable-sudo: true
           egress-policy: block
           allowed-endpoints: >
             files.pythonhosted.org:443
             github.com:443
             oziproject.dev:443
@@ -75,15 +75,15 @@
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
     permissions:
         id-token: write
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
           disable-sudo: true
           egress-policy: block
           allowed-endpoints: >
             files.pythonhosted.org:443
             github.com:443
             oziproject.dev:443
@@ -99,15 +99,15 @@
           python-version: "3.12"
 
   checkpoint:
     runs-on: ubuntu-latest
     needs: [checkpoint-cp310-ubuntu-latest, checkpoint-cp311-ubuntu-latest, checkpoint-cp312-ubuntu-latest]
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
           disable-sudo: true
           egress-policy: block
 
   release:
     needs: checkpoint
     runs-on: ubuntu-latest
@@ -125,15 +125,15 @@
       hashes: ${{ steps.release.outputs.hashes }}
       tag: ${{ steps.release.outputs.tag }}
     permissions:
       contents: write
       id-token: write
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
           disable-sudo: true
           egress-policy: block
           allowed-endpoints: >
             api.github.com:443
             files.pythonhosted.org:443
             fulcio.sigstore.dev:443
@@ -170,15 +170,15 @@
     if: needs.release.outputs.drafted == 'true'
     permissions:
       actions: read
       contents: write
       id-token: write
     steps:
     - name: Harden Runner
-      uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
+      uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
       with:
         disable-sudo: true
         egress-policy: block
         allowed-endpoints: >
           api.github.com:443
           upload.pypi.org:443
           uploads.github.com:443
```

### Comparing `OZI-1.2.1/.github/workflows/scorecard.yml` & `OZI-1.2.2/.github/workflows/scorecard.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
       id-token: write
       # Uncomment the permissions below if installing in a private repository.
       # contents: read
       # actions: read
 
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
           disable-sudo: true
           egress-policy: block
           allowed-endpoints: >
             api.github.com:443
             api.osv.dev:443
             api.securityscorecards.dev:443
```

### Comparing `OZI-1.2.1/.gitignore` & `OZI-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/CHANGELOG.md` & `OZI-1.2.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,48 @@
 # CHANGELOG
+## 1.2.2 (2024-04-30)
+
+### :arrow_up:
+
+* :arrow_up: Bump step-security/harden-runner from 2.7.0 to 2.7.1
+
+Bumps [step-security/harden-runner](https://github.com/step-security/harden-runner) from 2.7.0 to 2.7.1.
+- [Release notes](https://github.com/step-security/harden-runner/releases)
+- [Commits](https://github.com/step-security/harden-runner/compare/63c24ba6bd7ba022e95695ff85de572c04a18142...a4aa98b93cab29d9b1101a6143fb8bce00e2eac4)
+
+---
+updated-dependencies:
+- dependency-name: step-security/harden-runner
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`3184386`](https://github.com/OZI-Project/OZI/commit/3184386d8308b4604d6f6c832940045176ec1e2d))
+
+* :arrow_up: Bump actions/dependency-review-action from 4.2.5 to 4.3.1
+
+Bumps [actions/dependency-review-action](https://github.com/actions/dependency-review-action) from 4.2.5 to 4.3.1.
+- [Release notes](https://github.com/actions/dependency-review-action/releases)
+- [Commits](https://github.com/actions/dependency-review-action/compare/5bbc3ba658137598168acb2ab73b21c432dd411b...e58c696e52cac8e62d61cc21fda89565d71505d7)
+
+---
+updated-dependencies:
+- dependency-name: actions/dependency-review-action
+  dependency-type: direct:production
+  update-type: version-update:semver-minor
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`1f7e9f1`](https://github.com/OZI-Project/OZI/commit/1f7e9f199315405bc2a17af147c41047ace16aa3))
+
+### Other
+
+* :memo: update docstrings for 1.2 (#429)
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`d72f67c`](https://github.com/OZI-Project/OZI/commit/d72f67c298a0dee02ad6abc3006b875b3067b397))
+
 ## 1.2.1 (2024-04-28)
 
 ### :arrow_up:
 
 * :arrow_up: Bump OZI-Project/release 0.1.18 &gt; 0.1.17
 
 * :arrow_up: Update dist-workflow.yml - release 0.1.18 &gt; 0.1.17
```

### Comparing `OZI-1.2.1/LICENSE.txt` & `OZI-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/PKG-INFO` & `OZI-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: OZI
-Version: 1.2.1
+Version: 1.2.2
 Summary: Packager for Python projects using Meson.
-Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.2.1.tar.gz
+Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.2.2.tar.gz
 Home-page: https://oziproject.dev/
 Author: Eden Rose Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
 Keywords: meson,packaging,wheel
 Project-URL: Bug Tracker, https://github.com/rjdbcm/ozi/issues
 Project-URL: Community, https://github.com/orgs/OZI-Project/discussions
```

### Comparing `OZI-1.2.1/README.rst` & `OZI-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/meson.build` & `OZI-1.2.2/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/meson.options` & `OZI-1.2.2/meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/__main__.py` & `OZI-1.2.2/ozi/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/actions.py` & `OZI-1.2.2/ozi/actions.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/comment.py` & `OZI-1.2.2/ozi/comment.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/fix/__main__.py` & `OZI-1.2.2/ozi/fix/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/fix/build_definition.py` & `OZI-1.2.2/ozi/fix/build_definition.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/fix/meson.build` & `OZI-1.2.2/ozi/fix/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/fix/missing.py` & `OZI-1.2.2/ozi/fix/missing.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/fix/parser.py` & `OZI-1.2.2/ozi/fix/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/fix/rewrite_command.py` & `OZI-1.2.2/ozi/fix/rewrite_command.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/lint/meson.build` & `OZI-1.2.2/ozi/lint/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/lint/pyright/meson.build` & `OZI-1.2.2/ozi/lint/pyright/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/meson.build` & `OZI-1.2.2/ozi/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/meson.py` & `OZI-1.2.2/ozi/meson.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/new/__main__.py` & `OZI-1.2.2/ozi/new/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/new/meson.build` & `OZI-1.2.2/ozi/new/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/new/parser.py` & `OZI-1.2.2/ozi/new/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/new/validate.py` & `OZI-1.2.2/ozi/new/validate.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/pkg_extra.py` & `OZI-1.2.2/ozi/pkg_extra.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/render.py` & `OZI-1.2.2/ozi/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # ozi/render.py
 # Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
 # See LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
-"""Rendering utilities for the OZI project templates."""
+"""Rendering utilities for the OZI project templates.
+
+.. versionremoved:: 1.2
+   The function ``load_environment`` was moved to ``blastpipe.ozi_templates``
+
+"""
 from pathlib import Path
 from warnings import warn
 
 from blastpipe.ozi_templates.filter import underscorify  # pyright: ignore
 from git import InvalidGitRepositoryError
 from git import Repo
 from jinja2 import Environment
```

### Comparing `OZI-1.2.1/ozi/scripts/core_metadata_template.py` & `OZI-1.2.2/ozi/scripts/core_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/scripts/meson.build` & `OZI-1.2.2/ozi/scripts/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/scripts/meson_dist_setuptools_scm.py` & `OZI-1.2.2/ozi/scripts/meson_dist_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/scripts/meson_setuptools_scm.py` & `OZI-1.2.2/ozi/scripts/meson_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/scripts/render_requirements.py` & `OZI-1.2.2/ozi/scripts/render_requirements.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/scripts/replace_ruff_target_version.py` & `OZI-1.2.2/ozi/scripts/replace_ruff_target_version.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/scripts/scm_version_snip.py` & `OZI-1.2.2/ozi/scripts/scm_version_snip.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/scripts/to_distribution_template.py` & `OZI-1.2.2/ozi/scripts/to_distribution_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/scripts/version_metadata_template.py` & `OZI-1.2.2/ozi/scripts/version_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/spdx.py` & `OZI-1.2.2/ozi/spdx.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/spec/_license.py` & `OZI-1.2.2/ozi/spec/_license.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/spec/_spec.py` & `OZI-1.2.2/ozi/spec/_spec.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/spec/base.py` & `OZI-1.2.2/ozi/spec/base.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/spec/ci.py` & `OZI-1.2.2/ozi/spec/ci.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/spec/meson.build` & `OZI-1.2.2/ozi/spec/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/spec/pkg.py` & `OZI-1.2.2/ozi/spec/pkg.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/spec/project.py` & `OZI-1.2.2/ozi/spec/project.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/spec/python.py` & `OZI-1.2.2/ozi/spec/python.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/spec/src.py` & `OZI-1.2.2/ozi/spec/src.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/tap.py` & `OZI-1.2.2/ozi/tap.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/trove.py` & `OZI-1.2.2/ozi/trove.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/vendor/email_validator/__init__.py` & `OZI-1.2.2/ozi/vendor/email_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/vendor/email_validator/__main__.py` & `OZI-1.2.2/ozi/vendor/email_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/vendor/email_validator/deliverability.py` & `OZI-1.2.2/ozi/vendor/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/vendor/email_validator/exceptions_types.py` & `OZI-1.2.2/ozi/vendor/email_validator/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/vendor/email_validator/meson.build` & `OZI-1.2.2/ozi/vendor/email_validator/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/vendor/email_validator/rfc_constants.py` & `OZI-1.2.2/ozi/vendor/email_validator/rfc_constants.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/vendor/email_validator/syntax.py` & `OZI-1.2.2/ozi/vendor/email_validator/syntax.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/vendor/email_validator/validate_email.py` & `OZI-1.2.2/ozi/vendor/email_validator/validate_email.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/ozi/vendor/meson.build` & `OZI-1.2.2/ozi/vendor/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/pyproject.toml` & `OZI-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/templates/CHANGELOG.md.j2` & `OZI-1.2.2/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/tests/meson.build` & `OZI-1.2.2/tests/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/tests/test_ozi_fix.py` & `OZI-1.2.2/tests/test_ozi_fix.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/tests/test_ozi_new.py` & `OZI-1.2.2/tests/test_ozi_new.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.1/tests/test_tap.py` & `OZI-1.2.2/tests/test_tap.py`

 * *Files identical despite different names*

