# Comparing `tmp/dbt_postgres-1.8.0b4.tar.gz` & `tmp/dbt_postgres-1.8.0b5.tar.gz`

## Comparing `dbt_postgres-1.8.0b4.tar` & `dbt_postgres-1.8.0b5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/adapters/postgres/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/adapters/postgres/__version__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/adapters/postgres/column.py
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/adapters/postgres/connections.py
--rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/adapters/postgres/impl.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/adapters/postgres/relation.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/adapters/postgres/relation_configs/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/adapters/postgres/relation_configs/constants.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/adapters/postgres/relation_configs/index.py
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/adapters/postgres/relation_configs/materialized_view.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/dbt_project.yml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/profile_template.yml
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/sample_profiles.yml
--rw-r--r--   0        0        0     9374 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/adapters.sql
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/catalog.sql
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations.sql
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/timestamps.sql
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/materializations/incremental_strategies.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/materializations/snapshot_merge.sql
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/materialized_view/alter.sql
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/materialized_view/create.sql
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/materialized_view/describe.sql
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/materialized_view/drop.sql
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/materialized_view/rename.sql
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/table/drop.sql
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/table/rename.sql
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/table/replace.sql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/view/drop.sql
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/view/rename.sql
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/view/replace.sql
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/utils/any_value.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/utils/dateadd.sql
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/utils/datediff.sql
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/utils/last_day.sql
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/utils/listagg.sql
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/dbt/include/postgres/macros/utils/split_part.sql
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/LICENSE
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/README.md
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/pyproject.toml
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b4/PKG-INFO
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/__version__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/column.py
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/connections.py
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/impl.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation_configs/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation_configs/constants.py
+-rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation_configs/index.py
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation_configs/materialized_view.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/dbt_project.yml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/profile_template.yml
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/sample_profiles.yml
+-rw-r--r--   0        0        0     9373 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/adapters.sql
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/catalog.sql
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations.sql
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/timestamps.sql
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/materializations/incremental_strategies.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/create.sql
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/describe.sql
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/rename.sql
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/table/drop.sql
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/table/rename.sql
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/table/replace.sql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/view/drop.sql
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/view/rename.sql
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/view/replace.sql
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/any_value.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/split_part.sql
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/LICENSE
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/README.md
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/pyproject.toml
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/PKG-INFO
```

### Comparing `dbt_postgres-1.8.0b4/dbt/adapters/postgres/connections.py` & `dbt_postgres-1.8.0b5/dbt/adapters/postgres/connections.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from contextlib import contextmanager
 from dataclasses import dataclass
 from typing import Optional, Union
 
 from dbt.adapters.contracts.connection import AdapterResponse, Credentials
 from dbt.adapters.events.logging import AdapterLogger
+from dbt.adapters.events.types import TypeCodeNotFound
 from dbt.adapters.sql import SQLConnectionManager
 from dbt_common.exceptions import DbtDatabaseError, DbtRuntimeError
+from dbt_common.events.functions import warn_or_error
 from dbt_common.helper_types import Port
 from mashumaro.jsonschema.annotations import Maximum, Minimum
 import psycopg2
 from typing_extensions import Annotated
 
 
 logger = AdapterLogger("Postgres")
@@ -199,8 +201,9 @@
         return AdapterResponse(_message=message, code=code, rows_affected=rows)
 
     @classmethod
     def data_type_code_to_name(cls, type_code: Union[int, str]) -> str:
         if type_code in psycopg2.extensions.string_types:
             return psycopg2.extensions.string_types[type_code].name
         else:
+            warn_or_error(TypeCodeNotFound(type_code=type_code))
             return f"unknown type_code {type_code}"
```

### Comparing `dbt_postgres-1.8.0b4/dbt/adapters/postgres/impl.py` & `dbt_postgres-1.8.0b5/dbt/adapters/postgres/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b4/dbt/adapters/postgres/relation.py` & `dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import FrozenSet, Optional, Set
+from typing import FrozenSet, List, Optional
 
 from dbt.adapters.base.relation import BaseRelation
 from dbt.adapters.contracts.relation import RelationConfig, RelationType
 from dbt.adapters.relation_configs import (
     RelationConfigChangeAction,
     RelationResults,
 )
@@ -16,27 +16,30 @@
     PostgresMaterializedViewConfig,
     PostgresMaterializedViewConfigChangeCollection,
 )
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class PostgresRelation(BaseRelation):
-    renameable_relations: FrozenSet[RelationType] = field(default_factory=lambda: frozenset(
-        {
-            RelationType.View,
-            RelationType.Table,
-            RelationType.MaterializedView,
-        }
-    ))
-    replaceable_relations: FrozenSet[RelationType] = field(default_factory=lambda: frozenset(
-        {
-            RelationType.View,
-            RelationType.Table,
-        }
-    ))
+    renameable_relations: FrozenSet[RelationType] = field(
+        default_factory=lambda: frozenset(
+            {
+                RelationType.View,
+                RelationType.Table,
+            }
+        )
+    )
+    replaceable_relations: FrozenSet[RelationType] = field(
+        default_factory=lambda: frozenset(
+            {
+                RelationType.View,
+                RelationType.Table,
+            }
+        )
+    )
 
     def __post_init__(self):
         # Check for length of Postgres table/view names.
         # Check self.type to exclude test relation identifiers
         if (
             self.identifier is not None
             and self.type is not None
@@ -72,33 +75,37 @@
             return config_change_collection
         return None
 
     def _get_index_config_changes(
         self,
         existing_indexes: FrozenSet[PostgresIndexConfig],
         new_indexes: FrozenSet[PostgresIndexConfig],
-    ) -> Set[PostgresIndexConfigChange]:
+    ) -> List[PostgresIndexConfigChange]:
         """
         Get the index updates that will occur as a result of a new run
 
         There are four scenarios:
 
         1. Indexes are equal -> don't return these
         2. Index is new -> create these
         3. Index is old -> drop these
         4. Indexes are not equal -> drop old, create new -> two actions
 
-        Returns: a set of index updates in the form {"action": "drop/create", "context": <IndexConfig>}
+        *Note:*
+            The order of the operations matters here because if the same index is dropped and recreated
+            (e.g. via --full-refresh) then we need to drop it first, then create it.
+
+        Returns: an ordered list of index updates in the form {"action": "drop/create", "context": <IndexConfig>}
         """
-        drop_changes = set(
+        drop_changes = [
             PostgresIndexConfigChange.from_dict(
                 {"action": RelationConfigChangeAction.drop, "context": index}
             )
             for index in existing_indexes.difference(new_indexes)
-        )
-        create_changes = set(
+        ]
+        create_changes = [
             PostgresIndexConfigChange.from_dict(
                 {"action": RelationConfigChangeAction.create, "context": index}
             )
             for index in new_indexes.difference(existing_indexes)
-        )
-        return set().union(drop_changes, create_changes)  # type: ignore
+        ]
+        return drop_changes + create_changes
```

### Comparing `dbt_postgres-1.8.0b4/dbt/adapters/postgres/relation_configs/index.py` & `dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation_configs/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     gist = "gist"
     spgist = "spgist"
     gin = "gin"
     brin = "brin"
 
     @classmethod
     def default(cls) -> "PostgresIndexMethod":
-        return cls.btree
+        return cls("btree")
 
 
 @dataclass(frozen=True, eq=True, unsafe_hash=True)
 class PostgresIndexConfig(RelationConfigBase, RelationConfigValidationMixin):
     """
     This config fallows the specs found here:
     https://www.postgresql.org/docs/current/sql-createindex.html
```

### Comparing `dbt_postgres-1.8.0b4/dbt/adapters/postgres/relation_configs/materialized_view.py` & `dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation_configs/materialized_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,16 @@
             ],
         }
         return config_dict
 
 
 @dataclass
 class PostgresMaterializedViewConfigChangeCollection:
-    indexes: Set[PostgresIndexConfigChange] = field(default_factory=set)
+    indexes: List[PostgresIndexConfigChange] = field(default_factory=list)
 
     @property
     def requires_full_refresh(self) -> bool:
         return any(index.requires_full_refresh for index in self.indexes)
 
     @property
     def has_changes(self) -> bool:
-        return self.indexes != set()
+        return self.indexes != []
```

### Comparing `dbt_postgres-1.8.0b4/dbt/include/postgres/macros/adapters.sql` & `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/adapters.sql`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
   create {% if index_config.unique -%}
     unique
   {%- endif %} index if not exists
   "{{ index_name }}"
   on {{ relation }} {% if index_config.type -%}
     using {{ index_config.type }}
   {%- endif %}
-  ({{ comma_separated_columns }});
+  ({{ comma_separated_columns }})
 {%- endmacro %}
 
 {% macro postgres__create_schema(relation) -%}
   {% if relation.database -%}
     {{ adapter.verify_database(relation.database) }}
   {%- endif -%}
   {%- call statement('create_schema') -%}
```

### Comparing `dbt_postgres-1.8.0b4/dbt/include/postgres/macros/catalog.sql` & `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations.sql` & `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b4/dbt/include/postgres/macros/timestamps.sql` & `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b4/dbt/include/postgres/macros/materializations/snapshot_merge.sql` & `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/materialized_view/alter.sql` & `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b4/dbt/include/postgres/macros/relations/table/replace.sql` & `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/table/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b4/dbt/include/postgres/macros/utils/datediff.sql` & `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b4/dbt/include/postgres/macros/utils/listagg.sql` & `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b4/.gitignore` & `dbt_postgres-1.8.0b5/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b4/LICENSE` & `dbt_postgres-1.8.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b4/README.md` & `dbt_postgres-1.8.0b5/README.md`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b4/pyproject.toml` & `dbt_postgres-1.8.0b5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -55,64 +55,38 @@
 [tool.hatch.version]
 path = "dbt/adapters/postgres/__version__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
     "dbt-adapters @ git+https://github.com/dbt-labs/dbt-adapters.git",
     "dbt-common @ git+https://github.com/dbt-labs/dbt-common.git",
+    'pre-commit==3.7.0;python_version>="3.9"',
+    'pre-commit==3.5.0;python_version=="3.8"',
 ]
-
-[tool.hatch.envs.lint]
-detached = true
-dependencies = [
-    "black>=24.3",
-    "flake8",
-    "Flake8-pyproject",
-]
-[tool.hatch.envs.lint.scripts]
-all = [
-    "black",
-    "flake8",
-]
-black = "python -m black ."
-flake8 = "python -m flake8 ."
-
-[tool.hatch.envs.typecheck]
-dependencies = [
-    "mypy",
-    "types-protobuf",
-    "types-pytz",
-]
-[tool.hatch.envs.typecheck.scripts]
-all = "python -m mypy ."
+[tool.hatch.envs.default.scripts]
+dev = "pre-commit install"
+code-quality = "pre-commit run --all-files"
 
 [tool.hatch.envs.unit-tests]
 dependencies = [
+    "dbt-adapters @ git+https://github.com/dbt-labs/dbt-adapters.git",
+    "dbt-common @ git+https://github.com/dbt-labs/dbt-common.git",
+    "dbt-core @ git+https://github.com/dbt-labs/dbt-core.git#subdirectory=core",
     "freezegun",
     "pytest",
     "pytest-dotenv",
     "pytest-mock",
     "pytest-xdist",
 ]
-extra-dependencies = [
-    # TODO: remove `dbt-core` dependencies from unit tests
-    "dbt-adapters @ git+https://github.com/dbt-labs/dbt-adapters.git",
-    "dbt-common @ git+https://github.com/dbt-labs/dbt-common.git",
-    "dbt-core @ git+https://github.com/dbt-labs/dbt-core.git#subdirectory=core",
-]
 [tool.hatch.envs.unit-tests.scripts]
 all = "python -m pytest {args:tests/unit}"
 
 [tool.hatch.envs.integration-tests]
 template = "unit-tests"
 extra-dependencies = [
-    # TODO: remove `dbt-core` dependencies from integration tests
-    "dbt-adapters @ git+https://github.com/dbt-labs/dbt-adapters.git",
-    "dbt-common @ git+https://github.com/dbt-labs/dbt-common.git",
-    "dbt-core @ git+https://github.com/dbt-labs/dbt-core.git#subdirectory=core",
     "dbt-tests-adapter @ git+https://github.com/dbt-labs/dbt-adapters.git#subdirectory=dbt-tests-adapter",
 ]
 [tool.hatch.envs.integration-tests.env-vars]
 DBT_TEST_USER_1 = "dbt_test_user_1"
 DBT_TEST_USER_2 = "dbt_test_user_2"
 DBT_TEST_USER_3 = "dbt_test_user_3"
 [tool.hatch.envs.integration-tests.scripts]
@@ -121,16 +95,14 @@
 [tool.hatch.envs.build]
 detached = true
 dependencies = [
     "wheel",
     "twine",
     "check-wheel-contents",
 ]
-
-
 [tool.hatch.envs.build.scripts]
 check-all = [
     "- check-wheel",
     "- check-sdist",
 ]
 check-wheel = [
     "twine check dist/*",
@@ -139,39 +111,13 @@
 ]
 check-sdist = [
     "check-wheel-contents dist/*.whl --ignore W007,W008",
     "find ./dist/dbt_postgres-*.gz -maxdepth 1 -type f | xargs python -m pip install --force-reinstall --find-links=dist/",
     "pip freeze | grep dbt-postgres",
 ]
 
-[tool.black]
-line-length = 99
-target-version = ['py38']
-
-[tool.flake8]
-select = ["E", "W", "F"]
-ignore = ["E203", "E501", "E741", "W503", "W504"]
-exclude = ["tests", "venv", ".hatch_venvs"]
-per-file-ignores = ["*/__init__.py: F401"]
-
-[tool.mypy]
-namespace_packages = true
-show_error_codes = true
-explicit_package_bases = true
-ignore_missing_imports = true
-pretty = true
-files = [
-    "dbt/adapters/postgres",
-    "tests/unit",
-]
-exclude = [
-    "tests/functional",
-    "venv",
-    ".hatch_venvs",
-]
-
 [tool.pytest]
 env_files = ["test.env"]
 testpaths = [
     "tests/functional",
     "tests/unit",
-]
+]
```

### Comparing `dbt_postgres-1.8.0b4/PKG-INFO` & `dbt_postgres-1.8.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbt-postgres
-Version: 1.8.0b4
+Version: 1.8.0b5
 Summary: The set of adapter protocols and base functionality that supports integration with dbt-core
 Project-URL: Homepage, https://github.com/dbt-labs/dbt-postgres
 Project-URL: Documentation, https://docs.getdbt.com
 Project-URL: Repository, https://github.com/dbt-labs/dbt-postgres.git
 Project-URL: Issues, https://github.com/dbt-labs/dbt-postgres/issues
 Project-URL: Changelog, https://github.com/dbt-labs/dbt-postgres/blob/main/CHANGELOG.md
 Author-email: dbt Labs <info@dbtlabs.com>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: dbt-postgres Version: 1.8.0b4 Summary: The set of
+Metadata-Version: 2.3 Name: dbt-postgres Version: 1.8.0b5 Summary: The set of
 adapter protocols and base functionality that supports integration with dbt-
 core Project-URL: Homepage, https://github.com/dbt-labs/dbt-postgres Project-
 URL: Documentation, https://docs.getdbt.com Project-URL: Repository, https://
 github.com/dbt-labs/dbt-postgres.git Project-URL: Issues, https://github.com/
 dbt-labs/dbt-postgres/issues Project-URL: Changelog, https://github.com/dbt-
 labs/dbt-postgres/blob/main/CHANGELOG.md Author-email: dbt Labs
 dbtlabs.com> Maintainer-email: dbt Labs
```

