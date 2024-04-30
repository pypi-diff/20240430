# Comparing `tmp/xplordb-0.13.3.tar.gz` & `tmp/xplordb-0.13.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplordb-0.13.3.tar", last modified: Wed Apr 17 07:28:10 2024, max compression
+gzip compressed data, was "xplordb-0.13.4.tar", last modified: Tue Apr 30 12:24:19 2024, max compression
```

## Comparing `xplordb-0.13.3.tar` & `xplordb-0.13.4.tar`

### file list

```diff
@@ -1,293 +1,296 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.490671 xplordb-0.13.3/
--rw-rw-rw-   0 root         (0) root         (0)    34459 2024-04-17 07:28:00.000000 xplordb-0.13.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-17 07:28:00.000000 xplordb-0.13.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5407 2024-04-17 07:28:10.490671 xplordb-0.13.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4695 2024-04-17 07:28:00.000000 xplordb-0.13.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7339 2024-04-17 07:28:00.000000 xplordb-0.13.3/README.txt
--rw-rw-rw-   0 root         (0) root         (0)     1110 2024-04-17 07:28:10.490671 xplordb-0.13.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1736 2024-04-17 07:28:00.000000 xplordb-0.13.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.434672 xplordb-0.13.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 07:28:00.000000 xplordb-0.13.3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5383 2024-04-17 07:28:00.000000 xplordb-0.13.3/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1495 2024-04-17 07:28:00.000000 xplordb-0.13.3/tests/test_create_db.py
--rw-rw-rw-   0 root         (0) root         (0)     8675 2024-04-17 07:28:00.000000 xplordb-0.13.3/tests/test_import_data.py
--rw-rw-rw-   0 root         (0) root         (0)    15489 2024-04-17 07:28:00.000000 xplordb-0.13.3/tests/test_import_ddl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.435672 xplordb-0.13.3/xplordb/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/create_db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.437672 xplordb-0.13.3/xplordb/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/datamodel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/datamodel/collar.py
--rw-rw-rw-   0 root         (0) root         (0)     1357 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/datamodel/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2303 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/datamodel/lith.py
--rw-rw-rw-   0 root         (0) root         (0)     1881 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/datamodel/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     1358 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/datamodel/person.py
--rw-rw-rw-   0 root         (0) root         (0)     1500 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/datamodel/survey.py
--rw-rw-rw-   0 root         (0) root         (0)     8310 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/import_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5145 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/import_ddl.py
--rw-rw-rw-   0 root         (0) root         (0)     3090 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/minimal_dao.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.431672 xplordb-0.13.3/xplordb/schema/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.437672 xplordb-0.13.3/xplordb/schema/assay/
--rw-rw-rw-   0 root         (0) root         (0)     1545 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/assay.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.438672 xplordb-0.13.3/xplordb/schema/assay/functions/
--rw-rw-rw-   0 root         (0) root         (0)     7789 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/functions/flat_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     9397 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/functions/flat_ppm.sql
--rw-rw-rw-   0 root         (0) root         (0)    11681 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/functions/import.sql
--rw-rw-rw-   0 root         (0) root         (0)     1377 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/functions/structural_types.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.441672 xplordb-0.13.3/xplordb/schema/assay/populate/
--rw-rw-rw-   0 root         (0) root         (0)  1438090 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/populate/assay.sql
--rw-rw-rw-   0 root         (0) root         (0)     4458 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/populate/batch.sql
--rw-rw-rw-   0 root         (0) root         (0)   163953 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/populate/flat_method.sql
--rw-rw-rw-   0 root         (0) root         (0)   125897 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/populate/flat_ppm.sql
--rw-rw-rw-   0 root         (0) root         (0)    28371 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/populate/raw.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.442672 xplordb-0.13.3/xplordb/schema/assay/table/
--rw-rw-rw-   0 root         (0) root         (0)     8504 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/table/assay.sql
--rw-rw-rw-   0 root         (0) root         (0)     7813 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/table/batch.sql
--rw-rw-rw-   0 root         (0) root         (0)     3800 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/table/flat_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     3783 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/table/flat_ppm.sql
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/table/raw.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.442672 xplordb-0.13.3/xplordb/schema/assay/views/
--rw-rw-rw-   0 root         (0) root         (0)     3789 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/views/assay.sql
--rw-rw-rw-   0 root         (0) root         (0)     6317 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/assay/views/intercepts.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.442672 xplordb-0.13.3/xplordb/schema/dem/
--rw-rw-rw-   0 root         (0) root         (0)     1601 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dem/dem.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.443672 xplordb-0.13.3/xplordb/schema/dem/functions/
--rw-rw-rw-   0 root         (0) root         (0)     2503 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dem/functions/alos_cap_update_example.sql
--rw-rw-rw-   0 root         (0) root         (0)     1583 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dem/functions/cap_alos_example.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.443672 xplordb-0.13.3/xplordb/schema/dem/populate/
--rw-rw-rw-   0 root         (0) root         (0)   987241 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dem/populate/capricorn.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.444672 xplordb-0.13.3/xplordb/schema/dem/table/
--rw-rw-rw-   0 root         (0) root         (0)     4689 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dem/table/capricorn.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.444672 xplordb-0.13.3/xplordb/schema/dh/
--rw-rw-rw-   0 root         (0) root         (0)     1591 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/dh.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.448672 xplordb-0.13.3/xplordb/schema/dh/functions/
--rw-rw-rw-   0 root         (0) root         (0)     1533 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/check_depth_m.sql
--rw-rw-rw-   0 root         (0) root         (0)     1473 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/check_from_m.sql
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/check_to_m.sql
--rw-rw-rw-   0 root         (0) root         (0)     3576 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/dh_planned_trace.sql
--rw-rw-rw-   0 root         (0) root         (0)     4346 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/dh_trace.sql
--rw-rw-rw-   0 root         (0) root         (0)     2323 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/dog_leg.sql
--rw-rw-rw-   0 root         (0) root         (0)     1473 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/geom_update_xyz.sql
--rw-rw-rw-   0 root         (0) root         (0)     1227 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/planned_trace_update.sql
--rw-rw-rw-   0 root         (0) root         (0)     2286 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/populate_display_table.sql
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/populate_metadata_table.sql
--rw-rw-rw-   0 root         (0) root         (0)     1597 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/trace_update_row.sql
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/trace_update_surv.sql
--rw-rw-rw-   0 root         (0) root         (0)     1966 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/trace_update_tables_all.sql
--rw-rw-rw-   0 root         (0) root         (0)     2030 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/trace_update_tables_hole.sql
--rw-rw-rw-   0 root         (0) root         (0)     2118 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/trace_update_tables_hole_trigger.sql
--rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/trace_update_xyz.sql
--rw-rw-rw-   0 root         (0) root         (0)     1331 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/update_dh_sg_immersion.sql
--rw-rw-rw-   0 root         (0) root         (0)     1392 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/update_gis_geom_dh_collar_ll.sql
--rw-rw-rw-   0 root         (0) root         (0)     1344 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/functions/update_srid_dh.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.453672 xplordb-0.13.3/xplordb/schema/dh/populate/
--rw-rw-rw-   0 root         (0) root         (0)     1833 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/alteration.sql
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/assay.sql
--rw-rw-rw-   0 root         (0) root         (0)    23036 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/collar.sql
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/collar_view.sql
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/collar_view_geom.sql
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/collar_view_geom_trace.sql
--rw-rw-rw-   0 root         (0) root         (0)     1889 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/core_recovery.sql
--rw-rw-rw-   0 root         (0) root         (0)    18284 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/details.sql
--rw-rw-rw-   0 root         (0) root         (0)     3933 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/event.sql
--rw-rw-rw-   0 root         (0) root         (0)    46676 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/lith.sql
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/minerals.sql
--rw-rw-rw-   0 root         (0) root         (0)    44305 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/oxidation.sql
--rw-rw-rw-   0 root         (0) root         (0)     1983 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/petrology.sql
--rw-rw-rw-   0 root         (0) root         (0)    62270 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/sample.sql
--rw-rw-rw-   0 root         (0) root         (0)     1819 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/sample_image.sql
--rw-rw-rw-   0 root         (0) root         (0)    44351 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/sample_quality.sql
--rw-rw-rw-   0 root         (0) root         (0)     1818 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/sample_weight.sql
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/serial_id_add.sql
--rw-rw-rw-   0 root         (0) root         (0)     1869 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/sg.sql
--rw-rw-rw-   0 root         (0) root         (0)     1802 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/struc.sql
--rw-rw-rw-   0 root         (0) root         (0)    13228 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/surv.sql
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/surv_points.sql
--rw-rw-rw-   0 root         (0) root         (0)     1809 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/populate/vein.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.453672 xplordb-0.13.3/xplordb/schema/dh/sequences/
--rw-rw-rw-   0 root         (0) root         (0)     1310 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/sequences/results_seq.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.457671 xplordb-0.13.3/xplordb/schema/dh/table/
--rw-rw-rw-   0 root         (0) root         (0)     9193 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/alteration.sql
--rw-rw-rw-   0 root         (0) root         (0)    13796 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/collar.sql
--rw-rw-rw-   0 root         (0) root         (0)     9104 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/core_recovery.sql
--rw-rw-rw-   0 root         (0) root         (0)     9961 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/details.sql
--rw-rw-rw-   0 root         (0) root         (0)     5870 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/event.sql
--rw-rw-rw-   0 root         (0) root         (0)     7546 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/lith.sql
--rw-rw-rw-   0 root         (0) root         (0)     1973 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/metadata.sql
--rw-rw-rw-   0 root         (0) root         (0)     8950 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/minerals.sql
--rw-rw-rw-   0 root         (0) root         (0)     6336 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/oxidation.sql
--rw-rw-rw-   0 root         (0) root         (0)    10724 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/petrology.sql
--rw-rw-rw-   0 root         (0) root         (0)     8739 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/sample.sql
--rw-rw-rw-   0 root         (0) root         (0)     7399 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/sample_image.sql
--rw-rw-rw-   0 root         (0) root         (0)     7602 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/sample_quality.sql
--rw-rw-rw-   0 root         (0) root         (0)     7848 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/sample_weight.sql
--rw-rw-rw-   0 root         (0) root         (0)     9694 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/sg.sql
--rw-rw-rw-   0 root         (0) root         (0)     7388 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/struc.sql
--rw-rw-rw-   0 root         (0) root         (0)    13185 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/surv.sql
--rw-rw-rw-   0 root         (0) root         (0)     8515 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/table/vein.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.458672 xplordb-0.13.3/xplordb/schema/dh/trigger/
--rw-rw-rw-   0 root         (0) root         (0)     1863 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/trigger/details_trigger.sql
--rw-rw-rw-   0 root         (0) root         (0)     1699 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/trigger/lith_trigger.sql
--rw-rw-rw-   0 root         (0) root         (0)     1759 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/trigger/oxidation_trigger.sql
--rw-rw-rw-   0 root         (0) root         (0)     1819 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/trigger/sample_quality_trigger.sql
--rw-rw-rw-   0 root         (0) root         (0)     1722 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/trigger/sample_trigger.sql
--rw-rw-rw-   0 root         (0) root         (0)     1300 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/trigger/table_trace_update.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.459672 xplordb-0.13.3/xplordb/schema/dh/views/
--rw-rw-rw-   0 root         (0) root         (0)     2927 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/views/collar_view.sql
--rw-rw-rw-   0 root         (0) root         (0)     2953 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/views/collar_view_geom.sql
--rw-rw-rw-   0 root         (0) root         (0)     2977 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/views/collar_view_geom_trace.sql
--rw-rw-rw-   0 root         (0) root         (0)     2560 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/views/serial_id_add.sql
--rw-rw-rw-   0 root         (0) root         (0)     2838 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/dh/views/surv_points.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.459672 xplordb-0.13.3/xplordb/schema/display/
--rw-rw-rw-   0 root         (0) root         (0)     1618 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/display/display.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.460672 xplordb-0.13.3/xplordb/schema/display/functions/
--rw-rw-rw-   0 root         (0) root         (0)     4522 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/display/functions/display_effective_trace.sql
--rw-rw-rw-   0 root         (0) root         (0)     3772 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/display/functions/display_planned_trace.sql
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/display/functions/display_trace.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.460672 xplordb-0.13.3/xplordb/schema/display/table/
--rw-rw-rw-   0 root         (0) root         (0)     3116 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/display/table/display_collar.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.460672 xplordb-0.13.3/xplordb/schema/display/trigger/
--rw-rw-rw-   0 root         (0) root         (0)     1275 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/display/trigger/collar_trigger.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.460672 xplordb-0.13.3/xplordb/schema/qa/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.461671 xplordb-0.13.3/xplordb/schema/qa/populate/
--rw-rw-rw-   0 root         (0) root         (0)     1821 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/qa/populate/dh.sql
--rw-rw-rw-   0 root         (0) root         (0)     2225 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/qa/populate/qc_type.sql
--rw-rw-rw-   0 root         (0) root         (0)     1871 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/qa/populate/sd_values.sql
--rw-rw-rw-   0 root         (0) root         (0)     1933 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/qa/populate/surf.sql
--rw-rw-rw-   0 root         (0) root         (0)     1591 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/qa/qa.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.462672 xplordb-0.13.3/xplordb/schema/qa/table/
--rw-rw-rw-   0 root         (0) root         (0)     7888 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/qa/table/dh.sql
--rw-rw-rw-   0 root         (0) root         (0)     3695 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/qa/table/qc_type.sql
--rw-rw-rw-   0 root         (0) root         (0)     7653 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/qa/table/sd_values.sql
--rw-rw-rw-   0 root         (0) root         (0)     4941 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/qa/table/surf.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.462672 xplordb-0.13.3/xplordb/schema/ref/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.462672 xplordb-0.13.3/xplordb/schema/ref/fk_creation/
--rw-rw-rw-   0 root         (0) root         (0)     1236 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/fk_creation/company_person.sql
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/fk_creation/person_datasets.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.463672 xplordb-0.13.3/xplordb/schema/ref/functions/
--rw-rw-rw-   0 root         (0) root         (0)     1710 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/functions/update_lab_method_code.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.472671 xplordb-0.13.3/xplordb/schema/ref/populate/
--rw-rw-rw-   0 root         (0) root         (0)     1827 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/assay_result_code.sql
--rw-rw-rw-   0 root         (0) root         (0)     2277 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/azimuth_type.sql
--rw-rw-rw-   0 root         (0) root         (0)     2214 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/company.sql
--rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/company_type.sql
--rw-rw-rw-   0 root         (0) root         (0)     1937 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/core_type.sql
--rw-rw-rw-   0 root         (0) root         (0)     1934 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/data_sets.sql
--rw-rw-rw-   0 root         (0) root         (0)     4042 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/data_source.sql
--rw-rw-rw-   0 root         (0) root         (0)     2753 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/dh_survey_instrument.sql
--rw-rw-rw-   0 root         (0) root         (0)     2951 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/dh_survey_method.sql
--rw-rw-rw-   0 root         (0) root         (0)    15758 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/elements.sql
--rw-rw-rw-   0 root         (0) root         (0)     1859 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/event.sql
--rw-rw-rw-   0 root         (0) root         (0)     1799 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/event_code.sql
--rw-rw-rw-   0 root         (0) root         (0)     1799 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/geomagnetic_declination.sql
--rw-rw-rw-   0 root         (0) root         (0)     1842 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/grid_id.sql
--rw-rw-rw-   0 root         (0) root         (0)     1900 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/hole_status.sql
--rw-rw-rw-   0 root         (0) root         (0)     2119 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/hole_type.sql
--rw-rw-rw-   0 root         (0) root         (0)     4652 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/lab.sql
--rw-rw-rw-   0 root         (0) root         (0)     9390 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/lab_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     1786 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/lab_method_code.sql
--rw-rw-rw-   0 root         (0) root         (0)     2182 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/lab_o_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     3184 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/lease.sql
--rw-rw-rw-   0 root         (0) root         (0)     2572 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/lithology.sql
--rw-rw-rw-   0 root         (0) root         (0)     2063 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/location_confidence_m.sql
--rw-rw-rw-   0 root         (0) root         (0)     3882 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/minerals.sql
--rw-rw-rw-   0 root         (0) root         (0)     1940 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/oxidation.sql
--rw-rw-rw-   0 root         (0) root         (0)     2135 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/person.sql
--rw-rw-rw-   0 root         (0) root         (0)     2021 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/preferred.sql
--rw-rw-rw-   0 root         (0) root         (0)     1778 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/program.sql
--rw-rw-rw-   0 root         (0) root         (0)     2628 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/prospect.sql
--rw-rw-rw-   0 root         (0) root         (0)    99025 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/qgis_projects.sql
--rw-rw-rw-   0 root         (0) root         (0)     1923 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/rl_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     3141 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/sample_class.sql
--rw-rw-rw-   0 root         (0) root         (0)     1991 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/sample_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     2652 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/sample_type.sql
--rw-rw-rw-   0 root         (0) root         (0)     2416 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/sg_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     1784 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/strat_name.sql
--rw-rw-rw-   0 root         (0) root         (0)     1711 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/struc.sql
--rw-rw-rw-   0 root         (0) root         (0)     1771 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/survey_instrument.sql
--rw-rw-rw-   0 root         (0) root         (0)     2051 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/survey_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     2350 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/units.sql
--rw-rw-rw-   0 root         (0) root         (0)     2074 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/populate/xrf_instrument.sql
--rw-rw-rw-   0 root         (0) root         (0)     1601 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/ref.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.482671 xplordb-0.13.3/xplordb/schema/ref/table/
--rw-rw-rw-   0 root         (0) root         (0)     3561 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/assay_result_code.sql
--rw-rw-rw-   0 root         (0) root         (0)     3378 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/azimuth_type.sql
--rw-rw-rw-   0 root         (0) root         (0)     3770 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/company.sql
--rw-rw-rw-   0 root         (0) root         (0)     3574 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/company_type.sql
--rw-rw-rw-   0 root         (0) root         (0)     3256 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/core_type.sql
--rw-rw-rw-   0 root         (0) root         (0)     5127 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/data_sets.sql
--rw-rw-rw-   0 root         (0) root         (0)     6093 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/data_source.sql
--rw-rw-rw-   0 root         (0) root         (0)     3133 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/dh_survey_instrument.sql
--rw-rw-rw-   0 root         (0) root         (0)     3455 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/dh_survey_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     8543 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/elements.sql
--rw-rw-rw-   0 root         (0) root         (0)     3521 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/event.sql
--rw-rw-rw-   0 root         (0) root         (0)     3651 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/event_code.sql
--rw-rw-rw-   0 root         (0) root         (0)     5327 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/geomagnetic_declination.sql
--rw-rw-rw-   0 root         (0) root         (0)     4035 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/grid_id.sql
--rw-rw-rw-   0 root         (0) root         (0)     3654 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/hole_status.sql
--rw-rw-rw-   0 root         (0) root         (0)     3611 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/hole_type.sql
--rw-rw-rw-   0 root         (0) root         (0)     4509 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/lab.sql
--rw-rw-rw-   0 root         (0) root         (0)     6434 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/lab_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     2867 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/lab_method_code.sql
--rw-rw-rw-   0 root         (0) root         (0)     3574 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/lab_o_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     6185 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/lease.sql
--rw-rw-rw-   0 root         (0) root         (0)     4978 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/lithology.sql
--rw-rw-rw-   0 root         (0) root         (0)     3559 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/location_confidence_m.sql
--rw-rw-rw-   0 root         (0) root         (0)     3757 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/minerals.sql
--rw-rw-rw-   0 root         (0) root         (0)     3616 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/oxidation.sql
--rw-rw-rw-   0 root         (0) root         (0)     4573 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/person.sql
--rw-rw-rw-   0 root         (0) root         (0)     3625 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/preferred.sql
--rw-rw-rw-   0 root         (0) root         (0)     2957 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/program.sql
--rw-rw-rw-   0 root         (0) root         (0)     6048 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/prospect.sql
--rw-rw-rw-   0 root         (0) root         (0)     2330 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/qgis_projects.sql
--rw-rw-rw-   0 root         (0) root         (0)     3436 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/rl_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     3340 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/sample_class.sql
--rw-rw-rw-   0 root         (0) root         (0)     3707 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/sample_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     3655 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/sample_type.sql
--rw-rw-rw-   0 root         (0) root         (0)     2980 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/sg_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     4541 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/strat_name.sql
--rw-rw-rw-   0 root         (0) root         (0)     3129 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/struc.sql
--rw-rw-rw-   0 root         (0) root         (0)     3228 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/survey_instrument.sql
--rw-rw-rw-   0 root         (0) root         (0)     3743 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/survey_method.sql
--rw-rw-rw-   0 root         (0) root         (0)     3493 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/units.sql
--rw-rw-rw-   0 root         (0) root         (0)     2998 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/table/xrf_instrument.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.483671 xplordb-0.13.3/xplordb/schema/ref/trigger/
--rw-rw-rw-   0 root         (0) root         (0)     1245 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/ref/trigger/lab_method_trigger.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.483671 xplordb-0.13.3/xplordb/schema/surf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.483671 xplordb-0.13.3/xplordb/schema/surf/functions/
--rw-rw-rw-   0 root         (0) root         (0)     1436 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/surf/functions/update_gis_geom_sample_ll.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.483671 xplordb-0.13.3/xplordb/schema/surf/populate/
--rw-rw-rw-   0 root         (0) root         (0)    34228 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/surf/populate/sample.sql
--rw-rw-rw-   0 root         (0) root         (0)     1611 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/surf/surf.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.484671 xplordb-0.13.3/xplordb/schema/surf/table/
--rw-rw-rw-   0 root         (0) root         (0)    13584 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/surf/table/sample.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.484671 xplordb-0.13.3/xplordb/schema/v/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.484671 xplordb-0.13.3/xplordb/schema/v/populate/
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/v/populate/missing_samples.sql
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/v/populate/missing_surv.sql
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/v/v.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.485671 xplordb-0.13.3/xplordb/schema/v/views/
--rw-rw-rw-   0 root         (0) root         (0)     2806 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/v/views/missing_samples.sql
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema/v/views/missing_surv.sql
--rw-rw-rw-   0 root         (0) root         (0)     9052 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     5110 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/sql_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.485671 xplordb-0.13.3/xplordb/sqlalchemy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/sqlalchemy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      894 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/sqlalchemy/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.487671 xplordb-0.13.3/xplordb/sqlalchemy/dh/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/sqlalchemy/dh/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/sqlalchemy/dh/collar.py
--rw-rw-rw-   0 root         (0) root         (0)      972 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/sqlalchemy/dh/lith.py
--rw-rw-rw-   0 root         (0) root         (0)     1347 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/sqlalchemy/dh/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/sqlalchemy/dh/survey.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.487671 xplordb-0.13.3/xplordb/sqlalchemy/ref/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/sqlalchemy/ref/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      658 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/sqlalchemy/ref/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/sqlalchemy/ref/lithcode.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2024-04-17 07:28:00.000000 xplordb-0.13.3/xplordb/sqlalchemy/ref/person.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:28:10.488671 xplordb-0.13.3/xplordb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5407 2024-04-17 07:28:10.000000 xplordb-0.13.3/xplordb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9752 2024-04-17 07:28:10.000000 xplordb-0.13.3/xplordb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 07:28:10.000000 xplordb-0.13.3/xplordb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2024-04-17 07:28:10.000000 xplordb-0.13.3/xplordb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-17 07:28:10.000000 xplordb-0.13.3/xplordb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.762575 xplordb-0.13.4/
+-rw-rw-rw-   0 root         (0) root         (0)    34459 2024-04-30 12:24:07.000000 xplordb-0.13.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-30 12:24:07.000000 xplordb-0.13.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-04-30 12:24:19.762575 xplordb-0.13.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4695 2024-04-30 12:24:07.000000 xplordb-0.13.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7339 2024-04-30 12:24:07.000000 xplordb-0.13.4/README.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2024-04-30 12:24:19.763575 xplordb-0.13.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2024-04-30 12:24:07.000000 xplordb-0.13.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.703576 xplordb-0.13.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 12:24:07.000000 xplordb-0.13.4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5383 2024-04-30 12:24:07.000000 xplordb-0.13.4/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2024-04-30 12:24:07.000000 xplordb-0.13.4/tests/test_create_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     8675 2024-04-30 12:24:07.000000 xplordb-0.13.4/tests/test_import_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    15489 2024-04-30 12:24:07.000000 xplordb-0.13.4/tests/test_import_ddl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.704576 xplordb-0.13.4/xplordb/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/create_db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.707576 xplordb-0.13.4/xplordb/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/datamodel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/datamodel/collar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1357 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/datamodel/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2303 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/datamodel/lith.py
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/datamodel/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/datamodel/person.py
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/datamodel/survey.py
+-rw-rw-rw-   0 root         (0) root         (0)     8310 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/import_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5145 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/import_ddl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3090 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/minimal_dao.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.699576 xplordb-0.13.4/xplordb/schema/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.707576 xplordb-0.13.4/xplordb/schema/assay/
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/assay.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.708576 xplordb-0.13.4/xplordb/schema/assay/functions/
+-rw-rw-rw-   0 root         (0) root         (0)     7789 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/functions/flat_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     9397 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/functions/flat_ppm.sql
+-rw-rw-rw-   0 root         (0) root         (0)    11681 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/functions/import.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/functions/structural_types.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.711576 xplordb-0.13.4/xplordb/schema/assay/populate/
+-rw-rw-rw-   0 root         (0) root         (0)  1438090 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/populate/assay.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4458 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/populate/batch.sql
+-rw-rw-rw-   0 root         (0) root         (0)   163953 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/populate/flat_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)   125897 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/populate/flat_ppm.sql
+-rw-rw-rw-   0 root         (0) root         (0)    28371 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/populate/raw.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.712576 xplordb-0.13.4/xplordb/schema/assay/table/
+-rw-rw-rw-   0 root         (0) root         (0)     8504 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/table/assay.sql
+-rw-rw-rw-   0 root         (0) root         (0)     7813 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/table/batch.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3800 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/table/flat_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3783 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/table/flat_ppm.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/table/raw.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.713576 xplordb-0.13.4/xplordb/schema/assay/views/
+-rw-rw-rw-   0 root         (0) root         (0)     3789 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/views/assay.sql
+-rw-rw-rw-   0 root         (0) root         (0)     6317 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/assay/views/intercepts.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.713576 xplordb-0.13.4/xplordb/schema/dem/
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dem/dem.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.713576 xplordb-0.13.4/xplordb/schema/dem/functions/
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dem/functions/alos_cap_update_example.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1583 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dem/functions/cap_alos_example.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.713576 xplordb-0.13.4/xplordb/schema/dem/populate/
+-rw-rw-rw-   0 root         (0) root         (0)   987241 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dem/populate/capricorn.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.715576 xplordb-0.13.4/xplordb/schema/dem/table/
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dem/table/capricorn.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.715576 xplordb-0.13.4/xplordb/schema/dh/
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/dh.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.719576 xplordb-0.13.4/xplordb/schema/dh/functions/
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/check_depth_m.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/check_from_m.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/check_to_m.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3576 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/dh_planned_trace.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4346 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/dh_trace.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2323 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/dog_leg.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/geom_update_xyz.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/planned_trace_update.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2286 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/populate_display_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/populate_metadata_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1597 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/trace_update_row.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/trace_update_surv.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/trace_update_tables_all.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/trace_update_tables_hole.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2118 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/trace_update_tables_hole_trigger.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/trace_update_xyz.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/update_dh_sg_immersion.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1392 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/update_gis_geom_dh_collar_ll.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/functions/update_srid_dh.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.725576 xplordb-0.13.4/xplordb/schema/dh/populate/
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/alteration.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/assay.sql
+-rw-rw-rw-   0 root         (0) root         (0)    23036 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/collar.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/collar_view.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/collar_view_geom.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/collar_view_geom_trace.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/core_recovery.sql
+-rw-rw-rw-   0 root         (0) root         (0)    18284 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/details.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3933 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/event.sql
+-rw-rw-rw-   0 root         (0) root         (0)    46676 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/lith.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/minerals.sql
+-rw-rw-rw-   0 root         (0) root         (0)    44305 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/oxidation.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1983 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/petrology.sql
+-rw-rw-rw-   0 root         (0) root         (0)    62270 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/sample.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1819 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/sample_image.sql
+-rw-rw-rw-   0 root         (0) root         (0)    44351 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/sample_quality.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1818 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/sample_weight.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/serial_id_add.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/sg.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/struc.sql
+-rw-rw-rw-   0 root         (0) root         (0)    13228 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/surv.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/surv_points.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1809 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/populate/vein.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.725576 xplordb-0.13.4/xplordb/schema/dh/sequences/
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/sequences/results_seq.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.729575 xplordb-0.13.4/xplordb/schema/dh/table/
+-rw-rw-rw-   0 root         (0) root         (0)     9193 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/alteration.sql
+-rw-rw-rw-   0 root         (0) root         (0)    13796 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/collar.sql
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/core_recovery.sql
+-rw-rw-rw-   0 root         (0) root         (0)     9961 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/details.sql
+-rw-rw-rw-   0 root         (0) root         (0)     5870 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/event.sql
+-rw-rw-rw-   0 root         (0) root         (0)     7546 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/lith.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/metadata.sql
+-rw-rw-rw-   0 root         (0) root         (0)     8950 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/minerals.sql
+-rw-rw-rw-   0 root         (0) root         (0)     6336 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/oxidation.sql
+-rw-rw-rw-   0 root         (0) root         (0)    10724 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/petrology.sql
+-rw-rw-rw-   0 root         (0) root         (0)     8739 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/sample.sql
+-rw-rw-rw-   0 root         (0) root         (0)     7399 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/sample_image.sql
+-rw-rw-rw-   0 root         (0) root         (0)     7602 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/sample_quality.sql
+-rw-rw-rw-   0 root         (0) root         (0)     7848 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/sample_weight.sql
+-rw-rw-rw-   0 root         (0) root         (0)     9694 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/sg.sql
+-rw-rw-rw-   0 root         (0) root         (0)     7388 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/struc.sql
+-rw-rw-rw-   0 root         (0) root         (0)    13185 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/surv.sql
+-rw-rw-rw-   0 root         (0) root         (0)     8515 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/table/vein.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.731576 xplordb-0.13.4/xplordb/schema/dh/trigger/
+-rw-rw-rw-   0 root         (0) root         (0)     1863 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/trigger/details_trigger.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/trigger/lith_trigger.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1759 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/trigger/oxidation_trigger.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1819 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/trigger/sample_quality_trigger.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/trigger/sample_trigger.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/trigger/table_trace_update.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.732576 xplordb-0.13.4/xplordb/schema/dh/views/
+-rw-rw-rw-   0 root         (0) root         (0)     2927 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/views/collar_view.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2953 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/views/collar_view_geom.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2977 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/views/collar_view_geom_trace.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2560 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/views/serial_id_add.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2838 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/dh/views/surv_points.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.732576 xplordb-0.13.4/xplordb/schema/display/
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/display/display.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.733575 xplordb-0.13.4/xplordb/schema/display/functions/
+-rw-rw-rw-   0 root         (0) root         (0)     4522 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/display/functions/display_effective_trace.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3772 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/display/functions/display_planned_trace.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/display/functions/display_trace.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.733575 xplordb-0.13.4/xplordb/schema/display/table/
+-rw-rw-rw-   0 root         (0) root         (0)     3116 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/display/table/display_collar.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.733575 xplordb-0.13.4/xplordb/schema/display/trigger/
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/display/trigger/collar_trigger.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.733575 xplordb-0.13.4/xplordb/schema/qa/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.734575 xplordb-0.13.4/xplordb/schema/qa/populate/
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/qa/populate/dh.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/qa/populate/qc_type.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1871 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/qa/populate/sd_values.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1933 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/qa/populate/surf.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/qa/qa.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.735575 xplordb-0.13.4/xplordb/schema/qa/table/
+-rw-rw-rw-   0 root         (0) root         (0)     7888 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/qa/table/dh.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3695 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/qa/table/qc_type.sql
+-rw-rw-rw-   0 root         (0) root         (0)     7653 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/qa/table/sd_values.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4941 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/qa/table/surf.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.736575 xplordb-0.13.4/xplordb/schema/ref/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.736575 xplordb-0.13.4/xplordb/schema/ref/fk_creation/
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/fk_creation/company_person.sql
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/fk_creation/person_datasets.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.736575 xplordb-0.13.4/xplordb/schema/ref/functions/
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/functions/update_lab_method_code.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.746575 xplordb-0.13.4/xplordb/schema/ref/populate/
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/assay_result_code.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/azimuth_type.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/company.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/company_type.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1937 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/core_type.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/data_sets.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4042 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/data_source.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2753 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/dh_survey_instrument.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/dh_survey_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)    15758 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/elements.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1859 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/event.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1799 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/event_code.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1799 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/geomagnetic_declination.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1842 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/grid_id.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1900 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/hole_status.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2119 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/hole_type.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4652 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/lab.sql
+-rw-rw-rw-   0 root         (0) root         (0)     9390 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/lab_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1786 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/lab_method_code.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/lab_o_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3184 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/lease.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2572 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/lithology.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/location_confidence_m.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3882 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/minerals.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1940 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/oxidation.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2135 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/person.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2021 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/preferred.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/program.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/prospect.sql
+-rw-rw-rw-   0 root         (0) root         (0)    99025 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/qgis_projects.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1923 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/rl_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3141 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/sample_class.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/sample_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2652 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/sample_type.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/sg_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1784 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/strat_name.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/struc.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1771 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/survey_instrument.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2051 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/survey_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/units.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2074 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/populate/xrf_instrument.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/ref.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.756575 xplordb-0.13.4/xplordb/schema/ref/table/
+-rw-rw-rw-   0 root         (0) root         (0)     3561 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/assay_result_code.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3378 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/azimuth_type.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3770 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/company.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/company_type.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3256 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/core_type.sql
+-rw-rw-rw-   0 root         (0) root         (0)     5127 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/data_sets.sql
+-rw-rw-rw-   0 root         (0) root         (0)     6093 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/data_source.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3133 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/dh_survey_instrument.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3455 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/dh_survey_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     8543 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/elements.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3521 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/event.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3651 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/event_code.sql
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/geomagnetic_declination.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4035 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/grid_id.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3654 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/hole_status.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3611 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/hole_type.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4509 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/lab.sql
+-rw-rw-rw-   0 root         (0) root         (0)     6434 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/lab_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2867 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/lab_method_code.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/lab_o_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     6185 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/lease.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4978 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/lithology.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3559 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/location_confidence_m.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3757 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/minerals.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3616 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/oxidation.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4573 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/person.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3625 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/preferred.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2957 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/program.sql
+-rw-rw-rw-   0 root         (0) root         (0)     6048 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/prospect.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2330 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/qgis_projects.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3436 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/rl_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3340 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/sample_class.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3707 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/sample_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3655 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/sample_type.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2980 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/sg_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4541 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/strat_name.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3129 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/struc.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3228 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/survey_instrument.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3743 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/survey_method.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3493 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/units.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2998 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/table/xrf_instrument.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.756575 xplordb-0.13.4/xplordb/schema/ref/trigger/
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/ref/trigger/lab_method_trigger.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.756575 xplordb-0.13.4/xplordb/schema/surf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.756575 xplordb-0.13.4/xplordb/schema/surf/functions/
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/surf/functions/update_gis_geom_sample_ll.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.757575 xplordb-0.13.4/xplordb/schema/surf/populate/
+-rw-rw-rw-   0 root         (0) root         (0)    34228 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/surf/populate/sample.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/surf/surf.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.757575 xplordb-0.13.4/xplordb/schema/surf/table/
+-rw-rw-rw-   0 root         (0) root         (0)    13584 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/surf/table/sample.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.757575 xplordb-0.13.4/xplordb/schema/v/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.758575 xplordb-0.13.4/xplordb/schema/v/populate/
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/v/populate/missing_samples.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/v/populate/missing_surv.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/v/v.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.758575 xplordb-0.13.4/xplordb/schema/v/views/
+-rw-rw-rw-   0 root         (0) root         (0)     2806 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/v/views/missing_samples.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema/v/views/missing_surv.sql
+-rw-rw-rw-   0 root         (0) root         (0)     9052 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     5110 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sql_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.758575 xplordb-0.13.4/xplordb/sqlalchemy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sqlalchemy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.759575 xplordb-0.13.4/xplordb/sqlalchemy/assay/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sqlalchemy/assay/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sqlalchemy/assay/structural_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      894 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sqlalchemy/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.760575 xplordb-0.13.4/xplordb/sqlalchemy/dh/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sqlalchemy/dh/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sqlalchemy/dh/collar.py
+-rw-rw-rw-   0 root         (0) root         (0)      972 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sqlalchemy/dh/lith.py
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sqlalchemy/dh/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sqlalchemy/dh/survey.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.761575 xplordb-0.13.4/xplordb/sqlalchemy/ref/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sqlalchemy/ref/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sqlalchemy/ref/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sqlalchemy/ref/lithcode.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2024-04-30 12:24:07.000000 xplordb-0.13.4/xplordb/sqlalchemy/ref/person.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:24:19.761575 xplordb-0.13.4/xplordb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-04-30 12:24:19.000000 xplordb-0.13.4/xplordb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9834 2024-04-30 12:24:19.000000 xplordb-0.13.4/xplordb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 12:24:19.000000 xplordb-0.13.4/xplordb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2024-04-30 12:24:19.000000 xplordb-0.13.4/xplordb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-30 12:24:19.000000 xplordb-0.13.4/xplordb.egg-info/top_level.txt
```

### Comparing `xplordb-0.13.3/LICENSE` & `xplordb-0.13.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/PKG-INFO` & `xplordb-0.13.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplordb
-Version: 0.13.3
+Version: 0.13.4
 Summary: Python module to read/write data into xplordb database
 Home-page: https://gitlab.com/geolandia/openlog/xplordb
 Author: Oslandia
 Author-email: geology@oslandia.com
 License: AGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `xplordb-0.13.3/README.md` & `xplordb-0.13.4/README.md`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/README.txt` & `xplordb-0.13.4/README.txt`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/setup.cfg` & `xplordb-0.13.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/setup.py` & `xplordb-0.13.4/setup.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/tests/conftest.py` & `xplordb-0.13.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/tests/test_create_db.py` & `xplordb-0.13.4/tests/test_create_db.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/tests/test_import_data.py` & `xplordb-0.13.4/tests/test_import_data.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/tests/test_import_ddl.py` & `xplordb-0.13.4/tests/test_import_ddl.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/create_db.py` & `xplordb-0.13.4/xplordb/create_db.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/datamodel/collar.py` & `xplordb-0.13.4/xplordb/datamodel/collar.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/datamodel/dataset.py` & `xplordb-0.13.4/xplordb/datamodel/dataset.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/datamodel/lith.py` & `xplordb-0.13.4/xplordb/datamodel/lith.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/datamodel/metadata.py` & `xplordb-0.13.4/xplordb/datamodel/metadata.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/datamodel/person.py` & `xplordb-0.13.4/xplordb/datamodel/person.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/datamodel/survey.py` & `xplordb-0.13.4/xplordb/datamodel/survey.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/import_data.py` & `xplordb-0.13.4/xplordb/import_data.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/import_ddl.py` & `xplordb-0.13.4/xplordb/import_ddl.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/minimal_dao.py` & `xplordb-0.13.4/xplordb/minimal_dao.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/assay.sql` & `xplordb-0.13.4/xplordb/schema/assay/assay.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/functions/flat_method.sql` & `xplordb-0.13.4/xplordb/schema/assay/functions/flat_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/functions/flat_ppm.sql` & `xplordb-0.13.4/xplordb/schema/assay/functions/flat_ppm.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/functions/import.sql` & `xplordb-0.13.4/xplordb/schema/assay/functions/import.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/functions/structural_types.sql` & `xplordb-0.13.4/xplordb/schema/assay/functions/structural_types.sql`

 * *Files 14% similar despite different names*

```diff
@@ -21,11 +21,13 @@
 -- __license__ = "AGPLv3"
 ----------------------------------------------------------------------------
 
 
 -- basic types and constraints
 CREATE DOMAIN assay.azimuth AS FLOAT CHECK(VALUE BETWEEN 0 AND 360);
 CREATE DOMAIN assay.dip AS FLOAT CHECK(VALUE BETWEEN -90 AND 90);
+-- 0 : reversed, 1 : normal, 2 : unknown
+CREATE DOMAIN assay.polarity AS INT CHECK(VALUE = 0 OR VALUE = 1  OR VALUE = 2);
 CREATE DOMAIN assay.kind AS VARCHAR CHECK(VALUE = 'line' OR VALUE = 'plane');
 
 -- composite type
-CREATE TYPE assay.spherical_data AS (azimuth assay.azimuth, dip assay.dip, kind assay.kind);
+CREATE TYPE assay.spherical_data AS (azimuth assay.azimuth, dip assay.dip, polarity assay.polarity, kind assay.kind);
```

### Comparing `xplordb-0.13.3/xplordb/schema/assay/populate/assay.sql` & `xplordb-0.13.4/xplordb/schema/assay/populate/assay.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/populate/batch.sql` & `xplordb-0.13.4/xplordb/schema/assay/populate/batch.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/populate/flat_method.sql` & `xplordb-0.13.4/xplordb/schema/assay/populate/flat_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/populate/flat_ppm.sql` & `xplordb-0.13.4/xplordb/schema/assay/populate/flat_ppm.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/populate/raw.sql` & `xplordb-0.13.4/xplordb/schema/assay/populate/raw.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/table/assay.sql` & `xplordb-0.13.4/xplordb/schema/assay/table/assay.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/table/batch.sql` & `xplordb-0.13.4/xplordb/schema/assay/table/batch.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/table/flat_method.sql` & `xplordb-0.13.4/xplordb/schema/assay/table/flat_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/table/flat_ppm.sql` & `xplordb-0.13.4/xplordb/schema/assay/table/flat_ppm.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/table/raw.sql` & `xplordb-0.13.4/xplordb/schema/assay/table/raw.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/views/assay.sql` & `xplordb-0.13.4/xplordb/schema/assay/views/assay.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/assay/views/intercepts.sql` & `xplordb-0.13.4/xplordb/schema/assay/views/intercepts.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dem/dem.sql` & `xplordb-0.13.4/xplordb/schema/dem/dem.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dem/functions/alos_cap_update_example.sql` & `xplordb-0.13.4/xplordb/schema/dem/functions/alos_cap_update_example.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dem/functions/cap_alos_example.sql` & `xplordb-0.13.4/xplordb/schema/dem/functions/cap_alos_example.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dem/populate/capricorn.sql` & `xplordb-0.13.4/xplordb/schema/dem/populate/capricorn.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dem/table/capricorn.sql` & `xplordb-0.13.4/xplordb/schema/dem/table/capricorn.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/dh.sql` & `xplordb-0.13.4/xplordb/schema/dh/dh.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/check_depth_m.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/check_depth_m.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/check_from_m.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/check_from_m.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/check_to_m.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/check_to_m.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/dh_planned_trace.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/dh_planned_trace.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/dh_trace.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/dh_trace.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/dog_leg.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/dog_leg.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/geom_update_xyz.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/geom_update_xyz.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/planned_trace_update.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/planned_trace_update.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/populate_display_table.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/populate_display_table.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/populate_metadata_table.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/populate_metadata_table.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/trace_update_row.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/trace_update_row.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/trace_update_surv.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/trace_update_surv.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/trace_update_tables_all.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/trace_update_tables_all.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/trace_update_tables_hole.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/trace_update_tables_hole.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/trace_update_tables_hole_trigger.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/trace_update_tables_hole_trigger.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/trace_update_xyz.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/trace_update_xyz.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/update_dh_sg_immersion.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/update_dh_sg_immersion.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/update_gis_geom_dh_collar_ll.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/update_gis_geom_dh_collar_ll.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/functions/update_srid_dh.sql` & `xplordb-0.13.4/xplordb/schema/dh/functions/update_srid_dh.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/alteration.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/alteration.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/assay.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/assay.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/collar.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/collar.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/collar_view.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/collar_view.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/collar_view_geom.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/collar_view_geom.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/collar_view_geom_trace.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/collar_view_geom_trace.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/core_recovery.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/core_recovery.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/details.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/details.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/event.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/event.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/lith.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/lith.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/minerals.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/minerals.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/oxidation.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/oxidation.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/petrology.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/petrology.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/sample.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/sample.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/sample_image.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/sample_image.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/sample_quality.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/sample_quality.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/sample_weight.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/sample_weight.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/serial_id_add.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/serial_id_add.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/sg.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/sg.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/struc.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/struc.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/surv.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/surv.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/surv_points.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/surv_points.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/populate/vein.sql` & `xplordb-0.13.4/xplordb/schema/dh/populate/vein.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/sequences/results_seq.sql` & `xplordb-0.13.4/xplordb/schema/dh/sequences/results_seq.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/alteration.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/alteration.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/collar.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/collar.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/core_recovery.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/core_recovery.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/details.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/details.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/event.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/event.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/lith.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/lith.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/metadata.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/metadata.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/minerals.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/minerals.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/oxidation.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/oxidation.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/petrology.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/petrology.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/sample.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/sample.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/sample_image.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/sample_image.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/sample_quality.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/sample_quality.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/sample_weight.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/sample_weight.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/sg.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/sg.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/struc.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/struc.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/surv.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/surv.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/table/vein.sql` & `xplordb-0.13.4/xplordb/schema/dh/table/vein.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/trigger/details_trigger.sql` & `xplordb-0.13.4/xplordb/schema/dh/trigger/details_trigger.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/trigger/lith_trigger.sql` & `xplordb-0.13.4/xplordb/schema/dh/trigger/lith_trigger.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/trigger/oxidation_trigger.sql` & `xplordb-0.13.4/xplordb/schema/dh/trigger/oxidation_trigger.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/trigger/sample_quality_trigger.sql` & `xplordb-0.13.4/xplordb/schema/dh/trigger/sample_quality_trigger.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/trigger/sample_trigger.sql` & `xplordb-0.13.4/xplordb/schema/dh/trigger/sample_trigger.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/trigger/table_trace_update.sql` & `xplordb-0.13.4/xplordb/schema/dh/trigger/table_trace_update.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/views/collar_view.sql` & `xplordb-0.13.4/xplordb/schema/dh/views/collar_view.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/views/collar_view_geom.sql` & `xplordb-0.13.4/xplordb/schema/dh/views/collar_view_geom.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/views/collar_view_geom_trace.sql` & `xplordb-0.13.4/xplordb/schema/dh/views/collar_view_geom_trace.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/views/serial_id_add.sql` & `xplordb-0.13.4/xplordb/schema/dh/views/serial_id_add.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/dh/views/surv_points.sql` & `xplordb-0.13.4/xplordb/schema/dh/views/surv_points.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/display/display.sql` & `xplordb-0.13.4/xplordb/schema/display/display.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/display/functions/display_effective_trace.sql` & `xplordb-0.13.4/xplordb/schema/display/functions/display_effective_trace.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/display/functions/display_planned_trace.sql` & `xplordb-0.13.4/xplordb/schema/display/functions/display_planned_trace.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/display/functions/display_trace.sql` & `xplordb-0.13.4/xplordb/schema/display/functions/display_trace.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/display/table/display_collar.sql` & `xplordb-0.13.4/xplordb/schema/display/table/display_collar.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/display/trigger/collar_trigger.sql` & `xplordb-0.13.4/xplordb/schema/display/trigger/collar_trigger.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/qa/populate/dh.sql` & `xplordb-0.13.4/xplordb/schema/qa/populate/dh.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/qa/populate/qc_type.sql` & `xplordb-0.13.4/xplordb/schema/qa/populate/qc_type.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/qa/populate/sd_values.sql` & `xplordb-0.13.4/xplordb/schema/qa/populate/sd_values.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/qa/populate/surf.sql` & `xplordb-0.13.4/xplordb/schema/qa/populate/surf.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/qa/qa.sql` & `xplordb-0.13.4/xplordb/schema/qa/qa.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/qa/table/dh.sql` & `xplordb-0.13.4/xplordb/schema/qa/table/dh.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/qa/table/qc_type.sql` & `xplordb-0.13.4/xplordb/schema/qa/table/qc_type.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/qa/table/sd_values.sql` & `xplordb-0.13.4/xplordb/schema/qa/table/sd_values.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/qa/table/surf.sql` & `xplordb-0.13.4/xplordb/schema/qa/table/surf.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/fk_creation/company_person.sql` & `xplordb-0.13.4/xplordb/schema/ref/fk_creation/company_person.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/functions/update_lab_method_code.sql` & `xplordb-0.13.4/xplordb/schema/ref/functions/update_lab_method_code.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/assay_result_code.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/assay_result_code.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/azimuth_type.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/azimuth_type.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/company.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/company.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/company_type.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/company_type.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/core_type.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/core_type.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/data_sets.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/data_sets.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/data_source.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/data_source.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/dh_survey_instrument.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/dh_survey_instrument.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/dh_survey_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/dh_survey_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/elements.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/elements.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/event.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/event.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/event_code.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/event_code.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/geomagnetic_declination.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/geomagnetic_declination.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/grid_id.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/grid_id.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/hole_status.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/hole_status.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/hole_type.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/hole_type.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/lab.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/lab.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/lab_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/lab_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/lab_method_code.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/lab_method_code.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/lab_o_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/lab_o_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/lease.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/lease.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/lithology.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/lithology.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/location_confidence_m.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/location_confidence_m.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/minerals.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/minerals.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/oxidation.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/oxidation.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/person.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/person.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/preferred.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/preferred.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/program.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/program.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/prospect.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/prospect.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/qgis_projects.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/qgis_projects.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/rl_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/rl_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/sample_class.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/sample_class.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/sample_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/sample_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/sample_type.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/sample_type.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/sg_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/sg_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/strat_name.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/strat_name.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/struc.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/struc.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/survey_instrument.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/survey_instrument.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/survey_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/survey_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/units.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/units.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/populate/xrf_instrument.sql` & `xplordb-0.13.4/xplordb/schema/ref/populate/xrf_instrument.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/ref.sql` & `xplordb-0.13.4/xplordb/schema/ref/ref.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/assay_result_code.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/assay_result_code.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/azimuth_type.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/azimuth_type.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/company.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/company.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/company_type.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/company_type.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/core_type.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/core_type.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/data_sets.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/data_sets.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/data_source.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/data_source.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/dh_survey_instrument.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/dh_survey_instrument.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/dh_survey_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/dh_survey_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/elements.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/elements.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/event.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/event.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/event_code.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/event_code.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/geomagnetic_declination.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/geomagnetic_declination.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/grid_id.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/grid_id.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/hole_status.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/hole_status.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/hole_type.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/hole_type.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/lab.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/lab.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/lab_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/lab_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/lab_method_code.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/lab_method_code.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/lab_o_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/lab_o_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/lease.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/lease.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/lithology.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/lithology.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/location_confidence_m.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/location_confidence_m.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/minerals.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/minerals.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/oxidation.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/oxidation.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/person.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/person.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/preferred.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/preferred.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/program.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/program.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/prospect.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/prospect.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/qgis_projects.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/qgis_projects.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/rl_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/rl_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/sample_class.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/sample_class.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/sample_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/sample_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/sample_type.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/sample_type.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/sg_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/sg_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/strat_name.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/strat_name.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/struc.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/struc.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/survey_instrument.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/survey_instrument.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/survey_method.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/survey_method.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/units.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/units.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/table/xrf_instrument.sql` & `xplordb-0.13.4/xplordb/schema/ref/table/xrf_instrument.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/ref/trigger/lab_method_trigger.sql` & `xplordb-0.13.4/xplordb/schema/ref/trigger/lab_method_trigger.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/surf/functions/update_gis_geom_sample_ll.sql` & `xplordb-0.13.4/xplordb/schema/surf/functions/update_gis_geom_sample_ll.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/surf/populate/sample.sql` & `xplordb-0.13.4/xplordb/schema/surf/populate/sample.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/surf/surf.sql` & `xplordb-0.13.4/xplordb/schema/surf/surf.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/surf/table/sample.sql` & `xplordb-0.13.4/xplordb/schema/surf/table/sample.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/v/populate/missing_samples.sql` & `xplordb-0.13.4/xplordb/schema/v/populate/missing_samples.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/v/populate/missing_surv.sql` & `xplordb-0.13.4/xplordb/schema/v/populate/missing_surv.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/v/v.sql` & `xplordb-0.13.4/xplordb/schema/v/v.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/v/views/missing_samples.sql` & `xplordb-0.13.4/xplordb/schema/v/views/missing_samples.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema/v/views/missing_surv.sql` & `xplordb-0.13.4/xplordb/schema/v/views/missing_surv.sql`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/schema.py` & `xplordb-0.13.4/xplordb/schema.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/sql_utils.py` & `xplordb-0.13.4/xplordb/sql_utils.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/sqlalchemy/base.py` & `xplordb-0.13.4/xplordb/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/sqlalchemy/dh/collar.py` & `xplordb-0.13.4/xplordb/sqlalchemy/dh/collar.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/sqlalchemy/dh/lith.py` & `xplordb-0.13.4/xplordb/sqlalchemy/dh/lith.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/sqlalchemy/dh/metadata.py` & `xplordb-0.13.4/xplordb/sqlalchemy/dh/metadata.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/sqlalchemy/dh/survey.py` & `xplordb-0.13.4/xplordb/sqlalchemy/dh/survey.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/sqlalchemy/ref/dataset.py` & `xplordb-0.13.4/xplordb/sqlalchemy/ref/dataset.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb/sqlalchemy/ref/person.py` & `xplordb-0.13.4/xplordb/sqlalchemy/ref/person.py`

 * *Files identical despite different names*

### Comparing `xplordb-0.13.3/xplordb.egg-info/PKG-INFO` & `xplordb-0.13.4/xplordb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplordb
-Version: 0.13.3
+Version: 0.13.4
 Summary: Python module to read/write data into xplordb database
 Home-page: https://gitlab.com/geolandia/openlog/xplordb
 Author: Oslandia
 Author-email: geology@oslandia.com
 License: AGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `xplordb-0.13.3/xplordb.egg-info/SOURCES.txt` & `xplordb-0.13.4/xplordb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,16 @@
 xplordb/schema/v/v.sql
 xplordb/schema/v/populate/missing_samples.sql
 xplordb/schema/v/populate/missing_surv.sql
 xplordb/schema/v/views/missing_samples.sql
 xplordb/schema/v/views/missing_surv.sql
 xplordb/sqlalchemy/__init__.py
 xplordb/sqlalchemy/base.py
+xplordb/sqlalchemy/assay/__init__.py
+xplordb/sqlalchemy/assay/structural_types.py
 xplordb/sqlalchemy/dh/__init__.py
 xplordb/sqlalchemy/dh/collar.py
 xplordb/sqlalchemy/dh/lith.py
 xplordb/sqlalchemy/dh/metadata.py
 xplordb/sqlalchemy/dh/survey.py
 xplordb/sqlalchemy/ref/__init__.py
 xplordb/sqlalchemy/ref/dataset.py
```

