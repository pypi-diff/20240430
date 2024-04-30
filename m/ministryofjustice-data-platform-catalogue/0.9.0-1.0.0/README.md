# Comparing `tmp/ministryofjustice_data_platform_catalogue-0.9.0.tar.gz` & `tmp/ministryofjustice_data_platform_catalogue-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ministryofjustice_data_platform_catalogue-0.9.0.tar", max compression
+gzip compressed data, was "ministryofjustice_data_platform_catalogue-1.0.0.tar", max compression
```

## Comparing `ministryofjustice_data_platform_catalogue-0.9.0.tar` & `ministryofjustice_data_platform_catalogue-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     3563 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/README.md
--rw-r--r--   0        0        0      213 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/__init__.py
--rw-r--r--   0        0        0      155 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/__init__.py
--rw-r--r--   0        0        0     2343 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/base.py
--rw-r--r--   0        0        0       65 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/__init__.py
--rw-r--r--   0        0        0    13045 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/datahub_client.py
--rw-r--r--   0        0        0        0 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/graphql/__init__.py
--rw-r--r--   0        0        0      694 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/graphql/facets.graphql
--rw-r--r--   0        0        0     3854 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/graphql/search.graphql
--rw-r--r--   0        0        0     9202 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/search.py
--rw-r--r--   0        0        0     8548 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/openmetadata.py
--rw-r--r--   0        0        0     2817 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/entities.py
--rw-r--r--   0        0        0     2224 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/search_types.py
--rw-r--r--   0        0        0      701 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4361 1970-01-01 00:00:00.000000 ministryofjustice_data_platform_catalogue-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     3041 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/README.md
+-rw-r--r--   0        0        0     3038 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/__init__.py
+-rw-r--r--   0        0        0    19189 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/datahub_client.py
+-rw-r--r--   0        0        0      544 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/__init__.py
+-rw-r--r--   0        0        0      694 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/facets.graphql
+-rw-r--r--   0        0        0      651 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/getChartDetails.graphql
+-rw-r--r--   0        0        0     2305 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/getDatasetDetails.graphql
+-rw-r--r--   0        0        0      519 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/getGlossaryTerms.graphql
+-rw-r--r--   0        0        0      656 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/listContainerEntities.graphql
+-rw-r--r--   0        0        0     5891 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/search.graphql
+-rw-r--r--   0        0        0     7194 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql_helpers.py
+-rw-r--r--   0        0        0    13517 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/search.py
+-rw-r--r--   0        0        0     7325 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/entities.py
+-rw-r--r--   0        0        0     2391 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/search_types.py
+-rw-r--r--   0        0        0      750 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3810 1970-01-01 00:00:00.000000 ministryofjustice_data_platform_catalogue-1.0.0/PKG-INFO
```

### Comparing `ministryofjustice_data_platform_catalogue-0.9.0/README.md` & `ministryofjustice_data_platform_catalogue-1.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -15,18 +15,14 @@
 ```shell
 pip install ministryofjustice-data-platform-catalogue
 ```
 
 ## Terminology
 
 - **Data assets** - Any databases, tables, or schemas within the metadata graph
-- **Data products** - Groupings of data assets that are published for
-  reuse across MOJ. In the data platform, the concepts of database and data
-  product are similar, but they may be represented as different entities in the
-  catalogue.
 - **Domains** - allow metadata to be grouped into different service areas that have
   their own governance, like HMCTS, HMPPS, OPG, etc.
 
 ## Example usage
 
 ```python
 from data_platform_catalogue import (
@@ -41,15 +37,16 @@
 data_product = DataProductMetadata(
     name = "my_data_product",
     description = "bla bla",
     version = "v1.0.0",
     owner = "7804c127-d677-4900-82f9-83517e51bb94",
     email = "justice@justice.gov.uk",
     retention_period_in_days = 365,
-    domain = "HMCTS",
+    domain = "LAA",
+    subdomain = "Legal Aid",
     dpia_required = False
 )
 
 table = TableMetadata(
   name = "my_table",
   description = "bla bla",
   column_details=[
@@ -127,17 +124,10 @@
 - roles, hasRoles
 - container
 
 ## Catalogue Implementations
 
 ### DataHub
 
-- Each data product within the MOJ data platform is created as a data product entity
 - Each table is created as a dataset in DataHub
 - Tables that reside in the same athena database (data_product_v1) should
   be placed within the same DataHub container.
-
-## OpenMetadata
-
-- Each MOJ data product is mapped to a database in the OpenMetadata catalogue
-- We populate the schema level in openmetdata with a generic entry of `Tables`
-- Each table is mapped to a table in openmetadata
```

### Comparing `ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/graphql/facets.graphql` & `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/facets.graphql`

 * *Files identical despite different names*

### Comparing `ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/search_types.py` & `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/search_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+"""Search types module."""
+
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum, auto
 from typing import Any
 
 
 class ResultType(Enum):
-    DATA_PRODUCT = auto()
+    """Result type."""
+
     TABLE = auto()
+    GLOSSARY_TERM = auto()
+    CHART = auto()
+    DATABASE = auto()
 
 
 @dataclass
 class MultiSelectFilter:
     """
     Values to filter the result set by
     """
@@ -44,22 +50,24 @@
     value: str
     label: str
     count: int
 
 
 @dataclass
 class SearchResult:
-    id: str
+    urn: str
     result_type: ResultType
     name: str
+    fully_qualified_name: str = ""
     description: str = ""
     matches: dict[str, str] = field(default_factory=dict)
     metadata: dict[str, Any] = field(default_factory=dict)
     tags: list[str] = field(default_factory=list)
-    last_updated: datetime | None = None
+    last_modified: datetime | None = None
+    created: datetime | None = None
 
 
 @dataclass
 class SearchFacets:
     facets: dict[str, list[FacetOption]] = field(default_factory=dict)
 
     def options(self, field_name) -> list[FacetOption]:
```

### Comparing `ministryofjustice_data_platform_catalogue-0.9.0/pyproject.toml` & `ministryofjustice_data_platform_catalogue-1.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,30 @@
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.isort]
+profile = "black"
+
+[tool.pylint]
+max-line-length = 120
+
 [tool.poetry]
 name = "ministryofjustice-data-platform-catalogue"
-version = "0.9.0"
+version = "1.0.0"
 description = "Library to integrate the MoJ data platform with the catalogue component."
 authors = ["MoJ Data Platform Team <data-platform-tech@digital.justice.gov.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "data_platform_catalogue" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-openmetadata-ingestion = "~1.2.0.1"
 acryl-datahub = { extras = ["datahub-rest"], version = "^0.12.1.3" }
 freezegun = "^1.4.0"
 deepdiff = "^6.7.1"
+pydantic = "2"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.11.0"
 pytest = "^7.4.2"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
```

### Comparing `ministryofjustice_data_platform_catalogue-0.9.0/PKG-INFO` & `ministryofjustice_data_platform_catalogue-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ministryofjustice-data-platform-catalogue
-Version: 0.9.0
+Version: 1.0.0
 Summary: Library to integrate the MoJ data platform with the catalogue component.
 License: MIT
 Author: MoJ Data Platform Team
 Author-email: data-platform-tech@digital.justice.gov.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: acryl-datahub[datahub-rest] (>=0.12.1.3,<0.13.0.0)
 Requires-Dist: deepdiff (>=6.7.1,<7.0.0)
 Requires-Dist: freezegun (>=1.4.0,<2.0.0)
-Requires-Dist: openmetadata-ingestion (>=1.2.0.1,<1.3.0.0)
+Requires-Dist: pydantic (==2)
 Description-Content-Type: text/markdown
 
 # Data platform catalogue
 
 This library is part of the Ministry of Justice data platform.
 
 It publishes object metadata to a data catalogue, so that the
@@ -34,18 +34,14 @@
 ```shell
 pip install ministryofjustice-data-platform-catalogue
 ```
 
 ## Terminology
 
 - **Data assets** - Any databases, tables, or schemas within the metadata graph
-- **Data products** - Groupings of data assets that are published for
-  reuse across MOJ. In the data platform, the concepts of database and data
-  product are similar, but they may be represented as different entities in the
-  catalogue.
 - **Domains** - allow metadata to be grouped into different service areas that have
   their own governance, like HMCTS, HMPPS, OPG, etc.
 
 ## Example usage
 
 ```python
 from data_platform_catalogue import (
@@ -60,15 +56,16 @@
 data_product = DataProductMetadata(
     name = "my_data_product",
     description = "bla bla",
     version = "v1.0.0",
     owner = "7804c127-d677-4900-82f9-83517e51bb94",
     email = "justice@justice.gov.uk",
     retention_period_in_days = 365,
-    domain = "HMCTS",
+    domain = "LAA",
+    subdomain = "Legal Aid",
     dpia_required = False
 )
 
 table = TableMetadata(
   name = "my_table",
   description = "bla bla",
   column_details=[
@@ -146,18 +143,11 @@
 - roles, hasRoles
 - container
 
 ## Catalogue Implementations
 
 ### DataHub
 
-- Each data product within the MOJ data platform is created as a data product entity
 - Each table is created as a dataset in DataHub
 - Tables that reside in the same athena database (data_product_v1) should
   be placed within the same DataHub container.
 
-## OpenMetadata
-
-- Each MOJ data product is mapped to a database in the OpenMetadata catalogue
-- We populate the schema level in openmetdata with a generic entry of `Tables`
-- Each table is mapped to a table in openmetadata
-
```

