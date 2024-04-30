# Comparing `tmp/sqlmodel_slim-0.0.1.tar.gz` & `tmp/sqlmodel_slim-0.0.18.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "sqlmodel_slim-0.0.18.dev1.tar", last modified: Tue Apr 30 00:53:18 2024, max compression
```

## Comparing `sqlmodel_slim-0.0.1.tar` & `sqlmodel_slim-0.0.18.dev1.tar`

### file list

```diff
@@ -1,7 +1,554 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sqlmodel_slim-0.0.1/src/sqlmodel_slim/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 sqlmodel_slim-0.0.1/src/sqlmodel_slim/__init__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 sqlmodel_slim-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 sqlmodel_slim-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 sqlmodel_slim-0.0.1/README.md
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 sqlmodel_slim-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 sqlmodel_slim-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-30 00:53:16.363206 sqlmodel_slim-0.0.18.dev1/LICENSE
+-rw-r--r--   0        0        0     8320 2024-04-30 00:53:16.363206 sqlmodel_slim-0.0.18.dev1/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/advanced/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/advanced/decimal/__init__.py
+-rw-r--r--   0        0        0     1631 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/advanced/decimal/tutorial001.py
+-rw-r--r--   0        0        0     1597 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/advanced/decimal/tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/automatic_id_none_refresh/__init__.py
+-rw-r--r--   0        0        0    10192 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/automatic_id_none_refresh/annotations/en/tutorial002.md
+-rw-r--r--   0        0        0     2084 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/automatic_id_none_refresh/tutorial001.py
+-rw-r--r--   0        0        0     2049 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/automatic_id_none_refresh/tutorial001_py310.py
+-rw-r--r--   0        0        0     2438 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/automatic_id_none_refresh/tutorial002.py
+-rw-r--r--   0        0        0     2403 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/automatic_id_none_refresh/tutorial002_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial001/__init__.py
+-rw-r--r--   0        0        0      667 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial001/app.py
+-rw-r--r--   0        0        0      231 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial001/database.py
+-rw-r--r--   0        0        0      652 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial001/models.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial001_py310/__init__.py
+-rw-r--r--   0        0        0      667 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial001_py310/app.py
+-rw-r--r--   0        0        0      231 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial001_py310/database.py
+-rw-r--r--   0        0        0      602 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial001_py310/models.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial001_py39/__init__.py
+-rw-r--r--   0        0        0      667 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial001_py39/app.py
+-rw-r--r--   0        0        0      231 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial001_py39/database.py
+-rw-r--r--   0        0        0      646 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial001_py39/models.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002/__init__.py
+-rw-r--r--   0        0        0      694 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002/app.py
+-rw-r--r--   0        0        0      231 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002/database.py
+-rw-r--r--   0        0        0      497 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002/hero_model.py
+-rw-r--r--   0        0        0      371 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002/team_model.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002_py310/__init__.py
+-rw-r--r--   0        0        0      694 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002_py310/app.py
+-rw-r--r--   0        0        0      231 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002_py310/database.py
+-rw-r--r--   0        0        0      488 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002_py310/hero_model.py
+-rw-r--r--   0        0        0      352 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002_py310/team_model.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002_py39/__init__.py
+-rw-r--r--   0        0        0      694 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002_py39/app.py
+-rw-r--r--   0        0        0      231 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002_py39/database.py
+-rw-r--r--   0        0        0      497 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002_py39/hero_model.py
+-rw-r--r--   0        0        0      365 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/code_structure/tutorial002_py39/team_model.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/create_tables/__init__.py
+-rw-r--r--   0        0        0      797 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/create_tables/tutorial001.py
+-rw-r--r--   0        0        0      756 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/create_tables/tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/delete/__init__.py
+-rw-r--r--   0        0        0     2314 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/delete/tutorial001.py
+-rw-r--r--   0        0        0     2273 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/delete/tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/insert/__init__.py
+-rw-r--r--   0        0        0     1911 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/insert/tutorial001.py
+-rw-r--r--   0        0        0     1870 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/insert/tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/select/__init__.py
+-rw-r--r--   0        0        0     2194 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/select/tutorial001.py
+-rw-r--r--   0        0        0     2153 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/select/tutorial001_py310.py
+-rw-r--r--   0        0        0     2174 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/select/tutorial002.py
+-rw-r--r--   0        0        0     2133 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/select/tutorial002_py310.py
+-rw-r--r--   0        0        0     2188 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/select/tutorial003.py
+-rw-r--r--   0        0        0     2147 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/select/tutorial003_py310.py
+-rw-r--r--   0        0        0     2190 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/select/tutorial004.py
+-rw-r--r--   0        0        0     2149 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/select/tutorial004_py310.py
+-rw-r--r--   0        0        0     2217 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/select/tutorial005.py
+-rw-r--r--   0        0        0     2176 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/select/tutorial005_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/update/__init__.py
+-rw-r--r--   0        0        0     2116 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/update/tutorial001.py
+-rw-r--r--   0        0        0     2075 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/connect/update/tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/create_db_and_table/__init__.py
+-rw-r--r--   0        0        0     2248 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/create_db_and_table/annotations/en/tutorial003.md
+-rw-r--r--   0        0        0      409 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/create_db_and_table/tutorial001.py
+-rw-r--r--   0        0        0      374 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/create_db_and_table/tutorial001_py310.py
+-rw-r--r--   0        0        0      498 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/create_db_and_table/tutorial002.py
+-rw-r--r--   0        0        0      463 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/create_db_and_table/tutorial002_py310.py
+-rw-r--r--   0        0        0      615 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/create_db_and_table/tutorial003.py
+-rw-r--r--   0        0        0      572 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/create_db_and_table/tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/delete/__init__.py
+-rw-r--r--   0        0        0     2452 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/delete/annotations/en/tutorial002.md
+-rw-r--r--   0        0        0     2796 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/delete/tutorial001.py
+-rw-r--r--   0        0        0     2761 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/delete/tutorial001_py310.py
+-rw-r--r--   0        0        0     2907 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/delete/tutorial002.py
+-rw-r--r--   0        0        0     2872 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/delete/tutorial002_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/annotations/en/test_main_001.md
+-rw-r--r--   0        0        0     1639 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/annotations/en/test_main_002.md
+-rw-r--r--   0        0        0     1792 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/annotations/en/test_main_003.md
+-rw-r--r--   0        0        0     1083 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/annotations/en/test_main_004.md
+-rw-r--r--   0        0        0     2103 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/annotations/en/test_main_005.md
+-rw-r--r--   0        0        0      949 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/annotations/en/test_main_006.md
+-rw-r--r--   0        0        0     2693 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/main.py
+-rw-r--r--   0        0        0     1208 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/test_extra_coverage.py
+-rw-r--r--   0        0        0     3626 2024-04-30 00:53:16.399206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/test_main.py
+-rw-r--r--   0        0        0      991 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/test_main_001.py
+-rw-r--r--   0        0        0      959 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/test_main_002.py
+-rw-r--r--   0        0        0      978 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/test_main_003.py
+-rw-r--r--   0        0        0     1008 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/test_main_004.py
+-rw-r--r--   0        0        0     1066 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/test_main_005.py
+-rw-r--r--   0        0        0     1171 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001/test_main_006.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/annotations/en/test_main_001.md
+-rw-r--r--   0        0        0     1639 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/annotations/en/test_main_002.md
+-rw-r--r--   0        0        0     1792 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/annotations/en/test_main_003.md
+-rw-r--r--   0        0        0     1083 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/annotations/en/test_main_004.md
+-rw-r--r--   0        0        0     2103 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/annotations/en/test_main_005.md
+-rw-r--r--   0        0        0      949 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/annotations/en/test_main_006.md
+-rw-r--r--   0        0        0     2643 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/main.py
+-rw-r--r--   0        0        0     1208 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/test_extra_coverage.py
+-rw-r--r--   0        0        0     3626 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/test_main.py
+-rw-r--r--   0        0        0      991 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/test_main_001.py
+-rw-r--r--   0        0        0      959 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/test_main_002.py
+-rw-r--r--   0        0        0      978 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/test_main_003.py
+-rw-r--r--   0        0        0     1008 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/test_main_004.py
+-rw-r--r--   0        0        0     1066 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/test_main_005.py
+-rw-r--r--   0        0        0     1171 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py310/test_main_006.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/annotations/en/test_main_001.md
+-rw-r--r--   0        0        0     1639 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/annotations/en/test_main_002.md
+-rw-r--r--   0        0        0     1792 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/annotations/en/test_main_003.md
+-rw-r--r--   0        0        0     1083 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/annotations/en/test_main_004.md
+-rw-r--r--   0        0        0     2103 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/annotations/en/test_main_005.md
+-rw-r--r--   0        0        0      949 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/annotations/en/test_main_006.md
+-rw-r--r--   0        0        0     2687 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/main.py
+-rw-r--r--   0        0        0     1208 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/test_extra_coverage.py
+-rw-r--r--   0        0        0     3626 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/test_main.py
+-rw-r--r--   0        0        0      991 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/test_main_001.py
+-rw-r--r--   0        0        0      959 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/test_main_002.py
+-rw-r--r--   0        0        0      978 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/test_main_003.py
+-rw-r--r--   0        0        0     1008 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/test_main_004.py
+-rw-r--r--   0        0        0     1066 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/test_main_005.py
+-rw-r--r--   0        0        0     1171 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/app_testing/tutorial001_py39/test_main_006.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/delete/__init__.py
+-rw-r--r--   0        0        0     2652 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/delete/tutorial001.py
+-rw-r--r--   0        0        0     2602 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/delete/tutorial001_py310.py
+-rw-r--r--   0        0        0     2646 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/delete/tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/limit_and_offset/__init__.py
+-rw-r--r--   0        0        0     1659 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/limit_and_offset/tutorial001.py
+-rw-r--r--   0        0        0     1618 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/limit_and_offset/tutorial001_py310.py
+-rw-r--r--   0        0        0     1653 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/limit_and_offset/tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/multiple_models/__init__.py
+-rw-r--r--   0        0        0     1364 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/multiple_models/tutorial001.py
+-rw-r--r--   0        0        0     1317 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/multiple_models/tutorial001_py310.py
+-rw-r--r--   0        0        0     1358 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/multiple_models/tutorial001_py39.py
+-rw-r--r--   0        0        0     1271 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/multiple_models/tutorial002.py
+-rw-r--r--   0        0        0     1230 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/multiple_models/tutorial002_py310.py
+-rw-r--r--   0        0        0     1265 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/multiple_models/tutorial002_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/read_one/__init__.py
+-rw-r--r--   0        0        0     1568 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/read_one/tutorial001.py
+-rw-r--r--   0        0        0     1527 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/read_one/tutorial001_py310.py
+-rw-r--r--   0        0        0     1562 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/read_one/tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/relationships/__init__.py
+-rw-r--r--   0        0        0     5156 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/relationships/tutorial001.py
+-rw-r--r--   0        0        0     5082 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/relationships/tutorial001_py310.py
+-rw-r--r--   0        0        0     5150 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/relationships/tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/response_model/__init__.py
+-rw-r--r--   0        0        0     1091 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/response_model/tutorial001.py
+-rw-r--r--   0        0        0     1050 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/response_model/tutorial001_py310.py
+-rw-r--r--   0        0        0     1085 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/response_model/tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/session_with_dependency/__init__.py
+-rw-r--r--   0        0        0     2693 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/session_with_dependency/tutorial001.py
+-rw-r--r--   0        0        0     2643 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/session_with_dependency/tutorial001_py310.py
+-rw-r--r--   0        0        0     2687 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/session_with_dependency/tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/simple_hero_api/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/simple_hero_api/tutorial001.py
+-rw-r--r--   0        0        0     1002 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/simple_hero_api/tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/teams/__init__.py
+-rw-r--r--   0        0        0     4955 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/teams/tutorial001.py
+-rw-r--r--   0        0        0     4887 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/teams/tutorial001_py310.py
+-rw-r--r--   0        0        0     4949 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/teams/tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/update/__init__.py
+-rw-r--r--   0        0        0     2287 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/update/tutorial001.py
+-rw-r--r--   0        0        0     2237 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/update/tutorial001_py310.py
+-rw-r--r--   0        0        0     2281 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/update/tutorial001_py39.py
+-rw-r--r--   0        0        0     2863 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/update/tutorial002.py
+-rw-r--r--   0        0        0     2810 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/update/tutorial002_py310.py
+-rw-r--r--   0        0        0     2857 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/fastapi/update/tutorial002_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/indexes/__init__.py
+-rw-r--r--   0        0        0     1219 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/indexes/tutorial001.py
+-rw-r--r--   0        0        0     1184 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/indexes/tutorial001_py310.py
+-rw-r--r--   0        0        0     1631 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/indexes/tutorial002.py
+-rw-r--r--   0        0        0     1596 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/indexes/tutorial002_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/insert/__init__.py
+-rw-r--r--   0        0        0     1971 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/insert/annotations/en/tutorial003.md
+-rw-r--r--   0        0        0      924 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/insert/tutorial001.py
+-rw-r--r--   0        0        0      889 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/insert/tutorial001_py310.py
+-rw-r--r--   0        0        0      925 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/insert/tutorial002.py
+-rw-r--r--   0        0        0      890 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/insert/tutorial002_py310.py
+-rw-r--r--   0        0        0     1018 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/insert/tutorial003.py
+-rw-r--r--   0        0        0      983 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/insert/tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/many_to_many/__init__.py
+-rw-r--r--   0        0        0     2434 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/many_to_many/tutorial001.py
+-rw-r--r--   0        0        0     2356 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/many_to_many/tutorial001_py310.py
+-rw-r--r--   0        0        0     2428 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/many_to_many/tutorial001_py39.py
+-rw-r--r--   0        0        0     3203 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/many_to_many/tutorial002.py
+-rw-r--r--   0        0        0     3125 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/many_to_many/tutorial002_py310.py
+-rw-r--r--   0        0        0     3197 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/many_to_many/tutorial002_py39.py
+-rw-r--r--   0        0        0     3834 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/many_to_many/tutorial003.py
+-rw-r--r--   0        0        0     3756 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/many_to_many/tutorial003_py310.py
+-rw-r--r--   0        0        0     3828 2024-04-30 00:53:16.403206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/many_to_many/tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/offset_and_limit/__init__.py
+-rw-r--r--   0        0        0     1618 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/offset_and_limit/tutorial001.py
+-rw-r--r--   0        0        0     1583 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/offset_and_limit/tutorial001_py310.py
+-rw-r--r--   0        0        0     1628 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/offset_and_limit/tutorial002.py
+-rw-r--r--   0        0        0     1593 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/offset_and_limit/tutorial002_py310.py
+-rw-r--r--   0        0        0     1628 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/offset_and_limit/tutorial003.py
+-rw-r--r--   0        0        0     1593 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/offset_and_limit/tutorial003_py310.py
+-rw-r--r--   0        0        0     1649 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/offset_and_limit/tutorial004.py
+-rw-r--r--   0        0        0     1614 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/offset_and_limit/tutorial004_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/__init__.py
+-rw-r--r--   0        0        0     1638 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial001.py
+-rw-r--r--   0        0        0     1603 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial001_py310.py
+-rw-r--r--   0        0        0     1637 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial002.py
+-rw-r--r--   0        0        0     1602 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial002_py310.py
+-rw-r--r--   0        0        0     1645 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial003.py
+-rw-r--r--   0        0        0     1610 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial003_py310.py
+-rw-r--r--   0        0        0     1636 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial004.py
+-rw-r--r--   0        0        0     1601 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial004_py310.py
+-rw-r--r--   0        0        0     1635 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial005.py
+-rw-r--r--   0        0        0     1600 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial005_py310.py
+-rw-r--r--   0        0        0     1589 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial006.py
+-rw-r--r--   0        0        0     1554 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial006_py310.py
+-rw-r--r--   0        0        0     1636 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial007.py
+-rw-r--r--   0        0        0     1601 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial007_py310.py
+-rw-r--r--   0        0        0     1538 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial008.py
+-rw-r--r--   0        0        0     1503 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial008_py310.py
+-rw-r--r--   0        0        0     1541 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial009.py
+-rw-r--r--   0        0        0     1506 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/one/tutorial009_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/back_populates/__init__.py
+-rw-r--r--   0        0        0     4538 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/back_populates/tutorial001.py
+-rw-r--r--   0        0        0     4488 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/back_populates/tutorial001_py310.py
+-rw-r--r--   0        0        0     4532 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/back_populates/tutorial001_py39.py
+-rw-r--r--   0        0        0     4582 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/back_populates/tutorial002.py
+-rw-r--r--   0        0        0     4532 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/back_populates/tutorial002_py310.py
+-rw-r--r--   0        0        0     4576 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/back_populates/tutorial002_py39.py
+-rw-r--r--   0        0        0     1584 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/back_populates/tutorial003.py
+-rw-r--r--   0        0        0     1522 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/back_populates/tutorial003_py310.py
+-rw-r--r--   0        0        0     1578 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/back_populates/tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/create_and_update_relationships/__init__.py
+-rw-r--r--   0        0        0     3364 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/create_and_update_relationships/tutorial001.py
+-rw-r--r--   0        0        0     3314 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/create_and_update_relationships/tutorial001_py310.py
+-rw-r--r--   0        0        0     3358 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/create_and_update_relationships/tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/define_relationship_attributes/__init__.py
+-rw-r--r--   0        0        0     2025 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/define_relationship_attributes/tutorial001.py
+-rw-r--r--   0        0        0     1975 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/define_relationship_attributes/tutorial001_py310.py
+-rw-r--r--   0        0        0     2019 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/define_relationship_attributes/tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/read_relationships/__init__.py
+-rw-r--r--   0        0        0     3852 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/read_relationships/tutorial001.py
+-rw-r--r--   0        0        0     3802 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/read_relationships/tutorial001_py310.py
+-rw-r--r--   0        0        0     3846 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/read_relationships/tutorial001_py39.py
+-rw-r--r--   0        0        0     4085 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/read_relationships/tutorial002.py
+-rw-r--r--   0        0        0     4035 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/read_relationships/tutorial002_py310.py
+-rw-r--r--   0        0        0     4079 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/relationship_attributes/read_relationships/tutorial002_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/select/__init__.py
+-rw-r--r--   0        0        0     2174 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/select/annotations/en/tutorial002.md
+-rw-r--r--   0        0        0     1141 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/select/tutorial001.py
+-rw-r--r--   0        0        0     1106 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/select/tutorial001_py310.py
+-rw-r--r--   0        0        0     1252 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/select/tutorial002.py
+-rw-r--r--   0        0        0     1217 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/select/tutorial002_py310.py
+-rw-r--r--   0        0        0     1141 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/select/tutorial003.py
+-rw-r--r--   0        0        0     1106 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/select/tutorial003_py310.py
+-rw-r--r--   0        0        0     1085 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/select/tutorial004.py
+-rw-r--r--   0        0        0     1050 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/select/tutorial004_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/update/__init__.py
+-rw-r--r--   0        0        0     1712 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/update/annotations/en/tutorial002.md
+-rw-r--r--   0        0        0     4270 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/update/annotations/en/tutorial004.md
+-rw-r--r--   0        0        0     1788 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/update/tutorial001.py
+-rw-r--r--   0        0        0     1753 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/update/tutorial001_py310.py
+-rw-r--r--   0        0        0     1860 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/update/tutorial002.py
+-rw-r--r--   0        0        0     1825 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/update/tutorial002_py310.py
+-rw-r--r--   0        0        0     2218 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/update/tutorial003.py
+-rw-r--r--   0        0        0     2183 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/update/tutorial003_py310.py
+-rw-r--r--   0        0        0     2392 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/update/tutorial004.py
+-rw-r--r--   0        0        0     2357 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/update/tutorial004_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/__init__.py
+-rw-r--r--   0        0        0     1172 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial001.py
+-rw-r--r--   0        0        0     1137 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial001_py310.py
+-rw-r--r--   0        0        0     1172 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial002.py
+-rw-r--r--   0        0        0     1137 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial002_py310.py
+-rw-r--r--   0        0        0     1583 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial003.py
+-rw-r--r--   0        0        0     1548 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial003_py310.py
+-rw-r--r--   0        0        0     1584 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial004.py
+-rw-r--r--   0        0        0     1549 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial004_py310.py
+-rw-r--r--   0        0        0     1583 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial005.py
+-rw-r--r--   0        0        0     1548 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial005_py310.py
+-rw-r--r--   0        0        0     1584 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial006.py
+-rw-r--r--   0        0        0     1549 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial006_py310.py
+-rw-r--r--   0        0        0     1605 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial007.py
+-rw-r--r--   0        0        0     1570 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial007_py310.py
+-rw-r--r--   0        0        0     1599 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial008.py
+-rw-r--r--   0        0        0     1564 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial008_py310.py
+-rw-r--r--   0        0        0     1609 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial009.py
+-rw-r--r--   0        0        0     1574 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial009_py310.py
+-rw-r--r--   0        0        0     1604 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial010.py
+-rw-r--r--   0        0        0     1569 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial010_py310.py
+-rw-r--r--   0        0        0     1594 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial011.py
+-rw-r--r--   0        0        0     1559 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/docs_src/tutorial/where/tutorial011_py310.py
+-rw-r--r--   0        0        0     1723 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/pdm_build.py
+-rw-r--r--   0        0        0     2750 2024-04-30 00:53:18.935236 sqlmodel_slim-0.0.18.dev1/pyproject.toml
+-rw-r--r--   0        0        0       74 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/requirements-docs-tests.txt
+-rw-r--r--   0        0        0      484 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/requirements-docs.txt
+-rw-r--r--   0        0        0      243 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/requirements-tests.txt
+-rw-r--r--   0        0        0       85 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/requirements.txt
+-rw-r--r--   0        0        0     4671 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/scripts/docs.py
+-rwxr-xr-x   0        0        0      114 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/scripts/format.sh
+-rw-r--r--   0        0        0     1812 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/scripts/generate_select.py
+-rwxr-xr-x   0        0        0      137 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/scripts/lint.sh
+-rwxr-xr-x   0        0        0      175 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/scripts/test.sh
+-rw-r--r--   0        0        0     6811 2024-04-30 00:53:16.407206 sqlmodel_slim-0.0.18.dev1/sqlmodel/__init__.py
+-rw-r--r--   0        0        0    21556 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/_compat.py
+-rw-r--r--   0        0        0      850 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/default.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/ext/asyncio/__init__.py
+-rw-r--r--   0        0        0     4970 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/ext/asyncio/session.py
+-rw-r--r--   0        0        0    33561 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/main.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/orm/__init__.py
+-rw-r--r--   0        0        0     5237 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/orm/session.py
+-rw-r--r--   0        0        0       67 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/pool/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/py.typed
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/sql/__init__.py
+-rw-r--r--   0        0        0      170 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/sql/base.py
+-rw-r--r--   0        0        0    14619 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/sql/expression.py
+-rw-r--r--   0        0        0     9075 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/sql/expression.py.jinja2
+-rw-r--r--   0        0        0     1969 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/sqlmodel/sql/sqltypes.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/__init__.py
+-rw-r--r--   0        0        0     2333 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_advanced/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_advanced/test_decimal/__init__.py
+-rw-r--r--   0        0        0      970 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_advanced/test_decimal/test_tutorial001.py
+-rw-r--r--   0        0        0     1002 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_advanced/test_decimal/test_tutorial001_py310.py
+-rw-r--r--   0        0        0      842 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_default.py
+-rw-r--r--   0        0        0      690 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_deprecations.py
+-rw-r--r--   0        0        0     3977 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_enums.py
+-rw-r--r--   0        0        0     1291 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_field_sa_args_kwargs.py
+-rw-r--r--   0        0        0     3173 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_field_sa_column.py
+-rw-r--r--   0        0        0     1994 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_field_sa_relationship.py
+-rw-r--r--   0        0        0      701 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_fields_set.py
+-rw-r--r--   0        0        0     1039 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_instance_no_args.py
+-rw-r--r--   0        0        0     4232 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_main.py
+-rw-r--r--   0        0        0      536 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_missing_type.py
+-rw-r--r--   0        0        0     5250 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_nullable.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_pydantic/__init__.py
+-rw-r--r--   0        0        0     1545 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_pydantic/test_field.py
+-rw-r--r--   0        0        0      797 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_query.py
+-rw-r--r--   0        0        0      764 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_sqlalchemy_type_errors.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_automatic_id_none_refresh/__init__.py
+-rw-r--r--   0        0        0     4167 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_automatic_id_none_refresh/test_tutorial001_py310_tutorial002_py310.py
+-rw-r--r--   0        0        0     4116 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_automatic_id_none_refresh/test_tutorial001_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_code_structure/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_code_structure/test_tutorial001.py
+-rw-r--r--   0        0        0      906 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_code_structure/test_tutorial001_py310.py
+-rw-r--r--   0        0        0      903 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_code_structure/test_tutorial001_py39.py
+-rw-r--r--   0        0        0      874 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_code_structure/test_tutorial002.py
+-rw-r--r--   0        0        0      906 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_code_structure/test_tutorial002_py310.py
+-rw-r--r--   0        0        0      903 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_code_structure/test_tutorial002_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_create_connected_tables/__init__.py
+-rw-r--r--   0        0        0      480 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_create_connected_tables/test_tutorial001.py
+-rw-r--r--   0        0        0      537 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_create_connected_tables/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_delete/__init__.py
+-rw-r--r--   0        0        0     1557 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_delete/test_tutorial001.py
+-rw-r--r--   0        0        0     1589 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_delete/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_insert/__init__.py
+-rw-r--r--   0        0        0     1126 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_insert/test_tutorial001.py
+-rw-r--r--   0        0        0     1158 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_insert/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_select/__init__.py
+-rw-r--r--   0        0        0     2114 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_select/test_tutorial001_py310_tutorial002_py310.py
+-rw-r--r--   0        0        0     2063 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_select/test_tutorial001_tutorial002.py
+-rw-r--r--   0        0        0     1939 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_select/test_tutorial003.py
+-rw-r--r--   0        0        0     1971 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_select/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     1329 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_select/test_tutorial004.py
+-rw-r--r--   0        0        0     1361 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_select/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     1418 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_select/test_tutorial005.py
+-rw-r--r--   0        0        0     1450 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_select/test_tutorial005_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_update/__init__.py
+-rw-r--r--   0        0        0     1335 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_update/test_tutorial001.py
+-rw-r--r--   0        0        0     1367 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_connect/test_update/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_create_db_and_table/__init__.py
+-rw-r--r--   0        0        0      709 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_create_db_and_table/test_tutorial001.py
+-rw-r--r--   0        0        0      741 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_create_db_and_table/test_tutorial001_py310.py
+-rw-r--r--   0        0        0      447 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_create_db_and_table/test_tutorial002.py
+-rw-r--r--   0        0        0      503 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_create_db_and_table/test_tutorial002_py310.py
+-rw-r--r--   0        0        0      447 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_create_db_and_table/test_tutorial003.py
+-rw-r--r--   0        0        0      503 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_create_db_and_table/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_delete/__init__.py
+-rw-r--r--   0        0        0     2030 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_delete/test_tutorial001_py310_tutorial002_py310.py
+-rw-r--r--   0        0        0     1979 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_delete/test_tutorial001_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_app_testing/__init__.py
+-rw-r--r--   0        0        0      670 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_app_testing/test_tutorial001_py310_tests_main.py
+-rw-r--r--   0        0        0      667 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_app_testing/test_tutorial001_py39_tests_main.py
+-rw-r--r--   0        0        0      516 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_app_testing/test_tutorial001_tests001.py
+-rw-r--r--   0        0        0      516 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_app_testing/test_tutorial001_tests002.py
+-rw-r--r--   0        0        0      516 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_app_testing/test_tutorial001_tests003.py
+-rw-r--r--   0        0        0      516 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_app_testing/test_tutorial001_tests004.py
+-rw-r--r--   0        0        0      781 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_app_testing/test_tutorial001_tests005.py
+-rw-r--r--   0        0        0      928 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_app_testing/test_tutorial001_tests006.py
+-rw-r--r--   0        0        0      613 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_app_testing/test_tutorial001_tests_main.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.411206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_delete/__init__.py
+-rw-r--r--   0        0        0    16866 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_delete/test_tutorial001.py
+-rw-r--r--   0        0        0    16923 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_delete/test_tutorial001_py310.py
+-rw-r--r--   0        0        0    16920 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_delete/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_limit_and_offset/__init__.py
+-rw-r--r--   0        0        0    11924 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_limit_and_offset/test_tutorial001.py
+-rw-r--r--   0        0        0    11981 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_limit_and_offset/test_tutorial001_py310.py
+-rw-r--r--   0        0        0    11978 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_limit_and_offset/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_multiple_models/__init__.py
+-rw-r--r--   0        0        0     9151 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_multiple_models/test_tutorial001.py
+-rw-r--r--   0        0        0     9207 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_multiple_models/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     9205 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_multiple_models/test_tutorial001_py39.py
+-rw-r--r--   0        0        0     9151 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_multiple_models/test_tutorial002.py
+-rw-r--r--   0        0        0     9208 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_multiple_models/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     9205 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_multiple_models/test_tutorial002_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_read_one/__init__.py
+-rw-r--r--   0        0        0     9384 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_read_one/test_tutorial001.py
+-rw-r--r--   0        0        0     9441 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_read_one/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     9438 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_read_one/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_relationships/__init__.py
+-rw-r--r--   0        0        0    35511 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_relationships/test_tutorial001.py
+-rw-r--r--   0        0        0    35568 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_relationships/test_tutorial001_py310.py
+-rw-r--r--   0        0        0    35565 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_relationships/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_response_model/__init__.py
+-rw-r--r--   0        0        0     6774 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_response_model/test_tutorial001.py
+-rw-r--r--   0        0        0     6831 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_response_model/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     6828 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_response_model/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_session_with_dependency/__init__.py
+-rw-r--r--   0        0        0    16883 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_session_with_dependency/test_tutorial001.py
+-rw-r--r--   0        0        0    16957 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_session_with_dependency/test_tutorial001_py310.py
+-rw-r--r--   0        0        0    16954 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_session_with_dependency/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_simple_hero_api/__init__.py
+-rw-r--r--   0        0        0     6846 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_simple_hero_api/test_tutorial001.py
+-rw-r--r--   0        0        0     6903 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_simple_hero_api/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_teams/__init__.py
+-rw-r--r--   0        0        0    31621 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_teams/test_tutorial001.py
+-rw-r--r--   0        0        0    31678 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_teams/test_tutorial001_py310.py
+-rw-r--r--   0        0        0    31675 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_teams/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_update/__init__.py
+-rw-r--r--   0        0        0    15803 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_update/test_tutorial001.py
+-rw-r--r--   0        0        0    15860 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_update/test_tutorial001_py310.py
+-rw-r--r--   0        0        0    15857 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_update/test_tutorial001_py39.py
+-rw-r--r--   0        0        0    19162 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_update/test_tutorial002.py
+-rw-r--r--   0        0        0    19219 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_update/test_tutorial002_py310.py
+-rw-r--r--   0        0        0    19216 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_fastapi/test_update/test_tutorial002_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_indexes/__init__.py
+-rw-r--r--   0        0        0     1393 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_indexes/test_tutorial001.py
+-rw-r--r--   0        0        0     1425 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_indexes/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     1484 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_indexes/test_tutorial002.py
+-rw-r--r--   0        0        0     1516 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_indexes/test_tutorial002_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_insert/__init__.py
+-rw-r--r--   0        0        0     1013 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_insert/test_tutorial001.py
+-rw-r--r--   0        0        0     1069 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_insert/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     1013 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_insert/test_tutorial002.py
+-rw-r--r--   0        0        0     1069 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_insert/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     1013 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_insert/test_tutorial003.py
+-rw-r--r--   0        0        0     1069 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_insert/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_limit_and_offset/__init__.py
+-rw-r--r--   0        0        0      875 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_limit_and_offset/test_tutorial001.py
+-rw-r--r--   0        0        0      907 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_limit_and_offset/test_tutorial001_py310.py
+-rw-r--r--   0        0        0      874 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_limit_and_offset/test_tutorial002.py
+-rw-r--r--   0        0        0      906 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_limit_and_offset/test_tutorial002_py310.py
+-rw-r--r--   0        0        0      712 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_limit_and_offset/test_tutorial003.py
+-rw-r--r--   0        0        0      744 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_limit_and_offset/test_tutorial003_py310.py
+-rw-r--r--   0        0        0      697 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_limit_and_offset/test_tutorial004.py
+-rw-r--r--   0        0        0      729 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_limit_and_offset/test_tutorial004_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_many_to_many/__init__.py
+-rw-r--r--   0        0        0     1304 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_many_to_many/test_tutorial001.py
+-rw-r--r--   0        0        0     1336 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_many_to_many/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     1333 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_many_to_many/test_tutorial001_py39.py
+-rw-r--r--   0        0        0     2117 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_many_to_many/test_tutorial002.py
+-rw-r--r--   0        0        0     2149 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_many_to_many/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     2146 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_many_to_many/test_tutorial002_py39.py
+-rw-r--r--   0        0        0     1842 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_many_to_many/test_tutorial003.py
+-rw-r--r--   0        0        0     1874 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_many_to_many/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     1871 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_many_to_many/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/__init__.py
+-rw-r--r--   0        0        0      668 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial001.py
+-rw-r--r--   0        0        0      700 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial001_py310.py
+-rw-r--r--   0        0        0      468 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial002.py
+-rw-r--r--   0        0        0      500 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial002_py310.py
+-rw-r--r--   0        0        0      585 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial003.py
+-rw-r--r--   0        0        0      617 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     1117 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial004.py
+-rw-r--r--   0        0        0     1149 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     1103 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial005.py
+-rw-r--r--   0        0        0     1135 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial005_py310.py
+-rw-r--r--   0        0        0      585 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial006.py
+-rw-r--r--   0        0        0      617 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial006_py310.py
+-rw-r--r--   0        0        0      585 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial007.py
+-rw-r--r--   0        0        0      617 2024-04-30 00:53:16.415206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial007_py310.py
+-rw-r--r--   0        0        0      585 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial008.py
+-rw-r--r--   0        0        0      617 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial008_py310.py
+-rw-r--r--   0        0        0      468 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial009.py
+-rw-r--r--   0        0        0      500 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_one/test_tutorial009_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_back_populates/__init__.py
+-rw-r--r--   0        0        0     7134 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_back_populates/test_tutorial001.py
+-rw-r--r--   0        0        0     7166 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_back_populates/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     7163 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_back_populates/test_tutorial001_py39.py
+-rw-r--r--   0        0        0     6839 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_back_populates/test_tutorial002.py
+-rw-r--r--   0        0        0     6871 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_back_populates/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     6868 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_back_populates/test_tutorial002_py39.py
+-rw-r--r--   0        0        0      624 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_back_populates/test_tutorial003.py
+-rw-r--r--   0        0        0      681 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_back_populates/test_tutorial003_py310.py
+-rw-r--r--   0        0        0      678 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_back_populates/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_create_and_update_relationships/__init__.py
+-rw-r--r--   0        0        0     2167 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_create_and_update_relationships/test_tutorial001.py
+-rw-r--r--   0        0        0     2199 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_create_and_update_relationships/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     2196 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_create_and_update_relationships/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_define_relationship_attributes/__init__.py
+-rw-r--r--   0        0        0     1180 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_define_relationship_attributes/test_tutorial001.py
+-rw-r--r--   0        0        0     1212 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_define_relationship_attributes/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     1209 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_define_relationship_attributes/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_read_relationships/__init__.py
+-rw-r--r--   0        0        0     2390 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_read_relationships/test_tutorial001.py
+-rw-r--r--   0        0        0     2422 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_read_relationships/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     2419 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_read_relationships/test_tutorial001_py39.py
+-rw-r--r--   0        0        0     3444 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_read_relationships/test_tutorial002.py
+-rw-r--r--   0        0        0     3476 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_read_relationships/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     3473 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_relationship_attributes/test_read_relationships/test_tutorial002_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_select/__init__.py
+-rw-r--r--   0        0        0     1379 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_select/test_tutorial001_py310_tutorial002_py310.py
+-rw-r--r--   0        0        0     1328 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_select/test_tutorial001_tutorial002.py
+-rw-r--r--   0        0        0     1422 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_select/test_tutorial003_py310_tutorial004_py310.py
+-rw-r--r--   0        0        0     1371 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_select/test_tutorial003_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_update/__init__.py
+-rw-r--r--   0        0        0     1257 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_update/test_tutorial001_py310_tutorial002_py310.py
+-rw-r--r--   0        0        0     1206 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_update/test_tutorial001_tutorial002.py
+-rw-r--r--   0        0        0     1609 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_update/test_tutorial003_py310_tutorial004_py310.py
+-rw-r--r--   0        0        0     1558 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_update/test_tutorial003_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/__init__.py
+-rw-r--r--   0        0        0      644 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial001.py
+-rw-r--r--   0        0        0      676 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial001_py310.py
+-rw-r--r--   0        0        0      735 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial002.py
+-rw-r--r--   0        0        0      767 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     1112 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial003.py
+-rw-r--r--   0        0        0     1144 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     1197 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial004.py
+-rw-r--r--   0        0        0     1229 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial004_py310.py
+-rw-r--r--   0        0        0      547 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial005.py
+-rw-r--r--   0        0        0      579 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial005_py310.py
+-rw-r--r--   0        0        0      634 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial006.py
+-rw-r--r--   0        0        0      666 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial006_py310.py
+-rw-r--r--   0        0        0      629 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial007.py
+-rw-r--r--   0        0        0      661 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial007_py310.py
+-rw-r--r--   0        0        0      629 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial008.py
+-rw-r--r--   0        0        0      661 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial008_py310.py
+-rw-r--r--   0        0        0      835 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial009.py
+-rw-r--r--   0        0        0      867 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial009_py310.py
+-rw-r--r--   0        0        0      835 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial010.py
+-rw-r--r--   0        0        0      867 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial010_py310.py
+-rw-r--r--   0        0        0     1197 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial011.py
+-rw-r--r--   0        0        0     1229 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_tutorial/test_where/test_tutorial011_py310.py
+-rw-r--r--   0        0        0     1817 2024-04-30 00:53:16.419206 sqlmodel_slim-0.0.18.dev1/tests/test_validation.py
+-rw-r--r--   0        0        0     9763 1970-01-01 00:00:00.000000 sqlmodel_slim-0.0.18.dev1/PKG-INFO
```

### Comparing `sqlmodel_slim-0.0.1/LICENSE.txt` & `sqlmodel_slim-0.0.18.dev1/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,21 @@
-MIT License
+The MIT License (MIT)
 
-Copyright (c) 2023-present Sebastián Ramírez <tiangolo@gmail.com>
+Copyright (c) 2021 Sebastián Ramírez
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `sqlmodel_slim-0.0.1/pyproject.toml` & `sqlmodel_slim-0.0.18.dev1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,157 +1,127 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
 
 [project]
 name = "sqlmodel-slim"
-dynamic = ["version"]
-description = ''
+dynamic = []
+description = "SQLModel, SQL databases in Python, designed for simplicity, compatibility, and robustness."
 readme = "README.md"
 requires-python = ">=3.7"
-license = "MIT"
-keywords = []
 authors = [
-  { name = "Sebastián Ramírez", email = "tiangolo@gmail.com" },
+    { name = "Sebastián Ramírez", email = "tiangolo@gmail.com" },
 ]
 classifiers = [
-  "Development Status :: 4 - Beta",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
+    "Development Status :: 4 - Beta",
+    "Framework :: AsyncIO",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Science/Research",
+    "Intended Audience :: System Administrators",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Database",
+    "Topic :: Database :: Database Engines/Servers",
+    "Topic :: Internet",
+    "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
+    "Topic :: Internet :: WWW/HTTP",
+    "Typing :: Typed",
+]
+dependencies = [
+    "SQLAlchemy >=2.0.0,<2.1.0",
+    "pydantic >=1.10.13,<3.0.0",
 ]
-dependencies = []
+version = "0.0.18.dev1"
 
 [project.urls]
-Documentation = "https://github.com/tiangolo/sqlmodel#readme"
-Issues = "https://github.com/tiangolo/sqlmodel/issues"
-Source = "https://github.com/tiangolo/sqlmodel"
+Homepage = "https://github.com/tiangolo/sqlmodel"
+Documentation = "https://sqlmodel.tiangolo.com"
+Repository = "https://github.com/tiangolo/sqlmodel"
+
+[tool.pdm]
+distribution = true
+
+[tool.pdm.version]
+source = "file"
+path = "sqlmodel/__init__.py"
+
+[tool.pdm.build]
+source-includes = [
+    "tests/",
+    "docs_src/",
+    "requirements*.txt",
+    "scripts/",
+    "sqlmodel/sql/expression.py.jinja2",
+]
+
+[tool.tiangolo._internal-slim-build.packages.sqlmodel-slim.project]
+name = "sqlmodel-slim"
 
-[tool.hatch.version]
-path = "src/sqlmodel_slim/__about__.py"
+[tool.tiangolo._internal-slim-build.packages.sqlmodel.project.optional-dependencies]
 
-[tool.hatch.envs.default]
-dependencies = [
-  "coverage[toml]>=6.5",
-  "pytest",
-]
-[tool.hatch.envs.default.scripts]
-test = "pytest {args:tests}"
-test-cov = "coverage run -m pytest {args:tests}"
-cov-report = [
-  "- coverage combine",
-  "coverage report",
-]
-cov = [
-  "test-cov",
-  "cov-report",
+[tool.coverage.run]
+parallel = true
+source = [
+    "docs_src",
+    "tests",
+    "sqlmodel",
 ]
+context = "${CONTEXT}"
 
-[[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+[tool.coverage.report]
+exclude_lines = [
+    "pragma: no cover",
+    "@overload",
+    "if __name__ == \"__main__\":",
+    "if TYPE_CHECKING:",
+]
+
+[tool.mypy]
+strict = true
+
+[[tool.mypy.overrides]]
+module = "sqlmodel.sql.expression"
+warn_unused_ignores = false
+
+[[tool.mypy.overrides]]
+module = "docs_src.*"
+disallow_incomplete_defs = false
+disallow_untyped_defs = false
+disallow_untyped_calls = false
 
-[tool.hatch.envs.lint]
-detached = true
-dependencies = [
-  "black>=23.1.0",
-  "mypy>=1.0.0",
-  "ruff>=0.0.243",
-]
-[tool.hatch.envs.lint.scripts]
-typing = "mypy --install-types --non-interactive {args:src/sqlmodel_slim tests}"
-style = [
-  "ruff {args:.}",
-  "black --check --diff {args:.}",
-]
-fmt = [
-  "black {args:.}",
-  "ruff --fix {args:.}",
-  "style",
-]
-all = [
-  "style",
-  "typing",
-]
-
-[tool.black]
-target-version = ["py37"]
-line-length = 120
-skip-string-normalization = true
-
-[tool.ruff]
-target-version = "py37"
-line-length = 120
+[tool.ruff.lint]
 select = [
-  "A",
-  "ARG",
-  "B",
-  "C",
-  "DTZ",
-  "E",
-  "EM",
-  "F",
-  "FBT",
-  "I",
-  "ICN",
-  "ISC",
-  "N",
-  "PLC",
-  "PLE",
-  "PLR",
-  "PLW",
-  "Q",
-  "RUF",
-  "S",
-  "T",
-  "TID",
-  "UP",
-  "W",
-  "YTT",
+    "E",
+    "W",
+    "F",
+    "I",
+    "B",
+    "C4",
+    "UP",
 ]
 ignore = [
-  # Allow non-abstract empty methods in abstract base classes
-  "B027",
-  # Allow boolean positional values in function calls, like `dict.get(... True)`
-  "FBT003",
-  # Ignore checks for possible passwords
-  "S105", "S106", "S107",
-  # Ignore complexity
-  "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
-]
-unfixable = [
-  # Don't touch unused imports
-  "F401",
-]
-
-[tool.ruff.isort]
-known-first-party = ["sqlmodel_slim"]
-
-[tool.ruff.flake8-tidy-imports]
-ban-relative-imports = "all"
-
-[tool.ruff.per-file-ignores]
-# Tests can use magic values, assertions, and relative imports
-"tests/**/*" = ["PLR2004", "S101", "TID252"]
-
-[tool.coverage.run]
-source_pkgs = ["sqlmodel_slim", "tests"]
-branch = true
-parallel = true
-omit = [
-  "src/sqlmodel_slim/__about__.py",
+    "E501",
+    "B008",
+    "C901",
+    "W191",
 ]
 
-[tool.coverage.paths]
-sqlmodel_slim = ["src/sqlmodel_slim", "*/sqlmodel-slim/src/sqlmodel_slim"]
-tests = ["tests", "*/sqlmodel-slim/tests"]
+[tool.ruff.lint.per-file-ignores]
 
-[tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
+[tool.ruff.lint.isort]
+known-third-party = [
+    "sqlmodel",
+    "sqlalchemy",
+    "pydantic",
+    "fastapi",
 ]
+
+[tool.ruff.lint.pyupgrade]
+keep-runtime-typing = true
```

