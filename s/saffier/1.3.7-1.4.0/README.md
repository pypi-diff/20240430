# Comparing `tmp/saffier-1.3.7.tar.gz` & `tmp/saffier-1.4.0.tar.gz`

## Comparing `saffier-1.3.7.tar` & `saffier-1.4.0.tar`

### file list

```diff
@@ -1,118 +1,119 @@
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/__init__.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/__main__.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/exceptions.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/py.typed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/testclient.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/types.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/__init__.py
--rw-r--r--   0        0        0    11167 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/base.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/cli.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/constants.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/decorators.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/env.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/__init__.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/branches.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/check.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/current.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/downgrade.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/edit.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/heads.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/history.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/init.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/inspectdb.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/list_templates.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/makemigrations.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/merge.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/migrate.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/revision.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/show.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/stamp.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/shell/__init__.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/shell/enums.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/shell/ipython.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/shell/ptpython.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/operations/shell/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/templates/default/README
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/templates/default/alembic.ini.mako
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/templates/default/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/cli/templates/default/script.py.mako
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/conf/enums.py
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/conf/functional.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/conf/global_settings.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/conf/module_import.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/contrib/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/contrib/multi_tenancy/__init__.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/contrib/multi_tenancy/base.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/contrib/multi_tenancy/exceptions.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/contrib/multi_tenancy/metaclasses.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/contrib/multi_tenancy/models.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/contrib/multi_tenancy/registry.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/contrib/multi_tenancy/settings.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/contrib/multi_tenancy/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/contrib/sqlalchemy/fields.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/contrib/sqlalchemy/protocols.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/contrib/sqlalchemy/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/__init__.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/datastructures.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/events.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/connection/__init__.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/connection/database.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/connection/registry.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/connection/schemas.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/constants.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/context_vars.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/datastructures.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/fields/__init__.py
--rw-r--r--   0        0        0    15920 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/fields/_internal.py
--rw-r--r--   0        0        0    17253 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/fields/base.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/models/__init__.py
--rw-r--r--   0        0        0     9071 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/models/base.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/models/managers.py
--rw-r--r--   0        0        0    18975 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/models/metaclasses.py
--rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/models/model.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/models/model_proxy.py
--rw-r--r--   0        0        0    11786 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/models/row.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/models/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/models/mixins/__init__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/models/mixins/generics.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/querysets/__init__.py
--rw-r--r--   0        0        0    38799 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/querysets/base.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/querysets/clauses.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/querysets/mixins.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/querysets/prefetch.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/querysets/protocols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/relationships/__init__.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/relationships/related.py
--rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/db/relationships/relation.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/extras/__init__.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/extras/base.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/extras/extra.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/signals/__init__.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/signals/handlers.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/signals/signal.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/terminal/__init__.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/terminal/base.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/terminal/print.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/terminal/terminal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/utils/__init__.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/utils/base.py
--rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/utils/formats.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/utils/models.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/utils/schemas.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/utils/sync.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/core/utils/unique.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/protocols/__init__.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/protocols/many_relationship.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/protocols/queryset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/utils/__init__.py
--rw-r--r--   0        0        0    12013 2020-02-02 00:00:00.000000 saffier-1.3.7/saffier/utils/inspect.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-1.3.7/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-1.3.7/LICENSE
--rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 saffier-1.3.7/README.md
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 saffier-1.3.7/pyproject.toml
--rw-r--r--   0        0        0    12657 2020-02-02 00:00:00.000000 saffier-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/__init__.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/__main__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/exceptions.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/py.typed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/testclient.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/types.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/__init__.py
+-rw-r--r--   0        0        0    12795 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/base.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/cli.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/constants.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/decorators.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/env.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/__init__.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/branches.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/check.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/current.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/downgrade.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/edit.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/heads.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/history.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/init.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/inspectdb.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/list_templates.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/makemigrations.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/merge.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/migrate.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/revision.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/show.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/stamp.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/shell/__init__.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/shell/enums.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/operations/shell/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/templates/default/README
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/templates/default/alembic.ini.mako
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/templates/default/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/cli/templates/default/script.py.mako
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/conf/enums.py
+-rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/conf/functional.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/conf/global_settings.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/conf/module_import.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/contrib/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/contrib/multi_tenancy/__init__.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/contrib/multi_tenancy/base.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/contrib/multi_tenancy/exceptions.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/contrib/multi_tenancy/metaclasses.py
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/contrib/multi_tenancy/models.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/contrib/multi_tenancy/registry.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/contrib/multi_tenancy/settings.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/contrib/multi_tenancy/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/contrib/sqlalchemy/fields.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/contrib/sqlalchemy/protocols.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/contrib/sqlalchemy/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/__init__.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/datastructures.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/events.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/connection/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/connection/database.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/connection/registry.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/connection/schemas.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/constants.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/context_vars.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/datastructures.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/fields/__init__.py
+-rw-r--r--   0        0        0    15920 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/fields/_internal.py
+-rw-r--r--   0        0        0    17225 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/fields/base.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/models/__init__.py
+-rw-r--r--   0        0        0     9071 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/models/base.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/models/managers.py
+-rw-r--r--   0        0        0    18975 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/models/metaclasses.py
+-rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/models/model.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/models/model_proxy.py
+-rw-r--r--   0        0        0    11786 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/models/row.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/models/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/models/mixins/__init__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/models/mixins/generics.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/querysets/__init__.py
+-rw-r--r--   0        0        0    38799 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/querysets/base.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/querysets/clauses.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/querysets/mixins.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/querysets/prefetch.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/querysets/protocols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/relationships/__init__.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/relationships/related.py
+-rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/db/relationships/relation.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/extras/__init__.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/extras/base.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/extras/extra.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/signals/__init__.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/signals/handlers.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/signals/signal.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/terminal/base.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/terminal/print.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/terminal/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/utils/__init__.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/utils/base.py
+-rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/utils/formats.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/utils/models.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/utils/schemas.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/utils/sync.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/core/utils/unique.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/protocols/__init__.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/protocols/many_relationship.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/protocols/queryset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/utils/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/utils/compat.py
+-rw-r--r--   0        0        0    12013 2020-02-02 00:00:00.000000 saffier-1.4.0/saffier/utils/inspect.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-1.4.0/LICENSE
+-rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 saffier-1.4.0/README.md
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 saffier-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12658 2020-02-02 00:00:00.000000 saffier-1.4.0/PKG-INFO
```

### Comparing `saffier-1.3.7/saffier/__init__.py` & `saffier-1.4.0/saffier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.7"
+__version__ = "1.4.0"
 
 from saffier.conf import settings
 from saffier.conf.global_settings import SaffierSettings
 
 from .cli import Migrate
 from .core.connection.database import Database
 from .core.connection.registry import Registry
```

### Comparing `saffier-1.3.7/saffier/exceptions.py` & `saffier-1.4.0/saffier/exceptions.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/base.py` & `saffier-1.4.0/saffier/cli/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import argparse
+import inspect
 import os
 import typing
-from typing import TYPE_CHECKING, Any, Callable, Optional
+import warnings
+from importlib import import_module
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional
 
 from alembic import __version__ as __alembic_version__
 from alembic import command
 from alembic.config import Config as AlembicConfig
 
 from saffier.cli.constants import DEFAULT_TEMPLATE_NAME, SAFFIER_DB
 from saffier.cli.decorators import catch_errors
 from saffier.core.extras.base import BaseExtra
+from saffier.utils.compat import is_class_and_subclass
 
 if TYPE_CHECKING:
     from saffier.core.connection.registry import Registry
 
 alembic_version = tuple(int(v) for v in __alembic_version__.split(".")[0:3])
 object_setattr = object.__setattr__
 
@@ -55,30 +59,72 @@
     if there isn't any.
     """
 
     def __init__(
         self,
         app: typing.Any,
         registry: "Registry",
+        model_apps: Dict[str, str] = None,
         compare_type: bool = True,
         render_as_batch: bool = True,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
 
         self.app = app
         self.configure_callbacks: typing.List[Callable] = []
         self.registry = registry
+        self.model_apps = model_apps or {}
+
+        assert isinstance(
+            self.model_apps, dict
+        ), "`model_apps` must be a dict of 'app_name:location' format."
+
+        models = self.check_db_models(self.model_apps)
+
+        for name, _ in models.items():
+            if name in self.registry.models:
+                warnings.warn(
+                    f"There is already a model with the name {name} declared. Overriding the model will occur unless you rename it.",
+                    stacklevel=2,
+                )
+
+        if self.registry.models:
+            self.registry.models = {**models, **self.registry.models}
+        else:
+            self.registry.models = models
+
         self.directory = "migrations"
         self.alembic_ctx_kwargs = kwargs
         self.alembic_ctx_kwargs["compare_type"] = compare_type
         self.alembic_ctx_kwargs["render_as_batch"] = render_as_batch
 
         self.set_saffier_extension(app)
 
+    def check_db_models(self, model_apps: Dict[str, str]) -> Dict[str, Any]:
+        """
+        Goes through all the model applications declared in the migrate and
+        adds them into the registry.
+        """
+        from saffier.core.db.models import Model, ReflectModel
+
+        models: Dict[str, Any] = {}
+
+        for _, location in model_apps.items():
+            module = import_module(location)
+            members = inspect.getmembers(
+                module,
+                lambda attr: is_class_and_subclass(attr, Model)
+                and not attr.meta.abstract
+                and not is_class_and_subclass(attr, ReflectModel),
+            )
+            for name, model in members:
+                models[name] = model
+        return models
+
     def set_saffier_extension(self, app: Any) -> None:
         """
         Sets a saffier dictionary for the app object.
         """
         migrate = MigrateConfig(self, self.registry, **self.alembic_ctx_kwargs)
         object_setattr(app, SAFFIER_DB, {})
         app._saffier_db["migrate"] = migrate
```

### Comparing `saffier-1.3.7/saffier/cli/cli.py` & `saffier-1.4.0/saffier/cli/cli.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/env.py` & `saffier-1.4.0/saffier/cli/env.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/__init__.py` & `saffier-1.4.0/saffier/cli/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/branches.py` & `saffier-1.4.0/saffier/cli/operations/branches.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/downgrade.py` & `saffier-1.4.0/saffier/cli/operations/downgrade.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/heads.py` & `saffier-1.4.0/saffier/cli/operations/heads.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/history.py` & `saffier-1.4.0/saffier/cli/operations/history.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/init.py` & `saffier-1.4.0/saffier/cli/operations/init.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/inspectdb.py` & `saffier-1.4.0/saffier/cli/operations/inspectdb.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/makemigrations.py` & `saffier-1.4.0/saffier/cli/operations/makemigrations.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/merge.py` & `saffier-1.4.0/saffier/cli/operations/merge.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/migrate.py` & `saffier-1.4.0/saffier/cli/operations/migrate.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/revision.py` & `saffier-1.4.0/saffier/cli/operations/revision.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/stamp.py` & `saffier-1.4.0/saffier/cli/operations/stamp.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/shell/base.py` & `saffier-1.4.0/saffier/cli/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/shell/ipython.py` & `saffier-1.4.0/saffier/cli/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/shell/ptpython.py` & `saffier-1.4.0/saffier/cli/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/operations/shell/utils.py` & `saffier-1.4.0/saffier/cli/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/templates/default/alembic.ini.mako` & `saffier-1.4.0/saffier/cli/templates/default/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/cli/templates/default/env.py` & `saffier-1.4.0/saffier/cli/templates/default/env.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/conf/__init__.py` & `saffier-1.4.0/saffier/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/conf/functional.py` & `saffier-1.4.0/saffier/conf/functional.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/conf/global_settings.py` & `saffier-1.4.0/saffier/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/conf/module_import.py` & `saffier-1.4.0/saffier/conf/module_import.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/contrib/multi_tenancy/base.py` & `saffier-1.4.0/saffier/contrib/multi_tenancy/base.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/contrib/multi_tenancy/metaclasses.py` & `saffier-1.4.0/saffier/contrib/multi_tenancy/metaclasses.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/contrib/multi_tenancy/models.py` & `saffier-1.4.0/saffier/contrib/multi_tenancy/models.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/contrib/multi_tenancy/settings.py` & `saffier-1.4.0/saffier/contrib/multi_tenancy/settings.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/contrib/multi_tenancy/utils.py` & `saffier-1.4.0/saffier/contrib/multi_tenancy/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/contrib/sqlalchemy/fields.py` & `saffier-1.4.0/saffier/contrib/sqlalchemy/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/contrib/sqlalchemy/protocols.py` & `saffier-1.4.0/saffier/contrib/sqlalchemy/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/datastructures.py` & `saffier-1.4.0/saffier/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/events.py` & `saffier-1.4.0/saffier/core/events.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/sync.py` & `saffier-1.4.0/saffier/core/sync.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/connection/database.py` & `saffier-1.4.0/saffier/core/connection/database.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/connection/registry.py` & `saffier-1.4.0/saffier/core/connection/registry.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/connection/schemas.py` & `saffier-1.4.0/saffier/core/connection/schemas.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/context_vars.py` & `saffier-1.4.0/saffier/core/db/context_vars.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/datastructures.py` & `saffier-1.4.0/saffier/core/db/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/fields/__init__.py` & `saffier-1.4.0/saffier/core/db/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/fields/_internal.py` & `saffier-1.4.0/saffier/core/db/fields/_internal.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/fields/base.py` & `saffier-1.4.0/saffier/core/db/fields/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,20 @@
     Boolean,
     Date,
     DateTime,
     Decimal,
     Email,
     Float,
     Integer,
+    Password,
+    SaffierField,
+    String,
+    Time,
 )
 from saffier.core.db.fields._internal import IPAddress as CoreIPAddress
-from saffier.core.db.fields._internal import Password, SaffierField, String, Time
 from saffier.core.terminal import Print
 
 if typing.TYPE_CHECKING:
     from saffier import Model
 
 terminal = Print()
 CHAR_LIMIT = 63
```

### Comparing `saffier-1.3.7/saffier/core/db/models/base.py` & `saffier-1.4.0/saffier/core/db/models/base.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/models/managers.py` & `saffier-1.4.0/saffier/core/db/models/managers.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/models/metaclasses.py` & `saffier-1.4.0/saffier/core/db/models/metaclasses.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/models/model.py` & `saffier-1.4.0/saffier/core/db/models/model.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/models/model_proxy.py` & `saffier-1.4.0/saffier/core/db/models/model_proxy.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/models/row.py` & `saffier-1.4.0/saffier/core/db/models/row.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/models/utils.py` & `saffier-1.4.0/saffier/core/db/models/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/models/mixins/generics.py` & `saffier-1.4.0/saffier/core/db/models/mixins/generics.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/querysets/base.py` & `saffier-1.4.0/saffier/core/db/querysets/base.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/querysets/clauses.py` & `saffier-1.4.0/saffier/core/db/querysets/clauses.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/querysets/mixins.py` & `saffier-1.4.0/saffier/core/db/querysets/mixins.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/querysets/prefetch.py` & `saffier-1.4.0/saffier/core/db/querysets/prefetch.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/relationships/related.py` & `saffier-1.4.0/saffier/core/db/relationships/related.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/db/relationships/relation.py` & `saffier-1.4.0/saffier/core/db/relationships/relation.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/extras/extra.py` & `saffier-1.4.0/saffier/core/extras/extra.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/signals/handlers.py` & `saffier-1.4.0/saffier/core/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/signals/signal.py` & `saffier-1.4.0/saffier/core/signals/signal.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/terminal/base.py` & `saffier-1.4.0/saffier/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/terminal/print.py` & `saffier-1.4.0/saffier/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/terminal/terminal.py` & `saffier-1.4.0/saffier/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/utils/base.py` & `saffier-1.4.0/saffier/core/utils/base.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/utils/formats.py` & `saffier-1.4.0/saffier/core/utils/formats.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/utils/models.py` & `saffier-1.4.0/saffier/core/utils/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import typing
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Type
 
-from orjson import OPT_OMIT_MICROSECONDS  # noqa
-from orjson import OPT_SERIALIZE_NUMPY  # noqa
-from orjson import dumps
+from orjson import (
+    OPT_OMIT_MICROSECONDS,  # noqa
+    OPT_SERIALIZE_NUMPY,  # noqa
+    dumps,
+)
 
 import saffier
 from saffier.core.db.fields import DateField, DateTimeField
 
 saffier_setattr = object.__setattr__
 
 if TYPE_CHECKING:
```

### Comparing `saffier-1.3.7/saffier/core/utils/schemas.py` & `saffier-1.4.0/saffier/core/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/core/utils/unique.py` & `saffier-1.4.0/saffier/core/utils/unique.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/protocols/many_relationship.py` & `saffier-1.4.0/saffier/protocols/many_relationship.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/protocols/queryset.py` & `saffier-1.4.0/saffier/protocols/queryset.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/saffier/utils/inspect.py` & `saffier-1.4.0/saffier/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/LICENSE` & `saffier-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saffier-1.3.7/README.md` & `saffier-1.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 weaknesses and specific use cases.
 
 This ORM is built on the top of SQLAlchemy core and aims to simplify the way the setup and queries
 are done into a more common and familiar interface.
 
 ## Before continuing
 
-If you are looking for something more **Pyadntic** oriented where you can take literally advantage
+If you are looking for something more **Pydantic** oriented where you can take literally advantage
 of everything that Pydantic can offer, then instead of continuing with Saffier, have a look at
 its ***data ORM brother***, [Edgy](https://edgy.tarsild.io).
 
 **Edgy** its extremely powerful as well with a key difference that its **100% Pydantic** which means
 you can leverage the technology if you already familiar with it.
 
 No worries, it is not completely different from Saffier, in fact, it was designed with the same principles and what it changes for you
```

### Comparing `saffier-1.3.7/pyproject.toml` & `saffier-1.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -74,22 +74,22 @@
 [project.scripts]
 saffier = "saffier.__main__:run_cli"
 
 [project.optional-dependencies]
 test = [
     "asyncpg>=0.27.0,<1",
     "asyncmy>=0.2.7,<0.3.0",
-    "esmerald>=2.0.0",
+    "esmerald>=3.0.0",
     "httpx>=0.25.0,<0.30.0",
     "pytest>=7.1.3,<9.0.0",
-    "pytest-cov>=2.12.0,<5.0.0",
+    "pytest-cov>=2.12.0,<6.0.0",
     "pytest-asyncio >=0.19.0",
-    "mypy==1.8.0",
+    "mypy==1.10.0",
     "flake8>=5.0.4",
-    "black==24.2.0",
+    "black==24.4.2",
     "isort>=5.0.6,<6.0.0",
     "freezegun>=1.2.2,<2.0.0",
     "mock==5.1.0",
     "pymysql>=1.0.2,<2.0.0",
     "types-orjson==3.6.2",
     "ruff>=0.0.256,<1.0.0",
 ]
@@ -147,27 +147,17 @@
 no_implicit_optional = false
 show_error_codes = true
 disallow_incomplete_defs = true
 disable_error_code = "attr-defined,arg-type,override,misc"
 warn_unused_ignores = true
 warn_redundant_casts = true
 
-[tool.ruff]
-select = [
-    "E", # pycodestyle errors
-    "W", # pycodestyle warnings
-    "F", # pyflakes
-    "C", # flake8-comprehensions
-    "B", # flake8-bugbear
-]
-ignore = [
-    "E501", # line too long, handled by black
-    "B008", # do not perform function calls in argument defaults
-    "C901", # too complex
-]
+[tool.ruff.lint]
+select = ["E", "W", "F", "C", "B", "I"]
+ignore = ["E501", "B008", "C901", "B026"]
 
 exclude = ["docs_src/*"]
 
 [[tool.mypy.overrides]]
 module = "saffier.tests.*"
 ignore_missing_imports = true
 check_untyped_defs = true
```

### Comparing `saffier-1.3.7/PKG-INFO` & `saffier-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: saffier
-Version: 1.3.7
+Version: 1.4.0
 Summary: The only python ORM you will ever need.
 Project-URL: Homepage, https://github.com/tarsil/saffier
 Project-URL: Documentation, https://saffier.tarsild.io/
 Project-URL: Changelog, https://saffier.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/saffier
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -76,25 +76,25 @@
 Provides-Extra: ptpython
 Requires-Dist: ptpython<4.0.0,>=3.0.23; extra == 'ptpython'
 Provides-Extra: sqlite
 Requires-Dist: databasez[sqlite]; extra == 'sqlite'
 Provides-Extra: test
 Requires-Dist: asyncmy<0.3.0,>=0.2.7; extra == 'test'
 Requires-Dist: asyncpg<1,>=0.27.0; extra == 'test'
-Requires-Dist: black==24.2.0; extra == 'test'
-Requires-Dist: esmerald>=2.0.0; extra == 'test'
+Requires-Dist: black==24.4.2; extra == 'test'
+Requires-Dist: esmerald>=3.0.0; extra == 'test'
 Requires-Dist: flake8>=5.0.4; extra == 'test'
 Requires-Dist: freezegun<2.0.0,>=1.2.2; extra == 'test'
 Requires-Dist: httpx<0.30.0,>=0.25.0; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'test'
 Requires-Dist: mock==5.1.0; extra == 'test'
-Requires-Dist: mypy==1.8.0; extra == 'test'
+Requires-Dist: mypy==1.10.0; extra == 'test'
 Requires-Dist: pymysql<2.0.0,>=1.0.2; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.19.0; extra == 'test'
-Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
+Requires-Dist: pytest-cov<6.0.0,>=2.12.0; extra == 'test'
 Requires-Dist: pytest<9.0.0,>=7.1.3; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
 Requires-Dist: types-orjson==3.6.2; extra == 'test'
 Provides-Extra: testing
 Requires-Dist: sqlalchemy-utils>=0.40.0; extra == 'testing'
 Description-Content-Type: text/markdown
 
@@ -140,15 +140,15 @@
 weaknesses and specific use cases.
 
 This ORM is built on the top of SQLAlchemy core and aims to simplify the way the setup and queries
 are done into a more common and familiar interface.
 
 ## Before continuing
 
-If you are looking for something more **Pyadntic** oriented where you can take literally advantage
+If you are looking for something more **Pydantic** oriented where you can take literally advantage
 of everything that Pydantic can offer, then instead of continuing with Saffier, have a look at
 its ***data ORM brother***, [Edgy](https://edgy.tarsild.io).
 
 **Edgy** its extremely powerful as well with a key difference that its **100% Pydantic** which means
 you can leverage the technology if you already familiar with it.
 
 No worries, it is not completely different from Saffier, in fact, it was designed with the same principles and what it changes for you
```

