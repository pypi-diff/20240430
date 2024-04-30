# Comparing `tmp/geneweaver_db-0.3.2.tar.gz` & `tmp/geneweaver_db-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_db-0.3.2.tar", max compression
+gzip compressed data, was "geneweaver_db-0.3.3.tar", max compression
```

## Comparing `geneweaver_db-0.3.2.tar` & `geneweaver_db-0.3.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11356 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/LICENSE
--rw-r--r--   0        0        0     2162 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/README.md
--rw-r--r--   0        0        0      953 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      156 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/__init__.py
--rw-r--r--   0        0        0      132 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/aio/__init__.py
--rw-r--r--   0        0        0     3134 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/aio/gene.py
--rw-r--r--   0        0        0     4802 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/aio/geneset.py
--rw-r--r--   0        0        0     2189 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/aio/publication.py
--rw-r--r--   0        0        0     1310 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/aio/species.py
--rw-r--r--   0        0        0      692 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/aio/threshold.py
--rw-r--r--   0        0        0       56 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/core/__init__.py
--rw-r--r--   0        0        0      845 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/core/cursor.py
--rw-r--r--   0        0        0      145 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/core/settings.py
--rw-r--r--   0        0        0     1769 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/core/settings_class.py
--rw-r--r--   0        0        0      438 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/exceptions.py
--rw-r--r--   0        0        0    10316 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/gene.py
--rw-r--r--   0        0        0     8651 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/geneset.py
--rw-r--r--   0        0        0     7887 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/geneset_value.py
--rw-r--r--   0        0        0     2063 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/publication.py
--rw-r--r--   0        0        0       42 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/__init__.py
--rw-r--r--   0        0        0     4859 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/gene.py
--rw-r--r--   0        0        0      364 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/geneset/__init__.py
--rw-r--r--   0        0        0     1351 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/geneset/const.py
--rw-r--r--   0        0        0     4785 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/geneset/read.py
--rw-r--r--   0        0        0     3928 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/geneset/utils.py
--rw-r--r--   0        0        0     4014 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/geneset/write.py
--rw-r--r--   0        0        0      982 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/project.py
--rw-r--r--   0        0        0     4683 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/publication.py
--rw-r--r--   0        0        0       60 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/search/__init__.py
--rw-r--r--   0        0        0       50 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/search/search.py
--rw-r--r--   0        0        0     1571 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/search/utils.py
--rw-r--r--   0        0        0     1603 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/species.py
--rw-r--r--   0        0        0     1959 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/threshold.py
--rw-r--r--   0        0        0     1776 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/query/utils.py
--rw-r--r--   0        0        0     1249 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/species.py
--rw-r--r--   0        0        0      664 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/threshold.py
--rw-r--r--   0        0        0     6887 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/user.py
--rw-r--r--   0        0        0     3085 2024-04-25 19:22:58.338404 geneweaver_db-0.3.2/src/geneweaver/db/utils.py
--rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 geneweaver_db-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2162 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/README.md
+-rw-r--r--   0        0        0      953 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/aio/__init__.py
+-rw-r--r--   0        0        0     3134 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/aio/gene.py
+-rw-r--r--   0        0        0     4802 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/aio/geneset.py
+-rw-r--r--   0        0        0     2189 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/aio/publication.py
+-rw-r--r--   0        0        0     1310 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/aio/species.py
+-rw-r--r--   0        0        0      809 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/aio/threshold.py
+-rw-r--r--   0        0        0       56 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/core/__init__.py
+-rw-r--r--   0        0        0      845 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/core/cursor.py
+-rw-r--r--   0        0        0      145 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/core/settings.py
+-rw-r--r--   0        0        0     1769 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/core/settings_class.py
+-rw-r--r--   0        0        0      438 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/exceptions.py
+-rw-r--r--   0        0        0    10316 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/gene.py
+-rw-r--r--   0        0        0     8651 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/geneset.py
+-rw-r--r--   0        0        0     7887 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/geneset_value.py
+-rw-r--r--   0        0        0     2063 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/publication.py
+-rw-r--r--   0        0        0       42 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/__init__.py
+-rw-r--r--   0        0        0     4859 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/gene.py
+-rw-r--r--   0        0        0      364 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/geneset/__init__.py
+-rw-r--r--   0        0        0     1351 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/geneset/const.py
+-rw-r--r--   0        0        0     4785 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/geneset/read.py
+-rw-r--r--   0        0        0     3928 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/geneset/utils.py
+-rw-r--r--   0        0        0     4014 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/geneset/write.py
+-rw-r--r--   0        0        0      982 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/project.py
+-rw-r--r--   0        0        0     4683 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/publication.py
+-rw-r--r--   0        0        0       60 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/search/__init__.py
+-rw-r--r--   0        0        0       50 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/search/search.py
+-rw-r--r--   0        0        0     1571 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/search/utils.py
+-rw-r--r--   0        0        0     1603 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/species.py
+-rw-r--r--   0        0        0     2897 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/threshold.py
+-rw-r--r--   0        0        0     1776 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/query/utils.py
+-rw-r--r--   0        0        0     1249 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/species.py
+-rw-r--r--   0        0        0      775 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/threshold.py
+-rw-r--r--   0        0        0     6887 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/user.py
+-rw-r--r--   0        0        0     3085 2024-04-30 18:22:40.704750 geneweaver_db-0.3.3/src/geneweaver/db/utils.py
+-rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 geneweaver_db-0.3.3/PKG-INFO
```

### Comparing `geneweaver_db-0.3.2/LICENSE` & `geneweaver_db-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/README.md` & `geneweaver_db-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/pyproject.toml` & `geneweaver_db-0.3.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geneweaver-db"
-version = "0.3.2"
+version = "0.3.3"
 description = "Database Interaction Services for GeneWeaver"
 authors = ["Jax Computational Sciences <cssc@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://thejacksonlaboratory.github.io/geneweaver-docs/"
 repository = "https://github.com/TheJacksonLaboratory/geneweaver-db"
 packages = [
```

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/aio/gene.py` & `geneweaver_db-0.3.3/src/geneweaver/db/aio/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/aio/geneset.py` & `geneweaver_db-0.3.3/src/geneweaver/db/aio/geneset.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/aio/publication.py` & `geneweaver_db-0.3.3/src/geneweaver/db/aio/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/aio/species.py` & `geneweaver_db-0.3.3/src/geneweaver/db/aio/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/aio/threshold.py` & `geneweaver_db-0.3.3/src/geneweaver/db/threshold.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Geneset thresholding database functions."""
 
 from geneweaver.core.schema.score import GenesetScoreType
 from geneweaver.db.query import threshold as threshold_query
-from psycopg import AsyncCursor
+from psycopg import Cursor
 
 
-async def set_geneset_threshold(
-    cursor: AsyncCursor,
+def set_geneset_threshold(
+    cursor: Cursor,
     geneset_id: int,
     geneset_score_type: GenesetScoreType,
 ) -> None:
     """Update the threshold of a geneset and its values.
 
-    :param cursor: An async database cursor.
+    :param cursor: An database cursor.
     :param geneset_id: The ID of the geneset to update.
     :param geneset_score_type: The score threshold to set.
     :return: Nothing.
     """
-    await cursor.execute(
+    cursor.execute(
         *threshold_query.set_geneset_threshold(geneset_id, geneset_score_type)
     )
+    cursor.execute(
+        *threshold_query.set_geneset_value_threshold(geneset_id, geneset_score_type)
+    )
```

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/core/cursor.py` & `geneweaver_db-0.3.3/src/geneweaver/db/core/cursor.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/core/settings_class.py` & `geneweaver_db-0.3.3/src/geneweaver/db/core/settings_class.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/gene.py` & `geneweaver_db-0.3.3/src/geneweaver/db/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/geneset.py` & `geneweaver_db-0.3.3/src/geneweaver/db/geneset.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/geneset_value.py` & `geneweaver_db-0.3.3/src/geneweaver/db/geneset_value.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/publication.py` & `geneweaver_db-0.3.3/src/geneweaver/db/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/query/gene.py` & `geneweaver_db-0.3.3/src/geneweaver/db/query/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/query/geneset/const.py` & `geneweaver_db-0.3.3/src/geneweaver/db/query/geneset/const.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/query/geneset/read.py` & `geneweaver_db-0.3.3/src/geneweaver/db/query/geneset/read.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/query/geneset/utils.py` & `geneweaver_db-0.3.3/src/geneweaver/db/query/geneset/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/query/geneset/write.py` & `geneweaver_db-0.3.3/src/geneweaver/db/query/geneset/write.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/query/project.py` & `geneweaver_db-0.3.3/src/geneweaver/db/query/project.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/query/publication.py` & `geneweaver_db-0.3.3/src/geneweaver/db/query/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/query/search/utils.py` & `geneweaver_db-0.3.3/src/geneweaver/db/query/search/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/query/species.py` & `geneweaver_db-0.3.3/src/geneweaver/db/query/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/query/threshold.py` & `geneweaver_db-0.3.3/src/geneweaver/db/query/threshold.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,34 +6,68 @@
 from psycopg.sql import SQL, Composed
 
 
 def set_geneset_threshold(
     geneset_id: int,
     geneset_score_type: GenesetScoreType,
 ) -> Tuple[Composed, dict]:
-    """Update the threshold of a geneset and its values.
+    """Update the threshold of a geneset.
+
+    After calling this query, the query in `update_geneset_value_threshold` should be
+    called.
 
     :param geneset_id: The ID of the geneset to update.
     :param geneset_score_type: An instance of GenesetScoreType, representing the new
     threshold to set.
     :return:  A query (and params) that can be executed on a cursor.
     """
+    if (
+        geneset_score_type.threshold_low
+        and geneset_score_type.threshold_low > geneset_score_type.threshold
+    ):
+        raise ValueError(
+            "geneset_score_type.threshold must be larger than "
+            "geneset_score_type.threshold_low"
+        )
+
     params = {
         "geneset_id": geneset_id,
         "score_type": int(geneset_score_type.score_type),
         "threshold_str": geneset_score_type.threshold_as_db_string(),
+    }
+    query = (
+        SQL("UPDATE geneset")
+        + SQL("SET gs_threshold_type = %(score_type)s,")
+        + SQL("gs_threshold = %(threshold_str)s")
+        + SQL("WHERE id = %(geneset_id)s;")
+    )
+
+    query = query.join(" ")
+
+    return query, params
+
+
+def set_geneset_value_threshold(
+    geneset_id: int,
+    geneset_score_type: GenesetScoreType,
+) -> Tuple[Composed, dict]:
+    """Update the threshold a geneset values.
+
+    :param geneset_id: The ID of the geneset to update.
+    :param geneset_score_type: An instance of GenesetScoreType, representing the new
+    threshold to set.
+    :return:  A query (and params) that can be executed on a cursor.
+    """
+    params = {
+        "geneset_id": geneset_id,
         "threshold_high": geneset_score_type.threshold,
     }
 
     query = SQL(
         """
-        UPDATE geneset
-        SET gs_threshold_type = %(score_type)s,
-            gs_threshold = %(threshold_str)s
-        WHERE id = %(geneset_id)s;
         UPDATE geneset_value
             SET gsv_in_threshold = CASE
         """
     )
     if geneset_score_type.threshold_low is not None:
         query = query + SQL(
             """
```

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/query/utils.py` & `geneweaver_db-0.3.3/src/geneweaver/db/query/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/species.py` & `geneweaver_db-0.3.3/src/geneweaver/db/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/threshold.py` & `geneweaver_db-0.3.3/src/geneweaver/db/aio/threshold.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Geneset thresholding database functions."""
 
 from geneweaver.core.schema.score import GenesetScoreType
 from geneweaver.db.query import threshold as threshold_query
-from psycopg import Cursor
+from psycopg import AsyncCursor
 
 
-def set_geneset_threshold(
-    cursor: Cursor,
+async def set_geneset_threshold(
+    cursor: AsyncCursor,
     geneset_id: int,
     geneset_score_type: GenesetScoreType,
 ) -> None:
     """Update the threshold of a geneset and its values.
 
-    :param cursor: An database cursor.
+    :param cursor: An async database cursor.
     :param geneset_id: The ID of the geneset to update.
     :param geneset_score_type: The score threshold to set.
     :return: Nothing.
     """
-    cursor.execute(
+    await cursor.execute(
         *threshold_query.set_geneset_threshold(geneset_id, geneset_score_type)
     )
+    await cursor.execute(
+        *threshold_query.set_geneset_value_threshold(geneset_id, geneset_score_type)
+    )
```

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/user.py` & `geneweaver_db-0.3.3/src/geneweaver/db/user.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/src/geneweaver/db/utils.py` & `geneweaver_db-0.3.3/src/geneweaver/db/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.2/PKG-INFO` & `geneweaver_db-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneweaver-db
-Version: 0.3.2
+Version: 0.3.3
 Summary: Database Interaction Services for GeneWeaver
 Home-page: https://thejacksonlaboratory.github.io/geneweaver-docs/
 License: Apache-2.0
 Author: Jax Computational Sciences
 Author-email: cssc@jax.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

