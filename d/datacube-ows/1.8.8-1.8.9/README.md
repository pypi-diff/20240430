# Comparing `tmp/datacube_ows-1.8.8.tar.gz` & `tmp/datacube_ows-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/datacube-ows/datacube-ows/dist/tmpx9naor0p/datacube_ows-1.8.8.tar", last modified: Tue May  4 00:55:37 2021, max compression
+gzip compressed data, was "/home/runner/work/datacube-ows/datacube-ows/dist/tmpjicq7mnz/datacube_ows-1.8.9.tar", last modified: Thu Jun  3 06:01:13 2021, max compression
```

## Comparing `datacube_ows-1.8.8.tar` & `datacube_ows-1.8.9.tar`

### file list

```diff
@@ -1,255 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      534 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.env_ows_root
--rw-r--r--   0 runner    (1001) docker     (121)      421 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.env_simple
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.github/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      658 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.github/ISSUE_TEMPLATE/code-change-failed-tests-report.md
--rw-r--r--   0 runner    (1001) docker     (121)      423 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.github/ISSUE_TEMPLATE/standard-issue-template.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.github/workflows/scan.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3754 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      991 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      923 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/.yamllint
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)      551 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2294 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10565 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/cfg_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1619 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/check-code-all.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      273 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/check-code.sh
--rw-r--r--   0 runner    (1001) docker     (121)     3852 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/create_tables.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5070 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/band_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4632 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/cfg_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/config_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (121)    11817 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/cube_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)    35430 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/data.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/gunicorn_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/legend_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/legend_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3943 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/mv_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     7641 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/ogc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4036 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/ogc_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    11842 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/ogc_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    82341 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/ows_cfg_example.py
--rw-r--r--   0 runner    (1001) docker     (121)    48252 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/ows_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)    11969 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/product_ranges.py
--rw-r--r--   0 runner    (1001) docker     (121)     2573 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/protocol_versions.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/query_profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows/sql/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/001_postgis_extension.sql
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/002_timezone.sql
--rw-r--r--   0 runner    (1001) docker     (121)     1884 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/010_create_new_time_view.sql
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/011_create_new_space_view_raw.sql
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/012_create_new_spacetime_view.sql
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/020_create_index_1.sql
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/021_create_index_2.sql
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/022_create_index_3.sql
--rw-r--r--   0 runner    (1001) docker     (121)      132 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/023_create_index_4.sql
--rw-r--r--   0 runner    (1001) docker     (121)      122 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/030_rename_old_space_time_view.sql
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/031_rename_new_space_time_view.sql
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/040_drop_old_space_time_view.sql
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/041_drop_old_time_view.sql
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/042_drop_old_space_view.sql
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/050_rename_new_space_view.sql
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/051_rename_new_time_view.sql
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/052_rename_index_1.sql
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/053_rename_index_2.sql
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/054_rename_index_3.sql
--rw-r--r--   0 runner    (1001) docker     (121)      113 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/055_rename_index_4.sql
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/060_grant.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/refresh/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/refresh/001_timezone.sql
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/refresh/002_refresh_time.sql
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/refresh/003_refresh_space.sql
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/extent_views/refresh/004_refresh_spacetime.sql
--rw-r--r--   0 runner    (1001) docker     (121)     1055 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/use_space_time.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows/sql/wms_schema/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows/sql/wms_schema/create/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/wms_schema/create/001_create_schema.sql
--rw-r--r--   0 runner    (1001) docker     (121)      341 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/wms_schema/create/002_create_product_rng.sql
--rw-r--r--   0 runner    (1001) docker     (121)      464 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/wms_schema/create/003_create_subproduct_rng.sql
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/wms_schema/create/004_create_multiproduct_rng.sql
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/sql/wms_schema/create/005_grant_requires_role.sql
--rw-r--r--   0 runner    (1001) docker     (121)     5104 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/startup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows/styles/
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/styles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows/styles/api/
--rw-r--r--   0 runner    (1001) docker     (121)      391 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/styles/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4197 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/styles/api/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4197 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/styles/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    16302 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/styles/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6580 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/styles/colormap.py
--rw-r--r--   0 runner    (1001) docker     (121)     5324 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/styles/component.py
--rw-r--r--   0 runner    (1001) docker     (121)     1961 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/styles/expr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2514 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/styles/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/styles/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (121)    21421 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/styles/ramp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     5082 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/templates/ogc_error.xml
--rw-r--r--   0 runner    (1001) docker     (121)      196 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/templates/ping.html
--rw-r--r--   0 runner    (1001) docker     (121)     2913 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/templates/test_client.html
--rw-r--r--   0 runner    (1001) docker     (121)     5077 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/templates/wcs_capabilities.xml
--rw-r--r--   0 runner    (1001) docker     (121)     6106 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/templates/wcs_desc_coverage.xml
--rw-r--r--   0 runner    (1001) docker     (121)    11817 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/templates/wms_capabilities.xml
--rw-r--r--   0 runner    (1001) docker     (121)     9185 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/templates/wmts_capabilities.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4737 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/tile_matrix_sets.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8312 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/update_ranges.py
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4420 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/wcs1.py
--rw-r--r--   0 runner    (1001) docker     (121)    20306 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/wcs1_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9403 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/wcs2.py
--rw-r--r--   0 runner    (1001) docker     (121)    14625 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/wcs2_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8761 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/wcs_scaler.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/wcs_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/wms.py
--rw-r--r--   0 runner    (1001) docker     (121)    18500 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/wms_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6382 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/wmts.py
--rw-r--r--   0 runner    (1001) docker     (121)      383 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/datacube_ows/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7046 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/datacube_ows.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/docker/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/docker/database/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docker/database/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)   222983 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docker/database/dump.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/docker/ows/
--rwxr-xr-x   0 runner    (1001) docker     (121)      284 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docker/ows/wait-for-db
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/docker/pyspy/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docker/pyspy/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)      493 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docker-compose.db.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      313 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docker-compose.prod.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docker-compose.pyspy.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6786 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     8799 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/cfg_colourmap_styles.rst
--rw-r--r--   0 runner    (1001) docker     (121)    17754 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/cfg_colourramp_styles.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11424 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/cfg_component_styles.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9356 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/cfg_functions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6932 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/cfg_global.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2245 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/cfg_hybrid_styles.rst
--rw-r--r--   0 runner    (1001) docker     (121)    32312 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/cfg_layers.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6585 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/cfg_style_api.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12516 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/cfg_styling.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3249 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/cfg_wcs.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4278 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/cfg_wms.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6629 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/cfg_wmts.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     8484 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)    10520 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3764 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/database.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/environment_variables.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      358 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4238 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6471 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/performance.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13171 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/style_howto_color_map.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9094 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/style_howto_color_ramp.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9965 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/style_howto_components.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6932 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/style_howto_components_nonlinear.rst
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/style_howto_legends.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10981 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/style_howto_transparency.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/styling_howto.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/integration_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/integration_tests/test_cfg_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/integration_tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3246 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/integration_tests/test_mv_index.py
--rw-r--r--   0 runner    (1001) docker     (121)      891 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/integration_tests/test_routes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/integration_tests/test_update_ranges.py
--rw-r--r--   0 runner    (1001) docker     (121)    49065 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/integration_tests/test_wcs_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     9252 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/integration_tests/test_wms_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     4399 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/integration_tests/test_wmts_server.py
--rw-r--r--   0 runner    (1001) docker     (121)    13774 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/integration_tests/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       76 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/lint-code.sh
--rw-r--r--   0 runner    (1001) docker     (121)      813 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/ows_cfg_report.json
--rw-r--r--   0 runner    (1001) docker     (121)    42354 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/ows_test_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)     5528 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      193 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      534 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2213 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      417 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/test_urls.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/tests/cfg/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/infinite_1.json
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/infinite_2.json
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/infinite_2a.json
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/infinite_2b.json
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/minimal_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      218 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/mixed_nested.json
--rw-r--r--   0 runner    (1001) docker     (121)      472 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/mixed_nested.py
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/nested.py
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/nested_1.json
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/nested_2.json
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/nested_3.json
--rw-r--r--   0 runner    (1001) docker     (121)      323 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/nested_4.json
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/simple.json
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/cfg/simple.py
--rw-r--r--   0 runner    (1001) docker     (121)    34820 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4279 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_band_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3935 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_cfg_bandidx.py
--rw-r--r--   0 runner    (1001) docker     (121)     5071 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_cfg_cache_ctrl.py
--rw-r--r--   0 runner    (1001) docker     (121)     4943 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_cfg_global.py
--rw-r--r--   0 runner    (1001) docker     (121)     6413 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_cfg_inclusion.py
--rw-r--r--   0 runner    (1001) docker     (121)    20063 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_cfg_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4165 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_cfg_metadata_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     6883 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_cfg_tile_matrix_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     7202 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_cfg_wcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_config_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (121)     8511 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     6603 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_legend_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_mpl_cmaps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2722 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_multidate_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      792 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_mv_selopts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_no_db_routes.py
--rw-r--r--   0 runner    (1001) docker     (121)     7337 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_ogc_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_ows_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)      459 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_pyproj.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_qprof.py
--rw-r--r--   0 runner    (1001) docker     (121)     2363 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_startup.py
--rw-r--r--   0 runner    (1001) docker     (121)    14553 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_style_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    20260 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_styles.py
--rw-r--r--   0 runner    (1001) docker     (121)     3580 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_time_res_method.py
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_wcs2_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11985 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_wcs_scaler.py
--rw-r--r--   0 runner    (1001) docker     (121)     7967 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/test_wms_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/update_ranges.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 00:55:37.000000 datacube_ows-1.8.8/wms_xsds/
--rw-r--r--   0 runner    (1001) docker     (121)    21612 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/wms_xsds/capabilities_1_3_0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     3932 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/wms_xsds/capabilities_extensions.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     3895 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/wms_xsds/capabilities_extensions_local.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/wms_xsds/exceptions_1_3_0.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    21818 2021-05-04 00:55:28.000000 datacube_ows-1.8.8/wms_xsds/wmtsGetCapabilities_response.xsd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)      596 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.env_ows_root
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.env_simple
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.github/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      658 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.github/ISSUE_TEMPLATE/code-change-failed-tests-report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.github/ISSUE_TEMPLATE/standard-issue-template.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1443 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      598 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.github/workflows/dockerfile-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1959 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1335 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1520 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.github/workflows/scan.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     4112 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      991 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (121)     3258 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1904 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)     1786 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2294 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      930 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10703 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/cfg_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1619 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/check-code-all.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      273 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/check-code.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     3510 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/code-of-conduct.md
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3852 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/create_tables.sql
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows/
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5279 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/band_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13044 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/cfg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1468 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/config_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18571 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2161 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/cube_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35639 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/gunicorn_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1722 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/legend_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/legend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4152 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/mv_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8017 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/ogc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4245 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/ogc_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12336 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/ogc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    82764 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/ows_cfg_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52736 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/ows_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12179 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/product_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2782 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/protocol_versions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1163 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/query_profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows/sql/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/001_postgis_extension.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/002_timezone.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     1884 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/010_create_new_time_view.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     2426 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/011_create_new_space_view_raw.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/012_create_new_spacetime_view.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/020_create_index_1.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/021_create_index_2.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/022_create_index_3.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/023_create_index_4.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/030_rename_old_space_time_view.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/031_rename_new_space_time_view.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/040_drop_old_space_time_view.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/041_drop_old_time_view.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/042_drop_old_space_view.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/050_rename_new_space_view.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/051_rename_new_time_view.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/052_rename_index_1.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/053_rename_index_2.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/054_rename_index_3.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/055_rename_index_4.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/060_grant.sql
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/refresh/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/refresh/001_timezone.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/refresh/002_refresh_time.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/refresh/003_refresh_space.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/extent_views/refresh/004_refresh_spacetime.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     1055 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/use_space_time.sql
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows/sql/wms_schema/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows/sql/wms_schema/create/
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/wms_schema/create/001_create_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/wms_schema/create/002_create_product_rng.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/wms_schema/create/003_create_subproduct_rng.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/wms_schema/create/004_create_multiproduct_rng.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/sql/wms_schema/create/005_grant_requires_role.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     6063 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/startup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows/styles/
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/styles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows/styles/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/styles/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5638 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/styles/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16988 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/styles/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6789 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/styles/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5533 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/styles/component.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2170 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/styles/expr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2723 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/styles/expression.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2523 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/styles/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21630 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/styles/ramp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     5082 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/templates/ogc_error.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/templates/ping.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2913 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/templates/test_client.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5077 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/templates/wcs_capabilities.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     6106 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/templates/wcs_desc_coverage.xml
+-rw-r--r--   0 runner    (1001) docker     (121)    11817 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/templates/wms_capabilities.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     9185 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/templates/wmts_capabilities.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     4946 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/tile_matrix_sets.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8521 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/update_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1300 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4629 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/wcs1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20515 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/wcs1_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9564 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/wcs2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14834 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/wcs2_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8970 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/wcs_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/wcs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2056 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/wms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18709 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/wms_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6591 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/wmts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/datacube_ows/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      930 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5632 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/datacube_ows.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/docker/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/docker/database/
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docker/database/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)   222983 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docker/database/dump.sql
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/docker/ows/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      284 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docker/ows/wait-for-db
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/docker/pyspy/
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docker/pyspy/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docker-compose.db.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docker-compose.prod.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docker-compose.pyspy.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1630 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     6786 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     8799 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/cfg_colourmap_styles.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    17754 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/cfg_colourramp_styles.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11424 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/cfg_component_styles.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9356 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/cfg_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11042 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/cfg_global.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2245 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/cfg_hybrid_styles.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    32697 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/cfg_layers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7771 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/cfg_style_api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12516 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/cfg_styling.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3249 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/cfg_wcs.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2508 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/cfg_wms.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6629 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/cfg_wmts.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8484 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15569 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3764 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/database.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3492 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/environment_variables.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4238 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6471 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)     1339 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13171 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/style_howto_color_map.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9315 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/style_howto_color_ramp.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10586 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/style_howto_components.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6934 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/style_howto_components_nonlinear.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/style_howto_legends.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10959 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/style_howto_transparency.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3227 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/styling_howto.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2224 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/styling_howto_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2688 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/license-headers.md
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/license-template.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)       76 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/lint-code.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/ows_cfg_report.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5528 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2554 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      417 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/test_urls.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/update_ranges.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-03 06:01:13.000000 datacube_ows-1.8.9/wms_xsds/
+-rw-r--r--   0 runner    (1001) docker     (121)    21612 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/wms_xsds/capabilities_1_3_0.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     3932 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/wms_xsds/capabilities_extensions.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     3895 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/wms_xsds/capabilities_extensions_local.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     1124 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/wms_xsds/exceptions_1_3_0.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    21818 2021-06-03 06:01:03.000000 datacube_ows-1.8.9/wms_xsds/wmtsGetCapabilities_response.xsd
```

### Comparing `datacube_ows-1.8.8/.env_ows_root` & `datacube_ows-1.8.9/.env_ows_root`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Set some default vars, you can overwrite these by creating env vars
+# Example docker env file for OWS instance with (multi-file) configuration.
 AWS_REGION=ap-southeast-2
 DB_HOSTNAME=postgres
 DB_PORT=5432
 DB_USERNAME=opendatacubeusername
 DB_PASSWORD=opendatacubepassword
 DB_DATABASE=opendatacube
 OWS_CFG_FILE=./ows_refactored/dev_af_ows_root_cfg.py
 AWS_NO_SIGN_REQUEST=yes
 # If you want to use pydev for interactive debugging
 PYDEV_DEBUG=
 # Will not work with pydev
 FLASK_ENV=development
 prometheus_multiproc_dir=/tmp
-PYTHONPATH=/code/ows_refactored
-DATACUBE_OWS_CFG=ows_refactored.dev_af_ows_root_cfg.ows_cfg
+PYTHONPATH=/code
+DATACUBE_OWS_CFG=ows_refactored.dev_af_ows_root_cfg.ows_cfg
```

### Comparing `datacube_ows-1.8.8/.github/.codecov.yml` & `datacube_ows-1.8.9/.github/.codecov.yml`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/.github/ISSUE_TEMPLATE/code-change-failed-tests-report.md` & `datacube_ows-1.8.9/.github/ISSUE_TEMPLATE/code-change-failed-tests-report.md`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/.github/workflows/docker.yml` & `datacube_ows-1.8.9/.github/workflows/docker.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 ---
-name: Docker
+name: Build Docker Image
 
 on:
   push:
     branches:
       - master
     paths:
       - "**"
+      - '!docs/**'
+      - '!*.rst'
+      - '!*.md'
+      - '!datacube_ows/__init__.py'
 
   release:
     types: [created, edited, published]
 
 env:
   ORG: opendatacube
   IMAGE: ows
```

### Comparing `datacube_ows-1.8.8/.github/workflows/lint.yml` & `datacube_ows-1.8.9/.github/workflows/lint.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 ---
-name: Linting
+name: Code Linting
 
 on:
   pull_request:
+    branches:
+      - 'master'
     paths:
       - '**'
+      - '.github/workflows/lint.yml'
+      - '!docs/**'
+      - '!*.rst'
+      - '!*.md'
+      - '!datacube_ows/__init__.py'
+      - '!.github/**'
 
   push:
+    branches:
+      - 'master'
     paths:
       - '**'
+      - '.github/workflows/lint.yml'
+      - '!docs/**'
+      - '!*.rst'
+      - '!*.md'
+      - '!datacube_ows/__init__.py'
+      - '!.github/**'
 
 env:
   ORG: opendatacube
   IMAGE: ows
   DB_USERNAME: opendatacubeusername
 
 jobs:
```

### Comparing `datacube_ows-1.8.8/.github/workflows/pypi.yml` & `datacube_ows-1.8.9/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/.github/workflows/scan.yml` & `datacube_ows-1.8.9/.github/workflows/scan.yml`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/.github/workflows/test.yml` & `datacube_ows-1.8.9/.github/workflows/test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 ---
 name: Tests
 
 on:
   pull_request:
+    branches:
+        - 'master'
     paths:
       - '**'
+      - '.github/workflows/test.yml'
+      - '!docs/**'
+      - '!*.rst'
+      - '!*.md'
+      - '!datacube_ows/__init__.py'
+      - '!.github/**'
 
   push:
+    branches:
+      - 'master'
     paths:
       - '**'
+      - '.github/workflows/test.yml'
+      - '!docs/**'
+      - '!*.rst'
+      - '!*.md'
+      - '!datacube_ows/__init__.py'
+      - '!.github/**'
 
 env:
   ORG: opendatacube
   IMAGE: ows
   DB_USERNAME: opendatacubeusername
 
 jobs:
```

### Comparing `datacube_ows-1.8.8/.gitignore` & `datacube_ows-1.8.9/.gitignore`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/.yamllint` & `datacube_ows-1.8.9/.yamllint`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/CONTRIBUTING.rst` & `datacube_ows-1.8.9/CONTRIBUTING.rst`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 ============
 Contributing
 ============
 
 Contributions are welcome, and they are greatly appreciated! Every
 little bit helps, and credit will always be given.
 
+We have a `code of conduct<code-of-conduct.md>`_, so please follow it in all your interactions with the project.
+
 You can contribute in many ways:
 
 Types of Contributions
 ----------------------
 
 Report Bugs
 ~~~~~~~~~~~
 
 Report bugs at https://github.com/opendatacube/datacube-ows/issues.
 
-
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
 Fix Bugs
@@ -54,26 +55,20 @@
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
 
 Get Started!
 ------------
 
-Ready to contribute? Here's how to set up `datacube-ows` for local development.
-
 1. Fork the `datacube-ows` repo on GitHub.
 2. Clone your fork locally::
 
     $ git clone git@github.com:your_name_here/datacube-ows.git
 
-3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
-
-    $ mkvirtualenv datacube-ows
-    $ cd datacube-ows/
-    $ python setup.py develop
+3. Follow the instructions in `README.rst<https://datacube-ows.readthedocs.io/en/latest/readme.html>`_  to build a working python environment.
 
 4. Create a branch for local development::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
@@ -94,20 +89,20 @@
 7. Submit a pull request through the GitHub website.
 
 Pull Request Guidelines
 -----------------------
 
 Before you submit a pull request, check that it meets these guidelines:
 
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated.
+1. The pull request should include tests (and should pass them - and all pre-existing tests!)
+2. If the pull request adds or modifies functionality, the docs should be updated.
 3. The pull request should work for Python 3.7+. Check the results of
    the github actions and make sure that your PR passes all checks and
    does not decrease test coverage.
 
-Tips
-----
-
-To run a subset of tests::
+Links
+-----
 
-$ pytest tests.test_band_utils
+In case you haven't found them yet, please checkout the following resources:
 
+* `Documentation <https://datacube-ows.readthedocs.io/en/latest>`_
+* `Slack <http://slack.opendatacube.org>`_
```

### Comparing `datacube_ows-1.8.8/Dockerfile` & `datacube_ows-1.8.9/Dockerfile`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,66 @@
-ARG V_BASE=-3.0.4
+ARG V_BASE=3.3.0
 ARG py_env_path=/env
 
 # Build python libs in env_builder
-FROM opendatacube/geobase:wheels${V_BASE} as env_builder
+FROM opendatacube/geobase-builder:${V_BASE} as env_builder
+
+# REVISIT: Does this do anything, given we've already declared it above?
 ARG py_env_path
 
 COPY requirements.txt /
-RUN /usr/local/bin/env-build-tool new /requirements.txt ${py_env_path}
+COPY constraints.txt /
+RUN /usr/local/bin/env-build-tool new /requirements.txt /constraints.txt ${py_env_path}
 
 ENV PATH=${py_env_path}/bin:$PATH \
     PYTHONPATH=${py_env_path}
 
 # Copy source code and install it
 RUN mkdir -p /code
 WORKDIR /code
-ADD . /code
+COPY . /code
+
+RUN echo "version=\"$(python setup.py --version)\"" > datacube_ows/_version.py \
+    && pip install --no-cache-dir .
 
-RUN echo "version=\"`python setup.py --version`\"" > datacube_ows/_version.py
-RUN pip install .
 
+## Only install pydev requirements if arg PYDEV_DEBUG is set to 'yes'
+ARG PYDEV_DEBUG="no"
+RUN if [ "$PYDEV_DEBUG" = "yes" ]; then \
+    pip install --no-cache-dir pydevd-pycharm~=211.7142.13 \
+;fi
 
 # Runner image starts here
-FROM opendatacube/geobase:runner${V_BASE}
+FROM opendatacube/geobase-runner:${V_BASE}
+
 
 ENV LC_ALL=C.UTF-8 \
     DEBIAN_FRONTEND=noninteractive \
     SHELL=bash
 
-RUN apt-get update && apt install -y \
+ENV PATH="/env/bin:${PATH}"
+
+RUN apt-get update && apt-get install -y --no-install-recommends\
     curl \
     gnupg \
-    && rm -rf /var/lib/apt/lists/*
-
-# Install postgres client 11
-RUN curl https://www.postgresql.org/media/keys/ACCC4CF8.asc | apt-key add - && \
-    sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt/ bionic-pgdg main" > /etc/apt/sources.list.d/pgdg.list' && \
-    apt-get update && apt-get install -y \
-    postgresql-client-11 \
+    postgresql-client-12 \
     && rm -rf /var/lib/apt/lists/*
 
 # Configure user
-RUN useradd -m -s /bin/bash -N -g 100 -u 1000 ows
+RUN useradd -m -s /bin/bash -N -g 100 -u 1001 ows
 WORKDIR "/home/ows"
 
 # Copy python libs, add them to the path, configure GDAL
 ARG py_env_path
-COPY --chown=1000:100 --from=env_builder $py_env_path $py_env_path
+COPY --from=env_builder ${py_env_path} ${py_env_path}
 ENV PATH=${py_env_path}/bin:$PATH \
     PYTHONPATH=${py_env_path} \
     GDAL_DISABLE_READDIR_ON_OPEN="EMPTY_DIR" \
     CPL_VSIL_CURL_ALLOWED_EXTENSIONS=".tif, .tiff" \
     GDAL_HTTP_MAX_RETRY="10" \
-    GDAL_HTTP_RETRY_DELAY="1" 
+    GDAL_HTTP_RETRY_DELAY="1"
 
-## Only install pydev requirements if arg PYDEV_DEBUG is set to 'yes'
-ARG PYDEV_DEBUG="no"
-RUN if [ "$PYDEV_DEBUG"="yes" ]; then \
-    pip install pydevd-pycharm~=211.7142.13 \
-;fi
 
 RUN chown 1000:100 /dev/shm
 
 USER ows
-CMD gunicorn -b '0.0.0.0:8000' --workers=3 --threads=2 -k gevent --timeout 121 --pid /home/ows/gunicorn.pid --log-level info --worker-tmp-dir /dev/shm --config python:datacube_ows.gunicorn_config datacube_ows.wsgi
+CMD ["gunicorn", "-b", "0.0.0.0:8000", "--workers=3", "--threads=2", "-k", "gevent", "--timeout", "121", "--pid", "/home/ows/gunicorn.pid", "--log-level", "info", "--worker-tmp-dir", "/dev/shm", "--config", "python:datacube_ows.gunicorn_config", "datacube_ows.wsgi"]
```

### Comparing `datacube_ows-1.8.8/HISTORY.rst` & `datacube_ows-1.8.9/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/LICENSE` & `datacube_ows-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/Makefile` & `datacube_ows-1.8.9/Makefile`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/PKG-INFO` & `datacube_ows-1.8.9/datacube_ows.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-Metadata-Version: 1.1
-Name: datacube_ows
-Version: 1.8.8
+Metadata-Version: 2.1
+Name: datacube-ows
+Version: 1.8.9
 Summary: Open Data Cube Open Web Services
 Home-page: https://github.com/opendatacube/datacube-ows
 Author: Open Data Cube
 Author-email: earth.observation@ga.gov.au
 License: Apache Software License 2.0
-Description: 
-        ============
-        datacube-ows
-        ============
-        
-        Open Web Services for the Open Datacube.
-        
-        * Free software: Apache Software License 2.0
-        * Documentation: https://datacube-ows.readthedocs.io.
-        
-        Features
-        --------
-        
-        * Leverages the power of the Open Data Cube, including support for COGs on S3.
-        * Supports WMS and WMTS.
-        * Experimental support for WCS (1.0, 2.0, 2.1).
-            
-            
 Keywords: datacube,wms,wcs
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.5
+License-File: LICENSE
+
+
+============
+datacube-ows
+============
+
+Open Web Services for the Open Datacube.
+
+* Free software: Apache Software License 2.0
+* Documentation: https://datacube-ows.readthedocs.io.
+
+Features
+--------
+
+* Leverages the power of the Open Data Cube, including support for COGs on S3.
+* Supports WMS and WMTS.
+* Experimental support for WCS (1.0, 2.0, 2.1).
+
+    
+
```

### Comparing `datacube_ows-1.8.8/README.rst` & `datacube_ows-1.8.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -19,30 +19,33 @@
 
 Datacube Open Web Services
 
 
 * Free software: Apache Software License 2.0
 * Documentation: https://datacube-ows.readthedocs.io.
 
-
 Features
 --------
 
 * Leverages the power of the Open Data Cube, including support for COGs on S3.
 * Supports WMS and WMTS.
 * Experimental support for WCS (1.0, 2.0, 2.1).
 
-Note on Naming
---------------
+Community
+---------
+
+This project welcomes community participation.
 
-This project originally supported WMS only and was known as "datacube_wms".
+`Join the ODC Slack <http://slack.opendatacube.org>`__ if you need help
+setting up or using this project, or the Open Data Cube more generally.
+Conversation about datacube-ows is mostly concentrated in the Slack
+channel ``#wms``.
 
-There are still a handful of file and object names in the codebase that
-include the substring "wms" although they are actually more general.
-These names will be updated to "ows" as time permits.
+Please help us to keep the Open Data Cube community open and inclusive by
+reading and following our `Code of Conduct <code-of-conduct.md>`__.
 
 Setup
 -----
 
 Datacube_ows (and datacube_core itself) has many complex dependencies on particular versions of
 geospatial libraries.  Dependency conflicts are almost unavoidable in environments that also contain
 other large complex geospatial software packages.  We therefore strongly recommend some kind of
```

### Comparing `datacube_ows-1.8.8/check-code-all.sh` & `datacube_ows-1.8.9/check-code-all.sh`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/create_tables.sql` & `datacube_ows-1.8.9/create_tables.sql`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/datacube_ows/band_utils.py` & `datacube_ows-1.8.9/datacube_ows/band_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import division
 
 import numpy
 
 # Style index functions
```

### Comparing `datacube_ows-1.8.8/datacube_ows/config_toolkit.py` & `datacube_ows-1.8.9/datacube_ows/config_toolkit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from copy import deepcopy
 
 
 def deepinherit(parent, child):
     expanded = deepcopy(parent)
     deepupdate(expanded, child)
     return expanded
```

### Comparing `datacube_ows-1.8.8/datacube_ows/cube_pool.py` & `datacube_ows-1.8.9/datacube_ows/cube_pool.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import, division, print_function
 
 import logging
 from contextlib import contextmanager
 from threading import Lock
 
 from datacube import Datacube
```

### Comparing `datacube_ows-1.8.8/datacube_ows/data.py` & `datacube_ows-1.8.9/datacube_ows/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import
 
 import json
 import logging
 import re
 from collections import OrderedDict
 from datetime import datetime
```

### Comparing `datacube_ows-1.8.8/datacube_ows/legend_generator.py` & `datacube_ows-1.8.9/datacube_ows/legend_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import
 
 import io
 import logging
 
 import matplotlib
 import numpy as np
```

### Comparing `datacube_ows-1.8.8/datacube_ows/mv_index.py` & `datacube_ows-1.8.9/datacube_ows/mv_index.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 import json
 from enum import Enum
 
 from datacube.utils.geometry import Geometry as ODCGeom
 from geoalchemy2 import Geometry
 from psycopg2.extras import DateTimeTZRange
 from sqlalchemy import SMALLINT, Column, MetaData, Table, or_, select, text
```

### Comparing `datacube_ows-1.8.8/datacube_ows/ogc.py` & `datacube_ows-1.8.9/datacube_ows/ogc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 import sys
 import traceback
 from time import monotonic
 
 from flask import g, render_template, request
 from flask_log_request_id import current_request_id
 
@@ -25,19 +30,21 @@
 
 # Initialisation of external libraries - controlled by environment variables.
 initialise_debugging(_LOG)
 initialise_sentry(_LOG)
 initialise_aws_credentials(_LOG)
 
 # Prepare parsed configuration object
-parse_config_file()
+cfg = parse_config_file()
 
 # Initialise Flask
 app = initialise_flask(__name__)
 
+babel = initialise_babel(cfg, app)
+
 # Initialisation of external libraries that depend on Flask
 # (controlled by environment variables)
 metrics = initialise_prometheus(app, _LOG)
 
 # Protocol/Version lookup table
 OWS_SUPPORTED = supported_versions()
 
@@ -67,15 +74,15 @@
         elif op in WCS_REQUESTS:
             return ogc_svc_impl("wcs")
         elif op:
             # Should we return a WMS or WCS exception if there is no service specified?
             # Defaulting to WMS because that's what we already have.
             raise WMSException("Invalid service and/or request", locator="Service and request parameters")
         else:
-            cfg = get_config()
+            cfg = get_config()   # pylint: disable=redefined-outer-name
             url = nocase_args.get('Host', nocase_args['url_root'])
             base_url = get_service_base_url(cfg.allowed_urls, url)
             return (render_template(
                             "index.html",
                             cfg=cfg,
                             supported=OWS_SUPPORTED,
                             base_url=base_url,
@@ -164,14 +171,15 @@
         return (render_template("ping.html", status="Up"), 200, resp_headers({"Content-Type": "text/html"}))
     else:
         return (render_template("ping.html", status="Down"), 500, resp_headers({"Content-Type": "text/html"}))
 
 
 @app.route("/legend/<string:layer>/<string:style>/legend.png")
 def legend(layer, style, dates=None):
+    # pylint: disable=redefined-outer-name
     cfg = get_config()
     product = cfg.product_index.get(layer)
     if not product:
         return ("Unknown Layer", 404, resp_headers({"Content-Type": "text/plain"}))
     if dates is None:
         args = lower_get_args()
         ndates = int(args.get("ndates", 0))
@@ -193,14 +201,15 @@
 def append_request_id(response):
     response.headers.add("X-REQUEST-ID", current_request_id())
     return response
 
 
 @app.before_request
 def start_timer():
+    # pylint: disable=assigning-non-slot
     g.ogc_start_time = monotonic()
 
 
 @app.after_request
 def log_time_and_request_response(response):
     time_taken = int((monotonic() - g.ogc_start_time) * 1000)
     _LOG.info("request: %s returned status: %d and took: %d ms", request.url, response.status_code, time_taken)
```

### Comparing `datacube_ows-1.8.8/datacube_ows/ogc_exceptions.py` & `datacube_ows-1.8.9/datacube_ows/ogc_exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import, division, print_function
 
 import traceback as tb
 
 from flask import render_template
 from ows.common.types import OWSException, Version
 from ows.common.v20.encoders import xml_encode_exception_report
```

### Comparing `datacube_ows-1.8.8/datacube_ows/ogc_utils.py` & `datacube_ows-1.8.9/datacube_ows/ogc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import, division, print_function
 
 import datetime
 import logging
 import re
 from importlib import import_module
 from itertools import chain
@@ -59,16 +64,16 @@
 def tz_for_dataset(ds):
     return tz_for_geometry(ds.extent)
 
 
 def tz_for_coord(lon, lat):
     try:
         tzn = tf.timezone_at(lng=lon, lat=lat)
-    except:
-        print("Woah!")
+    except Exception as e:
+        _LOG.warning("Timezone detection failed for lat %f, lon %s (%s)", lat, lon, str(e))
         raise
     if not tzn:
         raise NoTimezoneException("tz find failed.")
     return timezone(tzn)
 
 
 def local_solar_date_range(geobox, date):
@@ -327,15 +332,20 @@
     if height is None:
         scale_y = - scale_x
         height = round((miny - maxy) / scale_y)
     affine = Affine.translation(minx, maxy) * Affine.scale(scale_x, scale_y)
     return geometry.GeoBox(width, height, affine, crs)
 
 
-def xarray_image_as_png(img_data, mask=None):
+def xarray_image_as_png(img_data, mask=None, loop_over=None):
+    if loop_over:
+        return [
+            xarray_image_as_png(img_data.sel(**{loop_over: coord}), mask=mask)
+            for coord in img_data.coords[loop_over].values
+        ]
     band_index = {
         "red": 1,
         "green": 2,
         "blue": 3,
         "alpha": 4,
     }
     xcoord = None
@@ -375,7 +385,9 @@
                 if mask is None:
                     alpha_mask = numpy.empty(last_band.shape).astype('uint8')
                     alpha_mask.fill(255)
                 else:
                     alpha_mask = numpy.where(mask, 255, 0).astype('uint8')
                 thing.write_band(4, alpha_mask)
         return memfile.read()
+
+
```

### Comparing `datacube_ows-1.8.8/datacube_ows/ows_cfg_example.py` & `datacube_ows-1.8.9/datacube_ows/ows_cfg_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 # pylint: skip-file
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
+
 
 # Example configuration file for datacube_ows.
 #
 # For detailed formal documentation see:
 #
 #   https://datacube-ows.readthedocs.io/en/latest/configuration.html
 #
@@ -1288,14 +1294,37 @@
                 "postcode": "12345",
                 "country": "Elbonia",
             },
             "telephone": "+61 2 1234 5678",
             "fax": "+61 2 1234 6789",
             "email": "test@example.com",
         },
+        # Attribution.
+        #
+        # This provides a way to identify the source of the data used in a WMS layer or layers.
+        # This entire section is optional.  If provided, it is taken as the
+        # default attribution for any layer that does not override it.
+        "attribution": {
+            # Attribution must contain at least one of ("title", "url" and "logo")
+            # A human readable title for the attribution - e.g. the name of the attributed organisation
+            "title": "Acme Satellites",
+            # The associated - e.g. URL for the attributed organisation
+            "url": "http://www.acme.com/satellites",
+            # Logo image - e.g. for the attributed organisation
+            "logo": {
+                # Image width in pixels (optional)
+                "width": 370,
+                # Image height in pixels (optional)
+                "height": 73,
+                # URL for the logo image. (required if logo specified)
+                "url": "https://www.acme.com/satellites/images/acme-370x73.png",
+                # Image MIME type for the logo - should match type referenced in the logo url (required if logo specified.)
+                "format": "image/png",
+            }
+        },
         # If fees are charged for the use of the service, these can be described here in free text.
         # If blank or not included, defaults to "none".
         "fees": "",
         # If there are constraints on access to the service, they can be described here in free text.
         # If blank or not included, defaults to "none".
         "access_constraints": "",
         # Supported co-ordinate reference systems. Any coordinate system supported by GDAL and Proj.4J can be used.
@@ -1308,14 +1337,19 @@
                 "horizontal_coord": "x",
                 "vertical_coord": "y",
             },
             "EPSG:4326": {  # WGS-84
                 "geographic": True,
                 "vertical_coord_first": True
             },
+            "EPSG:3111": {  # VicGrid94 for delwp.vic.gov.au
+               "geographic": False,
+                "horizontal_coord": "x",
+                "vertical_coord": "y",
+            },
             "EPSG:3577": {  # GDA-94, internal representation
                 "geographic": False,
                 "horizontal_coord": "x",
                 "vertical_coord": "y",
             },
         },
     },   #### End of "global" section.
@@ -1330,35 +1364,15 @@
         "s3_url": "http://data.au",
         "s3_bucket": "s3_bucket_name",
         "s3_aws_zone": "ap-southeast-2",
         # Max tile height/width for wms.  (N.B. Does not apply to WMTS)
         # Optional, defaults to 256x256
         "max_width": 512,
         "max_height": 512,
-        # Attribution. This provides a way to identify the source of the data used in a layer or layers.
-        # This entire section is optional.  If provided, it is taken as the
-        # default attribution for any layer that does not override it.
-        "attribution": {
-            # Attribution must contain at least one of ("title", "url" and "logo")
-            # A human readable title for the attribution - e.g. the name of the attributed organisation
-            "title": "Acme Satellites",
-            # The associated - e.g. URL for the attributed organisation
-            "url": "http://www.acme.com/satellites",
-            # Logo image - e.g. for the attributed organisation
-            "logo": {
-                # Image width in pixels (optional)
-                "width": 370,
-                # Image height in pixels (optional)
-                "height": 73,
-                # URL for the logo image. (required if logo specified)
-                "url": "https://www.acme.com/satellites/images/acme-370x73.png",
-                # Image MIME type for the logo - should match type referenced in the logo url (required if logo specified.)
-                "format": "image/png",
-            }
-        },
+
         # These define the AuthorityURLs.
         # They represent the authorities that define the "Identifiers" defined layer by layer below.
         # The spec allows AuthorityURLs to be defined anywhere on the Layer heirarchy, but datacube_ows treats them
         # as global entities.
         # Required if identifiers are to be declared for any layer.
         "authorities": {
             # The authorities dictionary maps names to authority urls.
@@ -1919,11 +1933,7 @@
             "styling": {
                 "default_style": "mangrove",
                 "styles": [style_mangrove],
             }
         } ##### End of mangrove_cover definition
     ]  ##### End of "layers" list.
 } #### End of example configuration object
-
-
-
-
```

### Comparing `datacube_ows-1.8.8/datacube_ows/ows_configuration.py` & `datacube_ows-1.8.9/datacube_ows/ows_configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,39 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
+
 #
 #  Note this is NOT the configuration file!
 #
 #  This is a Python module containing the classes and functions used to load and parse configuration files.
 #
 #  Refer to the documentation for information on how to configure datacube_ows.
 #
-
+import datetime
 import json
 import logging
 import math
 import os
 from collections.abc import Mapping
 from importlib import import_module
 
+from babel.messages.catalog import Catalog
+from babel.messages.pofile import read_po
 from datacube.utils import geometry
 from ows import Version
 from slugify import slugify
 
 from datacube_ows.config_utils import (FlagProductBands, OWSConfigEntry,
                                        OWSEntryNotFound,
                                        OWSExtensibleConfigEntry, OWSFlagBand,
-                                       cfg_expand, import_python_obj,
+                                       OWSMetadataConfig, cfg_expand,
+                                       get_file_loc, import_python_obj,
                                        load_json_obj)
 from datacube_ows.cube_pool import cube, get_cube, release_cube
 from datacube_ows.ogc_utils import (ConfigException, FunctionWrapper,
                                     create_geobox, day_summary_date_range,
                                     local_solar_date_range, month_date_range,
                                     year_date_range)
 from datacube_ows.styles import StyleDef
@@ -40,16 +49,15 @@
         cfg_env = path
     else:
         cfg_env = os.environ.get("DATACUBE_OWS_CFG")
     if not cfg_env:
         from datacube_ows.ows_cfg import ows_cfg as cfg
     elif "/" in cfg_env or cfg_env.endswith(".json"):
         cfg = load_json_obj(cfg_env)
-        abs_path =  os.path.abspath(cfg_env)
-        cwd = os.path.dirname(abs_path)
+        cwd = get_file_loc(cfg_env)
     elif "." in cfg_env:
         cfg = import_python_obj(cfg_env)
     elif cfg_env.startswith("{"):
         cfg = json.loads(cfg_env)
         abs_path = os.path.abspath(cfg_env)
         cwd = os.path.dirname(abs_path)
     else:
@@ -119,17 +127,17 @@
         return [self.band_label(b) for b in self.band_cfg]
 
     def band_nodata_vals(self):
         return [self.nodata_val(b) for b in self.band_cfg if b in self.band_cfg]
 
 
 class AttributionCfg(OWSConfigEntry):
-    def __init__(self, cfg):
+    def __init__(self, cfg, owner):
         super().__init__(cfg)
-        self.title = cfg.get("title")
+        self.owner = owner
         self.url = cfg.get("url")
         logo = cfg.get("logo")
         if not self.title and not self.url and not logo:
             raise ConfigException("At least one of title, url and logo is required in an attribution definition")
         if not logo:
             self.logo_width = None
             self.logo_height = None
@@ -139,20 +147,24 @@
             self.logo_width = logo.get("width")
             self.logo_height = logo.get("height")
             self.logo_url = logo.get("url")
             self.logo_fmt = logo.get("format")
             if not self.logo_url or not self.logo_fmt:
                 raise ConfigException("url and format must both be specified in an attribution logo.")
 
+    @property
+    def title(self):
+        return self.owner.attribution_title
+
     @classmethod
-    def parse(cls, cfg):
+    def parse(cls, cfg, owner):
         if not cfg:
             return None
         else:
-            return cls(cfg)
+            return cls(cfg, owner)
 
 
 class SuppURL(OWSConfigEntry):
     @classmethod
     def parse_list(cls, cfg):
         if not cfg:
             return []
@@ -161,72 +173,81 @@
     def __init__(self, cfg):
         super().__init__(cfg)
         self.url = cfg["url"]
         self.format = cfg["format"]
 
 
 
-class OWSLayer(OWSConfigEntry):
+class OWSLayer(OWSMetadataConfig):
+    METADATA_KEYWORDS = True
+    METADATA_ATTRIBUTION = True
+
     named = False
-    def __init__(self, cfg, parent_layer=None, **kwargs):
+    def __init__(self, cfg, object_label, parent_layer=None, **kwargs):
         super().__init__(cfg, **kwargs)
+        self.object_label = object_label
         self.global_cfg = kwargs["global_cfg"]
         self.parent_layer = parent_layer
 
-        if "title" not in cfg:
-            raise ConfigException("Layer without title found under parent layer %s" % str(parent_layer))
-        self.title = cfg["title"]
-        if "abstract" in cfg:
-            self.abstract = cfg["abstract"]
-        elif parent_layer:
-            self.abstract = parent_layer.abstract
-        else:
-            raise ConfigException("No abstract supplied for top-level layer %s" % self.title)
-        # Accumulate keywords
-        self.keywords = set()
-        if self.parent_layer:
-            for word in self.parent_layer.keywords:
-                self.keywords.add(word)
-        else:
-            for word in self.global_cfg.keywords:
-                self.keywords.add(word)
-        for word in cfg.get("keywords", []):
-            self.keywords.add(word)
+        self.parse_metadata(cfg)
         # Inherit or override attribution
         if "attribution" in cfg:
-            self.attribution = AttributionCfg.parse(cfg.get("attribution"))
+            self.attribution = AttributionCfg.parse(cfg.get("attribution"), self)
         elif parent_layer:
             self.attribution = self.parent_layer.attribution
         else:
             self.attribution = self.global_cfg.attribution
 
+    def global_config(self):
+        return self.global_cfg
+
+    def can_inherit_from(self):
+        if self.parent_layer:
+            return self.parent_layer
+        else:
+            return self.global_cfg
+
+    def get_obj_label(self):
+        return self.object_label
+
     def layer_count(self):
         return 0
 
     def unready_layer_count(self):
         return 0
 
     def __str__(self):
         return "OWSLayer Config: %s" % self.title
 
 
 class OWSFolder(OWSLayer):
-    def __init__(self, cfg, global_cfg, parent_layer=None, **kwargs):
-        super().__init__(cfg, parent_layer, global_cfg=global_cfg, **kwargs)
+    def __init__(self, cfg, global_cfg, parent_layer=None, sibling=0, **kwargs):
+        if "label" in cfg:
+            obj_lbl = f"folder.{cfg['label']}"
+        elif parent_layer:
+            obj_lbl = f"{parent_layer.object_label}.{sibling}"
+        else:
+            obj_lbl = f"folder.{sibling}"
+        if obj_lbl in global_cfg.folder_index:
+            raise ConfigException(f"Duplicate folder label: {obj_lbl}")
+        super().__init__(cfg, parent_layer=parent_layer, object_label=obj_lbl, global_cfg=global_cfg, **kwargs)
         self.slug_name = slugify(self.title, separator="_")
         self.unready_layers = []
         self.child_layers = []
         if "layers" not in cfg:
             raise ConfigException("No layers section in folder layer %s" % self.title)
+        child = 0
         for lyr_cfg in cfg["layers"]:
             try:
-                lyr = parse_ows_layer(lyr_cfg, global_cfg, parent_layer=self)
+                lyr = parse_ows_layer(lyr_cfg, global_cfg=global_cfg, parent_layer=self, sibling=child)
                 self.unready_layers.append(lyr)
             except ConfigException as e:
                 _LOG.error("Could not parse layer: %s", str(e))
+            child += 1
+        global_cfg.folder_index[obj_lbl] = self
 
     def unready_layer_count(self):
         return sum([l.layer_count() for l in self.unready_layers])
 
     def layer_count(self):
         return sum([l.layer_count() for l in self.child_layers])
 
@@ -304,15 +325,15 @@
 
 class OWSNamedLayer(OWSExtensibleConfigEntry, OWSLayer):
     INDEX_KEYS = ["layer"]
     named = True
 
     def __init__(self, cfg, global_cfg, parent_layer=None, **kwargs):
         name = cfg["name"]
-        super().__init__(cfg, global_cfg=global_cfg, parent_layer=parent_layer,
+        super().__init__(cfg, object_label=f"layer.{name}", global_cfg=global_cfg, parent_layer=parent_layer,
                          keyvals={"layer": name},
                          **kwargs)
         self.name = name
         cfg = self._raw_cfg
         self.hide = False
         try:
             self.parse_product_names(cfg)
@@ -380,15 +401,14 @@
 #        if "extractor" in sub_prod_cfg:
 #            self.sub_product_extractor = FunctionWrapper(self, sub_prod_cfg["extractor"])
 #        else:
 #            self.sub_product_extractor = None
         # And finally, add to the global product index.
         self.global_cfg.product_index[self.name] = self
 
-
     # pylint: disable=attribute-defined-outside-init
     def make_ready(self, dc, *args, **kwargs):
         self.products = []
         self.low_res_products = []
         for i, prod_name in enumerate(self.product_names):
             if self.low_res_product_names:
                 low_res_prod_name = self.low_res_product_names[i]
@@ -846,22 +866,22 @@
             raise ConfigException(f"'low_res_product' entry in flags section of multi-product layer {self.name} - use 'low_res_products' only")
         return {
             "pq_names": pq_names,
             "pq_low_res_names": pq_low_res_names,
         }
 
 
-def parse_ows_layer(cfg, global_cfg, parent_layer=None):
+def parse_ows_layer(cfg, global_cfg, parent_layer=None, sibling=0):
     if cfg.get("name", None):
         if cfg.get("multi_product", False):
             return OWSMultiProductLayer(cfg, global_cfg, parent_layer)
         else:
             return OWSProductLayer(cfg, global_cfg, parent_layer)
     else:
-        return OWSFolder(cfg, global_cfg, parent_layer)
+        return OWSFolder(cfg, global_cfg, parent_layer=parent_layer, sibling=sibling)
 
 
 class WCSFormat:
     @staticmethod
     def from_cfg(cfg):
         renderers = []
         for name, fmt in cfg.items():
@@ -910,31 +930,83 @@
         if isinstance(version, str):
             version = int(version.split(".")[0])
         elif isinstance(version, Version):
             version = version.major
         return self.renderers[version]
 
 
-class OWSConfig(OWSConfigEntry):
+class ContactInfo(OWSConfigEntry):
+    def __init__(self, cfg, global_cfg):
+        super().__init__(cfg)
+        self.global_cfg = global_cfg
+        self.person = cfg.get("person")
+
+        class Address(OWSConfigEntry):
+            def __init__(self, cfg):
+                super().__init__(cfg)
+                self.type = cfg.get("type")
+                self.address = cfg.get("address")
+                self.city = cfg.get("city")
+                self.state = cfg.get("state")
+                self.postcode = cfg.get("postcode")
+                self.country = cfg.get("country")
+
+            @classmethod
+            def parse(cls, cfg):
+                if not cfg:
+                    return None
+                else:
+                    return cls(cfg)
+
+        self.address = Address.parse(cfg.get("address"))
+        self.telephone = cfg.get("telephone")
+        self.fax = cfg.get("fax")
+        self.email = cfg.get("email")
+
+    @property
+    def organisation(self):
+        return self.global_cfg.contact_org
+
+    @property
+    def position(self):
+        return self.global_cfg.contact_position
+
+    @classmethod
+    def parse(cls, cfg, global_cfg):
+        if cfg:
+            return cls(cfg, global_cfg)
+        else:
+            return None
+
+
+class OWSConfig(OWSMetadataConfig):
     _instance = None
     initialised = False
 
     def __new__(cls, *args, **kwargs):
         if not cls._instance or kwargs.get("refresh"):
             cls._instance = super().__new__(cls)
         return cls._instance
 
-    def __init__(self, refresh=False, cfg=None):
+    METADATA_KEYWORDS = True
+    METADATA_ATTRIBUTIONS = True
+    METADATA_FEES = True
+    METADATA_ACCESS_CONSTRAINTS = True
+    METADATA_CONTACT_INFO = True
+
+    default_abstract = ""
+
+    def __init__(self, refresh=False, cfg=None, ignore_msgfile=False):
         if not self.initialised or refresh:
+            self.msgfile = None
             if not cfg:
                 cfg = read_config()
             super().__init__(cfg)
-            self.initialised = True
             try:
-                self.parse_global(cfg["global"])
+                self.parse_global(cfg["global"], ignore_msgfile)
             except KeyError as e:
                 raise ConfigException(
                     "Missing required config entry in 'global' section: %s" % str(e)
                 )
 
             if self.wms or self.wmts:
                 self.parse_wms(cfg.get("wms", {}))
@@ -960,41 +1032,85 @@
                     self.parse_wmts(cfg.get("wmts", {}))
                 else:
                     self.parse_wmts({})
             except KeyError as e:
                 raise ConfigException(
                     "Missing required config entry in 'wmts' section (with WCS enabled): %s" % str(e)
                 )
+            self.catalog = None
+            self.initialised = True
 
     #pylint: disable=attribute-defined-outside-init
     def make_ready(self, dc, *args, **kwargs):
+        if self.msg_file_name:
+            try:
+                with open(self.msg_file_name, "rb") as fp:
+                    self.set_msg_src(read_po(fp, locale=self.default_locale, domain=self.message_domain))
+            except FileNotFoundError:
+                _LOG.warning("Message file %s does not exist - using metadata from config file", self.msg_file_name)
+        else:
+            self.set_msg_src(None)
         self.native_product_index = {}
         self.root_layer_folder.make_ready(dc, *args, **kwargs)
         super().make_ready(dc, *args, **kwargs)
 
-    def parse_global(self, cfg):
+    def export_metadata(self):
+        if self.catalog is None:
+            now = datetime.datetime.now()
+            self.catalog = Catalog(locale=self.default_locale,
+                                   domain=self.message_domain,
+                                   header_comment=f"""# Translations for datacube-ows metadata instance:
+#      {self.title}
+#
+# {self.contact_info.organisation} {now.isoformat()} 
+#""",
+                                   project=self.title,
+                                   version=f"{now.isoformat()}",
+                                   copyright_holder=self.contact_info.organisation,
+                                   msgid_bugs_address=self.contact_info.email,
+                                   creation_date=now,
+                                   revision_date=now,
+                                   fuzzy=False)
+            for k, v in self._metadata_registry.items():
+                if self._inheritance_registry[k]:
+                    continue
+                if k in [
+                        "folder.ows_root_hidden.title",
+                        "folder.ows_root_hidden.abstract",
+                        "folder.ows_root_hidden.local_keywords",
+                 ]:
+                    continue
+                self.catalog.add(id=k, string=v, auto_comments=[v])
+        return self.catalog
+
+    def parse_global(self, cfg, ignore_msgfile):
         self._response_headers = cfg.get("response_headers", {})
         self.wms = cfg.get("services", {}).get("wms", True)
         self.wmts = cfg.get("services", {}).get("wmts", True)
         self.wcs = cfg.get("services", {}).get("wcs", False)
         if not self.wms and not self.wmts and not self.wcs:
             raise ConfigException("At least one service must be active.")
-        self.title = cfg["title"]
+        self.locales = cfg.get("supported_languages", ["en"])
+        if len(self.locales) < 1:
+            raise ConfigException("You must support at least one language.")
+        self.default_locale = self.locales[0]
+        self.message_domain = cfg.get("message_domain", "ows_cfg")
+        self.translations_dir = cfg.get("translations_directory")
+        self.internationalised = self.translations_dir and len(self.locales) > 1
+        if self.internationalised:
+            _LOG.info("Internationalisation enabled.")
+        if ignore_msgfile:
+            self.msg_file_name = None
+        else:
+            self.msg_file_name = cfg.get("message_file")
+        self.parse_metadata(cfg)
         self.allowed_urls = cfg["allowed_urls"]
         self.info_url = cfg["info_url"]
-        self.abstract = cfg.get("abstract")
-        self.contact_info = cfg.get("contact_info", {})
-        self.keywords = cfg.get("keywords", [])
-        self.fees = cfg.get("fees")
-        self.access_constraints = cfg.get("access_constraints")
-        # self.use_extent_views = cfg.get("use_extent_views", False)
-        if not self.fees:
-            self.fees = "none"
-        if not self.access_constraints:
-            self.access_constraints = "none"
+        self.contact_info = ContactInfo.parse(cfg.get("contact_info"), self)
+        self.attribution = AttributionCfg.parse(cfg.get("attribution"), self)
 
         def make_gml_name(name):
             if name.startswith("EPSG:"):
                 return f"http://www.opengis.net/def/crs/EPSG/0/{name[5:]}"
             else:
                 return name
 
@@ -1036,17 +1152,18 @@
         if not self.wms and not self.wmts:
             cfg = {}
         self.s3_bucket = cfg.get("s3_bucket", "")
         self.s3_url = cfg.get("s3_url", "")
         self.s3_aws_zone = cfg.get("s3_aws_zone", "")
         self.wms_max_width = cfg.get("max_width", 256)
         self.wms_max_height = cfg.get("max_height", 256)
-        self.attribution = AttributionCfg.parse(cfg.get("attribution"))
         self.authorities = cfg.get("authorities", {})
         self.user_band_math_extension = cfg.get("user_band_math_extension", False)
+        if "attribution" in cfg:
+            _LOG.warning("Attribution entry in top level 'wms' section will be ignored. Attribution should be moved to the 'global' section")
 
     def parse_wcs(self, cfg):
         if self.wcs:
             if not isinstance(cfg, Mapping):
                 raise ConfigException("WCS section missing (and WCS is enabled)")
             self.wcs_formats = WCSFormat.from_cfg(cfg["formats"])
             self.wcs_formats_by_name = {
@@ -1084,21 +1201,22 @@
             if len(identifier.split()) != 1:
                 raise ConfigException(f"Invalid identifier: {identifier}")
             if identifier in self.tile_matrix_sets:
                 raise ConfigException(f"Tile matrix set identifiers must be unique: {identifier}")
             self.tile_matrix_sets[identifier] = TileMatrixSet(identifier, tms, self)
 
     def parse_layers(self, cfg):
+        self.folder_index = {}
         self.product_index = {}
         self.declare_unready("native_product_index")
         self.root_layer_folder = OWSFolder({
             "title": "Root Folder (hidden)",
-            "abstract": ".",
+            "label": "ows_root_hidden",
             "layers": cfg
-        }, self, None)
+        }, global_cfg=self, parent_layer=None)
 
     @property
     def layers(self):
         return self.root_layer_folder.child_layers
 
     def alias_bboxes(self, bboxes):
         out = {}
```

### Comparing `datacube_ows-1.8.8/datacube_ows/product_ranges.py` & `datacube_ows-1.8.9/datacube_ows/product_ranges.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
+
 #pylint: skip-file
 
 from __future__ import absolute_import, division, print_function
 
 from datetime import datetime, timedelta, timezone
 
 import datacube
```

### Comparing `datacube_ows-1.8.8/datacube_ows/protocol_versions.py` & `datacube_ows-1.8.9/datacube_ows/protocol_versions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from datacube_ows.ogc_exceptions import (WCS1Exception, WCS2Exception,
                                          WMSException, WMTSException)
 from datacube_ows.ows_configuration import get_config
 from datacube_ows.wcs1 import handle_wcs1
 from datacube_ows.wcs2 import handle_wcs2
 from datacube_ows.wms import handle_wms
 from datacube_ows.wmts import handle_wmts
```

### Comparing `datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/010_create_new_time_view.sql` & `datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/010_create_new_time_view.sql`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/datacube_ows/sql/extent_views/create/011_create_new_space_view_raw.sql` & `datacube_ows-1.8.9/datacube_ows/sql/extent_views/create/011_create_new_space_view_raw.sql`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/datacube_ows/sql/use_space_time.sql` & `datacube_ows-1.8.9/datacube_ows/sql/use_space_time.sql`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/datacube_ows/startup_utils.py` & `datacube_ows-1.8.9/datacube_ows/startup_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,46 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import, division, print_function
 
 import logging
 import os
 import warnings
 
 import sentry_sdk
 from datacube.utils.aws import configure_s3_access
 from flask import Flask, request
+from flask_babel import Babel
 from flask_log_request_id import RequestID, RequestIDLogFilter
 from prometheus_flask_exporter.multiprocess import \
     GunicornInternalPrometheusMetrics
 from rasterio.errors import NotGeoreferencedWarning
 from sentry_sdk.integrations.flask import FlaskIntegration
 
 from datacube_ows.ows_configuration import get_config
 
 __all__ = [
+    'initialise_babel',
     'initialise_logger',
     'initialise_ignorable_warnings',
     'initialise_debugging',
     'initialise_sentry',
     'initialise_aws_credentials',
     'parse_config_file',
     'initialise_flask',
     'initialise_prometheus',
     'initialise_prometheus_register',
+    'generate_locale_selector'
 ]
 
 
+
 def initialise_logger(name=None):
     handler = logging.StreamHandler()
     handler.setFormatter(logging.Formatter("[%(asctime)s] %(name)s [%(request_id)s] [%(levelname)s] %(message)s"))
     handler.addFilter(RequestIDLogFilter())
     _LOG = logging.getLogger(name)
     _LOG.addHandler(handler)
     # If invoked using Gunicorn, link our root logger to the gunicorn logger
@@ -99,16 +108,18 @@
     elif log:
         log.warning("Environment variable $AWS_DEFAULT_REGION not set.  (This warning can be ignored if all data is stored locally.)")
 
 
 def parse_config_file(log=None):
     # Cache a parsed config file object
     # (unless deferring to first request)
+    cfg = None
     if not os.environ.get("DEFER_CFG_PARSE"):
-        get_config()
+        cfg = get_config()
+    return cfg
 
 
 def initialise_flask(name):
     app = Flask(name.split('.')[0])
     RequestID(app)
     return app
 
@@ -133,7 +144,26 @@
                     'query_request': lambda: request.args.get('request'),
                     'query_service': lambda: request.args.get('service'),
                     'query_layers': lambda: request.args.get('layers'),
                     'query_url': lambda: request.full_path
                 }
             )
         )
+
+
+def generate_locale_selector(locales):
+    def selector_template():
+        return request.accept_languages.best_match(locales)
+    return selector_template
+
+def initialise_babel(cfg, app):
+    if cfg and cfg.internationalised:
+        app.config["BABEL_TRANSLATION_DIRECTORIES"] = cfg.translations_dir
+        babel = Babel(app,
+                      default_locale=cfg.locales[0],
+                      default_domain=cfg.message_domain,
+                      configure_jinja=False
+                      )
+        babel.localeselector(generate_locale_selector(cfg.locales))
+        return babel
+    else:
+        return None
```

### Comparing `datacube_ows-1.8.8/datacube_ows/styles/api/base.py` & `datacube_ows-1.8.9/datacube_ows/styles/api/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
+import xarray
+
 from datacube_ows.startup_utils import initialise_ignorable_warnings
 from datacube_ows.styles.base import StandaloneProductProxy, StyleDefBase
 
 initialise_ignorable_warnings()
 
 
 def StandaloneStyle(cfg):
@@ -17,40 +24,58 @@
     :return: A OWS Style Definition object, prepared to work in standalone mode.
     """
     style = StyleDefBase(StandaloneProductProxy(), cfg, stand_alone=True)
     style.make_ready(None)
     return style
 
 
-def apply_ows_style(style, data, valid_data_mask=None):
+def apply_ows_style(style, data, loop_over=None, valid_data_mask=None):
     """
     Apply an OWS style to an ODC XArray to generate a styled image.
 
     :param style: An OWS Style object, as created by StandaloneStyle()
     :param data: An xarray Dataset, as generated by datacube.load_data()
             Note that the Dataset must contain all of the band names referenced by the standalone style
             configuration.  (The names of the data variables in the dataset must exactly match
             the band names in the configuration.  None of the band aliasing techniques normally
             supported by OWS can work in standalone mode.)
             For bands that are used as bitmaps (i.e. either for masking with pq_mask or colour coding
             in value_map), the data_variable must have a valid flag_definition attribute.
+    :param loop_over: (optional) A string which is the name of a dimension in the data to loop over,
+            for bulk processing.  E.g. if set to "time", the output will have the same time dimension
+            coordinates as the input, with the single-date style being applied to each time slice
+            in the input data independently.
     :param valid_data_mask: (optional) An xarray DataArray mask, with dimensions and coordinates matching data.
     :return: An xarray Dataset, with the same dimensions and coordinates as data, and four data_vars of
             8 bit signed integer data named red, green, blue and alpha, representing an 24bit RGBA image.
     """
-    return style.transform_data(
-            data,
-            style.to_mask(
-                    data,
+    if loop_over is None:
+        return style.transform_data(
+                data,
+                style.to_mask(
+                        data,
+                        valid_data_mask
+                )
+        )
+    image_slices = []
+    for coord in data[loop_over].values:
+        d_slice = data.sel(**{loop_over: coord})
+        image_slices.append(
+            style.transform_data(
+                d_slice,
+                style.to_mask(
+                    d_slice,
                     valid_data_mask
+                )
             )
-    )
+        )
+    return xarray.concat(image_slices, data[loop_over])
 
 
-def apply_ows_style_cfg(cfg, data, valid_data_mask=None):
+def apply_ows_style_cfg(cfg, data, loop_over=None, valid_data_mask=None):
     """
     Apply an OWS style configuration to an ODC XArray to generate a styled image.
 
     :param cfg: A valid OWS Style definition configuration dictionary.
 
         Refer to the documentation for the valid syntax:
 
@@ -58,22 +83,27 @@
     :param data: An xarray Dataset, as generated by datacube.load_data()
             Note that the Dataset must contain all of the band names referenced by the standalone style
             configuration.  (The names of the data variables in the dataset must exactly match
             the band names in the configuration.  None of the band aliasing techniques normally
             supported by OWS can work in standalone mode.)
             For bands that are used as bitmaps (i.e. either for masking with pq_mask or colour coding
             in value_map), the data_variable must have a valid flag_definition attribute.
+    :param loop_over: (optional) A string which is the name of a dimension in the data to loop over,
+            for bulk processing.  E.g. if set to "time", the output will have the same time dimension
+            coordinates as the input, with the single-date style being applied to each time slice
+            in the input data independently.
     :param valid_data_mask: (optional) An xarray DataArray mask, with dimensions and coordinates matching data.
     :return: An xarray Dataset, with the same dimensions and coordinates as data, and four data_vars of
             8 bit signed integer data named red, green, blue and alpha, representing an 24bit RGBA image.
     """
     return apply_ows_style(
         StandaloneStyle(cfg),
         data,
-        valid_data_mask
+        loop_over=loop_over,
+        valid_data_mask=valid_data_mask
     )
 
 
 def generate_ows_legend_style(style, ndates=0):
     """
 
     :param style: An OWS Style object, as created by StandaloneStyle()
```

### Comparing `datacube_ows-1.8.8/datacube_ows/styles/base.py` & `datacube_ows-1.8.9/datacube_ows/styles/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,33 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 import io
 import logging
 
 import numpy as np
 import xarray as xr
 from datacube.utils.masking import make_mask
 from PIL import Image
 
 from datacube_ows.config_utils import (FlagProductBands, OWSConfigEntry,
                                        OWSEntryNotFound,
                                        OWSExtensibleConfigEntry,
-                                       OWSFlagBandStandalone)
+                                       OWSFlagBandStandalone,
+                                       OWSMetadataConfig)
 from datacube_ows.legend_utils import get_image_from_url
 from datacube_ows.ogc_exceptions import WMSException
 from datacube_ows.ogc_utils import ConfigException, FunctionWrapper
 
 _LOG = logging.getLogger(__name__)
 
 
-class StyleDefBase(OWSExtensibleConfigEntry):
+class StyleDefBase(OWSExtensibleConfigEntry, OWSMetadataConfig):
     INDEX_KEYS = ["layer", "style"]
     auto_legend = False
     include_in_feature_info = False
 
     def __new__(cls, product=None, style_cfg=None, stand_alone=False, defer_multi_date=False, user_defined=False):
         if product and style_cfg:
             style_cfg = cls.expand_inherit(style_cfg, global_cfg=product.global_cfg,
@@ -33,14 +39,17 @@
                                keyval_defaults={"layer": product.name})
             subclass = cls.determine_subclass(style_cfg)
             if not subclass:
                 raise ConfigException(f"Invalid style in layer {product.name} - could not determine style type")
             return super().__new__(subclass)
         return super().__new__(cls)
 
+    default_title = "Stand-Alone Style"
+    default_abstract = "Stand-Alone Style"
+
     def __init__(self, product, style_cfg, stand_alone=False, defer_multi_date=False, user_defined=False):
         super().__init__(style_cfg,
                          global_cfg=product.global_cfg,
                          keyvals={
                                 "layer": product.name,
                                 "style": style_cfg.get("name", "stand_alone")
                          },
@@ -50,25 +59,24 @@
                              }
                          },
                          keyval_defaults={
                              "layer": product.name
                          })
         style_cfg = self._raw_cfg
         self.stand_alone = stand_alone
+        if self.stand_alone:
+            self._metadata_registry = {}
         self.user_defined = user_defined
         self.local_band_map = style_cfg.get("band_map", {})
         self.product = product
         if self.stand_alone:
             self.name = style_cfg.get("name", "stand_alone")
-            self.title = style_cfg.get("title", "Stand Alone Style")
-            self.abstract = style_cfg.get("abstract", "Stand Alone Style")
         else:
             self.name = style_cfg["name"]
-            self.title = style_cfg["title"]
-            self.abstract = style_cfg["abstract"]
+        self.parse_metadata(style_cfg)
         self.masks = [StyleMask(mask_cfg, self) for mask_cfg in style_cfg.get("pq_masks", [])]
         if self.stand_alone:
             self.flag_products = []
         else:
             self.flag_products = FlagProductBands.build_list_from_masks(self.masks)
 
         self.raw_needed_bands = set()
@@ -76,14 +84,20 @@
         self.declare_unready("needed_bands")
         self.declare_unready("flag_bands")
 
         self.parse_legend_cfg(style_cfg.get("legend", {}))
         if not defer_multi_date:
             self.parse_multi_date(style_cfg)
 
+    def global_config(self):
+        return self.product.global_cfg
+
+    def get_obj_label(self):
+        return f"style.{self.product.name}.{self.name}"
+
     # pylint: disable=attribute-defined-outside-init
     def make_ready(self, dc, *args, **kwargs):
         self.needed_bands = set()
         self.pq_product_bands = []
         self.flag_bands = set()
         for band in self.raw_needed_bands:
             self.needed_bands.add(self.local_band(band))
@@ -136,15 +150,18 @@
             if mask.flags:
                 odc_mask = make_mask(pq_data, **mask.flags)
             else:
                 odc_mask = pq_data == mask.enum
             odc_mask = odc_mask.squeeze(dim="time", drop=True)
             return odc_mask
 
-        date_count = len(data.coords["time"])
+        if not data.coords["time"].shape:
+            date_count = 1
+        else:
+            date_count = len(data.coords["time"])
         if date_count > 1:
             # TODO multidate
             mdh = self.get_multi_date_handler(date_count)
             if extra_mask is not None:
                 extra_mask = mdh.collapse_mask(extra_mask)
             mask_maker = mdh.make_mask
         else:
@@ -177,17 +194,22 @@
         else:
             alpha = img_data.alpha
         alpha = alpha.where(mask, other=0)
         img_data = img_data.assign({"alpha": alpha})
         return img_data
 
     def transform_data(self, data, mask):
-        date_count = len(data.coords["time"])
+        if not data.time.shape:
+            date_count = 1
+        else:
+            date_count = len(data.coords["time"])
+            if date_count == 1:
+                data = data.squeeze(dim="time", drop=True)
         if date_count == 1:
-            img_data = self.transform_single_date_data(data.squeeze(dim="time", drop=True))
+            img_data = self.transform_single_date_data(data)
         else:
             mdh = self.get_multi_date_handler(date_count)
             img_data = mdh.transform_data(data)
         img_data = self.apply_mask_to_image(img_data, mask)
         return img_data
 
     def transform_single_date_data(self, data):
@@ -402,11 +424,15 @@
 
 
 class BandIdxProxy:
     def band(self, band):
         return band
 
 
+class GlobalCfgProxy:
+    internationalised = False
+
+
 class StandaloneProductProxy:
     name = "standalone"
-    global_cfg = None
+    global_cfg = GlobalCfgProxy()
     band_idx = BandIdxProxy()
```

### Comparing `datacube_ows-1.8.8/datacube_ows/styles/colormap.py` & `datacube_ows-1.8.9/datacube_ows/styles/colormap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 import logging
 from datetime import datetime
 
 import numpy
 from colour import Color
 from datacube.utils.masking import make_mask
 from matplotlib import patches as mpatches
```

### Comparing `datacube_ows-1.8.8/datacube_ows/styles/component.py` & `datacube_ows-1.8.9/datacube_ows/styles/component.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 import numpy as np
 from xarray import DataArray, Dataset
 
 from datacube_ows.ogc_utils import ConfigException, FunctionWrapper
 from datacube_ows.styles.base import StyleDefBase
 
 # pylint: disable=abstract-method
```

### Comparing `datacube_ows-1.8.8/datacube_ows/styles/expr.py` & `datacube_ows-1.8.9/datacube_ows/styles/expr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 import lark
 
 
 def formula_parser():
     return lark.Lark("""
                 ?expr: num_expr | bool_expr
```

### Comparing `datacube_ows-1.8.8/datacube_ows/styles/expression.py` & `datacube_ows-1.8.9/datacube_ows/styles/expression.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 import lark
 
 from datacube_ows.ogc_utils import ConfigException
 from datacube_ows.styles.expr import formula_parser
 
 identity = lambda ev, x: x
```

### Comparing `datacube_ows-1.8.8/datacube_ows/styles/hybrid.py` & `datacube_ows-1.8.9/datacube_ows/styles/hybrid.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from xarray import Dataset
 
 from datacube_ows.styles.base import StyleDefBase
 from datacube_ows.styles.component import ComponentStyleDef
 from datacube_ows.styles.ramp import ColorRampDef
```

### Comparing `datacube_ows-1.8.8/datacube_ows/styles/ramp.py` & `datacube_ows-1.8.9/datacube_ows/styles/ramp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 import logging
 from collections import defaultdict
 from decimal import ROUND_HALF_UP, Decimal
 from math import isclose
 
 import matplotlib
 import numpy
```

### Comparing `datacube_ows-1.8.8/datacube_ows/templates/index.html` & `datacube_ows-1.8.9/datacube_ows/templates/index.html`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/datacube_ows/templates/ogc_error.xml` & `datacube_ows-1.8.9/datacube_ows/templates/ogc_error.xml`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/datacube_ows/templates/test_client.html` & `datacube_ows-1.8.9/datacube_ows/templates/test_client.html`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/datacube_ows/templates/wcs_capabilities.xml` & `datacube_ows-1.8.9/datacube_ows/templates/wcs_capabilities.xml`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/datacube_ows/templates/wcs_desc_coverage.xml` & `datacube_ows-1.8.9/datacube_ows/templates/wcs_desc_coverage.xml`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/datacube_ows/templates/wms_capabilities.xml` & `datacube_ows-1.8.9/datacube_ows/templates/wms_capabilities.xml`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/datacube_ows/templates/wmts_capabilities.xml` & `datacube_ows-1.8.9/datacube_ows/templates/wmts_capabilities.xml`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/datacube_ows/tile_matrix_sets.py` & `datacube_ows-1.8.9/datacube_ows/tile_matrix_sets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from datacube_ows.config_utils import OWSConfigEntry
 from datacube_ows.ogc_utils import ConfigException
 
 # Scale denominators for WebMercator QuadTree Scale Set, starting from zoom level 0.
 # Currently goes to zoom level 14, where the pixel size at the equator is ~10m (i.e. Sentinel2 resolution)
 # Taken from the WMTS 1.0.0 spec, Annex E.4
 # Don't even think about changing these numbers unless you really, really know what you are doing.
```

### Comparing `datacube_ows-1.8.8/datacube_ows/update_ranges.py` & `datacube_ows-1.8.9/datacube_ows/update_ranges.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/usr/bin/env python3
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 
 import os
 import re
 
 import click
 import pkg_resources
 import psycopg2
```

### Comparing `datacube_ows-1.8.8/datacube_ows/utils.py` & `datacube_ows-1.8.9/datacube_ows/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import, division, print_function
 
 import logging
 from functools import wraps
 from time import monotonic
```

### Comparing `datacube_ows-1.8.8/datacube_ows/wcs1.py` & `datacube_ows-1.8.9/datacube_ows/wcs1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import, division, print_function
 
 from flask import render_template
 
 from datacube_ows.ogc_exceptions import WCS1Exception
 from datacube_ows.ogc_utils import get_service_base_url
 from datacube_ows.ows_configuration import get_config
```

### Comparing `datacube_ows-1.8.8/datacube_ows/wcs1_utils.py` & `datacube_ows-1.8.9/datacube_ows/wcs1_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import, division, print_function
 
 import numpy
 import xarray
 from affine import Affine
 from datacube.utils import geometry
 from dateutil.parser import parse
```

### Comparing `datacube_ows-1.8.8/datacube_ows/wcs2.py` & `datacube_ows-1.8.9/datacube_ows/wcs2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import, division, print_function
 
 from flask import request
 from ows.common import WGS84BoundingBox
 from ows.common.v20.decoders import kvp_decode_get_capabilities
 from ows.gml import Grid, IrregularAxis, RegularAxis, SpatioTemporalType
 from ows.swe import Field
@@ -78,25 +83,25 @@
         title=cfg.title,
         abstract=cfg.abstract,
         keywords=cfg.keywords,
         fees=cfg.fees,
         access_constraints=[cfg.access_constraints],
         provider_name='',
         provider_site='',
-        individual_name=cfg.contact_info['person'],
-        organisation_name=cfg.contact_info['organisation'],
-        position_name=cfg.contact_info['position'],
-        phone_voice=cfg.contact_info['telephone'],
-        phone_facsimile=cfg.contact_info['fax'],
-        delivery_point=cfg.contact_info['address']['address'],
-        city=cfg.contact_info['address']['city'],
-        administrative_area=cfg.contact_info['address']['state'],
-        postal_code=cfg.contact_info['address']['postcode'],
-        country=cfg.contact_info['address']['country'],
-        electronic_mail_address=cfg.contact_info['email'],
+        individual_name=cfg.contact_info.person,
+        organisation_name=cfg.contact_info.organisation,
+        position_name=cfg.contact_info.position,
+        phone_voice=cfg.contact_info.telephone,
+        phone_facsimile=cfg.contact_info.fax,
+        delivery_point=cfg.contact_info.address.address,
+        city=cfg.contact_info.address.city,
+        administrative_area=cfg.contact_info.address.state,
+        postal_code=cfg.contact_info.address.postcode,
+        country=cfg.contact_info.address.country,
+        electronic_mail_address=cfg.contact_info.email,
         online_resource=base_url,
         # hours_of_service=,
         # contact_instructions=,
         # role=,
         coverage_summaries=[
             CoverageSummary(
                 identifier=product.name,
```

### Comparing `datacube_ows-1.8.8/datacube_ows/wcs2_utils.py` & `datacube_ows-1.8.9/datacube_ows/wcs2_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import, division, print_function
 
 import collections
 import logging
 
 import datacube
 from datacube.utils import geometry
```

### Comparing `datacube_ows-1.8.8/datacube_ows/wcs_scaler.py` & `datacube_ows-1.8.9/datacube_ows/wcs_scaler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from affine import Affine
 from datacube.utils import geometry
 
 
 class WCSScalerException(Exception):
     pass
```

### Comparing `datacube_ows-1.8.8/datacube_ows/wms.py` & `datacube_ows-1.8.9/datacube_ows/wms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import, division, print_function
 
 from flask import render_template
 
 from datacube_ows.data import feature_info, get_map
 from datacube_ows.legend_generator import legend_graphic
 from datacube_ows.ogc_exceptions import WMSException
```

### Comparing `datacube_ows-1.8.8/datacube_ows/wms_utils.py` & `datacube_ows-1.8.9/datacube_ows/wms_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import, division, print_function
 
 from datacube_ows.styles import StyleDef
 from datacube_ows.styles.expression import ExpressionException
 
 try:
     import regex as re
```

### Comparing `datacube_ows-1.8.8/datacube_ows/wmts.py` & `datacube_ows-1.8.9/datacube_ows/wmts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 from __future__ import absolute_import, division, print_function
 
 import logging
 
 from flask import render_template
 
 from datacube_ows.data import feature_info, get_map
```

### Comparing `datacube_ows-1.8.8/datacube_ows.egg-info/SOURCES.txt` & `datacube_ows-1.8.9/datacube_ows.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -11,34 +11,38 @@
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 cfg_parser.py
 check-code-all.sh
 check-code.sh
+code-of-conduct.md
+constraints.txt
 create_tables.sql
 docker-compose.db.yaml
 docker-compose.prod.yaml
 docker-compose.pyspy.yaml
 docker-compose.yaml
+license-headers.md
+license-template.txt
 lint-code.sh
 ows_cfg_report.json
-ows_test_cfg.py
 pylintrc
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 test_urls.sh
 update_ranges.py
 .github/.codecov.yml
 .github/ISSUE_TEMPLATE/code-change-failed-tests-report.md
 .github/ISSUE_TEMPLATE/standard-issue-template.md
 .github/workflows/docker.yml
+.github/workflows/dockerfile-lint.yml
 .github/workflows/lint.yml
 .github/workflows/pypi.yml
 .github/workflows/scan.yml
 .github/workflows/test.yml
 datacube_ows/__init__.py
 datacube_ows/_version.py
 datacube_ows/band_utils.py
@@ -108,15 +112,14 @@
 datacube_ows/sql/extent_views/refresh/004_refresh_spacetime.sql
 datacube_ows/sql/wms_schema/create/001_create_schema.sql
 datacube_ows/sql/wms_schema/create/002_create_product_rng.sql
 datacube_ows/sql/wms_schema/create/003_create_subproduct_rng.sql
 datacube_ows/sql/wms_schema/create/004_create_multiproduct_rng.sql
 datacube_ows/sql/wms_schema/create/005_grant_requires_role.sql
 datacube_ows/styles/__init__.py
-datacube_ows/styles/api.py
 datacube_ows/styles/base.py
 datacube_ows/styles/colormap.py
 datacube_ows/styles/component.py
 datacube_ows/styles/expr.py
 datacube_ows/styles/expression.py
 datacube_ows/styles/hybrid.py
 datacube_ows/styles/ramp.py
@@ -161,70 +164,14 @@
 docs/style_howto_color_map.rst
 docs/style_howto_color_ramp.rst
 docs/style_howto_components.rst
 docs/style_howto_components_nonlinear.rst
 docs/style_howto_legends.rst
 docs/style_howto_transparency.rst
 docs/styling_howto.rst
+docs/styling_howto_jupyter.rst
 docs/usage.rst
-integration_tests/__init__.py
-integration_tests/conftest.py
-integration_tests/test_cfg_parser.py
-integration_tests/test_layers.py
-integration_tests/test_mv_index.py
-integration_tests/test_routes.py
-integration_tests/test_update_ranges.py
-integration_tests/test_wcs_server.py
-integration_tests/test_wms_server.py
-integration_tests/test_wmts_server.py
-integration_tests/utils.py
-tests/__init__.py
-tests/conftest.py
-tests/test_band_utils.py
-tests/test_cfg_bandidx.py
-tests/test_cfg_cache_ctrl.py
-tests/test_cfg_global.py
-tests/test_cfg_inclusion.py
-tests/test_cfg_layer.py
-tests/test_cfg_metadata_types.py
-tests/test_cfg_tile_matrix_set.py
-tests/test_cfg_wcs.py
-tests/test_config_toolkit.py
-tests/test_data.py
-tests/test_legend_generator.py
-tests/test_mpl_cmaps.py
-tests/test_multidate_handler.py
-tests/test_mv_selopts.py
-tests/test_no_db_routes.py
-tests/test_ogc_utils.py
-tests/test_ows_configuration.py
-tests/test_pyproj.py
-tests/test_qprof.py
-tests/test_startup.py
-tests/test_style_api.py
-tests/test_styles.py
-tests/test_time_res_method.py
-tests/test_wcs2_utils.py
-tests/test_wcs_scaler.py
-tests/test_wms_utils.py
-tests/utils.py
-tests/cfg/README.txt
-tests/cfg/__init__.py
-tests/cfg/infinite_1.json
-tests/cfg/infinite_2.json
-tests/cfg/infinite_2a.json
-tests/cfg/infinite_2b.json
-tests/cfg/minimal_cfg.py
-tests/cfg/mixed_nested.json
-tests/cfg/mixed_nested.py
-tests/cfg/nested.py
-tests/cfg/nested_1.json
-tests/cfg/nested_2.json
-tests/cfg/nested_3.json
-tests/cfg/nested_4.json
-tests/cfg/simple.json
-tests/cfg/simple.py
 wms_xsds/capabilities_1_3_0.xsd
 wms_xsds/capabilities_extensions.xsd
 wms_xsds/capabilities_extensions_local.xsd
 wms_xsds/exceptions_1_3_0.xsd
 wms_xsds/wmtsGetCapabilities_response.xsd
```

### Comparing `datacube_ows-1.8.8/docker/database/dump.sql` & `datacube_ows-1.8.9/docker/database/dump.sql`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docker-compose.yaml` & `datacube_ows-1.8.9/docker-compose.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,16 @@
       DB_PORT: ${DB_PORT}
       DB_USERNAME: ${DB_USERNAME}
       DB_PASSWORD: ${DB_PASSWORD}
       DB_DATABASE: ${DB_DATABASE}
       # Where the config file is (must match the volume mount)
       WMS_CONFIG_PATH: /env/config/ows_cfg.py
       # Path from the PYTHONPATH to the config object (default PYTHONPATH is /env)
-      DATACUBE_OWS_CFG: config.ows_cfg.ows_cfg
+      PYTHONPATH: ${PYTHONPATH}
+      DATACUBE_OWS_CFG: ${DATACUBE_OWS_CFG}
       AWS_DEFAULT_REGION: ${AWS_REGION}
       # Talk to AWS without using credentials
       AWS_NO_SIGN_REQUEST: "${AWS_NO_SIGN_REQUEST}"
       # Enable Metrics
       prometheus_multiproc_dir: ${prometheus_multiproc_dir}
       # Dev flags
       FLASK_APP: /code/datacube_ows/ogc.py
```

### Comparing `datacube_ows-1.8.8/docs/Makefile` & `datacube_ows-1.8.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/cfg_colourmap_styles.rst` & `datacube_ows-1.8.9/docs/cfg_colourmap_styles.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/cfg_colourramp_styles.rst` & `datacube_ows-1.8.9/docs/cfg_colourramp_styles.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/cfg_component_styles.rst` & `datacube_ows-1.8.9/docs/cfg_component_styles.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/cfg_functions.rst` & `datacube_ows-1.8.9/docs/cfg_functions.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/cfg_hybrid_styles.rst` & `datacube_ows-1.8.9/docs/cfg_hybrid_styles.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/cfg_layers.rst` & `datacube_ows-1.8.9/docs/cfg_layers.rst`

 * *Files 3% similar despite different names*

```diff
@@ -105,14 +105,22 @@
 =============
 
 In addition to the `common elements <#common-elements>`_ described
 above, folder layers have a "layers" element which is a list of child
 layers (which may be named layers, folder layers with their own
 child layers).
 
+A folder layer may also have a `label` element which is used only
+for
+`metadata separation and internationalisation
+<https://datacube-ows.readthedocs.io/en/latest/configuration.html#metadata-separation-and-internationalisation>`_.
+Each folder's layer
+must be globally unique.  A unique label based on the folder's position
+in the folder hierarchy is generated if one is not supplied.
+
 E.g.
 
 ::
 
     "layers": [
         {
             "title": "Parent Folder",
```

### Comparing `datacube_ows-1.8.8/docs/cfg_style_api.rst` & `datacube_ows-1.8.9/docs/cfg_style_api.rst`

 * *Files 17% similar despite different names*

```diff
@@ -131,14 +131,49 @@
     with open("filename.png", "wb") as fp:
         fp.write(xarray_image_as_png(image)
 
 For more detailed examples,
 refer to the
 `styling how-to guide <https://datacube-ows.readthedocs.io/en/latest/styling_howto.html>`_.
 
+Bulk Processing
+---------------
+
+Bulk processing over a non-spatial dimension of the input data (usually time) is supported via the
+optional ``loop_over`` parameter to ``apply_ows_style``, ``apply_ows_style_cfg``, and
+``xarray_image_as_png``:
+
+::
+
+    from datacube import Datacube
+    from datacube_ows.styles.api import StandaloneStyle
+    from datacube_ows.styles.api import apply_ows_style, apply_ows_style_cfg
+    from datacube_ows.styles.api import xarray_image_as_png
+
+    cfg = {
+        # Some style config ...
+    }
+    style = StandaloneStyle(cfg)
+
+    # This ODC query returns data for multiple dates.
+    dc = Datacube()
+    data = dc.load( ...query parameters... )
+
+    # images is an xarray.Dataset with same time dimension coordinates as the input data.
+    # Each time slice is styled independently.
+    images = apply_ows_style(style, data, loop_over="time")
+
+    # This code will write out the images to the local filesystem as `filename00.png`, `filename01.png`, etc.
+
+    pngs = xarray_image_as_png(images, loop_over="time")
+    for i, png in enumerate(pngs):
+        with open(f"filename{i:02}.png", "wb") as fp:
+            fp.write(xarray_image_as_png(image)
+
+
 Auto-generating a legend image
 ------------------------------
 
 To generate a legend image from a ``StandaloneStyle`` object or a style config, use the
 ``generate_ows_legend_style_cfg`` or ``generate_ows_legend_style`` functions.  Both take an
 optional dates parameter, which can be either an integer or an iterable of date values (in any
 representation, only the length is used).
@@ -169,7 +204,8 @@
     image = generate_ows_legend_style(cfg, 2)
     # or
     image = generate_ows_legend_style_cfg(style, ["yesterday", "today"])
 
     # Write out as PNG:
     with open("filename.png", "wb") as fp:
         image.save(fp)
+
```

### Comparing `datacube_ows-1.8.8/docs/cfg_styling.rst` & `datacube_ows-1.8.9/docs/cfg_styling.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/cfg_wcs.rst` & `datacube_ows-1.8.9/docs/cfg_wcs.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/cfg_wmts.rst` & `datacube_ows-1.8.9/docs/cfg_wmts.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/conf.py` & `datacube_ows-1.8.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/configuration.rst` & `datacube_ows-1.8.9/docs/configuration.rst`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 =================
 
 .. toctree::
    :maxdepth: 2
    :hidden:
    :glob:
 
+   configuration
    cfg_global
    cfg_wms
    cfg_wmts
    cfg_wcs
    cfg_functions
    cfg_layers
    cfg_styling
@@ -31,16 +32,16 @@
 The behaviour of a datacube_ows server instance can be controlled, customised and extended by configuration files.
 
 Datacube OWS configuration files can be written in Python (as a static serialisable python dictionary) or as JSON.
 All examples in this documentation will always be presented in Python syntax.  JSON syntax is almost identical, but
 note that there are some important differences:
 
 1. JSON string literals must always be delimited with double quotes - so no Python-style single quote strings!
-2. JSON boolean literals are all lowercase (`true`, `false`) and Python boolean literals are title case (e.g.
-   `True`, `False`)
+2. JSON boolean literals are all lowercase (``true``, ``false``) and Python boolean literals are title case (e.g.
+   ``True``, ``False``)
 3. JSON does not allow commas after the last element of lists and objects (dictionaries in Python terms).
 4. JSON does not support comments of any kind.
 
 `This general introductory stuff is boring.  Take me straight to the description of the
 configuration file. <#general-config-structure>`_
 
 .. _location:
@@ -50,14 +51,18 @@
 
 Configuration is read by default from the ``ows_cfg object`` in ``datacube_ows/ows_cfg.py``
 but this can be overridden by setting the ``$DATACUBE_OWS_CFG`` environment variable.
 
 Configuration can be read from a python file, a json file, or a collection of python
 and/or json files.
 
+A json file can optionally also be fetched from AWS S3 if access to S3 is configured correctly for datacube_ows
+and the environment variable ``$DATACUBE_OWS_CFG_ALLOW_S3`` is set to ``YES``. Please note that this is not
+possible for configurations as python file.
+
 .. _DATACUBE_OWS_CFG:
 
 The DATACUBE_OWS_CFG Environment Variable
 =========================================
 
 The environment variable ``$DATACUBE_OWS_CFG`` is interpreted as follows (first matching
 alternative applies):
@@ -74,26 +79,33 @@
 
    Config loaded directly from the environment variable as **json** (not recommended)
 
 4. Ends in ".json", e.g. ``cfg_prod.json``
 
    Config loaded from **json** file in working directory.
 
-5. Contains a dot (.), e.g. ``package.sub_package.module.cfg_object_name``
+5. Has a valid ``s3://`` URL and a ``.json`` extension
+
+   The configuration is fetched from AWS S3 in json format.
+
+   N.B. Configuration can only be loaded from S3 if the environment variable ``$DATACUBE_OWS_CFG_ALLOW_S3``
+   is set to ``yes``, otherwise a ``ConfigurationException`` will be raised.
+
+6. Contains a dot (.), e.g. ``package.sub_package.module.cfg_object_name``
 
    Imported as python object (expected to be a dictionary).
 
    N.B. It is up to you to ensure that the Python file in question is in your Python path and
    that all package directories have a ``__init__.py`` file, etc.
 
-6. Valid python object name, e.g. ``cfg_prod``
+7. Valid python object name, e.g. ``cfg_prod``
 
    Imported as **python** from named object in ``datacube_ows/ows_cfg.py``
 
-7. Blank or not set
+8. Blank or not set
 
    Default to import ows_cfg object in ``datacube_ows/ows_cfg.py`` as described above.
 
 .. _inclusion:
 
 Inclusion: Breaking Up Config Into Multiple Files
 -------------------------------------------------
@@ -259,15 +271,115 @@
 Note that a layer or style can only inherit by name from a parent layer or style that has already
 been parsed by the config parser - i.e. it must appear earlier in the definition of the layers section.
 This restriction can be avoided using direct inheritance.
 
 Care should be taken of the special handling of lists in configuration:
 
 1. If the child entry is an empty list, this will replace the parent entry, resulting in an empty list.
-2. If the c
+2. If the child entry is a non-empty list, the values in the child list are appended to the parent entry, resulting
+   in a merged list.
+
+Metadata Separation and Internationalisation
+--------------------------------------------
+
+Human-readable metadata can simply be embedded directly in the configuration.  However in order to support
+use-cases like multi-language internationalisation and integrating metadata with external
+content management systems, all human-readable metadata in the OWS configuration can be extracted
+into a separate file and managed independently.
+
+Metadata Separation
++++++++++++++++++++
+
+To separate your metadata from config (either as an end in itself, or as preparation for internationalisation/translation):
+
+1. Add a unique ``label`` to each of your folder layers.
+
+   This step is optional, but strongly recommended. OWS will autogenerate
+   a unique but non-obvious label for each folder if you do not supply one.
+
+2. Run ``datacube-ows-cfg extract -m messages.po``
+
+   This extracts all the translatable/human-readable text from your config file, and writes it to the
+   named file in gettext "po" file format.
+
+3. Add ``"message_file": "/path/to/messages.po"`` to the global section of your OWS config file.
+
+   Subsequently, text in messages.po will over-ride text in the config file. Update as needed, restart
+   wsgi process to take effect. Any field not included in the message file will be loaded directly
+   from the config, as previously.
+
+The msgid's in the message file are symbolic. E.g.
+
+* ``global.title``: The title for the whole service.
+* ``folder.<label>.title``: The title for a folder, identified by label.
+* ``layer.<name>.title``: The title for a named layer, identified by name.
+* ``style.<layer_name>.<style_name>.title``: The title for a style, identified by layer name and style name.
+
+The msgstr's in the message file are the text used by OWS for global/layer/style metadata, in preference
+to the values in the config file.
+
+Fields that can be included in the message file are:
+
+*    Titles (global, folder, layer, style)
+*    Abstracts (global, folder, layer, style)
+*    Keywords (global, folder, layer)
+*    Attribution titles (global, folder, layer)
+*    Fees (global only)
+*    Access Constraints (global only)
+*    Contact Info Organisation (global only)
+*    Contact Info Position (global only)
+
+Internationalisation/Translation of Metadata
+++++++++++++++++++++++++++++++++++++++++++++
+
+Once you have extracted your metadata into a single file, separate from the main body of configuration,
+as described `above <#metadata-separation>`_, generate a translation catalog for every language you want
+translations for - including the "native" language that your messages file is already in:
+
+::
+
+    # Create new translation catalogs for English (en), German (de), French (Fr) and Swahili (Sw).
+
+    datacube-ows-cfg translation -n -D my_ows_project -d /config/translations -m /config/messages.po en de fr sw
+
+This will create the following files:
+
+::
+
+   /config/translations/en/LC_MESSAGES/my_ows_project.po
+   /config/translations/de/LC_MESSAGES/my_ows_project.po
+   /config/translations/fr/LC_MESSAGES/my_ows_project.po
+   /config/translations/sw/LC_MESSAGES/my_ows_project.po
+
+
+These files are currently identical, apart from the language in the header.  These files should be distributed to
+translators for the respective languages.  The translators keep the file in the same format, but replace
+the ``msg_str`` sections with the translated text in their language and return the translated message
+file to you.  Then you keep then save them into the directory structure above, replacing the untranslated
+templates.
+
+Once the translations have been placed in translations directory, they must be compiled:
+
+::
+
+    datacube-ows-cfg compile -D my_ows_project -d /config/translations en de fr sw
+
+This creates the following machine-readable message (.mo) files:
+
+::
+
+   /config/translations/en/LC_MESSAGES/my_ows_project.mo
+   /config/translations/de/LC_MESSAGES/my_ows_project.mo
+   /config/translations/fr/LC_MESSAGES/my_ows_project.mo
+   /config/translations/sw/LC_MESSAGES/my_ows_project.mo
+
+You can now update the
+`global section of your OWS Configuration <https://datacube-ows.readthedocs.io/en/latest/cfg_global.html#metadata-separation-and-internationalisation>`_
+section and restart the web service and
+you are serving multi-lingually!  (Adjust your client's "Accept-Language" header to test.)
 
 General Config Structure
 ------------------------
 
 At the top level, the Datacube OWS configuration is a single dictionary with the following elements:
 
 ::
```

### Comparing `datacube_ows-1.8.8/docs/database.rst` & `datacube_ows-1.8.9/docs/database.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/environment_variables.rst` & `datacube_ows-1.8.9/docs/environment_variables.rst`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 .. contents:: Table of Contents
 
 Datacube_ows configuration
 --------------------------
 
 The location of the `datacube configuration object <configuration.rst>`_
 is set via the ``$DATACUBE_OWS_CFG`` environment variable as described
-`here <configuration.rst>`_.
+`here <configuration.rst>`_. To enable the retrieval of a json configuration file from AWS S3,
+the ``$DATACUBE_OWS_CFG_ALLOW_S3`` environment variable needs to be set to ``YES``.
 
 Open DataCube Database Connection
 ---------------------------------
 
 The preferred method of configuring the ODC database is with the ``$DB_*``
 environment variables:
```

### Comparing `datacube_ows-1.8.8/docs/installation.rst` & `datacube_ows-1.8.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/make.bat` & `datacube_ows-1.8.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/performance.rst` & `datacube_ows-1.8.9/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/style_howto_color_map.rst` & `datacube_ows-1.8.9/docs/style_howto_color_map.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/docs/style_howto_color_ramp.rst` & `datacube_ows-1.8.9/docs/style_howto_color_ramp.rst`

 * *Files 5% similar despite different names*

```diff
@@ -60,23 +60,24 @@
 3. Change the range to ``[0, 1.0]``
 
 The Matplotlib ``ocean`` ramp runs from dark green to dark blue, then fading to white.
 so ``ocean_r`` is the reverse - from white through darker blues to dark green.
 So now we get white in the negative and zero areas, with positive areas
 getting darkening blues with close to 1.0 being dark green.
 
+This configuration also demonstrates another method for defining the index - with
+a simple expression language instead of referencing an explicit python function.
+The expression language includes band names and literal numbers, as well as simple
+arthimetic operators like `+ - / *` and parentheses for precedence.
+
 ::
 
     ndvi_unidirection_cfg = {
-        "index_function": {
-            "function": "datacube_ows.band_utils.norm_diff",
-            "mapped_bands": True,
-            "kwargs": {"band1": "nir", "band2": "red"},
-        },
-        "mpl_ramp": "ocean_r",
+        "index_expression": "(nir-red)/(nir+red)",
+        "mpl_ramp": "ocean_r",    #  ocean_r is the "ocean" ramp, reversed.
         "range": [0.0, 1.0]
     }
 
 .. image:: https://user-images.githubusercontent.com/4548530/112567708-6e4ec900-8e35-11eb-8c75-a6a1f35ef665.png
     :width: 600
 
 `View full size
```

### Comparing `datacube_ows-1.8.8/docs/style_howto_components.rst` & `datacube_ows-1.8.9/docs/style_howto_components.rst`

 * *Files 6% similar despite different names*

```diff
@@ -101,33 +101,44 @@
 
 .. image:: https://user-images.githubusercontent.com/4548530/112124234-3ddd1400-8c16-11eb-9d01-37b895010221.png
     :width: 1128
 
 Example: Mixing bands
 +++++++++++++++++++++
 
-What if we want to mix more than one band to make each channel? Here we average all three visible bands
+What if we want to mix more than one band to make each channel?  We can simply add more bands to the
+various colour channel dictionaries, with multiplying factors.  Normally we ensure that the multiplying
+factors for each channel sum to 1.0, so the result is a (possibly weighted) average of the input bands,
+but this is not enforced.
+
+Here we average all three visible bands
 into the red channel, put near infra-red in the green channel and average the two shortwave infrared
 bands to make the blue channel:
 
 ::
 
     all_bands_cfg = {
         "components": {
             "red": {
-             "red": 0.333,
-             "green": 0.333,
-             "blue": 0.333,
+                # Weighting factors should sum to (close to) 1.0
+                # 0.333 + 0.333 + 0.333 = 0.999 ~ 1.0
+                "red": 0.333,
+                "green": 0.333,
+                "blue": 0.333,
             },
             "green": {
-             "nir": 1.0
+                # Weighting factors should sum to (close to) 1.0
+                # So use 1.0 for a single band.
+                "nir": 1.0
             },
             "blue": {
-             "swir1": 0.5,
-             "swir2": 0.5,
+                # Weighting factors should sum to (close to) 1.0
+                # 0.5 + 0.5 = 1.0
+                "swir1": 0.5,
+                "swir2": 0.5,
             },
         },
         "scale_range": (50, 3000),
     }
 
 .. image:: https://user-images.githubusercontent.com/4548530/112124842-e8553700-8c16-11eb-9d60-a5a964d3a9ab.png
     :width: 600
```

### Comparing `datacube_ows-1.8.8/docs/style_howto_components_nonlinear.rst` & `datacube_ows-1.8.9/docs/style_howto_components_nonlinear.rst`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 the API.  This means it is up to your function to handle scaling to the (0,255) range.
 For example, given this function, containing a simple unscaled implementation of NDVI:
 
 ::
 
     def ndvi(data):
         # Returns data in range (-1, 1)
-        return (data["nir"] - data["red"]) / (data["nir"] + data["red")
+        return (data["nir"] - data["red"]) / (data["nir"] + data["red"])
 
 
 Using ``"green": ndvi,`` in the components dictionary would sort of work, but would
 return 0 for every pixel after conversion from floating point - which is probably
 not what we want. We can add scaling like this:
 
 ::
@@ -58,15 +58,15 @@
     def ndvi(data):
         # Calculate NDVI (-1.0 to 1.0)
         unscaled = (data["nir"] - data["red"])/(data["nir"] + data["red"])
 
         # Scale to [-1.0 - 1.0] to [0 - 255]
         scaled = ((unscaled + 1.0) * 255/2).clip(0, 255)
 
-        returned scaled
+        return scaled
 
     r_ndvi_b_fullrange_cfg = {
         "components": {
             "red": {"red": 1.0},
             "green": ndvi,
             "blue": {"blue": 1.0},
         },
@@ -99,15 +99,14 @@
 You can use the ``@scalable`` decorator provided by the API, and OWS's
 `extended function syntax <https://datacube-ows.readthedocs.io/en/latest/cfg_functions.html>`_
 for a more streamlined solution to scaling:
 
 Example: red-ndvi-blue (half scale)
 +++++++++++++++++++++++++++++++++++
 
-
 ::
 
     from datacube_ows.styles.api import scalable
 
     @scalable
     def scaled_ndvi(data):
         # Calculate NDVI (-1.0 to 1.0)
@@ -168,15 +167,15 @@
                     "band1": "nir",
                     "band2": "red",
                     "scale_from": (0.0, 1.0),
                     "scale_to": (0, 255)
                 }
             },
             "blue": {
-                "function": "datacube_ows.band_utils._diff",
+                "function": "datacube_ows.band_utils.norm_diff",
                 "kwargs": {
                     "band1": "green",
                     "band2": "nir",
                     "scale_from": (0.0, 1.0),
                     "scale_to": (0, 255)
                 }
             },
```

### Comparing `datacube_ows-1.8.8/docs/style_howto_transparency.rst` & `datacube_ows-1.8.9/docs/style_howto_transparency.rst`

 * *Files 2% similar despite different names*

```diff
@@ -69,17 +69,17 @@
         resolution=(-120,120),
         group_by="solar_day"
     )
 
     # Time coordinates come back slightly differently from the two products, so we need
     # to align them before we combine.
 
-    discrete_data.coords["time"] = parallel_data.coords["time"]
+    wofs_data.coords["time"] = fc_data.coords["time"]
     combined_data = xr.combine_by_coords(
-            [parallel_data, discrete_data],
+            [fc_data, wofs_data],
             join="exact")
 
 Example: No Masking
 &&&&&&&&&&&&&&&&&&&
 
 The main fractional cover view is component based view with "bare soil (bs)" band mapped to
 red, the "photosynthetic vegetation (pv)" band mapped to green and the "non-photosynthetic
@@ -87,17 +87,17 @@
 
 ::
 
     unmasked_fc_cfg =  {
         "components": {
             "red": {"bs": 1.0},
             "green": {"pv": 1.0},
-            "blue": {"npv": 1.0}},
+            "blue": {"npv": 1.0}
+        },
         "scale_range": [0.0, 100.0],
-        }
     }
 
 .. image:: https://user-images.githubusercontent.com/4548530/113671209-66c2d600-96f9-11eb-8354-43a64ec1d134.png
     :width: 600
 
 `View full size
 <https://user-images.githubusercontent.com/4548530/113671209-66c2d600-96f9-11eb-8354-43a64ec1d134.png>`_
@@ -113,17 +113,17 @@
 
 ::
 
     masked_fc_cfg =  {
         "components": {
             "red": {"bs": 1.0},
             "green": {"pv": 1.0},
-            "blue": {"npv": 1.0}},
-        "scale_range": [0.0, 100.0],
+            "blue": {"npv": 1.0}
         },
+        "scale_range": [0.0, 100.0],
         "pq_masks": [
             # Pixels must match all flags to remain visible.
             {
                 "band": "water",
                 "flags": {
                     "nodata": False,
                     "noncontiguous": False,
@@ -299,14 +299,15 @@
                     "scale_from": (0.0, 0.5),
                     "scale_to": (0, 255)
                 }
             },
         },
         "scale_range": (50, 3000),
     }
+
 .. image:: https://user-images.githubusercontent.com/4548530/113795937-5d854800-9791-11eb-9a49-25ea8cbced64.png
     :width: 600
 
 `View full size
 <https://user-images.githubusercontent.com/4548530/113795937-5d854800-9791-11eb-9a49-25ea8cbced64.png>`_
 
 `In the next chapter
```

### Comparing `datacube_ows-1.8.8/docs/styling_howto.rst` & `datacube_ows-1.8.9/docs/styling_howto.rst`

 * *Files 19% similar despite different names*

```diff
@@ -28,14 +28,19 @@
    generate test images from raw ODC data.
 2. demonstrate how to configure OWS styles with real-world examples.
 
 For thorough technical description of the configuration format,
 `see the configuration documentation
 <https://datacube-ows.readthedocs.io/en/latest/configuration.html>`_.
 
+Setting up an ODC environment and installing datacube-ows is also beyond the scope
+of this HOWTO, but if you are using a JupyterHubs based system like DEA Sandbox,
+a `Quick Start Guide <https://datacube-ows.readthedocs.io/en/latest/styling_howto_jupyter.html>`_
+is available.
+
 Introduction - Testing styles
 -----------------------------
 
 We'll start with a quick but complete walk through the process of creating an
 image with the API.
 
 First of all, you'll need some data.  Select a bounding box (in lat/long), a date,
```

### Comparing `datacube_ows-1.8.8/docs/usage.rst` & `datacube_ows-1.8.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/ows_cfg_report.json` & `datacube_ows-1.8.9/ows_cfg_report.json`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/pylintrc` & `datacube_ows-1.8.9/pylintrc`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/requirements.txt` & `datacube_ows-1.8.9/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 --extra-index-url="https://packages.dea.ga.gov.au"
-datacube[performance,s3]
+datacube[performance,s3]>=1.8.4.dev97
 pytest
 pytest-cov
 pylint==2.4.4
 flask
+flask-cors
 colour
 pandas==1.0.5
 scikit-image
-gevent==1.4.0
+gevent
 python-slugify
 geoalchemy2
-eventlet
 gunicorn
 gunicorn[gevent]
-gunicorn[eventlet]
 boto3
+moto
 rasterio>=1.0.9
 ruamel.yaml
 prometheus-client
 flask-log-request-id
 pytest-localserver
 pytest-mock
 requests
 watchdog
 timezonefinderL
 python-slugify
 bottleneck
+Babel
+Flask-Babel
 sentry-sdk
 blinker
 pyows
 lark-parser
 owslib==0.21.0
 pytest-helpers-namespace
 prometheus-flask-exporter
 setuptools_scm
 deepdiff
+s3fs
+fsspec
+regex
```

### Comparing `datacube_ows-1.8.8/setup.py` & `datacube_ows-1.8.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+# This file is part of datacube-ows, part of the Open Data Cube project.
+# See https://opendatacube.org for more information.
+#
+# Copyright (c) 2017-2021 OWS Contributors
+# SPDX-License-Identifier: Apache-2.0
 
 from setuptools import find_packages, setup
 
 requirements = [
     'datacube',
     'Flask',
     'flask_log_request_id',
     'requests',
     'affine',
     'click',
     'colour',
+    'fsspec',
     'lxml',
     'matplotlib',
     'numpy',
     'Pillow',
+    'Babel',
+    'Flask-Babel',
     'prometheus_client',
     'psycopg2',
     'python_dateutil',
     'pytz',
     'rasterio',
     'regex',
+    's3fs',
     'scikit-image',
     'timezonefinderL',
     'python-slugify',
     'geoalchemy',
     'lark-parser',
     'xarray',
     'pyows',
     'prometheus-flask-exporter',
     #
     'setuptools_scm'
 ]
 
 test_requirements = [
     # TODO: put package test requirements here
-    'pytest', 'pytest-cov', 'pytest_localserver', 'owslib', 'mock', 'pep8', 'pylint==1.6.4', 'pytest-helpers-namespace'
+    'pytest', 'pytest-cov', 'pytest_localserver', 'owslib', 'mock', 'pep8', 'pylint==1.6.4', 'pytest-helpers-namespace', 'moto'
 ]
 
 setup(
     name='datacube_ows',
     description="Open Data Cube Open Web Services",
     long_description="""
 ============
@@ -53,27 +62,27 @@
 
 Features
 --------
 
 * Leverages the power of the Open Data Cube, including support for COGs on S3.
 * Supports WMS and WMTS.
 * Experimental support for WCS (1.0, 2.0, 2.1).
-    
+
     """,
     author="Open Data Cube",
     author_email='earth.observation@ga.gov.au',
     url='https://github.com/opendatacube/datacube-ows',
     entry_points={
         'console_scripts': [
             'datacube-ows=datacube_ows.wsgi:main',
             'datacube-ows-update=datacube_ows.update_ranges:main',
-            'datacube-ows-cfg-parse=datacube_ows.cfg_parser:main'
+            'datacube-ows-cfg=datacube_ows.cfg_parser:main'
         ]
     },
-    packages=find_packages(),
+    packages=find_packages(exclude=["tests", "tests.cfg", "integration_tests", "integration_tests.cfg"]),
     include_package_data=True,
     install_requires=requirements,
     license="Apache Software License 2.0",
     zip_safe=False,
     keywords='datacube, wms, wcs',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
```

### Comparing `datacube_ows-1.8.8/wms_xsds/capabilities_1_3_0.xsd` & `datacube_ows-1.8.9/wms_xsds/capabilities_1_3_0.xsd`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/wms_xsds/capabilities_extensions.xsd` & `datacube_ows-1.8.9/wms_xsds/capabilities_extensions.xsd`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/wms_xsds/capabilities_extensions_local.xsd` & `datacube_ows-1.8.9/wms_xsds/capabilities_extensions_local.xsd`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/wms_xsds/exceptions_1_3_0.xsd` & `datacube_ows-1.8.9/wms_xsds/exceptions_1_3_0.xsd`

 * *Files identical despite different names*

### Comparing `datacube_ows-1.8.8/wms_xsds/wmtsGetCapabilities_response.xsd` & `datacube_ows-1.8.9/wms_xsds/wmtsGetCapabilities_response.xsd`

 * *Files identical despite different names*

