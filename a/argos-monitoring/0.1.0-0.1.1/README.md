# Comparing `tmp/argos_monitoring-0.1.0.tar.gz` & `tmp/argos_monitoring-0.1.1.tar.gz`

## Comparing `argos_monitoring-0.1.0.tar` & `argos_monitoring-0.1.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/__init__.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/agent.py
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/commands.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/logging.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/checks/__init__.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/checks/base.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/checks/checks.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/schemas/__init__.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/schemas/config.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/schemas/models.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/schemas/utils.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/__init__.py
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/alerting.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/main.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/models.py
--rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/queries.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/settings.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/migrations/alembic.ini
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/migrations/env.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/migrations/script.py.mako
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/migrations/versions/1a3497f9f71b_adding_configcache_model.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/migrations/versions/7d480e6f1112_initial_migrations.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/migrations/versions/defda3f2952d_add_on_delete_cascade_to_results_task_id.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/migrations/versions/e99bc35702c9_add_severity_to_task_and_add_severity_.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/routes/__init__.py
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/routes/api.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/routes/dependencies.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/routes/views.py
--rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/static/logo-64.png
--rw-r--r--   0        0        0   164276 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/static/logo.png
--rw-r--r--   0        0        0    73571 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/static/pico.min.css
--rw-r--r--   0        0        0   201142 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/static/pico.min.css.map
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/static/styles.css
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/templates/agents.html
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/templates/base.html
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/templates/domain.html
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/templates/domains.html
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/templates/index.html
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/templates/result.html
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/argos/server/templates/results.html
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/api.md
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/changelog.md
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/checks.md
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/cli.md
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/conf.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/configuration.md
--rw-r--r--   0        0        0    69099 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/dashboard.jpg
--rw-r--r--   0        0        0   120332 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/domains.jpg
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/index.md
--rw-r--r--   0        0        0    27284 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/_static/font-inter-cyrillic-ext.woff2
--rw-r--r--   0        0        0    17600 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/_static/font-inter-cyrillic.woff2
--rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/_static/font-inter-greek-ext.woff2
--rw-r--r--   0        0        0    22480 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/_static/font-inter-greek.woff2
--rw-r--r--   0        0        0    79940 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/_static/font-inter-latin-ext.woff2
--rw-r--r--   0        0        0    46704 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/_static/font-inter-latin.woff2
--rw-r--r--   0        0        0    10540 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/_static/font-inter-vietnamese.woff2
--rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/_static/fonts.css
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/_templates/repository.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/_templates/partials/webfonts.html
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/deployment/nginx.md
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/deployment/systemd.md
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/developer/dependencies.md
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/developer/installation.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/developer/migrations.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/developer/models.md
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/developer/new-check.md
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/developer/overview.md
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/developer/release.md
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/developer/requirements.md
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/developer/tests.md
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/installation/getting-started.md
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/docs/installation/postgresql.md
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/tests/test_api.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/tests/test_checks.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/tests/test_checks_base.py
--rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/tests/test_queries.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/tests/test_schemas_config.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/tests/test_schemas_utils.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/tests/websites.yaml
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/.gitignore
--rw-r--r--   0        0        0    34520 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/LICENSE
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/README.md
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 argos_monitoring-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/__init__.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/agent.py
+-rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/commands.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/logging.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/checks/__init__.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/checks/base.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/checks/checks.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/schemas/__init__.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/schemas/config.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/schemas/models.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/schemas/utils.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/__init__.py
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/alerting.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/main.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/models.py
+-rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/queries.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/settings.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/migrations/alembic.ini
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/migrations/env.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/migrations/script.py.mako
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/migrations/versions/1a3497f9f71b_adding_configcache_model.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/migrations/versions/7d480e6f1112_initial_migrations.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/migrations/versions/defda3f2952d_add_on_delete_cascade_to_results_task_id.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/migrations/versions/e99bc35702c9_add_severity_to_task_and_add_severity_.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/routes/__init__.py
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/routes/api.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/routes/dependencies.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/routes/views.py
+-rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/static/logo-64.png
+-rw-r--r--   0        0        0   164276 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/static/logo.png
+-rw-r--r--   0        0        0    73571 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/static/pico.min.css
+-rw-r--r--   0        0        0   201142 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/static/pico.min.css.map
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/static/styles.css
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/templates/agents.html
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/templates/base.html
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/templates/domain.html
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/templates/domains.html
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/templates/index.html
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/templates/result.html
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/argos/server/templates/results.html
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/api.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/changelog.md
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/checks.md
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/cli.md
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/configuration.md
+-rw-r--r--   0        0        0    69099 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/dashboard.jpg
+-rw-r--r--   0        0        0   120332 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/domains.jpg
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/index.md
+-rw-r--r--   0        0        0    27284 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/_static/font-inter-cyrillic-ext.woff2
+-rw-r--r--   0        0        0    17600 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/_static/font-inter-cyrillic.woff2
+-rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/_static/font-inter-greek-ext.woff2
+-rw-r--r--   0        0        0    22480 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/_static/font-inter-greek.woff2
+-rw-r--r--   0        0        0    79940 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/_static/font-inter-latin-ext.woff2
+-rw-r--r--   0        0        0    46704 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/_static/font-inter-latin.woff2
+-rw-r--r--   0        0        0    10540 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/_static/font-inter-vietnamese.woff2
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/_static/fonts.css
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/_templates/repository.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/_templates/partials/webfonts.html
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/deployment/nginx.md
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/deployment/systemd.md
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/developer/dependencies.md
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/developer/installation.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/developer/migrations.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/developer/models.md
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/developer/new-check.md
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/developer/overview.md
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/developer/release.md
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/developer/requirements.md
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/developer/tests.md
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/installation/getting-started.md
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/docs/installation/postgresql.md
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/tests/test_api.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/tests/test_checks.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/tests/test_checks_base.py
+-rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/tests/test_queries.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/tests/test_schemas_config.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/tests/test_schemas_utils.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/tests/websites.yaml
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/.gitignore
+-rw-r--r--   0        0        0    34520 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/README.md
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 argos_monitoring-0.1.1/PKG-INFO
```

### Comparing `argos_monitoring-0.1.0/argos/agent.py` & `argos_monitoring-0.1.1/argos/agent.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/commands.py` & `argos_monitoring-0.1.1/argos/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,24 @@
     @wraps(f)
     def wrapper(*args, **kwargs):
         return asyncio.run(f(*args, **kwargs))
 
     return wrapper
 
 
+def validate_config_access(ctx, param, value):
+    if os.path.isfile(value) and os.access(value, os.R_OK):
+        return value
+
+    if os.path.isfile(value):
+        raise click.BadParameter(f"the file {value} is not readabale.")
+
+    raise click.BadParameter(f"the file {value} does not exists or is not reachable.")
+
+
 @click.group()
 def cli():
     pass
 
 
 @cli.group()
 def server():
@@ -89,14 +99,15 @@
 @click.option("--port", default=8000, type=int, help="Port to bind")
 @click.option(
     "--config",
     default="config.yaml",
     help="Path of the configuration file. "
     "If ARGOS_YAML_FILE environment variable is set, its value will be used instead.",
     envvar="ARGOS_YAML_FILE",
+    callback=validate_config_access,
 )
 @click.option("--reload", is_flag=True, help="Enable hot reloading")
 def start(host, port, config, reload):
     """Starts the server (use only for testing or development!)
 
     See https://framasoft.frama.io/framaspace/argos/deployment/systemd.html#server
     for advices on how to start the server for production.
@@ -136,28 +147,30 @@
 )
 @click.option(
     "--config",
     default="config.yaml",
     help="Path of the configuration file. "
     "If ARGOS_YAML_FILE environment variable is set, its value will be used instead.",
     envvar="ARGOS_YAML_FILE",
+    callback=validate_config_access,
 )
 @coroutine
 async def cleandb(max_results, max_lock_seconds, config):
     """Clean the database (to run routinely)
 
     \b
     - Removes old results from the database.
     - Removes locks from tasks that have been locked for too long.
     """
+    # It’s mandatory to do it before the imports
+    os.environ["ARGOS_YAML_FILE"] = config
+
     # The imports are made here otherwise the agent will need server configuration files.
     from argos.server import queries
 
-    os.environ["ARGOS_YAML_FILE"] = config
-
     db = await get_db()
     removed = await queries.remove_old_results(db, max_results)
     updated = await queries.release_old_locks(db, max_lock_seconds)
 
     click.echo(f"{removed} results removed")
     click.echo(f"{updated} locks released")
 
@@ -165,25 +178,27 @@
 @server.command(short_help="Load or reload tasks’ configuration")
 @click.option(
     "--config",
     default="config.yaml",
     help="Path of the configuration file. "
     "If ARGOS_YAML_FILE environment variable is set, its value will be used instead.",
     envvar="ARGOS_YAML_FILE",
+    callback=validate_config_access,
 )
 @coroutine
 async def reload_config(config):
     """Read tasks’ configuration and add/delete tasks in database if needed"""
+    # It’s mandatory to do it before the imports
+    os.environ["ARGOS_YAML_FILE"] = config
+
     # The imports are made here otherwise the agent will need server configuration files.
     from argos.server import queries
     from argos.server.main import get_application, read_config
     from argos.server.settings import get_app_settings
 
-    os.environ["ARGOS_YAML_FILE"] = config
-
     appli = get_application()
     settings = get_app_settings()
     config = read_config(appli, settings)
 
     db = await get_db()
     changed = await queries.update_from_config(db, config)
 
@@ -194,23 +209,25 @@
 @server.command()
 @click.option(
     "--config",
     default="config.yaml",
     help="Path of the configuration file. "
     "If ARGOS_YAML_FILE environment variable is set, its value will be used instead.",
     envvar="ARGOS_YAML_FILE",
+    callback=validate_config_access,
 )
 @coroutine
 async def migrate(config):
     """Run database migrations"""
+    # It’s mandatory to do it before the imports
+    os.environ["ARGOS_YAML_FILE"] = config
+
     # The imports are made here otherwise the agent will need server configuration files.
     from argos.server.settings import get_app_settings
 
-    os.environ["ARGOS_YAML_FILE"] = config
-
     settings = get_app_settings()
 
     current_dir = os.path.dirname(__file__)
     alembic_cfg = Config(os.path.join(current_dir, "server/migrations/alembic.ini"))
     alembic_cfg.set_main_option("sqlalchemy.url", settings.database_url)
     command.upgrade(alembic_cfg, "head")
```

### Comparing `argos_monitoring-0.1.0/argos/checks/base.py` & `argos_monitoring-0.1.1/argos/checks/base.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/checks/checks.py` & `argos_monitoring-0.1.1/argos/checks/checks.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/schemas/config.py` & `argos_monitoring-0.1.1/argos/schemas/config.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/schemas/models.py` & `argos_monitoring-0.1.1/argos/schemas/models.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/schemas/utils.py` & `argos_monitoring-0.1.1/argos/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/alerting.py` & `argos_monitoring-0.1.1/argos/server/alerting.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/main.py` & `argos_monitoring-0.1.1/argos/server/main.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/models.py` & `argos_monitoring-0.1.1/argos/server/models.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/queries.py` & `argos_monitoring-0.1.1/argos/server/queries.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/settings.py` & `argos_monitoring-0.1.1/argos/server/settings.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/migrations/alembic.ini` & `argos_monitoring-0.1.1/argos/server/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/migrations/env.py` & `argos_monitoring-0.1.1/argos/server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/migrations/script.py.mako` & `argos_monitoring-0.1.1/argos/server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/migrations/versions/1a3497f9f71b_adding_configcache_model.py` & `argos_monitoring-0.1.1/argos/server/migrations/versions/1a3497f9f71b_adding_configcache_model.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/migrations/versions/7d480e6f1112_initial_migrations.py` & `argos_monitoring-0.1.1/argos/server/migrations/versions/7d480e6f1112_initial_migrations.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/migrations/versions/defda3f2952d_add_on_delete_cascade_to_results_task_id.py` & `argos_monitoring-0.1.1/argos/server/migrations/versions/defda3f2952d_add_on_delete_cascade_to_results_task_id.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/migrations/versions/e99bc35702c9_add_severity_to_task_and_add_severity_.py` & `argos_monitoring-0.1.1/argos/server/migrations/versions/e99bc35702c9_add_severity_to_task_and_add_severity_.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/routes/api.py` & `argos_monitoring-0.1.1/argos/server/routes/api.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/routes/dependencies.py` & `argos_monitoring-0.1.1/argos/server/routes/dependencies.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/routes/views.py` & `argos_monitoring-0.1.1/argos/server/routes/views.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/static/logo-64.png` & `argos_monitoring-0.1.1/argos/server/static/logo-64.png`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/static/logo.png` & `argos_monitoring-0.1.1/argos/server/static/logo.png`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/static/pico.min.css` & `argos_monitoring-0.1.1/argos/server/static/pico.min.css`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/static/pico.min.css.map` & `argos_monitoring-0.1.1/argos/server/static/pico.min.css.map`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/static/styles.css` & `argos_monitoring-0.1.1/argos/server/static/styles.css`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/templates/base.html` & `argos_monitoring-0.1.1/argos/server/templates/base.html`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/templates/domain.html` & `argos_monitoring-0.1.1/argos/server/templates/domain.html`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/templates/domains.html` & `argos_monitoring-0.1.1/argos/server/templates/domains.html`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/templates/index.html` & `argos_monitoring-0.1.1/argos/server/templates/index.html`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/argos/server/templates/results.html` & `argos_monitoring-0.1.1/argos/server/templates/results.html`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/api.md` & `argos_monitoring-0.1.1/docs/api.md`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/checks.md` & `argos_monitoring-0.1.1/docs/checks.md`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/cli.md` & `argos_monitoring-0.1.1/docs/cli.md`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/conf.py` & `argos_monitoring-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/configuration.md` & `argos_monitoring-0.1.1/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/dashboard.jpg` & `argos_monitoring-0.1.1/docs/dashboard.jpg`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/domains.jpg` & `argos_monitoring-0.1.1/docs/domains.jpg`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/index.md` & `argos_monitoring-0.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/_static/font-inter-cyrillic-ext.woff2` & `argos_monitoring-0.1.1/docs/_static/font-inter-cyrillic-ext.woff2`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/_static/font-inter-cyrillic.woff2` & `argos_monitoring-0.1.1/docs/_static/font-inter-cyrillic.woff2`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/_static/font-inter-greek-ext.woff2` & `argos_monitoring-0.1.1/docs/_static/font-inter-greek-ext.woff2`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/_static/font-inter-greek.woff2` & `argos_monitoring-0.1.1/docs/_static/font-inter-greek.woff2`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/_static/font-inter-latin-ext.woff2` & `argos_monitoring-0.1.1/docs/_static/font-inter-latin-ext.woff2`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/_static/font-inter-latin.woff2` & `argos_monitoring-0.1.1/docs/_static/font-inter-latin.woff2`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/_static/font-inter-vietnamese.woff2` & `argos_monitoring-0.1.1/docs/_static/font-inter-vietnamese.woff2`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/_static/fonts.css` & `argos_monitoring-0.1.1/docs/_static/fonts.css`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/developer/dependencies.md` & `argos_monitoring-0.1.1/docs/developer/dependencies.md`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/developer/migrations.md` & `argos_monitoring-0.1.1/docs/developer/migrations.md`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/developer/models.md` & `argos_monitoring-0.1.1/docs/developer/models.md`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/developer/new-check.md` & `argos_monitoring-0.1.1/docs/developer/new-check.md`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/developer/overview.md` & `argos_monitoring-0.1.1/docs/developer/overview.md`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/developer/release.md` & `argos_monitoring-0.1.1/docs/developer/release.md`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/docs/installation/getting-started.md` & `argos_monitoring-0.1.1/docs/installation/getting-started.md`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/tests/conftest.py` & `argos_monitoring-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/tests/test_api.py` & `argos_monitoring-0.1.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/tests/test_checks.py` & `argos_monitoring-0.1.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/tests/test_checks_base.py` & `argos_monitoring-0.1.1/tests/test_checks_base.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/tests/test_queries.py` & `argos_monitoring-0.1.1/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/tests/test_schemas_config.py` & `argos_monitoring-0.1.1/tests/test_schemas_config.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/tests/test_schemas_utils.py` & `argos_monitoring-0.1.1/tests/test_schemas_utils.py`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/LICENSE` & `argos_monitoring-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/README.md` & `argos_monitoring-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/pyproject.toml` & `argos_monitoring-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `argos_monitoring-0.1.0/PKG-INFO` & `argos_monitoring-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: argos-monitoring
-Version: 0.1.0
+Version: 0.1.1
 Summary: Distributed supervision tool for HTTP.
 Project-URL: homepage, https://framasoft.frama.io/framaspace/argos/
 Project-URL: repository, https://framagit.org/framasoft/framaspace/argos
 Project-URL: Funding, https://framasoft.org/en/#support
 Project-URL: Tracker, https://framagit.org/framasoft/framaspace/argos/-/issues
 Author-email: Alexis Métaireau <alexis@notmyidea.org>, Luc Didry <luc+argos@framasoft.org>
 License-File: LICENSE
```

