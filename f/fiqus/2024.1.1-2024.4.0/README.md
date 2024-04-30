# Comparing `tmp/fiqus-2024.1.1.tar.gz` & `tmp/fiqus-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fiqus-2024.1.1.tar", last modified: Fri Jan 12 14:34:40 2024, max compression
+gzip compressed data, was "fiqus-2024.4.0.tar", last modified: Tue Apr 30 14:32:54 2024, max compression
```

## Comparing `fiqus-2024.1.1.tar` & `fiqus-2024.4.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.923901 fiqus-2024.1.1/
--rw-rw-rw-   0        0        0     2153 2024-01-12 14:34:40.922903 fiqus-2024.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1717 2023-12-19 17:11:08.000000 fiqus-2024.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.848103 fiqus-2024.1.1/fiqus/
--rw-rw-rw-   0        0        0    13700 2023-12-19 17:11:08.000000 fiqus-2024.1.1/fiqus/MainFiQuS.py
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.863064 fiqus-2024.1.1/fiqus/data/
--rw-rw-rw-   0        0        0     5946 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/data/DataFiQuS.py
--rw-rw-rw-   0        0        0     6747 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/data/DataFiQuSCCT.py
--rw-rw-rw-   0        0        0     2176 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/data/DataFiQuSMultipole.py
--rw-rw-rw-   0        0        0   157467 2023-12-19 17:11:08.000000 fiqus-2024.1.1/fiqus/data/DataFiQuSPancake3D.py
--rw-rw-rw-   0        0        0     2156 2023-01-25 10:04:12.000000 fiqus-2024.1.1/fiqus/data/DataMultipole.py
--rw-rw-rw-   0        0        0     7816 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     1499 2023-01-25 10:25:31.000000 fiqus-2024.1.1/fiqus/data/DataWindingsCCT.py
--rw-rw-rw-   0        0        0     6712 2023-11-30 16:40:37.000000 fiqus-2024.1.1/fiqus/data/RegionsModelFiQuS.py
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.867054 fiqus-2024.1.1/fiqus/geom_generators/
--rw-rw-rw-   0        0        0    49745 2023-01-25 10:25:31.000000 fiqus-2024.1.1/fiqus/geom_generators/GeometryCCT.py
--rw-rw-rw-   0        0        0    24171 2023-01-25 10:04:12.000000 fiqus-2024.1.1/fiqus/geom_generators/GeometryMultipole.py
--rw-rw-rw-   0        0        0   159511 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/geom_generators/GeometryPancake3D.py
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/geom_generators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.871043 fiqus-2024.1.1/fiqus/getdp_runners/
--rw-rw-rw-   0        0        0     3012 2023-01-25 10:25:31.000000 fiqus-2024.1.1/fiqus/getdp_runners/RunGetdpCCT.py
--rw-rw-rw-   0        0        0     4172 2023-01-25 10:29:07.000000 fiqus-2024.1.1/fiqus/getdp_runners/RunGetdpMultipole.py
--rw-rw-rw-   0        0        0     9744 2023-11-30 16:40:37.000000 fiqus-2024.1.1/fiqus/getdp_runners/RunGetdpPancake3D.py
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/getdp_runners/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.873037 fiqus-2024.1.1/fiqus/mains/
--rw-rw-rw-   0        0        0     4414 2023-01-25 10:25:31.000000 fiqus-2024.1.1/fiqus/mains/MainCCT.py
--rw-rw-rw-   0        0        0     5075 2023-01-25 10:04:12.000000 fiqus-2024.1.1/fiqus/mains/MainMultipole.py
--rw-rw-rw-   0        0        0     8728 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/mains/MainPancake3D.py
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/mains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.878025 fiqus-2024.1.1/fiqus/mesh_generators/
--rw-rw-rw-   0        0        0    11338 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/mesh_generators/MeshCCT.py
--rw-rw-rw-   0        0        0    14221 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/mesh_generators/MeshMultipole.py
--rw-rw-rw-   0        0        0   100203 2024-01-10 17:12:01.000000 fiqus-2024.1.1/fiqus/mesh_generators/MeshPancake3D.py
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/mesh_generators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.884007 fiqus-2024.1.1/fiqus/parsers/
--rw-rw-rw-   0        0        0      675 2023-01-25 10:04:12.000000 fiqus-2024.1.1/fiqus/parsers/ParserDAT.py
--rw-rw-rw-   0        0        0     8408 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/parsers/ParserGetDPOnSection.py
--rw-rw-rw-   0        0        0     5098 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/parsers/ParserGetDPTimeTable.py
--rw-rw-rw-   0        0        0     1912 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/parsers/ParserMSH.py
--rw-rw-rw-   0        0        0    10121 2023-01-25 10:04:12.000000 fiqus-2024.1.1/fiqus/parsers/ParserPOS.py
--rw-rw-rw-   0        0        0     5984 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/parsers/ParserRES.py
--rw-rw-rw-   0        0        0        0 2023-01-25 10:04:12.000000 fiqus-2024.1.1/fiqus/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.887000 fiqus-2024.1.1/fiqus/plotters/
--rw-rw-rw-   0        0        0     6333 2022-10-07 09:26:40.000000 fiqus-2024.1.1/fiqus/plotters/PlotPythonCCT.py
--rw-rw-rw-   0        0        0      481 2022-10-07 09:27:59.000000 fiqus-2024.1.1/fiqus/plotters/PlotPythonMultipole.py
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.889992 fiqus-2024.1.1/fiqus/post_processors/
--rw-rw-rw-   0        0        0    28443 2023-01-25 10:25:31.000000 fiqus-2024.1.1/fiqus/post_processors/PostProcessCCT.py
--rw-rw-rw-   0        0        0    15601 2023-01-25 10:04:12.000000 fiqus-2024.1.1/fiqus/post_processors/PostProcessMultipole.py
--rw-rw-rw-   0        0        0    12879 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/post_processors/PostProcessPancake3D.py
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/post_processors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.890989 fiqus-2024.1.1/fiqus/pre_processors/
--rw-rw-rw-   0        0        0     9217 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/pre_processors/PreProcessCCT.py
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/pre_processors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.892984 fiqus-2024.1.1/fiqus/pro_assemblers/
--rw-rw-rw-   0        0        0     2770 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/pro_assemblers/ProAssembler.py
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/pro_assemblers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.893981 fiqus-2024.1.1/fiqus/pro_material_functions/
--rw-rw-rw-   0        0        0    17835 2022-10-13 15:51:29.000000 fiqus-2024.1.1/fiqus/pro_material_functions/ironBHcurves.pro
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.897054 fiqus-2024.1.1/fiqus/pro_templates/
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/pro_templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.902957 fiqus-2024.1.1/fiqus/pro_templates/combined/
--rw-rw-rw-   0        0        0    13524 2022-10-17 14:17:45.000000 fiqus-2024.1.1/fiqus/pro_templates/combined/CCT_template.pro
--rw-rw-rw-   0        0        0     7956 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/pro_templates/combined/Multipole_template.pro
--rw-rw-rw-   0        0        0   121686 2023-11-30 16:40:37.000000 fiqus-2024.1.1/fiqus/pro_templates/combined/Pancake3D_template.pro
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/pro_templates/combined/__init__.py
--rw-rw-rw-   0        0        0     5525 2023-11-16 07:58:41.000000 fiqus-2024.1.1/fiqus/pro_templates/combined/materials.pro
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.902957 fiqus-2024.1.1/fiqus/pro_templates/separated/
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/pro_templates/separated/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.905950 fiqus-2024.1.1/fiqus/utils/
--rw-rw-rw-   0        0        0    18356 2023-12-19 17:11:08.000000 fiqus-2024.1.1/fiqus/utils/Utils.py
--rw-rw-rw-   0        0        0        0 2022-09-20 07:12:19.000000 fiqus-2024.1.1/fiqus/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.854092 fiqus-2024.1.1/fiqus.egg-info/
--rw-rw-rw-   0        0        0     2153 2024-01-12 14:34:39.000000 fiqus-2024.1.1/fiqus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2233 2024-01-12 14:34:39.000000 fiqus-2024.1.1/fiqus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-12 14:34:39.000000 fiqus-2024.1.1/fiqus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1005 2024-01-12 14:34:39.000000 fiqus-2024.1.1/fiqus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-01-12 14:34:39.000000 fiqus-2024.1.1/fiqus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-12 14:34:40.923901 fiqus-2024.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1594 2024-01-12 14:34:34.000000 fiqus-2024.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.915923 fiqus-2024.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-12-19 17:11:08.000000 fiqus-2024.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0    15537 2024-01-10 17:12:01.000000 fiqus-2024.1.1/tests/test_FiQuS.py
--rw-rw-rw-   0        0        0     1740 2023-11-16 07:58:42.000000 fiqus-2024.1.1/tests/test_geometry_generators.py
--rw-rw-rw-   0        0        0     1720 2023-11-16 07:58:42.000000 fiqus-2024.1.1/tests/test_mesh_generators.py
--rw-rw-rw-   0        0        0     2140 2023-11-16 07:58:42.000000 fiqus-2024.1.1/tests/test_solvers.py
-drwxrwxrwx   0        0        0        0 2024-01-12 14:34:40.921906 fiqus-2024.1.1/tests/utils/
--rw-rw-rw-   0        0        0        0 2023-12-19 17:11:08.000000 fiqus-2024.1.1/tests/utils/__init__.py
--rw-rw-rw-   0        0        0    24147 2023-11-16 07:58:42.000000 fiqus-2024.1.1/tests/utils/fiqus_test_classes.py
--rw-rw-rw-   0        0        0     4149 2022-09-20 07:12:19.000000 fiqus-2024.1.1/tests/utils/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.238603 fiqus-2024.4.0/
+-rw-rw-rw-   0        0        0     4607 2024-04-30 14:32:54.237604 fiqus-2024.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1719 2024-04-30 14:27:57.000000 fiqus-2024.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.152605 fiqus-2024.4.0/fiqus/
+-rw-rw-rw-   0        0        0    13700 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/MainFiQuS.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.167606 fiqus-2024.4.0/fiqus/data/
+-rw-rw-rw-   0        0        0     6396 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0     7287 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataFiQuSCCT.py
+-rw-rw-rw-   0        0        0     2403 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataFiQuSMultipole.py
+-rw-rw-rw-   0        0        0   109796 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataFiQuSPancake3D.py
+-rw-rw-rw-   0        0        0     2304 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataMultipole.py
+-rw-rw-rw-   0        0        0     9036 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     1709 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/DataWindingsCCT.py
+-rw-rw-rw-   0        0        0     7162 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/RegionsModelFiQuS.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.172604 fiqus-2024.4.0/fiqus/geom_generators/
+-rw-rw-rw-   0        0        0    49745 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/geom_generators/GeometryCCT.py
+-rw-rw-rw-   0        0        0    24171 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/geom_generators/GeometryMultipole.py
+-rw-rw-rw-   0        0        0   167791 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/geom_generators/GeometryPancake3D.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/geom_generators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.177604 fiqus-2024.4.0/fiqus/getdp_runners/
+-rw-rw-rw-   0        0        0     3012 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/getdp_runners/RunGetdpCCT.py
+-rw-rw-rw-   0        0        0     4172 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/getdp_runners/RunGetdpMultipole.py
+-rw-rw-rw-   0        0        0     9744 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/getdp_runners/RunGetdpPancake3D.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/getdp_runners/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.182604 fiqus-2024.4.0/fiqus/mains/
+-rw-rw-rw-   0        0        0     4414 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mains/MainCCT.py
+-rw-rw-rw-   0        0        0     5075 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mains/MainMultipole.py
+-rw-rw-rw-   0        0        0    21524 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mains/MainPancake3D.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.187604 fiqus-2024.4.0/fiqus/mesh_generators/
+-rw-rw-rw-   0        0        0    11338 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mesh_generators/MeshCCT.py
+-rw-rw-rw-   0        0        0    14221 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mesh_generators/MeshMultipole.py
+-rw-rw-rw-   0        0        0   120547 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mesh_generators/MeshPancake3D.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/mesh_generators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.194604 fiqus-2024.4.0/fiqus/parsers/
+-rw-rw-rw-   0        0        0      675 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/ParserDAT.py
+-rw-rw-rw-   0        0        0     8408 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/ParserGetDPOnSection.py
+-rw-rw-rw-   0        0        0     5098 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/ParserGetDPTimeTable.py
+-rw-rw-rw-   0        0        0     1912 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/ParserMSH.py
+-rw-rw-rw-   0        0        0    10121 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/ParserPOS.py
+-rw-rw-rw-   0        0        0     5984 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/ParserRES.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.197607 fiqus-2024.4.0/fiqus/plotters/
+-rw-rw-rw-   0        0        0     6333 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/plotters/PlotPythonCCT.py
+-rw-rw-rw-   0        0        0      481 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/plotters/PlotPythonMultipole.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.205606 fiqus-2024.4.0/fiqus/post_processors/
+-rw-rw-rw-   0        0        0    28443 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/post_processors/PostProcessCCT.py
+-rw-rw-rw-   0        0        0    15649 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/post_processors/PostProcessMultipole.py
+-rw-rw-rw-   0        0        0    13195 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/post_processors/PostProcessPancake3D.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/post_processors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.208603 fiqus-2024.4.0/fiqus/pre_processors/
+-rw-rw-rw-   0        0        0     9217 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pre_processors/PreProcessCCT.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pre_processors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.211604 fiqus-2024.4.0/fiqus/pro_assemblers/
+-rw-rw-rw-   0        0        0     2770 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_assemblers/ProAssembler.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_assemblers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.212603 fiqus-2024.4.0/fiqus/pro_material_functions/
+-rw-rw-rw-   0        0        0    17835 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_material_functions/ironBHcurves.pro
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.213606 fiqus-2024.4.0/fiqus/pro_templates/
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.220603 fiqus-2024.4.0/fiqus/pro_templates/combined/
+-rw-rw-rw-   0        0        0    13524 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/combined/CCT_template.pro
+-rw-rw-rw-   0        0        0     7956 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/combined/Multipole_template.pro
+-rw-rw-rw-   0        0        0   146175 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/combined/Pancake3D_template.pro
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/combined/__init__.py
+-rw-rw-rw-   0        0        0     5525 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/combined/materials.pro
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.221603 fiqus-2024.4.0/fiqus/pro_templates/separated/
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/pro_templates/separated/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.222603 fiqus-2024.4.0/fiqus/utils/
+-rw-rw-rw-   0        0        0    18489 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/utils/Utils.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/fiqus/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.156604 fiqus-2024.4.0/fiqus.egg-info/
+-rw-rw-rw-   0        0        0     4607 2024-04-30 14:32:53.000000 fiqus-2024.4.0/fiqus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2233 2024-04-30 14:32:53.000000 fiqus-2024.4.0/fiqus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 14:32:53.000000 fiqus-2024.4.0/fiqus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1003 2024-04-30 14:32:53.000000 fiqus-2024.4.0/fiqus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-30 14:32:53.000000 fiqus-2024.4.0/fiqus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 14:32:54.239604 fiqus-2024.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1595 2024-04-30 14:32:44.000000 fiqus-2024.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.228606 fiqus-2024.4.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:27:57.000000 fiqus-2024.4.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    15537 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/test_FiQuS.py
+-rw-rw-rw-   0        0        0     2034 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/test_geometry_generators.py
+-rw-rw-rw-   0        0        0     2112 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/test_mesh_generators.py
+-rw-rw-rw-   0        0        0     4224 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/test_solvers.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:32:54.231604 fiqus-2024.4.0/tests/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0    24891 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/utils/fiqus_test_classes.py
+-rw-rw-rw-   0        0        0     4149 2024-04-30 14:28:07.000000 fiqus-2024.4.0/tests/utils/helpers.py
```

### Comparing `fiqus-2024.1.1/PKG-INFO` & `fiqus-2024.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,18 @@
-Metadata-Version: 2.1
-Name: fiqus
-Version: 2024.1.1
-Summary: Source code for STEAM FiQuS tool
-Home-page: https://gitlab.cern.ch/steam/fiqus
-Author: STEAM Team
-Author-email: steam-team@cern.ch
-Keywords: STEAM,FiQuS,CERN
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: build
-
 ![FiQuS logo](https://gitlab.cern.ch/steam/fiqus/-/raw/master/docs/images/FiQuS_name_logo.svg)
 
 # Introduction
-Source code for STEAM **FiQuS** (**Fi**nite Element Method **Qu**ench **S**imulation) tool.
+Source code for STEAM **FiQuS** (**Fi**nite Element **Qu**ench **S**imulator).
 
 # Publications
 
+- S. Atalay et al, "An open-source 3D FE quench simulation tool for no-insulation HTS pancake coils", in Superconductor Science and Technology, doi: [10.1088/1361-6668/ad3f83](https://doi.org/10.1088/1361-6668/ad3f83)
 - A. Vitrano et al, "An Open-Source Finite Element Quench Simulation Tool for Superconducting Magnets," in IEEE Transactions on Applied Superconductivity, vol. 33, no. 5, pp. 1-6, Aug. 2023, Art no. 4702006, doi: [10.1109/TASC.2023.3259332](https://ieeexplore.ieee.org/abstract/document/10077402).
-
 - M. Wozniak et al, "Fast Quench Propagation Conductor for Protecting Canted Cos-Theta Magnets," in IEEE Transactions on Applied Superconductivity, vol. 33, no. 5, pp. 1-5, Aug. 2023, Art no. 4701705, doi: [10.1109/TASC.2023.3247997](https://ieeexplore.ieee.org/document/10050158).
 
-- S. Atalay et al, "An Open-Source 3D FE Quench Simulation Tool for No-Insulation HTS Pancake Coils", in arXiv:2311.09177, doi: [10.48550/arXiv.2311.09177](https://doi.org/10.48550/arXiv.2311.09177)
-
 # Folder Structure
 ![FiQuS folder structure](https://gitlab.cern.ch/steam/fiqus/-/raw/master/docs/images/FiQuS_folder_structure.svg)
 
 # Installation
 
 ## Released version:
 ```pip install fiqus```
@@ -47,8 +29,8 @@
 # Contact
 steam-team@cern.ch
 
 # STEAM User Agreement
 By using any software of the STEAM framework, users agree with this document:
 https://edms.cern.ch/document/2024516
 
-(Copyright Â© 2022, CERN, Switzerland. All rights reserved.)
+(Copyright © 2022, CERN, Switzerland. All rights reserved.)
```

### Comparing `fiqus-2024.1.1/fiqus/MainFiQuS.py` & `fiqus-2024.4.0/fiqus/MainFiQuS.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/data/DataFiQuS.py` & `fiqus-2024.4.0/fiqus/data/DataFiQuS.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,48 +7,48 @@
 
 
 class MonoFiQuS(BaseModel):
     """
         Rutherford cable type
     """
     type: Literal['Mono']
-    bare_cable_width: float = None
-    bare_cable_height_mean: float = None
+    bare_cable_width: Optional[float] = None
+    bare_cable_height_mean: Optional[float] = None
 
 
 class RibbonFiQuS(BaseModel):
     """
         Rutherford cable type
     """
     type: Literal['Ribbon']
-    bare_cable_width: float = None
-    bare_cable_height_mean: float = None
+    bare_cable_width: Optional[float] = None
+    bare_cable_height_mean: Optional[float] = None
 
 
 class RutherfordFiQuS(BaseModel):
     """
         Rutherford cable type
     """
     type: Literal['Rutherford']
-    bare_cable_width: float = None
-    bare_cable_height_mean: float = None
+    bare_cable_width: Optional[float] = None
+    bare_cable_height_mean: Optional[float] = None
 
 
 class ConductorFiQuS(BaseModel):
     """
         Class for conductor type
     """
     cable: Union[RutherfordFiQuS, RibbonFiQuS, MonoFiQuS] = {'type': 'Rutherford'}
 
 
 class GeneralSetting(BaseModel):
     """
         Class for general information on the case study
     """
-    I_ref: List[float] = None
+    I_ref: Optional[List[float]] = None
 
 
 class ModelDataSetting(BaseModel):
     """
         Class for model data
     """
     general_parameters: GeneralSetting = GeneralSetting()
@@ -72,97 +72,97 @@
 
 
 class RunFiQuS(BaseModel):
     """
         Class for FiQuS run
     """
     type: Literal["start_from_yaml", "mesh_only", "geometry_only", "geometry_and_mesh", "pre_process_only", "mesh_and_solve_with_post_process_python", "solve_with_post_process_python", "solve_only", "post_process_getdp_only", "post_process_python_only", "post_process"] = Field(default="start_from_yaml", title="Run Type of FiQuS", description="FiQuS allows you to run the model in different ways. The run type can be specified here. For example, you can just create the geometry and mesh or just solve the model with previous mesh, etc.")
-    geometry: Union[str, int] = Field(default=None, title="Geometry Folder Key", description="This key will be appended to the geometry folder.")
-    mesh: Union[str, int] = Field(default=None, title="Mesh Folder Key", description="This key will be appended to the mesh folder.")
-    solution: Union[str, int] = Field(default=None, title="Solution Folder Key", description="This key will be appended to the solution folder.")
+    geometry: Optional[Union[str, int]] = Field(default=None, title="Geometry Folder Key", description="This key will be appended to the geometry folder.")
+    mesh: Optional[Union[str, int]] = Field(default=None, title="Mesh Folder Key", description="This key will be appended to the mesh folder.")
+    solution: Optional[Union[str, int]] = Field(default=None, title="Solution Folder Key", description="This key will be appended to the solution folder.")
     launch_gui: bool = Field(default=True, title="Launch GUI", description="If True, the GUI will be launched after the run.")
     overwrite: bool = Field(default=False, title="Overwrite", description="If True, the existing folders will be overwritten, otherwise new folders will be created.")
     comments: str = Field(default="", title="Comments", description="Comments for the run. These comments will be saved in the run_log.csv file.")
 
 
 class GeneralFiQuS(BaseModel):
     """
         Class for FiQuS general
     """
-    magnet_name: str = None
+    magnet_name: Optional[str] = None
 
 
 class EnergyExtraction(BaseModel):
     """
         Level 3: Class for FiQuS
     """
-    t_trigger: float = None
-    R_EE: float = None
-    power_R_EE: float = None
-    L: float = None
-    C: float = None
+    t_trigger: Optional[float] = None
+    R_EE: Optional[float] = None
+    power_R_EE: Optional[float] = None
+    L: Optional[float] = None
+    C: Optional[float] = None
 
 
 class QuenchHeaters(BaseModel):
     """
         Level 3: Class for FiQuS
     """
-    N_strips: int = None
-    t_trigger: List[float] = None
-    U0: List[float] = None
-    C: List[float] = None
-    R_warm: List[float] = None
-    w: List[float] = None
-    h: List[float] = None
+    N_strips: Optional[int] = None
+    t_trigger: Optional[List[float]] = None
+    U0: Optional[List[float]] = None
+    C: Optional[List[float]] = None
+    R_warm: Optional[List[float]] = None
+    w: Optional[List[float]] = None
+    h: Optional[List[float]] = None
     h_ins: List[List[float]] = []
     type_ins: List[List[str]] = []
     h_ground_ins: List[List[float]] = []
     type_ground_ins: List[List[str]] = []
-    l: List[float] = None
-    l_copper: List[float] = None
-    l_stainless_steel: List[float] = None
-    ids: List[int] = None
-    turns: List[int] = None
-    turns_sides: List[str] = None
+    l: Optional[List[float]] = None
+    l_copper: Optional[List[float]] = None
+    l_stainless_steel: Optional[List[float]] = None
+    ids: Optional[List[int]] = None
+    turns: Optional[List[int]] = None
+    turns_sides: Optional[List[str]] = None
 
 
 class Cliq(BaseModel):
     """
         Level 3: Class for FiQuS
     """
-    t_trigger: float = None
-    current_direction: List[int] = None
-    sym_factor: int = None
-    N_units: int = None
-    U0: float = None
-    C: float = None
-    R: float = None
-    L: float = None
-    I0: float = None
+    t_trigger: Optional[float] = None
+    current_direction: Optional[List[int]] = None
+    sym_factor: Optional[int] = None
+    N_units: Optional[int] = None
+    U0: Optional[float] = None
+    C: Optional[float] = None
+    R: Optional[float] = None
+    L: Optional[float] = None
+    I0: Optional[float] = None
 
 
 class Circuit(BaseModel):
     """
         Level 2: Class for FiQuS
     """
-    R_circuit: float = None
-    L_circuit: float = None
-    R_parallel: float = None
+    R_circuit: Optional[float] = None
+    L_circuit: Optional[float] = None
+    R_parallel: Optional[float] = None
 
 
 class PowerSupply(BaseModel):
     """
         Level 2: Class for FiQuS
     """
-    I_initial: float = None
-    t_off: float = None
+    I_initial: Optional[float] = None
+    t_off: Optional[float] = None
     t_control_LUT: List[float] = Field(None, title="Time Values for Current Source", description="This list of time values will be matched with the current values in I_control_LUT, and then these (t, I) points will be connected with straight lines.")
     I_control_LUT: List[float] = Field(None, title="Current Values for Current Source" ,description="This list of current values will be matched with the time values in t_control_LUT, and then these (t, I) points will be connected with straight lines.")
-    R_crowbar: float = None
-    Ud_crowbar: float = None
+    R_crowbar: Optional[float] = None
+    Ud_crowbar: Optional[float] = None
 
 
 class QuenchProtection(BaseModel):
     """
         Level 2: Class for FiQuS
     """
     energy_extraction:  EnergyExtraction = EnergyExtraction()
```

### Comparing `fiqus-2024.1.1/fiqus/data/DataFiQuSCCT.py` & `fiqus-2024.4.0/fiqus/data/DataFiQuSCCT.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 from pydantic import BaseModel
-from typing import (List, Literal)
+from typing import (List, Literal, Optional)
 
 
 class Winding_gFiQuS(BaseModel):  # Geometry related windings _inputs
     """
         Level 2: Class for FiQuS CCT
     """
-    names: List[str] = None  # name to use in gmsh and getdp
-    r_wms: List[float] = None  # radius of the middle of the winding
-    n_turnss: List[float] = None  # number of turns
-    ndpts: List[int] = None  # number of divisions of turn, i.e. number of hexagonal elements for each turn
-    ndpt_ins: List[int] = None  # number of divisions of terminals in
-    ndpt_outs: List[int] = None  # number of divisions of terminals in
-    lps: List[float] = None  # layer pitch
-    alphas: List[float] = None  # tilt angle
-    wwws: List[float] = None  # winding wire widths (assuming rectangular)
-    wwhs: List[float] = None  # winding wire heights (assuming rectangular)
+    names: Optional[List[str]] = None  # name to use in gmsh and getdp
+    r_wms: Optional[List[float]] = None  # radius of the middle of the winding
+    n_turnss: Optional[List[float]] = None  # number of turns
+    ndpts: Optional[List[int]] = None  # number of divisions of turn, i.e. number of hexagonal elements for each turn
+    ndpt_ins: Optional[List[int]] = None  # number of divisions of terminals in
+    ndpt_outs: Optional[List[int]] = None  # number of divisions of terminals in
+    lps: Optional[List[float]] = None  # layer pitch
+    alphas: Optional[List[float]] = None  # tilt angle
+    wwws: Optional[List[float]] = None  # winding wire widths (assuming rectangular)
+    wwhs: Optional[List[float]] = None  # winding wire heights (assuming rectangular)
 
 
 class Winding_s(BaseModel):  # Solution time used windings _inputs (materials and BC)
     """
         Level 2: Class for FiQuS CCT
     """
-    currents: List[float] = None  # current in the wire
-    sigmas: List[float] = None  # electrical conductivity
-    mu_rs: List[float] = None  # relative permeability
+    currents: Optional[List[float]] = None  # current in the wire
+    sigmas: Optional[List[float]] = None  # electrical conductivity
+    mu_rs: Optional[List[float]] = None  # relative permeability
 
 
 class FQPL_g(BaseModel):  # Geometry related fqpls _inputs
     """
         Level 2: Class for FiQuS CCT
     """
     names: List[str] = []  # name to use in gmsh and getdp
-    fndpls: List[int] = None  # fqpl number of divisions per length
-    fwws: List[float] = None  # fqpl wire widths (assuming rectangular) for theta = 0 this is x dimension
-    fwhs: List[float] = None  # fqpl wire heights (assuming rectangular) for theta = 0 this is y dimension
-    r_ins: List[float] = None  # radiuses for inner diameter for fqpl (radial (or x direction for theta=0) for placing the fqpl
-    r_bs: List[float] = None  # radiuses for bending the fqpl by 180 degrees
-    n_sbs: List[int] = None  # number of 'bending segmetns' for the 180 degrees turn
-    thetas: List[float] = None  # rotation in deg from x+ axis towards y+ axis about z axis.
-    z_starts: List[str] = None  # which air boundary to start at. These is string with either: z_min or z_max key from the Air region.
-    z_ends: List[float] = None  # z coordinate of loop end
+    fndpls: Optional[List[int]] = None  # fqpl number of divisions per length
+    fwws: Optional[List[float]] = None  # fqpl wire widths (assuming rectangular) for theta = 0 this is x dimension
+    fwhs: Optional[List[float]] = None  # fqpl wire heights (assuming rectangular) for theta = 0 this is y dimension
+    r_ins: Optional[List[float]] = None  # radiuses for inner diameter for fqpl (radial (or x direction for theta=0) for placing the fqpl
+    r_bs: Optional[List[float]] = None  # radiuses for bending the fqpl by 180 degrees
+    n_sbs: Optional[List[int]] = None  # number of 'bending segmetns' for the 180 degrees turn
+    thetas: Optional[List[float]] = None  # rotation in deg from x+ axis towards y+ axis about z axis.
+    z_starts: Optional[List[str]] = None  # which air boundary to start at. These is string with either: z_min or z_max key from the Air region.
+    z_ends: Optional[List[float]] = None  # z coordinate of loop end
 
 
 class FQPL_s(BaseModel):  # Solution time used fqpls _inputs (materials and BC)
     """
         Level 2: Class for FiQuS CCT
     """
     currents: List[float] = []  # current in the wire
@@ -52,46 +52,46 @@
     mu_rs: List[float] = []  # relative permeability
 
 
 class Former_gFiQuS(BaseModel):  # Geometry related formers _inputs
     """
         Level 2: Class for FiQuS CCT
     """
-    names: List[str] = None  # name to use in gmsh and getdp
-    r_ins: List[float] = None  # inner radius
-    r_outs: List[float] = None  # outer radius
-    z_mins: List[float] = None  # extend of former  in negative z direction
-    z_maxs: List[float] = None  # extend of former in positive z direction
+    names: Optional[List[str]] = None  # name to use in gmsh and getdp
+    r_ins: Optional[List[float]] = None  # inner radius
+    r_outs: Optional[List[float]] = None  # outer radius
+    z_mins: Optional[List[float]] = None  # extend of former  in negative z direction
+    z_maxs: Optional[List[float]] = None  # extend of former in positive z direction
 
 
 class Former_s(BaseModel):  # Solution time used formers _inputs (materials and BC)
     """
         Level 2: Class for FiQuS CCT
     """
-    sigmas: List[float] = None  # electrical conductivity
-    mu_rs: List[float] = None  # relative permeability
+    sigmas: Optional[List[float]] = None  # electrical conductivity
+    mu_rs: Optional[List[float]] = None  # relative permeability
 
 
 class Air_g(BaseModel):  # Geometry related air_region _inputs
     """
         Level 2: Class for FiQuS CCT
     """
-    name: str = None  # name to use in gmsh and getdp
-    sh_type: str = None  # cylinder or cuboid are possible
-    ar: float = None  # if box type is cuboid a is taken as a dimension, if cylinder then r is taken
-    z_min: float = None  # extend of air region in negative z direction
-    z_max: float = None  # extend of air region in positive z direction
+    name: Optional[str] = None  # name to use in gmsh and getdp
+    sh_type: Optional[str] = None  # cylinder or cuboid are possible
+    ar: Optional[float] = None  # if box type is cuboid a is taken as a dimension, if cylinder then r is taken
+    z_min: Optional[float] = None  # extend of air region in negative z direction
+    z_max: Optional[float] = None  # extend of air region in positive z direction
 
 
 class Air_s(BaseModel):  # Solution time used air _inputs (materials and BC)
     """
         Level 2: Class for FiQuS CCT
     """
-    sigma: float = None  # electrical conductivity
-    mu_r: float = None  # relative permeability
+    sigma: Optional[float] = None  # electrical conductivity
+    mu_r: Optional[float] = None  # relative permeability
 
 
 class GeometryCCTFiQuS(BaseModel):
     """
         Level 2: Class for FiQuS CCT for FiQuS input
     """
     windings: Winding_gFiQuS = Winding_gFiQuS()
@@ -100,47 +100,47 @@
     air: Air_g = Air_g()
 
 
 class MeshCCT(BaseModel):
     """
         Level 2: Class for FiQuS CCT
     """
-    MaxAspectWindings: float = None  # used in transfinite mesh_generators settings to define mesh_generators size along two longer lines of hex elements of windings
-    ThresholdSizeMin: float = None  # sets field control of Threshold SizeMin
-    ThresholdSizeMax: float = None  # sets field control of Threshold SizeMax
-    ThresholdDistMin: float = None  # sets field control of Threshold DistMin
-    ThresholdDistMax: float = None  # sets field control of Threshold DistMax
+    MaxAspectWindings: Optional[float] = None  # used in transfinite mesh_generators settings to define mesh_generators size along two longer lines of hex elements of windings
+    ThresholdSizeMin: Optional[float] = None  # sets field control of Threshold SizeMin
+    ThresholdSizeMax: Optional[float] = None  # sets field control of Threshold SizeMax
+    ThresholdDistMin: Optional[float] = None  # sets field control of Threshold DistMin
+    ThresholdDistMax: Optional[float] = None  # sets field control of Threshold DistMax
 
 
 class SolveCCT(BaseModel):
     """
         Level 2: Class for FiQuS CCT
     """
     windings: Winding_s = Winding_s()  # windings solution time _inputs
     fqpls: FQPL_s = FQPL_s()  # fqpls solution time _inputs
     formers: Former_s = Former_s()  # former solution time _inputs
     air: Air_s = Air_s()  # air solution time _inputs
-    pro_template: str = None  # file name of .pro template file
-    variables: List[str] = None  # Name of variable to post-process by GetDP, like B for magnetic flux density
-    volumes: List[str] = None  # Name of volume to post-process by GetDP, line Winding_1
-    file_exts: List[str] = None  # Name of file extensions to post-process by GetDP, like .pos
+    pro_template: Optional[str] = None  # file name of .pro template file
+    variables: Optional[List[str]] = None  # Name of variable to post-process by GetDP, like B for magnetic flux density
+    volumes: Optional[List[str]] = None  # Name of volume to post-process by GetDP, line Winding_1
+    file_exts: Optional[List[str]] = None  # Name of file extensions to post-process by GetDP, like .pos
 
 
 class PostprocCCTFiQuS(BaseModel):
     """
         Class for FiQuS CCT input file
     """
-    windings_wwns: List[int] = None  # wires in width direction numbers
-    windings_whns: List[int] = None  # wires in height direction numbers
-    additional_outputs: List[str] = None  # Name of software specific input files to prepare, like :LEDET3D
-    winding_order: List[int] = None
-    fqpl_export_trim_tol: List[float] = None  # this multiplier times winding extend gives 'z' coordinate above(below) which hexes are exported for LEDET, length of this list must match number of fqpls
-    variables: List[str] = None  # Name of variable to post-process by python Gmsh API, like B for magnetic flux density
-    volumes: List[str] = None  # Name of volume to post-process by python Gmsh API, line Winding_1
-    file_exts: List[str] = None  # Name of file extensions o post-process by python Gmsh API, like .pos
+    windings_wwns: Optional[List[int]] = None  # wires in width direction numbers
+    windings_whns: Optional[List[int]] = None  # wires in height direction numbers
+    additional_outputs: Optional[List[str]] = None  # Name of software specific input files to prepare, like :LEDET3D
+    winding_order: Optional[List[int]] = None
+    fqpl_export_trim_tol: Optional[List[float]] = None  # this multiplier times winding extend gives 'z' coordinate above(below) which hexes are exported for LEDET, length of this list must match number of fqpls
+    variables: Optional[List[str]] = None  # Name of variable to post-process by python Gmsh API, like B for magnetic flux density
+    volumes: Optional[List[str]] = None  # Name of volume to post-process by python Gmsh API, line Winding_1
+    file_exts: Optional[List[str]] = None  # Name of file extensions o post-process by python Gmsh API, like .pos
 
 
 class CCTDM(BaseModel):
     """
         Level 1: Class for FiQuS CCT
     """
     type: Literal['CCT_straight'] = "CCT_straight"
```

### Comparing `fiqus-2024.1.1/fiqus/data/DataFiQuSPancake3D.py` & `fiqus-2024.4.0/fiqus/data/DataFiQuSPancake3D.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,533 @@
+from typing import Literal, Optional, Annotated
+from contextvars import ContextVar
+import logging
+import math
+import pathlib
+import scipy.integrate
+from functools import cached_property
 from pydantic import (
     BaseModel,
     PositiveFloat,
     NonNegativeFloat,
     PositiveInt,
     Field,
-    validator,
-    root_validator,
+    field_validator,
+    model_validator,
+    computed_field,
+    ValidationInfo,
 )
-from typing import List, Literal, Union, Optional
-import math
-import logging
-import os
-import csv
-import scipy
+import pandas as pd
+import numpy as np
 import matplotlib
+from annotated_types import Len
 
 logger = logging.getLogger(__name__)
 
+# ======================================================================================
+# Available materials: =================================================================
+NormalMaterialName = Literal[
+    "Copper", "Hastelloy", "Silver", "Indium", "Stainless Steel"
+]
+SuperconductingMaterialName = Literal["HTSSuperPower"]
+# ======================================================================================
+# ======================================================================================
 
 # ======================================================================================
-# FUNDAMENTAL CLASSES STARTS ===========================================================
+# Material information: ================================================================
+resistivityMacroNames = {
+    "Copper": "MATERIAL_Resistivity_Copper_T_B",
+    "Hastelloy": "MATERIAL_Resistivity_Hastelloy_T",
+    "Silver": "MATERIAL_Resistivity_Silver_T_B",
+    "Indium": "MATERIAL_Resistivity_Indium_T",
+    "Stainless Steel": "MATERIAL_Resistivity_SSteel_T",
+}
+thermalConductivityMacroNames = {
+    "Copper": "MATERIAL_ThermalConductivity_Copper_T_B",
+    "Hastelloy": "MATERIAL_ThermalConductivity_Hastelloy_T",
+    "Silver": "MATERIAL_ThermalConductivity_Silver_T",
+    "Indium": "MATERIAL_ThermalConductivity_Indium_T",
+    "Stainless Steel": "MATERIAL_ThermalConductivity_SSteel_T",
+}
+heatCapacityMacroNames = {
+    "Copper": "MATERIAL_SpecificHeatCapacity_Copper_T",
+    "Hastelloy": "MATERIAL_SpecificHeatCapacity_Hastelloy_T",
+    "Silver": "MATERIAL_SpecificHeatCapacity_Silver_T",
+    "Indium": "MATERIAL_SpecificHeatCapacity_Indium_T",
+    "Stainless Steel": "MATERIAL_SpecificHeatCapacity_SSteel_T",
+}
+getdpTSAOnlyResistivityFunctions = {
+    "Indium": "TSA_CFUN_rhoIn_T_constantThickness_fct_only",
+    "Stainless Steel": None,
+}
+getdpTSAMassResistivityFunctions = {
+    "Indium": "TSA_CFUN_rhoIn_T_constantThickness_mass",
+    "Stainless Steel": None,
+}
+getdpTSAStiffnessResistivityFunctions = {
+    "Indium": "TSA_CFUN_rhoIn_T_constantThickness_stiffness",
+    "Stainless Steel": None,
+}
+getdpTSAMassThermalConductivityFunctions = {
+    "Indium": "TSA_CFUN_kIn_constantThickness_mass",
+    "Stainless Steel": "TSA_CFUN_kSteel_T_constantThickness_mass",
+}
+getdpTSAStiffnessThermalConductivityFunctions = {
+    "Indium": "TSA_CFUN_kIn_constantThickness_stiffness",
+    "Stainless Steel": "TSA_CFUN_kSteel_T_constantThickness_stiffness",
+}
+getdpTSAMassHeatCapacityFunctions = {
+    "Indium": "TSA_CFUN_CvIn_constantThickness_mass",
+    "Stainless Steel": "TSA_CFUN_CvSteel_T_constantThickness_mass",
+}
+getdpTSARHSFunctions = {
+    "Indium": "TSA_CFUN_rhoIn_T_constantThickness_rhs",
+    "Stainless Steel": None,
+}
+getdpTSATripleFunctions = {
+    "Indium": "TSA_CFUN_rhoIn_T_constantThickness_triple",
+    "Stainless Steel": None,
+}
+getdpCriticalCurrentDensityFunctions = {
+    "HTSSuperPower": "CFUN_HTS_JcFit_SUPERPOWER_T_B_theta",
+}
+# ======================================================================================
 # ======================================================================================
-class Pancake3DPosition(BaseModel):
-    # 1) User inputs:
 
-    # Optionals:
+# ======================================================================================
+# Available quantities: ================================================================
+PositionRequiredQuantityName = Literal[
+    "magneticField",
+    "axialComponentOfTheMagneticField",
+    "magnitudeOfMagneticField",
+    "currentDensity",
+    "magnitudeOfCurrentDensity",
+    "resistiveHeating",
+    "temperature",
+    "criticalCurrentDensity",
+    "heatFlux",
+    "resistivity",
+    "thermalConductivity",
+    "specificHeatCapacity",
+    "jHTSOverjCritical",
+    "criticalCurrent",
+    "debug",
+]
+PositionNotRequiredQuantityName = Literal[
+    "currentThroughCoil",
+    "voltageBetweenTerminals",
+    "inductance",
+    "timeConstant",
+    "totalResistiveHeating",
+    "magneticEnergy",
+]
+# ======================================================================================
+# ======================================================================================
+
+# ======================================================================================
+# Quantity information: ================================================================
+EMQuantities = [
+    "magneticField",
+    "magnitudeOfMagneticField",
+    "currentDensity",
+    "magnitudeOfCurrentDensity",
+    "resistiveHeating",
+    "criticalCurrentDensity",
+    "resistivity",
+    "jHTSOverjCritical",
+    "criticalCurrent",
+    "debug",
+    "inductance",
+    "timeConstant",
+    "currentThroughCoil",
+    "voltageBetweenTerminals",
+    "totalResistiveHeating",
+    "magneticEnergy",
+]
+ThermalQuantities = [
+    "temperature",
+    "heatFlux",
+    "thermalConductivity",
+    "specificHeatCapacity",
+    "debug",
+]
+quantityProperNames = {
+    "axialComponentOfTheMagneticField": "Axila Component of the Magnetic Field",
+    "magneticField": "Magnetic Field",
+    "magnitudeOfMagenticField": "Magnitude of Magnetic Field",
+    "currentDensity": "Current Density",
+    "magnitudeOfCurrentDensity": "Magnitude of Current Density",
+    "resistiveHeating": "Resistive Heating",
+    "temperature": "Temperature",
+    "currentThroughCoil": "Current Through Coil",
+    "voltageBetweenTerminals": "Voltage Between Terminals",
+    "criticalCurrentDensity": "Critical Current Density",
+    "heatFlux": "Heat Flux",
+    "resistivity": "Resistivity",
+    "thermalConductivity": "Thermal Conductivity",
+    "specificHeatCapacity": "Specific Heat Capacity",
+    "jHTSOverjCritical": "jHTS/jCritical",
+    "criticalCurrent": "Critical Current",
+    "debug": "Debug",
+    "inductance": "Inductance",
+    "timeConstant": "Time Constant",
+}
+
+quantityUnits = {
+    "axialComponentOfTheMagneticField": "T",
+    "magneticField": "T",
+    "magnitudeOfMagneticField": "T",
+    "currentDensity": "$A/m^2$",
+    "magnitudeOfCurrentDensity": "$A/m^2$",
+    "resistiveHeating": "W",
+    "temperature": "K",
+    "currentThroughCoil": "A",
+    "voltageBetweenTerminals": "V",
+    "criticalCurrentDensity": "$A/m^2$",
+    "heatFlux": "$W/m^2$",
+    "resistivity": "Ohm*m",
+    "thermalConductivity": "W/m*K",
+    "specificHeatCapacity": "J/kg*K",
+    "jHTSOverjCritical": "A/A",
+    "criticalCurrent": "A",
+    "debug": "1",
+    "inductance": "H",
+    "timeConstant": "s",
+}
+
+getdpQuantityNames = {
+    "axialComponentOfTheMagneticField": "RESULT_axialComponentOfTheMagneticField",
+    "magneticField": "RESULT_magneticField",
+    "magnitudeOfMagneticField": "RESULT_magnitudeOfMagneticField",
+    "currentDensity": "RESULT_currentDensity",
+    "magnitudeOfCurrentDensity": "RESULT_magnitudeOfCurrentDensity",
+    "resistiveHeating": "RESULT_resistiveHeating",
+    "temperature": "RESULT_temperature",
+    "currentThroughCoil": "RESULT_currentThroughCoil",
+    "voltageBetweenTerminals": "RESULT_voltageBetweenTerminals",
+    "criticalCurrentDensity": "RESULT_criticalCurrentDensity",
+    "heatFlux": "RESULT_heatFlux",
+    "resistivity": "RESULT_resistivity",
+    "thermalConductivity": "RESULT_thermalConductivity",
+    "specificHeatCapacity": "RESULT_specificHeatCapacity",
+    "jHTSOverjCritical": "RESULT_jHTSOverjCritical",
+    "criticalCurrent": "RESULT_criticalCurrent",
+    "debug": "RESULT_debug",
+    "inductance": "RESULT_inductance",
+    "timeConstant": "RESULT_timeConstant",
+}
+
+getdpPostOperationNames = {
+    "axialComponentOfTheMagneticField": "POSTOP_axialComponentOfTheMagneticField",
+    "magneticField": "POSTOP_magneticField",
+    "magnitudeOfMagneticField": "POSTOP_magnitudeOfMagneticField",
+    "currentDensity": "POSTOP_currentDensity",
+    "magnitudeOfCurrentDensity": "POSTOP_magnitudeOfCurrentDensity",
+    "resistiveHeating": "POSTOP_resistiveHeating",
+    "temperature": "POSTOP_temperature",
+    "currentThroughCoil": "POSTOP_currentThroughCoil",
+    "voltageBetweenTerminals": "POSTOP_voltageBetweenTerminals",
+    "criticalCurrentDensity": "POSTOP_criticalCurrentDensity",
+    "heatFlux": "POSTOP_heatFlux",
+    "resistivity": "POSTOP_resistivity",
+    "thermalConductivity": "POSTOP_thermalConductivity",
+    "specificHeatCapacity": "POSTOP_specificHeatCapacity",
+    "jHTSOverjCritical": "POSTOP_jHTSOverjCritical",
+    "criticalCurrent": "POSTOP_criticalCurrent",
+    "debug": "POSTOP_debug",
+    "inductance": "POSTOP_inductance",
+    "timeConstant": "POSTOP_timeConstant",
+}
+
+# ======================================================================================
+# ======================================================================================
+
+# Global variables
+geometry_input = ContextVar("geometry")
+mesh_input = ContextVar("mesh")
+solve_input = ContextVar("solve")
+input_file_path = ContextVar("input_file_path")
+all_break_points = []
+
+
+def getWindingOuterRadius():
+    """Return outer radius of the winding."""
+    geometry = geometry_input.get()
+    return (
+        geometry["winding"]["innerRadius"]
+        + geometry["winding"]["thickness"]
+        + geometry["winding"]["numberOfTurns"]
+        * (geometry["winding"]["thickness"] + geometry["contactLayer"]["thickness"])
+    )
+
+
+def getAirHeight():
+    """Return the height of the air."""
+    geometry = geometry_input.get()
+    h = (
+        geometry["numberOfPancakes"]
+        * (geometry["winding"]["height"] + geometry["gapBetweenPancakes"])
+        - geometry["gapBetweenPancakes"]
+        + 2 * geometry["air"]["axialMargin"]
+    )
+    return h
+
+
+def getTransitionNotchAngle():
+    """Return transition notch angle of the winding."""
+    mesh = mesh_input.get()
+
+    azimuthalNumberOfElementsPerTurn = max(
+        mesh["winding"]["azimuthalNumberOfElementsPerTurn"]
+    )
+
+    transitionNotchAngle = 2 * math.pi / azimuthalNumberOfElementsPerTurn
+
+    return transitionNotchAngle
+
+
+def checkIfAirOrTerminalMeshIsStructured():
+    geometry = geometry_input.get()
+    mesh = mesh_input.get()
+
+    structuredAirMesh = False
+    structuredTerminalMesh = False
+    if "air" in mesh:
+        structuredAirMesh = mesh["air"]["structured"]
+    if "terminals" in mesh:
+        structuredTerminalMesh = mesh["terminals"]["structured"]
+    structuredMesh = structuredAirMesh or structuredTerminalMesh
+
+    return structuredMesh
+
+
+# ======================================================================================
+# FUNDAMENTAL CLASSES STARTS ===========================================================
+# ======================================================================================
+class Pancake3DPositionInCoordinates(BaseModel):
     x: float = Field(
-        default=None,
         title="x coordinate",
         description="x coordinate of the position.",
     )
     y: float = Field(
-        default=None,
         title="y coordinate",
         description="y coordinate of the position.",
     )
     z: float = Field(
-        default=None,
         title="z coordinate",
         description="z coordinate of the position.",
     )
-    turnNumber: PositiveFloat = Field(
-        default=None,
+
+
+class Pancake3DPositionInTurnNumbers(BaseModel):
+    turnNumber: float = Field(
         title="Turn Number",
-        description="Winding turn number as a position input.",
+        description=(
+            "Winding turn number as a position input. It starts from 0 and it can be a"
+            " float."
+        ),
     )
-    whichPancakeCoil: PositiveInt = Field(
+    whichPancakeCoil: Optional[PositiveInt] = Field(
         default=None,
         title="Pancake Coil Number",
         description="The first pancake coil is 1, the second is 2, etc.",
     )
 
+    @field_validator("turnNumber")
+    @classmethod
+    def check_turnNumber(cls, turnNumber):
+        geometry = geometry_input.get()
+
+        if turnNumber < 0:
+            raise ValueError("Turn number cannot be less than 0.")
+        elif turnNumber > geometry["winding"]["numberOfTurns"]:
+            raise ValueError(
+                "Turn number cannot be greater than the number of turns of the winding"
+                f" ({geometry['numberOfPancakes']})."
+            )
+
+        return turnNumber
+
+    @field_validator("whichPancakeCoil")
+    @classmethod
+    def check_whichPancakeCoil(cls, whichPancakeCoil):
+        geometry = geometry_input.get()
+
+        if whichPancakeCoil is not None:
+            if whichPancakeCoil < 1:
+                raise ValueError(
+                    "Pancake coil numbers start from 1. Therefore, it cannot be less"
+                    " than 1."
+                )
+            elif whichPancakeCoil > geometry["numberOfPancakes"]:
+                raise ValueError(
+                    "Pancake coil number cannot be greater than the number of pancakes"
+                    f" ({geometry['numberOfPancakes']})."
+                )
+        else:
+            return 1
+
+        return whichPancakeCoil
+
+    def compute_coordinates(self):
+        geometry = geometry_input.get()
+        mesh = mesh_input.get()
+
+        if geometry["contactLayer"]["thinShellApproximation"]:
+            windingThickness = (
+                geometry["winding"]["thickness"]
+                + geometry["contactLayer"]["thickness"]
+                * (geometry["winding"]["numberOfTurns"] - 1)
+                / geometry["winding"]["numberOfTurns"]
+            )
+            gapThickness = 0
+        else:
+            windingThickness = geometry["winding"]["thickness"]
+            gapThickness = geometry["contactLayer"]["thickness"]
+
+        innerRadius = geometry["winding"]["innerRadius"]
+        initialTheta = 0.0
+        if isinstance(mesh["winding"]["azimuthalNumberOfElementsPerTurn"], list):
+            ane = mesh["winding"]["azimuthalNumberOfElementsPerTurn"][0]
+        elif isinstance(mesh["winding"]["azimuthalNumberOfElementsPerTurn"], int):
+            ane = mesh["winding"]["azimuthalNumberOfElementsPerTurn"]
+        else:
+            raise ValueError(
+                "The azimuthal number of elements per turn must be either an integer"
+                " or a list of integers."
+            )
+
+        numberOfPancakes = geometry["numberOfPancakes"]
+        gapBetweenPancakes = geometry["gapBetweenPancakes"]
+        windingHeight = geometry["winding"]["height"]
+
+        turnNumber = self.turnNumber
+        whichPancake = self.whichPancakeCoil
+
+        elementStartTurnNumber = math.floor(turnNumber / (1 / ane)) * (1 / ane)
+        elementEndTurnNumber = elementStartTurnNumber + 1 / ane
+
+        class point:
+            def __init__(self, x, y, z):
+                self.x = x
+                self.y = y
+                self.z = z
+
+            def __add__(self, other):
+                return point(self.x + other.x, self.y + other.y, self.z + other.z)
+
+            def __sub__(self, other):
+                return point(self.x - other.x, self.y - other.y, self.z - other.z)
+
+            def __mul__(self, scalar):
+                return point(self.x * scalar, self.y * scalar, self.z * scalar)
+
+            def __truediv__(self, scalar):
+                return point(self.x / scalar, self.y / scalar, self.z / scalar)
+
+            def rotate(self, degrees):
+                return point(
+                    self.x * math.cos(degrees) - self.y * math.sin(degrees),
+                    self.x * math.sin(degrees) + self.y * math.cos(degrees),
+                    self.z,
+                )
+
+            def normalize(self):
+                return self / math.sqrt(self.x**2 + self.y**2 + self.z**2)
+
+        if whichPancake % 2 == 1:
+            # If the spiral is counter-clockwise, the initial theta angle decreases,
+            # and r increases as the theta angle decreases.
+            multiplier = 1
+        elif whichPancake % 2 == 0:
+            # If the spiral is clockwise, the initial theta angle increases, and r
+            # increases as the theta angle increases.
+            multiplier = -1
+
+        # Mesh element's starting point:
+        elementStartTheta = 2 * math.pi * elementStartTurnNumber * multiplier
+        elementStartRadius = (
+            innerRadius
+            + elementStartTheta
+            / (2 * math.pi)
+            * (gapThickness + windingThickness)
+            * multiplier
+        )
+        elementStartPointX = elementStartRadius * math.cos(
+            initialTheta + elementStartTheta
+        )
+        elementStartPointY = elementStartRadius * math.sin(
+            initialTheta + elementStartTheta
+        )
+        elementStartPointZ = (
+            -(
+                numberOfPancakes * windingHeight
+                + (numberOfPancakes - 1) * gapBetweenPancakes
+            )
+            / 2
+            + windingHeight / 2
+            + (whichPancake - 1) * (windingHeight + gapBetweenPancakes)
+        )
+        elementStartPoint = point(
+            elementStartPointX, elementStartPointY, elementStartPointZ
+        )
+
+        # Mesh element's ending point:
+        elementEndTheta = 2 * math.pi * elementEndTurnNumber * multiplier
+        elementEndRadius = (
+            innerRadius
+            + elementEndTheta
+            / (2 * math.pi)
+            * (gapThickness + windingThickness)
+            * multiplier
+        )
+        elementEndPointX = elementEndRadius * math.cos(initialTheta + elementEndTheta)
+        elementEndPointY = elementEndRadius * math.sin(initialTheta + elementEndTheta)
+        elementEndPointZ = elementStartPointZ
+        elementEndPoint = point(elementEndPointX, elementEndPointY, elementEndPointZ)
+
+        turnNumberFraction = (turnNumber - elementStartTurnNumber) / (
+            elementEndTurnNumber - elementStartTurnNumber
+        )
+        location = (
+            elementStartPoint
+            + (elementEndPoint - elementStartPoint) * turnNumberFraction
+        ) + (elementEndPoint - elementStartPoint).rotate(
+            -math.pi / 2
+        ).normalize() * windingThickness / 2 * multiplier
+
+        return location.x, location.y, location.z
+
+    @computed_field
+    @cached_property
+    def x(self) -> float:
+        return self.compute_coordinates()[0]
+
+    @computed_field
+    @cached_property
+    def y(self) -> float:
+        return self.compute_coordinates()[1]
+
+    @computed_field
+    @cached_property
+    def z(self) -> float:
+        return self.compute_coordinates()[2]
+
+
+Pancake3DPosition = Pancake3DPositionInCoordinates | Pancake3DPositionInTurnNumbers
 
 # ======================================================================================
 # FUNDAMENTAL CLASSES ENDS =============================================================
 # ======================================================================================
 
 
 # ======================================================================================
 # GEOMETRY CLASSES STARTS ==============================================================
 # ======================================================================================
-
-
 class Pancake3DGeometryWinding(BaseModel):
-    # 1) User inputs:
-
     # Mandatory:
     r_i: PositiveFloat = Field(
         alias="innerRadius",
         title="Inner Radius",
         description="Inner radius of the winding.",
     )
     t: PositiveFloat = Field(
@@ -93,88 +552,161 @@
         default="winding",
         title="Winding Name",
         description="The The name to be used in the mesh..",
         examples=["winding", "myWinding"],
     )
     NofVolPerTurn: int = Field(
         default=2,
+        validate_default=True,
         alias="numberOfVolumesPerTurn",
         ge=2,
         title="Number of Volumes Per Turn (Advanced Input)",
         description="The number of volumes per turn (CAD related, not physical).",
     )
-    theta_i: float = Field(
-        default=0.0,
-        alias="startAngle",
-        title="Start Angle",
-        description="The start angle of the first pancake coil in radians.",
-    )
 
-    # 2) To be calculated:
-    r_o: PositiveFloat = Field(
-        default=None,
-        alias="outerRadius",
-        description="outer radius of the winding (calculated by FiQuS)",
-    )
-    turnTol: PositiveFloat = Field(
-        default=None,
-        alias="turnTolerance",
-        description="turn tolerance (CAD related, not physical) (calculated by FiQuS)",
-    )
-    spt: PositiveFloat = Field(
-        default=None,
-        alias="sectionsPerTurn",
-        description=(
-            "sections per turn (CAD related, not physical) (calculated by FiQuS)"
-        ),
-    )
-    totalTapeLength: PositiveFloat = Field(
-        default=None,
-        description="total length of the winding (calculated by FiQuS)",
-    )
-
-    @validator("NofVolPerTurn", allow_reuse=True)
+    @field_validator("NofVolPerTurn")
     @classmethod
-    def check_NofVolPerTurn(cls, value):
-        """
-        Checks if the number of volumes per turn is greater than 2.
+    def check_NofVolPerTurn(cls, NofVolPerTurn):
+        geometry = geometry_input.get()
+        mesh = mesh_input.get()
+
+        # Check if the NofVolPerTurn is compatible swith the azimuthal number of
+        # elements per turn:
+        for i, ane in enumerate(mesh["winding"]["azimuthalNumberOfElementsPerTurn"]):
+            if ane % NofVolPerTurn != 0:
+                raise ValueError(
+                    "The azimuthal number of elements per turn for the pancake coil"
+                    f" number {i+1} is ({ane}), but it must be divisible by the number"
+                    f" of volumes per turn ({geometry['winding']['NofVolPerTurn']})!"
+                    " So it needs to be rounded to"
+                    f" {math.ceil(ane/NofVolPerTurn)*NofVolPerTurn:.5f} or"
+                    f" {math.floor(ane/NofVolPerTurn)*NofVolPerTurn:.5f}."
+                )
+
+        structured = checkIfAirOrTerminalMeshIsStructured()
+
+        if structured:
+            # If the mesh is structured, the number of volumes per turn must be 4:
+            NofVolPerTurn = 4
+
+        return NofVolPerTurn
+
+    @computed_field
+    @cached_property
+    def theta_i(self) -> float:
+        """Return start angle of the winding."""
+        return 0.0
+
+    @computed_field
+    @cached_property
+    def r_o(self) -> float:
+        """Return outer radius of the winding."""
+        return getWindingOuterRadius()
+
+    @computed_field
+    @cached_property
+    def turnTol(self) -> float:
+        """Return turn tolerance of the winding."""
+        geometry: Pancake3DGeometry = geometry_input.get()
+        mesh: Pancake3DMesh = mesh_input.get()
 
-        :param cls: class
-        :type cls: class
-        :param value: number of volumes per turn
-        :type value: int
-        :return: number of volumes per turn
-        :rtype: int
-        """
-        if value < 2:
-            raise ValueError("Number of volumes per turn must be greater than 2!")
+        # Calculate the turn tolerance required due to the geometrymetry input:
+        # Turn tolerance is the smallest turn angle (in turns) that is allowed.
+        if "dimTol" in geometry:
+            dimTol = geometry["dimTol"]
+        else:
+            dimTol = 1e-8
+        turnTol = geometry["winding"]["numberOfTurns"] % 1
+        if math.isclose(turnTol, 0, abs_tol=dimTol):
+            turnTol = 0.5
 
-        return value
+        turnTolDueToTransition = getTransitionNotchAngle() / (2 * math.pi)
 
-    @validator("N", allow_reuse=True)
-    @classmethod
-    def check_N(cls, value):
-        """
-        Checks if the number of turns is equal to or greater than 3.
+        # Calculate the minimum turn tolerance possible due to the mesh input:
+        minimumTurnTol = 1 / min(mesh["winding"]["azimuthalNumberOfElementsPerTurn"])
 
-        :param cls: class
-        :type cls: class
-        :param value: number of turns
-        :type value: float
-        :return: number of turns
-        :rtype: float
-        """
-        if value < 3:
-            raise ValueError("Number of turns must be equal to or greater than 3!")
-        return value
+        if turnTol < minimumTurnTol:
+            numberOfTurns = geometry["winding"]["numberOfTurns"]
 
+            raise ValueError(
+                "The azimuthal number of elements per turn for one of the pancakes is"
+                f" {min(mesh['winding']['azimuthalNumberOfElementsPerTurn'])}, and the"
+                " number of turns is"
+                f" {numberOfTurns:.5f}."
+                " The number of turns must always be divisible by the (1/(the"
+                " azimuthal number of elements per turn)) to ensure conformality."
+                " Please change the number of turns or the azimuthal number of"
+                " elemenets per turn. The closest possible number of turns value is"
+                f" {round(numberOfTurns * min(mesh['winding']['azimuthalNumberOfElementsPerTurn']))/min(mesh['winding']['azimuthalNumberOfElementsPerTurn']):.5f}"
+            )
+        else:
+            # Minimum possible sections per turn is 16 (otherwise splines might collide
+            # into each other). But it should be greater than the number of volumes per
+            # turn and it should be divisible by both 1/turnTol and the number of
+            # volumes per turn.
+            sectionsPerTurn = 16
+            if "numberOfVolumesPerTurn" in geometry["winding"]:
+                numberOfVolumesPerTurn = geometry["winding"]["numberOfVolumesPerTurn"]
+            else:
+                numberOfVolumesPerTurn = 2
 
-class Pancake3DGeometryContactLayer(BaseModel):
-    # 1) User inputs:
+            while (
+                (
+                    math.fmod(sectionsPerTurn, (1 / turnTol)) > 1e-8
+                    and math.fmod(sectionsPerTurn, (1 / turnTol)) - (1 / turnTol)
+                    < -1e-8
+                )
+                or (
+                    math.fmod(sectionsPerTurn, (1 / turnTolDueToTransition)) > 1e-8
+                    and math.fmod(sectionsPerTurn, (1 / turnTolDueToTransition))
+                    - (1 / turnTolDueToTransition)
+                    < -1e-8
+                )
+                or sectionsPerTurn % numberOfVolumesPerTurn != 0
+                or sectionsPerTurn < numberOfVolumesPerTurn
+            ):
+                sectionsPerTurn += 1
+
+            # Sections per turn will set the turn tolerance value as well.
+            return 1.0 / sectionsPerTurn
 
+    @computed_field
+    @cached_property
+    def spt(self) -> float:
+        """Return sections per turn of the winding."""
+        return int(1.0 / self.turnTol)
+
+    @computed_field
+    @cached_property
+    def totalTapeLength(self) -> float:
+        """Return total tape length of the winding."""
+        geometry: Pancake3DGeometry = geometry_input.get()
+
+        # Calculate the total tape length of the coil:
+
+        # The same angle can be subtracted from both theta_1 and theta_2 to simplify the
+        # calculations:
+        theta2 = geometry["winding"]["numberOfTurns"] * 2 * math.pi
+        theta1 = 0
+
+        # Since r = a * theta + b, r_1 = b since theta_1 = 0:
+        b = geometry["winding"]["innerRadius"]
+
+        # Since r = a * theta + b, r_2 = a * theta2 + b:
+        a = (getWindingOuterRadius() - b) / theta2
+
+        def integrand(t):
+            return math.sqrt(a**2 + (a * t + b) ** 2)
+
+        totalTapeLength = abs(scipy.integrate.quad(integrand, theta1, theta2)[0])
+
+        return totalTapeLength
+
+
+class Pancake3DGeometryContactLayer(BaseModel):
     # Mandatory:
     tsa: bool = Field(
         alias="thinShellApproximation",
         title="Use Thin Shell Approximation",
         description=(
             "If True, the contact layer will be modeled with 2D shell elements (thin"
             " shell approximation), and if False, the contact layer will be modeled"
@@ -192,70 +724,99 @@
         default="contactLayer",
         title="Contact Layer Name",
         description="The name to be used in the mesh.",
         examples=["myContactLayer"],
     )
 
 
-class Pancake3DGeometryTerminal(BaseModel):
-    # 1) User inputs:
-
+class Pancake3DGeometryTerminalBase(BaseModel):
     # Mandatory:
-    name: str = Field(
-        title="Terminal Name",
-        description="The name to be used in the mesh.",
-        examples=["innerTerminal", "outerTeminal"],
-    )
     t: PositiveFloat = Field(
         alias="thickness",
         title="Terminal Thickness",
         description="Thickness of the terminal's tube.",
     )  # thickness
 
-    # 2) To be calculated:
-    r: PositiveFloat = Field(
-        default=None,
-        alias="radius",
-        description=(
-            "inner radius of the inner terminal or outer radius of the outer terminal"
-            " (calculated by FiQuS)"
-        ),
+    @field_validator("t")
+    @classmethod
+    def check_t(cls, t):
+        geometry = geometry_input.get()
+
+        if t < geometry["winding"]["thickness"] / 2:
+            raise ValueError(
+                "Terminal's thickness is smaller than half of the winding's thickness!"
+                " Please increase the terminal's thickness."
+            )
+
+        return t
+
+
+class Pancake3DGeometryInnerTerminal(Pancake3DGeometryTerminalBase):
+    name: str = Field(
+        default="innerTerminal",
+        title="Terminal Name",
+        description="The name to be used in the mesh.",
+        examples=["innerTerminal", "outerTeminal"],
     )
 
+    @computed_field
+    @cached_property
+    def r(self) -> float:
+        """Return inner radius of the inner terminal."""
+        geometry = geometry_input.get()
+
+        innerRadius = geometry["winding"]["innerRadius"] - 2 * self.t
+        if innerRadius < 0:
+            raise ValueError(
+                "Inner terminal's radius is smaller than 0! Please decrease the inner"
+                " terminal's thickness or increase the winding's inner radius."
+            )
+
+        return innerRadius
+
+
+class Pancake3DGeometryOuterTerminal(Pancake3DGeometryTerminalBase):
+    name: str = Field(
+        default="outerTerminal",
+        title="Terminal Name",
+        description="The name to be used in the mesh.",
+        examples=["innerTerminal", "outerTeminal"],
+    )
+
+    @computed_field
+    @cached_property
+    def r(self) -> float:
+        """Return outer radius of the outer terminal."""
+        outerRadius = getWindingOuterRadius() + 2 * self.t
+
+        return outerRadius
+
 
 class Pancake3DGeometryTerminals(BaseModel):
     # 1) User inputs:
-    i: Pancake3DGeometryTerminal = Field(alias="inner")
-    o: Pancake3DGeometryTerminal = Field(alias="outer")
+    i: Pancake3DGeometryInnerTerminal = Field(alias="inner")
+    o: Pancake3DGeometryOuterTerminal = Field(alias="outer")
 
     # Optionals:
     firstName: str = Field(
         default="firstTerminal", description="name of the first terminal"
     )
     lastName: str = Field(
         default="lastTerminal", description="name of the last terminal"
     )
 
+    @computed_field
+    @cached_property
+    def transitionNotchAngle(self) -> float:
+        """Return transition notch angle of the terminals."""
+        return getTransitionNotchAngle()
 
-class Pancake3DGeometryAir(BaseModel):
-    # 1) User inputs:
 
+class Pancake3DGeometryAirBase(BaseModel):
     # Mandatory:
-    r: PositiveFloat = Field(
-        default=None,
-        alias="radius",
-        title="Air Radius",
-        description="Radius of the air (for cylinder type air).",
-    )
-    a: PositiveFloat = Field(
-        default=None,
-        alias="sideLength",
-        title="Air Side Length",
-        description="Side length of the air (for cuboid type air).",
-    )
     margin: PositiveFloat = Field(
         alias="axialMargin",
         title="Axial Margin of the Air",
         description=(
             "Axial margin between the ends of the air and first/last pancake coils."
         ),
     )  # axial margin
@@ -263,31 +824,26 @@
     # Optionals:
     name: str = Field(
         default="air",
         title="Air Name",
         description="The name to be used in the mesh.",
         examples=["air", "myAir"],
     )
-    type: Literal["cylinder", "cuboid"] = Field(
-        default="cylinder",
-        title="Air Type",
-        description="Air can be a cylinder or cuboid.",
-    )
     shellTransformation: bool = Field(
         default=False,
         alias="shellTransformation",
         title="Use Shell Transformation",
         description=(
             "Generate outer shell air to apply shell transformation if True (GetDP"
             " related, not physical)"
         ),
     )
     shellTransformationMultiplier: float = Field(
         default=1.2,
-        gt=1,
+        gt=1.1,
         alias="shellTransformationMultiplier",
         title="Shell Transformation Multiplier (Advanced Input)",
         description=(
             "multiply the air's outer dimension by this value to get the shell's outer"
             " dimension"
         ),
     )
@@ -309,175 +865,271 @@
         title="Generate Gap Air with Fragment (Advanced Input)",
         description=(
             "generate the gap air with gmsh/model/occ/fragment if true (CAD related,"
             " not physical)"
         ),
     )
 
-    # 2) To be calculated:
-    h: PositiveFloat = Field(
-        default=None,
-        alias="height",
-        description="total height of the air (calculated by FiQuS)",
-    )
-    shellOuterRadius: PositiveFloat = Field(
-        default=None,
-        description="outer radius of the cylinder shell (calculated by FiQuS)",
-    )
-    shellSideLength: PositiveFloat = Field(
+    @field_validator("margin")
+    @classmethod
+    def check_margin(cls, margin):
+        geometry = geometry_input.get()
+        windingHeight = geometry["winding"]["height"]
+
+        if margin < windingHeight / 2:
+            raise ValueError(
+                "Axial margin is smaller than half of the winding's height! Please"
+                " increase the axial margin."
+            )
+
+        return margin
+
+    @computed_field
+    @cached_property
+    def h(self) -> float:
+        """Return total height of the air."""
+        h = getAirHeight()
+
+        return h
+
+
+class Pancake3DGeometryAirCylinder(Pancake3DGeometryAirBase):
+    type: Literal["cylinder"] = Field(default="cylinder", title="Air Type")
+    r: PositiveFloat = Field(
         default=None,
-        description="side length of the cuboid shell (calculated by FiQuS)",
+        alias="radius",
+        title="Air Radius",
+        description="Radius of the air (for cylinder type air).",
     )
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
+    @field_validator("r")
     @classmethod
-    def check_and_calculate_air(cls, values):
-        """
-        Checks if the radius or side length is specified for the air.
+    def check_r(cls, r):
+        geometry = geometry_input.get()
+        outerTerminalOuterRadius = (
+            getWindingOuterRadius() + 2 * geometry["terminals"]["outer"]["thickness"]
+        )
 
-        :param cls: class
-        :type cls: class
-        :param values: dictionary of air
-        :type values: dict
-        :return: dictionary of air
-        :rtype: dict
-        """
+        if r < outerTerminalOuterRadius * 1.5:
+            raise ValueError(
+                "Radius of the air must be at least 1.5 times the outer radius of the"
+                " winding! Please increase the radius of the air."
+            )
 
-        # If type is cylinder r must be specified, otherwise a must be specified:
-        if values["type"] == "cylinder":
-            if values["r"] is None:
-                raise ValueError("Radius must be specified for air!")
+        return r
 
-        elif values["type"] == "cuboid":
-            if values["a"] is None:
-                raise ValueError("Side length must be specified for air!")
+    @computed_field
+    @cached_property
+    def shellOuterRadius(self) -> float:
+        """Return outer radius of the air."""
+        shellOuterRadius = self.shellTransformationMultiplier * self.r
 
-        # Calculate shell transformation
-        if values["shellTransformation"]:
-            if values["type"] == "cylinder":
-                values["shellOuterRadius"] = (
-                    values["shellTransformationMultiplier"] * values["r"]
-                )
-            elif values["type"] == "cuboid":
-                values["shellSideLength"] = (
-                    values["shellTransformationMultiplier"] * values["a"]
-                )
+        return shellOuterRadius
 
-        return values
 
-    @validator("shellTransformationMultiplier", allow_reuse=True)
+class Pancake3DGeometryAirCuboid(Pancake3DGeometryAirBase):
+    type: Literal["cuboid"] = Field(default="cuboid", title="Air Type")
+    a: PositiveFloat = Field(
+        default=None,
+        alias="sideLength",
+        title="Air Side Length",
+        description="Side length of the air (for cuboid type air).",
+    )
+
+    @field_validator("a")
     @classmethod
-    def check_shellTransformationMultiplier(cls, value):
-        """
-        Checks if the shell transformation multiplier is greater than 1.
+    def check_a(cls, a):
+        geometry = geometry_input.get()
+        outerTerminalOuterRadius = (
+            getWindingOuterRadius() + 2 * geometry["terminals"]["outer"]["thickness"]
+        )
 
-        :param cls: class
-        :type cls: class
-        :param value: shell transformation multiplier
-        :type value: float
-        :return: shell transformation multiplier
-        :rtype: float
-        """
+        if a / 2 < outerTerminalOuterRadius * 1.5:
+            raise ValueError(
+                "Half of the side length of the air must be at least 1.5 times the"
+                " outer radius of the winding! Please increase the side length of the"
+                " air."
+            )
 
-        if value <= 1:
-            raise ValueError("Shell transformation multiplier must be greater than 1!")
+        return a
 
-        return value
+    @computed_field
+    @cached_property
+    def shellSideLength(self) -> float:
+        """Return outer radius of the air."""
+        shellSideLength = self.shellTransformationMultiplier * self.a
+
+        return shellSideLength
 
 
+Pancake3DGeometryAir = Annotated[
+    Pancake3DGeometryAirCylinder | Pancake3DGeometryAirCuboid,
+    Field(discriminator="type"),
+]
 # ======================================================================================
 # GEOMETRY CLASSES ENDS ================================================================
 # ======================================================================================
 
 
 # ======================================================================================
 # MESH CLASSES STARTS ==================================================================
 # ======================================================================================
 class Pancake3DMeshWinding(BaseModel):
-    # 1) User inputs:
-
     # Mandatory:
-    axne: Union[List[PositiveInt], PositiveInt] = Field(
+    axne: list[PositiveInt] | PositiveInt = Field(
         alias="axialNumberOfElements",
         title="Axial Number of Elements",
         description=(
             "The number of axial elements for the whole height of the coil. It can be"
             " either a list of integers to specify the value for each pancake coil"
             " separately or an integer to use the same setting for each pancake coil."
         ),
     )
 
-    ane: Union[List[PositiveInt], PositiveInt] = Field(
+    ane: list[PositiveInt] | PositiveInt = Field(
         alias="azimuthalNumberOfElementsPerTurn",
         title="Azimuthal Number of Elements Per Turn",
         description=(
             "The number of azimuthal elements per turn of the coil. It can be either a"
             " list of integers to specify the value for each pancake coil separately or"
             " an integer to use the same setting for each pancake coil."
         ),
     )
 
-    rne: Union[List[PositiveInt], PositiveInt] = Field(
+    rne: list[PositiveInt] | PositiveInt = Field(
         alias="radialNumberOfElementsPerTurn",
         title="Winding Radial Number of Elements Per Turn",
         description=(
             "The number of radial elements per tape of the winding. It can be either a"
             " list of integers to specify the value for each pancake coil separately or"
             " an integer to use the same setting for each pancake coil."
         ),
     )
 
     # Optionals:
-    axbc: Union[List[PositiveFloat], PositiveFloat] = Field(
+    axbc: list[PositiveFloat] | PositiveFloat = Field(
         default=[1],
         alias="axialDistributionCoefficient",
         title="Axial Bump Coefficients",
         description=(
             "If 1, it won't affect anything. If smaller than 1, elements will get finer"
             " in the axial direction at the ends of the coil. If greater than 1,"
             " elements will get coarser in the axial direction at the ends of the coil."
             " It can be either a list of floats to specify the value for each pancake"
             " coil separately or a float to use the same setting for each pancake coil."
         ),
     )
 
-    elementType: Union[
-        List[Literal["tetrahedron", "hexahedron", "prism"]],
-        Literal["tetrahedron", "hexahedron", "prism"],
-    ] = Field(
+    elementType: (
+        list[Literal["tetrahedron", "hexahedron", "prism"]]
+        | Literal["tetrahedron", "hexahedron", "prism"]
+    ) = Field(
         default=["tetrahedron"],
         title="Element Type",
         description=(
             "The element type of windings and contact layers. It can be either a"
             " tetrahedron, hexahedron, or a prism. It can be either a list of strings"
             " to specify the value for each pancake coil separately or a string to use"
             " the same setting for each pancake coil."
         ),
     )
 
+    @field_validator("axne", "ane", "rne", "axbc", "elementType")
+    @classmethod
+    def check_inputs(cls, value, info: ValidationInfo):
+        geometry = geometry_input.get()
 
-class Pancake3DMeshContactLayer(BaseModel):
-    # 1) User inputs:
+        numberOfPancakes = geometry["numberOfPancakes"]
 
-    # Mandatory:
+        structuredMesh = checkIfAirOrTerminalMeshIsStructured()
+
+        if not isinstance(value, list):
+            value = [value] * numberOfPancakes
+        elif len(value) == 1:
+            value = value * numberOfPancakes
+        else:
+            if len(value) != numberOfPancakes:
+                raise ValueError(
+                    "The length of the input list must be equal to the number of"
+                    " pancake coils!"
+                )
+        if info.field_name == "ane":
+            if value[0] < 7:
+                raise ValueError(
+                    "Azimuthal number of elements per turn must be greater than or"
+                    " equal to 7!"
+                )
+
+        if structuredMesh:
+            if len(set(value)) != 1:
+                raise ValueError(
+                    "If structured mesh is used, the same mesh setting must be used for"
+                    " all pancake coils!"
+                )
 
-    rne: List[PositiveInt] = Field(
+            if info.field_name == "elementType":
+                if value[0] != "tetrahedron":
+                    raise ValueError(
+                        "If structured air or terminal mesh is used, the element type"
+                        " must be tetrahedron!"
+                    )
+
+            if info.field_name == "ane":
+                if value[0] % 4 != 0:
+                    raise ValueError(
+                        "If structured mesh is used, the number of azimuthal elements"
+                        " per turn must be divisible by 4!"
+                    )
+
+        return value
+
+
+class Pancake3DMeshContactLayer(BaseModel):
+    # Mandatory:
+    rne: list[PositiveInt] = Field(
         alias="radialNumberOfElementsPerTurn",
         title="Contact Layer Radial Number of Elements Per Turn",
         description=(
             "The number of radial elements per tape of the contact layer. It can be"
             " either a list of integers to specify the value for each pancake coil"
             " separately or an integer to use the same setting for each pancake coil."
         ),
     )
 
+    @field_validator("rne")
+    @classmethod
+    def check_inputs(cls, value):
+        geometry = geometry_input.get()
+
+        structuredMesh = checkIfAirOrTerminalMeshIsStructured()
+
+        numberOfPancakeCoils = geometry["numberOfPancakes"]
+
+        if not isinstance(value, list):
+            value = [value] * numberOfPancakeCoils
+        elif len(value) == 1:
+            value = value * numberOfPancakeCoils
+        else:
+            if len(value) != numberOfPancakeCoils:
+                raise ValueError(
+                    "The length of the input list must be equal to the number of"
+                    " pancake coils!"
+                )
+
+        if structuredMesh:
+            if len(set(value)) != 1:
+                raise ValueError(
+                    "If structured mesh is used, the same mesh setting must be used for"
+                    " all pancake coils!"
+                )
+
+        return value
 
-class Pancake3DMeshAirAndTerminals(BaseModel):
-    # 1) User inputs:
 
+class Pancake3DMeshAirAndTerminals(BaseModel):
     # Optionals:
     structured: bool = Field(
         default=False,
         title="Structure Mesh",
         description=(
             "If True, the mesh will be structured. If False, the mesh will be"
             " unstructured."
@@ -493,49 +1145,178 @@
     )
 
 
 # ======================================================================================
 # MESH CLASSES ENDS ====================================================================
 # ======================================================================================
 
+
 # ======================================================================================
 # SOLVE CLASSES STARTS =================================================================
 # ======================================================================================
-
-
 class Pancake3DSolveAir(BaseModel):
     # 1) User inputs:
 
     # Mandatory:
     permeability: PositiveFloat = Field(
         title="Permeability of Air",
         description="Permeability of air.",
     )
 
 
 class Pancake3DSolveIcVsLength(BaseModel):
-    lengthValues: List[float] = Field(
+    lengthValues: list[float] = Field(
         title="Tape Length Values",
         description="Tape length values that corresponds to criticalCurrentValues.",
     )
-    criticalCurrentValues: List[float] = Field(
+    criticalCurrentValues: list[float] = Field(
         title="Critical Current Values",
         description="Critical current values that corresponds to lengthValues.",
     )
 
 
-class Pancake3DSolveCERNSuperConductorMaterial(BaseModel):
-    # 1) User inputs:
+class Pancake3DSolveMaterialBase(BaseModel):
+    name: str
+
+    # Optionals:
+    rrr: PositiveFloat = Field(
+        default=100,
+        alias="residualResistanceRatio",
+        title="Residual Resistance Ratio",
+        description=(
+            "Residual-resistivity ratio (also known as Residual-resistance ratio or"
+            " just RRR) is the ratio of the resistivity of a material at reference"
+            " temperature and at 0 K."
+        ),
+    )
+    rrrRefT: PositiveFloat = Field(
+        default=295,
+        alias="residualResistanceRatioReferenceTemperature",
+        title="Residual Resistance Ratio Reference Temperature",
+        description="Reference temperature for residual resistance ratio",
+    )
+
+    @computed_field
+    @cached_property
+    def resistivityMacroName(self) -> str:
+        """Return the resistivity macro name of the material."""
+        if self.name not in resistivityMacroNames:
+            return "NOT_DEFINED_IN_DATA_FIQUS_PANCAKE3D"
+
+        return resistivityMacroNames[self.name]
+
+    @computed_field
+    @cached_property
+    def thermalConductivityMacroName(self) -> str:
+        """Return the thermal conductivity macro name of the material."""
+        if self.name not in thermalConductivityMacroNames:
+            return "NOT_DEFINED_IN_DATA_FIQUS_PANCAKE3D"
+
+        return thermalConductivityMacroNames[self.name]
+
+    @computed_field
+    @cached_property
+    def heatCapacityMacroName(self) -> str:
+        """Return the heat capacity macro name of the material."""
+        if self.name not in heatCapacityMacroNames:
+            return "NOT_DEFINED_IN_DATA_FIQUS_PANCAKE3D"
+
+        return heatCapacityMacroNames[self.name]
+
+    @computed_field
+    @cached_property
+    def getdpTSAOnlyResistivityFunction(self) -> str:
+        """Return the GetDP function name of the material's resistivity."""
+        if self.name not in getdpTSAOnlyResistivityFunctions:
+            return "NOT_DEFINED_IN_DATA_FIQUS_PANCAKE3D"
+
+        return getdpTSAOnlyResistivityFunctions[self.name]
+
+    @computed_field
+    @cached_property
+    def getdpTSAMassResistivityFunction(self) -> str:
+        """Return the GetDP function name of the material's mass resistivity."""
+        if self.name not in getdpTSAMassResistivityFunctions:
+            return "NOT_DEFINED_IN_DATA_FIQUS_PANCAKE3D"
+
+        return getdpTSAMassResistivityFunctions[self.name]
+
+    @computed_field
+    @cached_property
+    def getdpTSAStiffnessResistivityFunction(self) -> str:
+        """Return the GetDP function name of the material's stiffness resistivity."""
+        if self.name not in getdpTSAStiffnessResistivityFunctions:
+            return "NOT_DEFINED_IN_DATA_FIQUS_PANCAKE3D"
+
+        return getdpTSAStiffnessResistivityFunctions[self.name]
+
+    @computed_field
+    @cached_property
+    def getdpTSAMassThermalConductivityFunction(self) -> str:
+        """Return the GetDP function name of the material's mass thermal conductivity."""
+        if self.name not in getdpTSAMassThermalConductivityFunctions:
+            return "NOT_DEFINED_IN_DATA_FIQUS_PANCAKE3D"
+
+        return getdpTSAMassThermalConductivityFunctions[self.name]
+
+    @computed_field
+    @cached_property
+    def getdpTSAStiffnessThermalConductivityFunction(self) -> str:
+        """Return the GetDP function name of the material's stiffness thermal conductivity."""
+        if self.name not in getdpTSAStiffnessThermalConductivityFunctions:
+            return "NOT_DEFINED_IN_DATA_FIQUS_PANCAKE3D"
+
+        return getdpTSAStiffnessThermalConductivityFunctions[self.name]
+
+    @computed_field
+    @cached_property
+    def getdpTSAMassHeatCapacityFunction(self) -> str:
+        """Return the GetDP function name of the material's mass heat capacity."""
+        if self.name not in getdpTSAMassHeatCapacityFunctions:
+            return "NOT_DEFINED_IN_DATA_FIQUS_PANCAKE3D"
+
+        return getdpTSAMassHeatCapacityFunctions[self.name]
+
+    @computed_field
+    @cached_property
+    def getdpTSARHSFunction(self) -> str:
+        """Return the GetDP function name of the material's RHS."""
+        if self.name not in getdpTSARHSFunctions:
+            return "NOT_DEFINED_IN_DATA_FIQUS_PANCAKE3D"
+
+        return getdpTSARHSFunctions[self.name]
+
+    @computed_field
+    @cached_property
+    def getdpTSATripleFunction(self) -> str:
+        """Return the GetDP function name of the material's triple."""
+        if self.name not in getdpTSATripleFunctions:
+            return "NOT_DEFINED_IN_DATA_FIQUS_PANCAKE3D"
+
+        return getdpTSATripleFunctions[self.name]
 
+
+class Pancake3DSolveNormalMaterial(Pancake3DSolveMaterialBase):
+    # Mandatory:
+    name: NormalMaterialName = Field(
+        title="Material Name",
+    )
+
+
+class Pancake3DSolveSuperconductingMaterial(Pancake3DSolveMaterialBase):
     # Mandatory:
-    name: Literal["HTSSuperPower"] = Field(
-        title="Superconductor Material Name",
-        description="Name of the superconductor material.",
+    name: SuperconductingMaterialName = Field(
+        title="Superconduncting Material Name",
     )
-    IcAtTinit: Union[PositiveFloat, str, Pancake3DSolveIcVsLength] = Field(
+    nValue: PositiveFloat = Field(
+        default=30,
+        alias="N-Value for E-J Power Law",
+        description="N-value for E-J power law.",
+    )
+    IcAtTinit: PositiveFloat | str | Pancake3DSolveIcVsLength = Field(
         alias="criticalCurrentAtInitialTemperature",
         title="Critical Current at Initial Temperature",
         description=(
             "Critical current at initial temperature. The critical current value will"
             " change with temperature depending on the superconductor material.\nEither"
             " the same critical current for the whole tape or the critical current with"
             " respect to the tape length can be specified. To specify the same critical"
@@ -545,1063 +1326,681 @@
             " will be linearly interpolated.\nIf a CSV file is to be used, the input"
             " should be the name of a CSV file (which is in the same folder as the"
             " input file) instead of a scalar. The first column of the CSV file will be"
             " the tape length, and the second column will be the critical current."
         ),
         examples=[230, "IcVSlength.csv"],
     )
-    nValue: PositiveFloat = Field(
-        default=30,
-        alias="N-Value for E-J Power Law",
-        description="N-value for E–J power law.",
-    )
 
     # Optionals:
-    relativeThickness: float = Field(
-        default=None,
-        le=1,
-        title="Relative Thickness (only for winding)",
-        description=(
-            "Winding tapes generally consist of more than one material. Therefore, when"
-            " materials are given as a list in winding, their relative thickness,"
-            " (thickness of the material) / (thickness of the winding), should be"
-            " specified."
-        ),
-    )
-
-    jCriticalScalingNormalToWinding: PositiveFloat = Field(
-        default=1,
-        title="Critical Current Scaling Normal to Winding",
-        description=(
-            "Critical current scaling normal to winding, i.e., along the c_axis. "
-            " We have Jc_cAxis = scalingFactor * Jc_abPlane."
-            " A factor of 1 means no scaling such that the HTS layer is isotropic."
-        ),
-    )
-
     electricFieldCriterion: PositiveFloat = Field(
         default=1e-4,
         title="Electric Field Criterion",
         description=(
             "The electric field that defines the critical current density, i.e., the"
             " electric field at which the current density reaches the critical current"
             " density."
         ),
     )
-
-    # 2) To be calculated:
-    IcValues: List[float] = Field(
-        default=None,
+    jCriticalScalingNormalToWinding: PositiveFloat = Field(
+        default=1,
+        title="Critical Current Scaling Normal to Winding",
         description=(
-            "Critical current values for corresponding tape lengths read from the CSV"
-            " file (calculated by FiQuS)."
+            "Critical current scaling normal to winding, i.e., along the c_axis. "
+            " We have Jc_cAxis = scalingFactor * Jc_abPlane."
+            " A factor of 1 means no scaling such that the HTS layer is isotropic."
         ),
     )
-    lengthValues: List[float] = Field(
-        default=None,
+    minimumPossibleResistivity: NonNegativeFloat = Field(
+        default=0,
+        title="Minimum Possible Resistivity",
         description=(
-            "Tape lengths for corresponding critical current values read from the CSV"
-            " file (calculated by FiQuS)."
+            "The resistivity of the winding won't be lower than this value, no matter"
+            " what."
         ),
     )
-    getdpCriticalCurrentDensityFunction: str = Field(
-        default=None,
+    maximumPossibleResistivity: PositiveFloat = Field(
+        default=1,
+        title="Maximum Possible Resistivity",
         description=(
-            "GetDP function name of the material's critical current density (calculated"
-            " by FiQuS)"
+            "The resistivity of the winding won't be higher than this value, no matter"
+            " what."
         ),
     )
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def assign_getdpFunction(cls, values):
-        """ """
-        functionNames = {
-            "HTSSuperPower": "CFUN_HTS_JcFit_SUPERPOWER_T_B_theta",
-        }
-
-        values["getdpCriticalCurrentDensityFunction"] = functionNames[values["name"]]
-
-        return values
-
-
-class Pancake3DSolveCERNPlating(BaseModel):
-    # Mandatory:
-    name: Literal["Copper"] = Field(
-        title="Material Name",
-        description="choices: Copper",
-    )
+    @computed_field
+    @cached_property
+    def IcValues(self) -> list[float]:
+        """Return the critical current values of the material."""
+        if hasattr(self.IcAtTinit, "criticalCurrentValues"):
+            return self.IcAtTinit.criticalCurrentValues
+        elif isinstance(self.IcAtTinit, str):
+            csv_file_path = pathlib.Path(input_file_path.get()).parent / self.IcAtTinit
+            # return the second column:
+            IcValues = list(pd.read_csv(csv_file_path, header=None).iloc[:, 1])
+            for Ic in IcValues:
+                if Ic < 0:
+                    raise ValueError(
+                        "Critical current values in the CSV file should be positive!"
+                    )
+            return IcValues
+        else:
+            return [self.IcAtTinit]
 
-    relativeWidth: float = Field(
-        default=0,
-        title="Relative width of plating",
-        le=1,
-        description=(
-            "HTS 2G coated conductor are typically plated, usually "
-            " using copper. The relative width of the plating is the "
-            " width of the plating divided by the width of the tape. "
-            " 0 means no plating."
-        ),
-    )
+    @computed_field
+    @cached_property
+    def lengthValues(self) -> list[float]:
+        """Return the length values of the material."""
+        if hasattr(self.IcAtTinit, "lengthValues"):
+            return self.IcAtTinit.lengthValues
+        elif isinstance(self.IcAtTinit, str):
+            csv_file_path = pathlib.Path(input_file_path.get()).parent / self.IcAtTinit
+            # return the first column:
+            lengthValues = list(pd.read_csv(csv_file_path, header=None).iloc[:, 0])
+            for length in lengthValues:
+                if length < 0:
+                    raise ValueError("Tape lengths in the CSV file should be positive!")
+            return lengthValues
+        else:
+            return [1]
 
+    @computed_field
+    @cached_property
+    def getdpCriticalCurrentDensityFunction(self) -> str:
+        """Return the GetDP function name of the material's critical current density."""
+        if self.name not in getdpCriticalCurrentDensityFunctions:
+            raise ValueError(
+                f"Critical current density of the material '{self.name}' is not defined"
+                " in FiQuS!"
+            )
 
-class Pancake3DSolveCERNNormalMaterial(BaseModel):
-    # 1) User inputs:
+        return getdpCriticalCurrentDensityFunctions[self.name]
 
-    # Mandatory:
-    name: Literal["Copper", "Hastelloy", "Silver", "Indium", "Stainless Steel"] = Field(
-        title="Material Name",
-        description="choices: Copper, Hastelloy, Silver, Indium, Stainless Steel",
-    )
 
-    # Optionals:
+class Pancake3DSolveHTSMaterialBase(BaseModel):
     relativeThickness: float = Field(
-        default=None,
         le=1,
         title="Relative Thickness (only for winding)",
         description=(
             "Winding tapes generally consist of more than one material. Therefore, when"
             " materials are given as a list in winding, their relative thickness,"
             " (thickness of the material) / (thickness of the winding), should be"
             " specified."
         ),
     )
-    rrr: PositiveFloat = Field(
-        default=100,
-        alias="residualResistanceRatio",
-        title="Residual Resistance Ratio",
-        description=(
-            "Residual-resistivity ratio (also known as Residual-resistance ratio or"
-            " just RRR) is the ratio of the resistivity of a material at reference"
-            " temperature and at 0 K."
-        ),
-    )
-    rrrRefT: PositiveFloat = Field(
-        default=295,
-        alias="residualResistanceRatioReferenceTemperature",
-        title="Residual Resistance Ratio Reference Temperature",
-        description="Reference temperature for residual resistance ratio",
-    )
 
-    # 2) To be calculated:
-    resistivityMacroName: str = Field(
-        default=None,
-        description=(
-            "GetDP function name of the material's resistivity (calculated by FiQuS)"
-        ),
-    )
-    thermalConductivityMacroName: str = Field(
-        default=None,
-        description=(
-            "GetDP function name of the material's thermal conductivity (calculated by"
-            " FiQuS)"
-        ),
-    )
-    heatCapacityMacroName: str = Field(
-        default=None,
-        description=(
-            "GetDP function name of the material's heat capacity (calculated by FiQuS)"
-        ),
-    )
 
-    getdpTSAMassResistivityFunction: str = Field(
-        default=None,
-        description=(
-            "GetDP function name of the shell material's mass resistivity (calculated"
-            " by FiQuS)"
-        ),
-    )
+class Pancake3DSolveHTSNormalMaterial(
+    Pancake3DSolveHTSMaterialBase, Pancake3DSolveNormalMaterial
+):
+    pass
 
-    getdpTSAStiffnessResistivityFunction: str = Field(
-        default=None,
-        description=(
-            "GetDP function name of the shell material's stiffness resistivity"
-            " (calculated by FiQuS)"
-        ),
-    )
 
-    getdpTSAMassThermalConductivityFunction: str = Field(
-        default=None,
-        description=(
-            "GetDP function name of the shell material's mass thermal conductivity"
-            " (calculated by FiQuS)"
-        ),
-    )
+class Pancake3DSolveHTSSuperconductingMaterial(
+    Pancake3DSolveHTSMaterialBase, Pancake3DSolveSuperconductingMaterial
+):
+    pass
 
-    getdpTSAStiffnessThermalConductivityFunction: str = Field(
-        default=None,
-        description=(
-            "GetDP function name of the shell material's stiffness thermal conductivity"
-            " (calculated by FiQuS)"
-        ),
-    )
-
-    getdpTSAMassHeatCapacityFunction: str = Field(
-        default=None,
-        description=(
-            "GetDP function name of the shell material's mass heat capacity (calculated"
-            " by FiQuS)"
-        ),
-    )
 
-    getdpTSARHSFunction: str = Field(
-        default=None,
-        description=(
-            "GetDP function name of the shell material's RHS (calculated by FiQuS)"
-        ),
+class Pancake3DSolveHTSShuntLayerMaterial(Pancake3DSolveNormalMaterial):
+    name: NormalMaterialName = Field(
+        default="Copper",
+        title="Material Name",
     )
-
-    getdpTSATripleFunction: str = Field(
-        default=None,
+    relativeHeight: float = Field(
+        default=0.0,
+        ge=0,
+        le=1,
+        title="Relative Height of the Shunt Layer",
         description=(
-            "GetDP function name of the shell material's triple (calculated by FiQuS)"
+            "HTS 2G coated conductor are typically plated, usually "
+            " using copper. The relative height of the shunt layer is the "
+            " width of the shunt layer divided by the width of the tape. "
+            " 0 means no shunt layer."
         ),
     )
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def assign_normal_getdp_functions(cls, values):
-        """ """
-        resistivityMacroNames = {
-            "Copper": "MATERIAL_Resistivity_Copper_T_B",
-            "Hastelloy": "MATERIAL_Resistivity_Hastelloy_T",
-            "Silver": "MATERIAL_Resistivity_Silver_T_B",
-            "Indium": "MATERIAL_Resistivity_Indium_T",
-            "Stainless Steel": "MATERIAL_Resistivity_SSteel_T",
-        }
-        thermalConductivityMacroNames = {
-            "Copper": "MATERIAL_ThermalConductivity_Copper_T_B",
-            "Hastelloy": "MATERIAL_ThermalConductivity_Hastelloy_T",
-            "Silver": "MATERIAL_ThermalConductivity_Silver_T",
-            "Indium": "MATERIAL_ThermalConductivity_Indium_T",
-            "Stainless Steel": "MATERIAL_ThermalConductivity_SSteel_T",
-        }
-        heatCapacityMacroNames = {
-            "Copper": "MATERIAL_SpecificHeatCapacity_Copper_T",
-            "Hastelloy": "MATERIAL_SpecificHeatCapacity_Hastelloy_T",
-            "Silver": "MATERIAL_SpecificHeatCapacity_Silver_T",
-            "Indium": "MATERIAL_SpecificHeatCapacity_Indium_T",
-            "Stainless Steel": "MATERIAL_SpecificHeatCapacity_SSteel_T",
-        }
-
-        if values["name"] in resistivityMacroNames:
-            values["resistivityMacroName"] = resistivityMacroNames[values["name"]]
-        if values["name"] in thermalConductivityMacroNames:
-            values["thermalConductivityMacroName"] = thermalConductivityMacroNames[
-                values["name"]
-            ]
-        if values["name"] in heatCapacityMacroNames:
-            values["heatCapacityMacroName"] = heatCapacityMacroNames[values["name"]]
-
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def assign_TSA_getdp_functions(cls, values):
-        resistivityMassFunctionNames = {
-            "Indium": "TSA_CFUN_rhoIn_T_constantThickness_mass",
-            "Stainless Steel": None,
-        }
-        resistivityStiffnessFunctionNames = {
-            "Indium": "TSA_CFUN_rhoIn_T_constantThickness_stiffness",
-            "Stainless Steel": None,
-        }
-        thermalConductivityMassFunctionNames = {
-            "Indium": "TSA_CFUN_kIn_constantThickness_mass",
-            "Stainless Steel": "TSA_CFUN_kSteel_T_constantThickness_mass",
-        }
-        thermalConductivityStiffnessFunctionNames = {
-            "Indium": "TSA_CFUN_kIn_constantThickness_stiffness",
-            "Stainless Steel": "TSA_CFUN_kSteel_T_constantThickness_stiffness",
-        }
-        heatCapacityMassFunctionNames = {
-            "Indium": "TSA_CFUN_CvIn_constantThickness_mass",
-            "Stainless Steel": "TSA_CFUN_CvSteel_T_constantThickness_mass",
-        }
-        rhsFunctionNames = {
-            "Indium": "TSA_CFUN_rhoIn_T_constantThickness_rhs",
-            "Stainless Steel": None,
-        }
-        tripleFunctionNames = {
-            "Indium": "TSA_CFUN_rhoIn_T_constantThickness_triple",
-            "Stainless Steel": None,
-        }
-
-        if values["name"] in resistivityMassFunctionNames:
-            values["getdpTSAMassResistivityFunction"] = resistivityMassFunctionNames[
-                values["name"]
-            ]
-        if values["name"] in resistivityStiffnessFunctionNames:
-            values[
-                "getdpTSAStiffnessResistivityFunction"
-            ] = resistivityStiffnessFunctionNames[values["name"]]
-        if values["name"] in thermalConductivityMassFunctionNames:
-            values[
-                "getdpTSAMassThermalConductivityFunction"
-            ] = thermalConductivityMassFunctionNames[values["name"]]
-
-        if values["name"] in thermalConductivityStiffnessFunctionNames:
-            values[
-                "getdpTSAStiffnessThermalConductivityFunction"
-            ] = thermalConductivityStiffnessFunctionNames[values["name"]]
-
-        if values["name"] in heatCapacityMassFunctionNames:
-            values["getdpTSAMassHeatCapacityFunction"] = heatCapacityMassFunctionNames[
-                values["name"]
-            ]
-
-        if values["name"] in rhsFunctionNames:
-            values["getdpTSARHSFunction"] = rhsFunctionNames[values["name"]]
-
-        if values["name"] in tripleFunctionNames:
-            values["getdpTSATripleFunction"] = tripleFunctionNames[values["name"]]
-
-        return values
-
 
 class Pancake3DSolveMaterial(BaseModel):
     # 1) User inputs:
 
     # Mandatory:
 
     # Optionals:
-    numberOfThinShellElements: PositiveInt = Field(
-        default=1,
-        title="Number of Thin Shell Elements (Advanced Input)",
-        description=(
-            "Number of thin shell elements in the FE formulation (GetDP related, not"
-            " physical and only used when TSA is set to True)"
-        ),
-    )
-    resistivity: PositiveFloat = Field(
+    resistivity: Optional[PositiveFloat] = Field(
         default=None,
         title="Resistivity",
         description=(
             "A scalar value. If this is given, material properties won't be used for"
             " resistivity."
         ),
     )
-    thermalConductivity: PositiveFloat = Field(
+    thermalConductivity: Optional[PositiveFloat] = Field(
         default=None,
         title="Thermal Conductivity",
         description=(
             "A scalar value. If this is given, material properties won't be used for"
             " thermal conductivity."
         ),
     )
-    specificHeatCapacity: PositiveFloat = Field(
+    specificHeatCapacity: Optional[PositiveFloat] = Field(
         default=None,
         title="Specific Heat Capacity",
         description=(
             "A scalar value. If this is given, material properties won't be used for"
             " specific heat capacity."
         ),
     )
-    material: Pancake3DSolveCERNNormalMaterial = Field(
+    material: Optional[Pancake3DSolveNormalMaterial] = Field(
         default=None,
         title="Material",
-        description="Material from CERN material library.",
+        description="Material from STEAM material library.",
     )
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
+    @model_validator(mode="after")
     @classmethod
-    def check_if_all_the_material_properties_are_given(cls, values):
-        """ """
-        if values["material"] is None:
-            if not (
-                values["resistivity"]
-                and values["thermalConductivity"]
-                and values["specificHeatCapacity"]
-            ):
+    def check_material(cls, model: "Pancake3DSolveMaterial"):
+        if model.material is None:
+            if model.resistivity is None:
                 raise ValueError(
-                    "Resistivity, thermal conductivity, and specific heat capacity must"
-                    " be specified if material is not specified!"
+                    "Resistivity of the material is not given, and no material is"
+                    " provided!"
                 )
-
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def check_if_more_than_one_property_is_given(cls, values):
-        """ """
-        if values["material"]:
-            if values["resistivity"]:
-                logger.warning(
-                    f"Constant resistivity value ({values['resistivity']}) will be used"
-                    f" instead of the nonlinear {values['material'].name}'s"
-                    " resistivity!"
-                )
-            if values["thermalConductivity"]:
-                logger.warning(
-                    "Constant thermal conductivity value"
-                    f" ({values['thermalConductivity']}) will be used instead of the"
-                    f" nonlinear {values['material'].name}'s thermal conductivity!"
+            if model.thermalConductivity is None:
+                raise ValueError(
+                    "Thermal conductivity of the material is not given, and no material"
+                    " is provided!"
                 )
-            if values["specificHeatCapacity"]:
-                logger.warning(
-                    "Constant specific heat capacity value"
-                    f" ({values['specificHeatCapacity']}) will be used instead of the"
-                    f" nonlinear {values['material'].name}'s specific heat capacity!"
+            if model.specificHeatCapacity is None:
+                raise ValueError(
+                    "Specific heat capacity of the material is not given, and no"
+                    " material is provided!"
                 )
 
-        return values
+        return model
+
+
+class Pancake3DSolveShuntLayerMaterial(Pancake3DSolveMaterial):
+    material: Optional[Pancake3DSolveHTSShuntLayerMaterial] = Field(
+        default=Pancake3DSolveHTSShuntLayerMaterial(),
+        title="Material",
+        description="Material from STEAM material library.",
+    )
 
 
 class Pancake3DSolveContactLayerMaterial(Pancake3DSolveMaterial):
-    resistivity: Union[PositiveFloat, Literal["perfectlyInsulating"]] = Field(
+    resistivity: PositiveFloat | Literal["perfectlyInsulating"] = Field(
         default=None,
         title="Resistivity",
         description=(
             'A scalar value or "perfectlyInsulating". If "perfectlyInsulating" is'
             " given, the contact layer will be perfectly insulating. If this value is"
             " given, material properties won't be used for resistivity."
         ),
     )
-
-
-class Pancake3DSolveTerminalMaterialAndBoundaryCondition(Pancake3DSolveMaterial):
-    cooling: Literal["adiabatic", "fixedTemperature", "cryocooler"] = Field(
-        default="fixedTemperature",
-        title="Cooling condition",
+    numberOfThinShellElements: PositiveInt = Field(
+        default=1,
+        title="Number of Thin Shell Elements (Advanced Input)",
         description=(
-            "Cooling condition of the terminal. It can be either adiabatic, fixed"
-            " temperature, or cryocooler."
+            "Number of thin shell elements in the FE formulation (GetDP related, not"
+            " physical and only used when TSA is set to True)"
         ),
     )
 
+    @field_validator("resistivity")
+    @classmethod
+    def checkPerfectlyInsulatingCase(cls, resistivity):
+        if resistivity == "perfectlyInsulating":
+            geometry = geometry_input.get()
+            if geometry["numberOfPancakes"] > 1:
+                raise ValueError(
+                    "Contact layer can't be perfectly insulating for multi-pancake"
+                    " coils!"
+                )
 
-class Pancake3DSolveWindingMaterial(BaseModel):
-    # 1) User inputs:
+        return resistivity
 
-    # Mandatory:
 
-    # Optionals:
-    resistivity: PositiveFloat = Field(
-        default=None,
-        title="Resistivity",
-        description=(
-            "A scalar value. If this is given, material properties won't be used for"
-            " resistivity."
-        ),
-    )
-    thermalConductivity: PositiveFloat = Field(
-        default=None,
-        title="Thermal Conductivity",
-        description=(
-            "A scalar value. If this is given, material properties won't be used for"
-            " thermal conductivity."
-        ),
-    )
-    specificHeatCapacity: PositiveFloat = Field(
-        default=None,
-        title="Specific Heat Capacity",
-        description=(
-            "A scalar value. If this is given, material properties won't be used for"
-            " specific heat capacity."
-        ),
-    )
-    minimumPossibleResistivity: NonNegativeFloat = Field(
-        default=0,
-        title="Minimum Possible Resistivity",
-        description=(
-            "The resistivity of the winding won't be lower than this value, no matter"
-            " what."
-        ),
-    )
-    maximumPossibleResistivity: PositiveFloat = Field(
-        default=1,
-        title="Maximum Possible Resistivity",
-        description=(
-            "The resistivity of the winding won't be higher than this value, no matter"
-            " what."
-        ),
-    )
-    material: List[
-        Union[
-            Pancake3DSolveCERNNormalMaterial, Pancake3DSolveCERNSuperConductorMaterial
-        ]
-    ] = Field(
-        default=None,
-        title="Winding Material",
-        description=(
-            "Because generally winding tapes consist of more than one material,"
-            " materials should be given as a list of Material dictionaries."
-        ),
-    )
+Pancake3DHTSMaterial = Annotated[
+    Pancake3DSolveHTSNormalMaterial | Pancake3DSolveHTSSuperconductingMaterial,
+    Field(discriminator="name"),
+]
 
-    plating: Pancake3DSolveCERNPlating = Field(
-        default=Pancake3DSolveCERNPlating(name="Copper", relativeWidth=0),
-        title="Tape plating",
-        description=(
-            "The plating of the winding tape. Only copper is supported for now."
-            "By default, the tape is not plated."
-        ),
-    )
 
-    # 2) To be calculated:
-    relativeThicknessOfNormalConductor: PositiveFloat = Field(
-        default=None,
-        description=(
-            "(thickness of the normal conductor) / (thickness of the winding)"
-            " (calculated by FiQuS)"
-        ),
-    )
-    relativeThicknessOfSuperConductor: PositiveFloat = Field(
+class Pancake3DSolveWindingMaterial(Pancake3DSolveMaterial):
+    material: Optional[list[Pancake3DHTSMaterial]] = Field(
         default=None,
-        description=(
-            "(thickness of the normal conductor) / (thickness of the winding)"
-            " (calculated by FiQuS)"
-        ),
-    )
-    normalConductors: List[Pancake3DSolveCERNNormalMaterial] = Field(
-        default=None, description="list of normal conductors (calculated by FiQuS)"
+        title="Materials of HTS CC",
+        description="List of materials of HTS CC.",
     )
-    superConductor: Pancake3DSolveCERNSuperConductorMaterial = Field(
-        default=None, description="super conductor used (calculated by FiQuS)"
+
+    shuntLayer: Pancake3DSolveShuntLayerMaterial = Field(
+        default=Pancake3DSolveShuntLayerMaterial(),
+        title="Shunt Layer Properties",
+        description="Material properties of the shunt layer.",
     )
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
+    @field_validator("material")
     @classmethod
-    def check_if_all_the_material_properties_are_given(cls, values):
-        """ """
-        if values["material"] is None:
-            if not (
-                values["resistivity"]
-                and values["thermalConductivity"]
-                and values["specificHeatCapacity"]
-            ):
+    def checkIfRelativeThicknessesSumToOne(cls, material):
+        if material is not None:
+            totalRelativeThickness = sum(
+                material.relativeThickness for material in material
+            )
+            if not math.isclose(totalRelativeThickness, 1, rel_tol=1e-3):
                 raise ValueError(
-                    "Resistivity, thermal conductivity, and specific heat capacity must"
-                    " be specified if material is not specified!"
+                    "Sum of relative thicknesses of HTS materials should be 1!"
                 )
 
-        return values
+        return material
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def calculate_relative_thicknesses(cls, values):
-        """ """
+    @computed_field
+    @cached_property
+    def relativeThicknessOfNormalConductor(self) -> PositiveFloat:
+        """Return the relative thickness of the normal conductor."""
+        if self.material is None:
+            return 0
+        else:
+            # look at normal materials inside self.material and sum their relativeThickness
+            return sum(
+                material.relativeThickness
+                for material in self.material
+                if isinstance(material, Pancake3DSolveHTSNormalMaterial)
+            )
 
-        totalNormalConductorThickness = 0
-        if values["material"]:
-            for material in values["material"]:
-                if isinstance(material, Pancake3DSolveCERNNormalMaterial):
-                    totalNormalConductorThickness = (
-                        totalNormalConductorThickness + material.relativeThickness
-                    )
+    @computed_field
+    @cached_property
+    def relativeThicknessOfSuperConductor(self) -> PositiveFloat:
+        """Return the relative thickness of the super conductor."""
+        if self.material is None:
+            return 0
+        else:
+            # look at superconducting materials inside self.material and sum their relativeThickness
+            return sum(
+                material.relativeThickness
+                for material in self.material
+                if isinstance(material, Pancake3DSolveHTSSuperconductingMaterial)
+            )
 
-            values["relativeThicknessOfNormalConductor"] = totalNormalConductorThickness
-            values["relativeThicknessOfSuperConductor"] = (
-                1 - totalNormalConductorThickness
-            )
-
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def create_normal_and_super_conductor_lists(cls, values):
-        """ """
-        if values["material"]:
-            values["normalConductors"] = []
-            values["superConductor"] = None
-            for material in values["material"]:
-                if isinstance(material, Pancake3DSolveCERNNormalMaterial):
-                    values["normalConductors"].append(material)
-                else:
-                    if values["superConductor"] is not None:
-                        raise ValueError("Only one super conductor must be specified!")
-                    values["superConductor"] = material
-
-        return values
-
-    @validator("material", allow_reuse=True)
-    @classmethod
-    def check_material(cls, value):
-        """"""
-        if value is not None:
-            totalRelativeThickness = 0
-            for material in value:
-                if material.relativeThickness is None:
-                    raise ValueError(
-                        "Relative thickness must be specified for winding material!"
-                    )
-                totalRelativeThickness = (
-                    totalRelativeThickness + material.relativeThickness
-                )
+    @computed_field
+    @cached_property
+    def normalConductors(self) -> list[Pancake3DSolveHTSNormalMaterial]:
+        """Return the normal conductors of the winding."""
+        if self.material is None:
+            return []
+        else:
+            return [
+                material
+                for material in self.material
+                if isinstance(material, Pancake3DSolveHTSNormalMaterial)
+            ]
 
-            if not math.isclose(totalRelativeThickness, 1):
+    @computed_field
+    @cached_property
+    def superConductor(self) -> Pancake3DSolveHTSSuperconductingMaterial:
+        """Return the super conductor of the winding."""
+        if self.material is None:
+            return None
+        else:
+            superConductors = [
+                material
+                for material in self.material
+                if isinstance(material, Pancake3DSolveHTSSuperconductingMaterial)
+            ]
+            if len(superConductors) == 0:
+                return None
+            elif len(superConductors) == 1:
+                return superConductors[0]
+            else:
                 raise ValueError(
-                    "Sum of the relative thicknesses of the winding materials must be"
-                    " equal to 1!"
-                )
-
-        return value
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def check_if_more_than_one_property_is_given(cls, values):
-        """ """
-        if values["material"]:
-            if values["resistivity"]:
-                logger.warning(
-                    f"Constant resistivity value ({values['resistivity']}) will be used"
-                    " instead of the nonlinear"
-                    f" {', '.join([material.name for material in values['material']])}'s"
-                    " resistivity!"
-                )
-            if values["thermalConductivity"]:
-                logger.warning(
-                    "Constant thermal conductivity value"
-                    f" ({values['thermalConductivity']}) will be used instead of the"
-                    " nonlinear"
-                    f" {', '.join([material.name for material in values['material']])}'s"
-                    " thermal conductivity!"
-                )
-            if values["specificHeatCapacity"]:
-                logger.warning(
-                    "Constant specific heat capacity value"
-                    f" ({values['specificHeatCapacity']}) will be used instead of the"
-                    " nonlinear"
-                    f" {', '.join([material.name for material in values['material']])}'s"
-                    " specific heat capacity!"
+                    "There should be only one superconductor in the winding!"
                 )
 
-        return values
 
+class Pancake3DSolveTerminalMaterialAndBoundaryCondition(Pancake3DSolveMaterial):
+    cooling: Literal["adiabatic", "fixedTemperature", "cryocooler"] = Field(
+        default="fixedTemperature",
+        title="Cooling condition",
+        description=(
+            "Cooling condition of the terminal. It can be either adiabatic, fixed"
+            " temperature, or cryocooler."
+        ),
+    )
+    transitionNotch: Pancake3DSolveMaterial = Field(
+        title="Transition Notch Properties",
+        description="Material properties of the transition notch volume.",
+    )
+    terminalContactLayer: Pancake3DSolveMaterial = Field(
+        title="Transition Layer Properties",
+        description=(
+            "Material properties of the transition layer between terminals and"
+            " windings."
+        ),
+    )
 
-class Pancake3DSolveTolerance(BaseModel):
-    # 1) User inputs:
 
+class Pancake3DSolveToleranceBase(BaseModel):
     # Mandatory:
-    quantity: Literal[
-        "solutionVector",
-        "totalResistiveHeating",
-        "voltageBetweenTerminals",
-        "resistiveHeating",
-        "temperature",
-        "magnitudeOfCurrentDensity",
-        "magnitudeOfMagneticField",
-        "axialComponentOfTheMagneticField",
-        "currentThroughCoil",
-        "magnitudeOfHeatFlux",
-        "magneticEnergy",
-    ] = Field(
-        title="Quantity",
-        description="Name of the quantity for tolerance.",
-    )
+    quantity: str
     relative: NonNegativeFloat = Field(
         title="Relative Tolerance",
         description="Relative tolerance for the quantity.",
     )
     absolute: NonNegativeFloat = Field(
         title="Absolute Tolerance", description="Absolute tolerance for the quantity"
     )
 
     # Optionals:
+    normType: Literal["L1Norm", "MeanL1Norm", "L2Norm", "MeanL2Norm", "LinfNorm"] = (
+        Field(
+            default="L2Norm",
+            alias="normType",
+            title="Norm Type",
+            description=(
+                "Sometimes, tolerances return a vector instead of a scalar (ex,"
+                " solutionVector). Then, the magnitude of the tolerance should be"
+                " calculated with a method. Norm type selects this method."
+            ),
+        )
+    )
+
+
+class Pancake3DSolvePositionRequiredTolerance(Pancake3DSolveToleranceBase):
+    # Mandatory:
+    quantity: PositionRequiredQuantityName = Field(
+        title="Quantity", description="Name of the quantity for tolerance."
+    )
     position: Pancake3DPosition = Field(
-        default=None,
         title="Probing Position of the Quantity",
         description="Probing position of the quantity for tolerance.",
     )
-    normType: Literal[
-        "L1Norm", "MeanL1Norm", "L2Norm", "MeanL2Norm", "LinfNorm"
-    ] = Field(
-        default="L2Norm",
-        alias="normType",
-        title="Norm Type",
-        description=(
-            "Sometimes, tolerances return a vector instead of a scalar (ex,"
-            " solutionVector). Then, the magnitude of the tolerance should be"
-            " calculated with a method. Norm type selects this method."
-        ),
-    )
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def check_if_position_is_required(clas, values):
-        """ """
-        positionRequiredQuantities = [
-            "resistiveHeating",
-            "temperature",
-            "magnitudeOfCurrentDensity",
-            "magnitudeOfMagneticField",
-            "axialComponentOfTheMagneticField",
-            "magnitudeOfHeatFlux",
+
+class Pancake3DSolvePositionNotRequiredTolerance(Pancake3DSolveToleranceBase):
+    # Mandatory:
+    quantity: (
+        Literal[
+            "solutionVector",
         ]
-        if values["quantity"] in positionRequiredQuantities:
-            if values["position"] is None:
-                raise ValueError(
-                    f"Position must be specified for {values['quantity']} tolerance!"
-                )
-            else:
-                coordinatesAreGiven = False
-                if (
-                    values["position"].x is not None
-                    and values["position"].y is not None
-                    and values["position"].z is not None
-                ):
-                    coordinatesAreGiven = True
-
-                turnNumberIsGiven = False
-                if values["position"].turnNumber is not None:
-                    turnNumberIsGiven = True
+        | PositionNotRequiredQuantityName
+    ) = Field(
+        title="Quantity",
+        description="Name of the quantity for tolerance.",
+    )
 
-                if coordinatesAreGiven and turnNumberIsGiven:
-                    raise ValueError(
-                        "Either xyz-coordinates or turn number can be specified!"
-                    )
-                elif turnNumberIsGiven:
-                    if (
-                        values["position"].x
-                        or values["position"].y
-                        or values["position"].z
-                    ):
-                        raise ValueError(
-                            "Either turn number or x, y, and z coordinates can be"
-                            " specified!"
-                        )
-                elif coordinatesAreGiven:
-                    pass
-                else:
-                    raise ValueError(
-                        "x, y, and z coordinates or turn number must be specified"
-                        " for position!"
-                    )
 
-        return values
+Pancake3DSolveTolerance = Annotated[
+    Pancake3DSolvePositionRequiredTolerance
+    | Pancake3DSolvePositionNotRequiredTolerance,
+    Field(discriminator="quantity"),
+]
 
-    @validator("quantity", allow_reuse=True)
-    @classmethod
-    def quantity_specific_warnings(cls, value):
-        if value == "totalResistiveHeating":
-            logger.warning(
-                "Calculation of total resistive heating might be slow for tolerances!"
-            )
 
-        return value
+class Pancake3DSolveSettingsWithTolerances(BaseModel):
+    tolerances: list[Pancake3DSolveTolerance] = Field(
+        title="Tolerances for Adaptive Time Stepping",
+        description=(
+            "Time steps or nonlinear iterations will be refined until the tolerances"
+            " are satisfied."
+        ),
+    )
 
+    @computed_field
+    @cached_property
+    def postOperationTolerances(self) -> list[Pancake3DSolveTolerance]:
+        """Return the post operation tolerances."""
+        tolerances = [
+            tolerance
+            for tolerance in self.tolerances
+            if "solutionVector" not in tolerance.quantity
+        ]
+        return tolerances
+
+    @computed_field
+    @cached_property
+    def systemTolerances(self) -> list[Pancake3DSolveTolerance]:
+        """Return the system tolerances."""
+        tolerances = [
+            tolerance
+            for tolerance in self.tolerances
+            if "solutionVector" in tolerance.quantity
+        ]
+        return tolerances
 
-class Pancake3DSolveAdaptiveTimeLoopSettings(BaseModel):
-    # 1) User inputs:
 
+class Pancake3DSolveAdaptiveTimeLoopSettings(Pancake3DSolveSettingsWithTolerances):
     # Mandatory:
     initialStep: PositiveFloat = Field(
-        default=None,
         alias="initialStep",
         title="Initial Step for Adaptive Time Stepping",
         description="Initial step for adaptive time stepping",
     )
     minimumStep: PositiveFloat = Field(
-        default=None,
         alias="minimumStep",
         title="Minimum Step for Adaptive Time Stepping",
         description=(
             "The simulation will be aborted if a finer time step is required than this"
             " minimum step value."
         ),
     )
     maximumStep: PositiveFloat = Field(
-        default=None,
         alias="maximumStep",
         description="Bigger steps than this won't be allowed",
     )
-    tolerances: List[Pancake3DSolveTolerance] = Field(
-        default=None,
-        title="Tolerances for Adaptive Time Stepping",
-        description=(
-            "Time steps will be adjusted so the predicted error of quantities below"
-            " will stay in the tolerance range. Tolerances will decide how fine the"
-            " time stepping will be."
-        ),
-    )
 
     # Optionals:
     integrationMethod: Literal[
         "Euler", "Gear_2", "Gear_3", "Gear_4", "Gear_5", "Gear_6"
     ] = Field(
         default="Euler",
         alias="integrationMethod",
         title="Integration Method",
         description="Integration method for transient analysis",
     )
-    breakPoints: List[float] = Field(
+    breakPoints_input: list[float] = Field(
         default=[0],
         alias="breakPoints",
         title="Break Points for Adaptive Time Stepping",
         description="Make sure to solve the system for these times.",
     )
 
-    # 2) To be calculated:
-    postOperationTolerances: List[Pancake3DSolveTolerance] = Field(
-        default=None,
-        description="post operation type tolerances (calculated by FiQuS)",
-    )
-    systemTolerances: List[Pancake3DSolveTolerance] = Field(
-        default=None,
-        description="system type tolerances (calculated by FiQuS)",
-    )
+    @field_validator("breakPoints_input")
+    @classmethod
+    def updateGlobalBreakPointsList(cls, breakPoints_input):
+        all_break_points.extend(breakPoints_input)
+        return breakPoints_input
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
+    @model_validator(mode="after")
     @classmethod
-    def check_time_steps(cls, values):
+    def check_time_steps(cls, model: "Pancake3DSolveAdaptiveTimeLoopSettings"):
         """
         Checks if the time steps are consistent.
 
         :param values: dictionary of time steps
         :type values: dict
         :return: dictionary of time steps
         :rtype: dict
         """
 
-        if values["initialStep"] < values["minimumStep"]:
+        if model.initialStep < model.minimumStep:
             raise ValueError(
                 "Initial time step cannot be smaller than the minimum time step!"
             )
 
-        if values["initialStep"] > values["maximumStep"]:
+        if model.initialStep > model.maximumStep:
             raise ValueError(
                 "Initial time step cannot be greater than the maximum time step!"
             )
 
-        if values["minimumStep"] > values["maximumStep"]:
+        if model.minimumStep > model.maximumStep:
             raise ValueError(
                 "Minimum time step cannot be greater than the maximum time step!"
             )
 
-        return values
+        return model
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def parse_tolerances(cls, values):
-        values["postOperationTolerances"] = []
-        values["systemTolerances"] = []
-
-        for tolerance in values["tolerances"]:
-            if tolerance.quantity == "solutionVector":
-                values["systemTolerances"].append(tolerance)
-            else:
-                values["postOperationTolerances"].append(tolerance)
-
-        return values
+    @computed_field
+    @cached_property
+    def breakPoints(self) -> list[float]:
+        """Return the break points for adaptive time stepping."""
+        breakPoints = list(set(all_break_points))
+        breakPoints.sort()
+        return breakPoints
 
 
 class Pancake3DSolveFixedTimeLoopSettings(BaseModel):
-    # 1) User inputs:
-
     # Mandatory:
     step: PositiveFloat = Field(
-        default=None,
         title="Step for Fixed Time Stepping",
         description="Time step for fixed time stepping.",
     )
 
 
 class Pancake3DSolveFixedLoopInterval(BaseModel):
-    # 1) User inputs:
+    # Mandatory:
     startTime: NonNegativeFloat = Field(
         title="Start Time of the Interval",
         description="Start time of the interval.",
     )
     endTime: NonNegativeFloat = Field(
         title="End Time of the Interval",
         description="End time of the interval.",
     )
     step: PositiveFloat = Field(
         title="Step for the Interval",
         description="Time step for the interval",
     )
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
+    @model_validator(mode="after")
     @classmethod
-    def check_time_steps(cls, values):
+    def check_time_steps(cls, model: "Pancake3DSolveFixedLoopInterval"):
         """
         Checks if the time steps are consistent.
 
         :param values: dictionary of time steps
         :type values: dict
         :return: dictionary of time steps
         :rtype: dict
         """
 
-        if values["startTime"] > values["endTime"]:
+        if model.startTime > model.endTime:
             raise ValueError("Start time cannot be greater than the end time!")
 
-        interval = values["endTime"] - values["startTime"]
+        interval = model.endTime - model.startTime
         if (
-            math.fmod(interval, values["step"]) > 1e-8
-            and math.fmod(interval, values["step"]) - values["step"] < -1e-8
+            math.fmod(interval, model.step) > 1e-8
+            and math.fmod(interval, model.step) - model.step < -1e-8
         ):
             raise ValueError("Time interval must be a multiple of the time step!")
 
-        return values
+        return model
 
 
-class Pancake3DSolveTime(BaseModel):
-    # 1) User inputs:
-    adaptive: Pancake3DSolveAdaptiveTimeLoopSettings = Field(
-        default=None,
-        alias="adaptiveSteppingSettings",
-        title="Adaptive Time Loop Settings",
-        description=(
-            "Adaptive time loop settings (only used if stepping type is adaptive)."
-        ),
-    )
-    fixed: Union[
-        List[Pancake3DSolveFixedLoopInterval], Pancake3DSolveFixedTimeLoopSettings
-    ] = Field(
-        default=None,
-        alias="fixedSteppingSettings",
-        title="Fixed Time Loop Settings",
-        description="Fixed time loop settings (only used if stepping type is fixed).",
-    )
-
+class Pancake3DSolveTimeBase(BaseModel):
     # Mandatory:
     start: float = Field(
         title="Start Time", description="Start time of the simulation."
     )
     end: float = Field(title="End Time", description="End time of the simulation.")
 
-    timeSteppingType: Literal["fixed", "adaptive"] = Field(
-        title="Time Stepping Type",
-        description="Time stepping type.",
-    )
-
     # Optionals:
     extrapolationOrder: Literal[0, 1, 2, 3] = Field(
         default=1,
         alias="extrapolationOrder",
         title="Extrapolation Order",
         description=(
             "Before solving for the next time steps, the previous solutions can be"
             " extrapolated for better convergence."
         ),
     )
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
+    @model_validator(mode="after")
     @classmethod
-    def check_mandotory_fields(cls, values):
+    def check_time_steps(cls, model: "Pancake3DSolveTimeBase"):
         """
-        Checks if the mandatory fields are specified.
-
-        :param values: dictionary of time loop settings
-        :type values: dict
-        :return: dictionary of time loop settings
+        Checks if the time steps are consistent.
         """
-        if values["timeSteppingType"] == "fixed":
-            if values["fixed"] is None:
-                raise ValueError(
-                    "Fixed time stepping step must be specified if time loop type is"
-                    " fixed!"
-                )
-        else:
-            if values["adaptive"].initialStep is None:
-                raise ValueError(
-                    "Initial time step must be specified if time loop type is adaptive!"
-                )
-            if values["adaptive"].minimumStep is None:
-                raise ValueError(
-                    "Minimum time step must be specified if time loop type is adaptive!"
-                )
-            if values["adaptive"].maximumStep is None:
-                raise ValueError(
-                    "Maximum time step must be specified if time loop type is adaptive!"
-                )
-            if values["adaptive"].tolerances is None:
-                raise ValueError(
-                    "Tolerances must be specified if time loop type is adaptive!"
-                )
 
-        return values
+        if model.start > model.end:
+            raise ValueError("Start time cannot be greater than the end time!")
+
+        return model
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
+
+class Pancake3DSolveTimeAdaptive(Pancake3DSolveTimeBase):
+    timeSteppingType: Literal["adaptive"] = "adaptive"
+    adaptive: Pancake3DSolveAdaptiveTimeLoopSettings = Field(
+        alias="adaptiveSteppingSettings",
+        title="Adaptive Time Loop Settings",
+        description=(
+            "Adaptive time loop settings (only used if stepping type is adaptive)."
+        ),
+    )
+
+    @model_validator(mode="after")
     @classmethod
-    def check_time(cls, values):
+    def check_time_steps(cls, model: "Pancake3DSolveTimeAdaptive"):
         """
-        Checks if the time values are consistent and multiples of the time step.
-
-        :param cls: class
-        :type cls: class
-        :param values: dictionary of time
-        :type values: dict
-        :return: dictionary of time
-        :rtype: dict
+        Checks if the time steps are consistent.
         """
-        if not (values["start"] < values["end"]):
-            raise ValueError(
-                "Time values are not consistent! Start time is greater than end time!"
-            )
+        if model.adaptive.initialStep > model.end:
+            raise ValueError("Initial time step cannot be greater than the end time!")
 
-        times = [
-            values["start"],
-            values["end"],
-        ]
+        return model
+
+
+class Pancake3DSolveTimeFixed(Pancake3DSolveTimeBase):
+    timeSteppingType: Literal["fixed"] = "fixed"
+    fixed: (
+        list[Pancake3DSolveFixedLoopInterval] | Pancake3DSolveFixedTimeLoopSettings
+    ) = Field(
+        alias="fixedSteppingSettings",
+        title="Fixed Time Loop Settings",
+        description="Fixed time loop settings (only used if stepping type is fixed).",
+    )
 
-        if values["timeSteppingType"] == "fixed":
-            # Check if all the times are multiples of the time step:
-            if hasattr(values["fixed"], "step"):
-                timeStep = values["fixed"].step
-                values["fixed"] = [
-                    Pancake3DSolveFixedLoopInterval(
-                        startTime=values["start"],
-                        endTime=values["end"],
-                        step=timeStep,
+    @model_validator(mode="after")
+    @classmethod
+    def check_time_steps(cls, model: "Pancake3DSolveTimeFixed"):
+        if isinstance(model.fixed, list):
+            for i in range(len(model.fixed) - 1):
+                if model.fixed[i].endTime != model.fixed[i + 1].startTime:
+                    raise ValueError(
+                        "End time of the previous interval must be equal to the start"
+                        " time of the next interval!"
                     )
-                ]
-            else:
-                for i in range(len(values["fixed"]) - 1):
-                    if values["fixed"][i + 1].startTime != values["fixed"][i].endTime:
-                        raise ValueError(
-                            "Time intervals are not consistent! End time of the"
-                            " interval is not equal to the start time of the next"
-                            " interval!"
-                        )
 
-            if values["fixed"][0].startTime > values["end"]:
+            if model.fixed[0].startTime != model.start:
                 raise ValueError(
-                    "Time intervals are not consistent! Start time of the first"
-                    " interval is greater than the end time of the simulation!"
+                    "Start time of the first interval must be equal to the start time"
+                    " of the simulation!"
                 )
 
-            for time in times:
-                for interval in values["fixed"]:
-                    if time >= interval.startTime and time < interval.endTime:
-                        startTime = interval.startTime
-                        timeStep = interval.step
-                if (
-                    math.fmod(time - startTime, timeStep) > 1e-8
-                    and math.fmod(time - startTime, timeStep) - timeStep < -1e-8
-                ):
-                    raise ValueError("Time values are not multiples of the time step!")
-
-        if values["timeSteppingType"] == "adaptive":
-            values["adaptive"].breakPoints = list(set(values["adaptive"].breakPoints))
-            values["adaptive"].breakPoints.sort()
+        else:
+            if model.fixed.step > model.end:
+                raise ValueError("Time step cannot be greater than the end time!")
 
-            if values["adaptive"].initialStep > values["end"]:
-                raise ValueError(
-                    "Initial time step is greater than the end time of the simulation!"
+            if not (
+                math.isclose(
+                    (model.end - model.start) % model.fixed.step, 0, abs_tol=1e-8
                 )
+            ):
+                raise ValueError("Time interval must be a multiple of the time step!")
+            
 
-        return values
+        return model
 
 
-class Pancake3DSolveNonlinearSolverSettings(BaseModel):
-    # 1) User inputs:
+Pancake3DSolveTime = Annotated[
+    Pancake3DSolveTimeAdaptive | Pancake3DSolveTimeFixed,
+    Field(discriminator="timeSteppingType"),
+]
 
-    # Mandatory:
-    tolerances: List[Pancake3DSolveTolerance] = Field(
-        default=None,
-        title="Tolerances for Nonlinear Solver",
-        description=(
-            "The nonlinear solver will check the tolerance quantities to make sure it"
-            " converged or not. If the quantities stay in the tolerance region after an"
-            " iteration, it will conclude that the nonlinear solver converged."
-        ),
-    )
 
+class Pancake3DSolveNonlinearSolverSettings(Pancake3DSolveSettingsWithTolerances):
     # Optionals:
     maxIter: PositiveInt = Field(
         default=100,
         alias="maximumNumberOfIterations",
         title="Maximum Number of Iterations",
         description="Maximum number of iterations allowed for the nonlinear solver.",
     )
@@ -1612,392 +2011,322 @@
         title="Relaxation Factor",
         description=(
             "Calculated step changes of the solution vector will be multiplied with"
             " this value for better convergence."
         ),
     )
 
-    # 2) To be calculated:
-    postOperationTolerances: List[Pancake3DSolveTolerance] = Field(
-        default=None,
-        description="post operation type tolerances (calculated by FiQuS)",
-    )
-    systemTolerances: List[Pancake3DSolveTolerance] = Field(
-        default=None,
-        description="system type tolerances (calculated by FiQuS)",
-    )
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def parse_tolerances(cls, values):
-        values["postOperationTolerances"] = []
-        values["systemTolerances"] = []
-
-        for tolerance in values["tolerances"]:
-            if tolerance.quantity == "solutionVector":
-                values["systemTolerances"].append(tolerance)
-            else:
-                values["postOperationTolerances"].append(tolerance)
-
-        return values
-
 
 class Pancake3DSolveInitialConditions(BaseModel):
     # 1) User inputs:
 
     # Mandatory:
     T: PositiveFloat = Field(
         alias="temperature",
         title="Initial Temperature",
         description="Initial temperature of the pancake coils.",
     )
 
 
 class Pancake3DSolveLocalDefect(BaseModel):
-    # 1) User inputs:
-
     # Mandatory:
     value: NonNegativeFloat = Field(
-        default=None,
         alias="value",
         title="Value",
         description="Value of the local defect.",
     )
-    transitionDuration: PositiveFloat = Field(
-        default=None,
-        title="Transition Duration",
-        description=(
-            "Transition duration of the local defect. If not given, the transition will"
-            " be instantly."
-        ),
-    )
-    whichPancakeCoil: PositiveInt = Field(
-        default=None,
-        title="Pancake Coil Number",
-        description="The first pancake coil is 1, the second is 2, etc.",
-    )
     startTurn: NonNegativeFloat = Field(
-        default=None,
         alias="startTurn",
         title="Start Turn",
         description="Start turn of the local defect.",
     )
     endTurn: PositiveFloat = Field(
-        default=None,
         alias="endTurn",
         title="End Turn",
         description="End turn of the local defect.",
     )
+
     startTime: NonNegativeFloat = Field(
-        default=None,
         alias="startTime",
         title="Start Time",
         description="Start time of the local defect.",
     )
 
-    # To be calculated:
-    zTop: float = Field(
-        default=None,
-        description="z-coordinate of the top of the pancake coil (calculated by FiQuS)",
-    )
-    zBottom: float = Field(
-        default=None,
+    # Optionals:
+    transitionDuration: NonNegativeFloat = Field(
+        default=0,
+        title="Transition Duration",
         description=(
-            "z-coordinate of the bottom of the pancake coil (calculated by FiQuS)"
+            "Transition duration of the local defect. If not given, the transition will"
+            " be instantly."
         ),
     )
+    whichPancakeCoil: Optional[PositiveInt] = Field(
+        default=None,
+        title="Pancake Coil Number",
+        description="The first pancake coil is 1, the second is 2, etc.",
+    )
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
+    @field_validator("startTime")
     @classmethod
-    def check_turns(cls, values):
-        """
-        Checks if the start turn is smaller than the end turn.
+    def updateGlobalBreakPointsList(cls, startTime):
+        all_break_points.append(startTime)
+        return startTime
 
-        :param values: dictionary of local defect
-        :type values: dict
-        :return: dictionary of local defect
-        :rtype: dict
-        """
-        if values["startTurn"] is not None:
-            if values["startTurn"] > values["endTurn"]:
-                raise ValueError("The start turn can not be greater than the end turn!")
-
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def check_entries(cls, values):
-        # Check if all of them None first:
-        AllNone = True
-        for key, value in values.items():
-            if value is not None:
-                AllNone = False
-                break
-        if not AllNone:
-            optionalEntries = ["transitionDuration", "zTop", "zBottom"]
-            for key, value in values.items():
-                if value is None and key not in optionalEntries:
-                    raise ValueError(
-                        f'"{key}" entry of the local defect must be specified!'
-                    )
+    @field_validator("startTime")
+    @classmethod
+    def check_start_time(cls, startTime):
+        solve = solve_input.get()
+        start_time = solve["time"]["start"]
+        end_time = solve["time"]["end"]
+
+        if startTime < start_time or startTime > end_time:
+            raise ValueError(
+                "Start time of the local defect should be between the start and end"
+                " times!"
+            )
+        
+        return startTime
+
+    @field_validator("endTurn")
+    @classmethod
+    def check_end_turn(cls, endTurn, info: ValidationInfo):
+        geometry = geometry_input.get()
+
+        if endTurn > geometry["winding"]["numberOfTurns"]:
+            raise ValueError(
+                "End turn of the local defect can't be greater than the number of"
+                " turns!"
+            )
 
-        return values
+        if endTurn < info.data["startTurn"]:
+            raise ValueError(
+                "End turn of the local defect can't be smaller than the start turn!"
+            )
+
+        return endTurn
+
+    @field_validator("whichPancakeCoil")
+    @classmethod
+    def check_which_pancake_coil(cls, whichPancakeCoil):
+        geometry = geometry_input.get()
+
+        if whichPancakeCoil is None:
+            if geometry["numberOfPancakes"] == 1:
+                whichPancakeCoil = 1
+            else:
+                raise ValueError(
+                    "whickPancakeCoil (pancake coil number) should be given if there"
+                    " are more than one pancake coil!"
+                )
+            
+        return whichPancakeCoil
+
+    @computed_field
+    @cached_property
+    def zTop(self) -> float:
+        """Return the z-coordinate of the top of the pancake coil."""
+        geometry = geometry_input.get()
+
+        zTop = self.zBottom + geometry["winding"]["height"]
+
+        return zTop
+
+    @computed_field
+    @cached_property
+    def zBottom(self) -> float:
+        """Return the z-coordinate of the bottom of the pancake coil."""
+        geometry = geometry_input.get()
+
+        if not self.whichPancakeCoil:
+            self.whichPancakeCoil = 1
+
+        zBottom = -(
+            geometry["numberOfPancakes"] * geometry["winding"]["height"]
+            + (geometry["numberOfPancakes"] - 1)
+            * geometry["gapBetweenPancakes"]
+        ) / 2 + (self.whichPancakeCoil - 1) * (
+            geometry["winding"]["height"] + geometry["gapBetweenPancakes"]
+        )
+
+        return zBottom
 
 
 class Pancake3DSolveLocalDefects(BaseModel):
     # 1) User inputs:
 
-    jCritical: Pancake3DSolveLocalDefect = Field(
-        default=Pancake3DSolveLocalDefect(),
+    jCritical: Optional[Pancake3DSolveLocalDefect] = Field(
+        default=None,
         alias="criticalCurrentDensity",
         title="Local Defect for Critical Current Density",
         description="Set critical current density locally.",
     )
 
+    @field_validator("jCritical")
+    @classmethod
+    def check_jCritical_local_defect(cls, jCritical):
+        if jCritical is not None:
+            solve = solve_input.get()
+
+            if "material" in solve["winding"]:
+                windingMaterials = [
+                    material["name"] for material in solve["winding"]["material"]
+                ]
+            else:
+                windingMaterials = []
+
+            superconducting_material_is_used = "HTSSuperPower" in windingMaterials
 
-class Pancake3DSolveSaveQuantity(BaseModel):
-    # 1) User inputs:
+            if not superconducting_material_is_used:
+                raise ValueError(
+                    "Local defects can only be set if superconducting material is used!"
+                )
+            
+        return jCritical
 
+
+class Pancake3DSolveQuantityBase(BaseModel):
     # Mandatory:
-    quantity: Literal[
-        "magneticField",
-        "magnitudeOfMagneticField",
-        "currentDensity",
-        "magnitudeOfCurrentDensity",
-        "resistiveHeating",
-        "temperature",
-        "voltageBetweenTerminals",
-        "currentThroughCoil",
-        "criticalCurrentDensity",
-        "heatFlux",
-        "resistivity",
-        "thermalConductivity",
-        "specificHeatCapacity",
-        "jHTSOverjCritical",
-        "criticalCurrent",
-        "magneticEnergy",
-    ] = Field(
+    quantity: PositionNotRequiredQuantityName | PositionRequiredQuantityName = Field(
         title="Quantity",
         description="Name of the quantity to be saved.",
     )
 
+    @computed_field
+    @cached_property
+    def getdpQuantityName(self) -> str:
+        """Return the GetDP name of the quantity."""
+        if self.quantity not in getdpQuantityNames:
+            raise ValueError(f"Quantity '{self.quantity}' is not defined in FiQuS!")
+
+        return getdpQuantityNames[self.quantity]
+
+    @computed_field
+    @cached_property
+    def getdpPostOperationName(self) -> str:
+        """Return the GetDP name of the post operation."""
+        if self.quantity not in getdpPostOperationNames:
+            raise ValueError(f"Quantity '{self.quantity}' is not defined in FiQuS!")
+
+        return getdpPostOperationNames[self.quantity]
+
+
+class Pancake3DSolveSaveQuantity(Pancake3DSolveQuantityBase):
     # Optionals:
-    timesToBeSaved: List[float] = Field(
-        default=None,
+    timesToBeSaved: list[float] = Field(
+        default=[],
         title="Times to be Saved",
         description=(
             "List of times that wanted to be saved. If not given, all the time steps"
             " will be saved."
         ),
     )
 
-    # 2) To be calculated:
-    getdpQuantityName: str = Field(
-        default=None,
-        description="name of the quantity name in GetDP (calculated by FiQuS)",
-    )
-    getdpPostOperationName: str = Field(
-        default=None,
-        description="name of the post operation in GetDP (calculated by FiQuS)",
-    )
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
+    @field_validator("timesToBeSaved")
     @classmethod
-    def assign_getdp_names(cls, values):
-        """ """
-        quantityNames = {
-            "magneticField": "RESULT_magneticField",
-            "magnitudeOfMagneticField": "RESULT_magnitudeOfMagneticField",
-            "currentDensity": "RESULT_currentDensity",
-            "magnitudeOfCurrentDensity": "RESULT_magnitudeOfCurrentDensity",
-            "resistiveHeating": "RESULT_resistiveHeating",
-            "temperature": "RESULT_temperature",
-            "currentThroughCoil": "RESULT_currentThroughCoil",
-            "voltageBetweenTerminals": "RESULT_voltageBetweenTerminals",
-            "criticalCurrentDensity": "RESULT_criticalCurrentDensity",
-            "heatFlux": "RESULT_heatFlux",
-            "resistivity": "RESULT_resistivity",
-            "thermalConductivity": "RESULT_thermalConductivity",
-            "specificHeatCapacity": "RESULT_specificHeatCapacity",
-            "jHTSOverjCritical": "RESULT_jHTSOverjCritical",
-            "criticalCurrent": "RESULT_criticalCurrent",
-            "debug": "RESULT_debug",
-            "magneticEnergy": "RESULT_magneticEnergy",
-        }
-        postOperationNames = {
-            "magneticField": "POSTOP_magneticField",
-            "magnitudeOfMagneticField": "POSTOP_magnitudeOfMagneticField",
-            "currentDensity": "POSTOP_currentDensity",
-            "magnitudeOfCurrentDensity": "POSTOP_magnitudeOfCurrentDensity",
-            "resistiveHeating": "POSTOP_resistiveHeating",
-            "temperature": "POSTOP_temperature",
-            "currentThroughCoil": "POSTOP_currentThroughCoil",
-            "voltageBetweenTerminals": "POSTOP_voltageBetweenTerminals",
-            "criticalCurrentDensity": "POSTOP_criticalCurrentDensity",
-            "heatFlux": "POSTOP_heatFlux",
-            "resistivity": "POSTOP_resistivity",
-            "thermalConductivity": "POSTOP_thermalConductivity",
-            "specificHeatCapacity": "POSTOP_specificHeatCapacity",
-            "jHTSOverjCritical": "POSTOP_jHTSOverjCritical",
-            "criticalCurrent": "POSTOP_criticalCurrent",
-            "debug": "POSTOP_debug",
-            "magneticEnergy": "POSTOP_magneticEnergy",
-        }
+    def updateGlobalBreakPointsList(cls, timesToBeSaved):
+        all_break_points.extend(timesToBeSaved)
+        return timesToBeSaved
 
-        values["getdpQuantityName"] = quantityNames[values["quantity"]]
-        values["getdpPostOperationName"] = postOperationNames[values["quantity"]]
+    @field_validator("timesToBeSaved")
+    @classmethod
+    def check_times_to_be_saved(cls, timesToBeSaved):
+        solve = solve_input.get()
+        start_time = solve["time"]["start"]
+        end_time = solve["time"]["end"]
 
-        return values
+        for time in timesToBeSaved:
+            if time < start_time or time > end_time:
+                raise ValueError(
+                    "Times to be saved should be between the start and end times!"
+                )
+            
+        return timesToBeSaved
 
 
 # ======================================================================================
 # SOLVE CLASSES ENDS ===================================================================
 # ======================================================================================
 
 # ======================================================================================
-# POSTPROCESS CLASSES STARTS ==============================================================
+# POSTPROCESS CLASSES STARTS ===========================================================
 # ======================================================================================
 
 
-class Pancake3DPostprocessTimeSeriesPlot(BaseModel):
-    # 1) User inputs:
+class Pancake3DPostprocessTimeSeriesPlotBase(Pancake3DSolveQuantityBase):
+    # Mandatory:
+    quantity: str
+
+    @computed_field
+    @cached_property
+    def fileName(self) -> str:
+        """Return the name of the file to be saved."""
+        return f"{self.quantity}(TimeSeriesPlot)"
+
+    @computed_field
+    @cached_property
+    def quantityProperName(self) -> str:
+        """Return the proper name of the quantity."""
+        if self.quantity not in quantityProperNames:
+            raise ValueError(
+                f"Quantity '{self.quantity}'s proper name is not defined! Please"
+                ' update the dictionary "quantityProperNames" in the file'
+                ' "fiqus/data/DataFiQuSPancake3D.py".'
+            )
+
+        return quantityProperNames[self.quantity]
+
+    @computed_field
+    @cached_property
+    def units(self) -> str:
+        """Return the units of the quantity."""
+        if self.quantity not in quantityUnits:
+            raise ValueError(
+                f"Quantity '{self.quantity}'s units are not defined! Please update"
+                ' the dictionary "quantityUnits" in the file'
+                ' "fiqus/data/DataFiQuSPancake3D.py".'
+            )
+
+        return quantityUnits[self.quantity]
+
+
+class Pancake3DPostprocessTimeSeriesPlotPositionRequired(
+    Pancake3DPostprocessTimeSeriesPlotBase
+):
+    # Mandatory:
+    quantity: PositionRequiredQuantityName = Field(
+        title="Quantity",
+        description="Name of the quantity to be plotted.",
+    )
 
     position: Pancake3DPosition = Field(
-        default=Pancake3DPosition(),
         title="Probing Position",
         description="Probing position of the quantity for time series plot.",
     )
-    quantity: Literal[
-        "magnitudeOfMagneticField",
-        "temperature",
-        "magnitudeOfCurrentDensity",
-        "resistiveHeating",
-        "axialComponentOfTheMagneticField",
-        "totalResistiveHeating",
-        "voltageBetweenTerminals",
-        "currentThroughCoil",
-        "magnitudeOfHeatFlux",
-        "resistivity",
-        "derivativeOfRhoWithRespectToJ",
-        "magneticEnergy",
-    ] = Field(
-        default=None,
+
+
+class Pancake3DPostprocessTimeSeriesPlotPositionNotRequired(
+    Pancake3DPostprocessTimeSeriesPlotBase
+):
+    # Mandatory:
+    quantity: PositionNotRequiredQuantityName = Field(
         title="Quantity",
         description="Name of the quantity to be plotted.",
     )
 
-    # 2) To be calculated:
-    fileName: str = Field(
-        default=None,
-        description="name of the file to be saved (calculated by FiQuS)",
-    )
-    quantityProperName: str = Field(
-        default=None,
-        description="proper name of the quantity (calculated by FiQuS)",
-    )
-    getdpQuantityName: str = Field(
-        default=None,
-        description="name of the quantity name in GetDP (calculated by FiQuS)",
-    )
-    units: str = Field(
-        default=None,
-        description="units of the quantity (calculated by FiQuS)",
-    )
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def assign_names(cls, values):
-        quantityNames = {
-            "magnitudeOfMagneticField": "RESULT_magnitudeOfMagneticField",
-            "temperature": "RESULT_temperature",
-            "magnitudeOfCurrentDensity": "RESULT_magnitudeOfCurrentDensity",
-            "resistiveHeating": "RESULT_resistiveHeating",
-            "axialComponentOfTheMagneticField": (
-                "RESULT_axialComponentOfTheMagneticField"
-            ),
-            "totalResistiveHeating": "RESULT_totalResistiveHeating",
-            "voltageBetweenTerminals": "RESULT_voltageBetweenTerminals",
-            "currentThroughCoil": "RESULT_currentThroughCoil",
-            "magnitudeOfHeatFlux": "RESULT_magnitudeOfHeatFlux",
-            "resistivity": "RESULT_resistivity",
-            "derivativeOfRhoWithRespectToJ": "RESULT_derivativeOfRhoWithRespectToJ",
-            "magneticEnergy": "RESULT_magneticEnergy",
-        }
-        units = {
-            "magnitudeOfMagneticField": "T",
-            "temperature": "K",
-            "magnitudeOfCurrentDensity": "A/m^2",
-            "resistiveHeating": "W/m^3",
-            "axialComponentOfTheMagneticField": "T",
-            "totalResistiveHeating": "W",
-            "voltageBetweenTerminals": "V",
-            "currentThroughCoil": "A",
-            "magnitudeOfHeatFlux": "W/m^2",
-            "resistivity": "Ohm*m",
-            "derivativeOfRhoWithRespectToJ": "Ohm*m^3/A",
-            "magneticEnergy": "J",
-        }
-        properNames = {
-            "magnitudeOfMagneticField": "Magnitude of the Magnetic Field",
-            "temperature": "Temperature",
-            "magnitudeOfCurrentDensity": "Magnitude of the Current Density",
-            "resistiveHeating": "Resistive Heating",
-            "axialComponentOfTheMagneticField": "Axial Component of the Magnetic Field",
-            "totalResistiveHeating": "Total Resistive Heating",
-            "voltageBetweenTerminals": "Voltage Between Terminals",
-            "currentThroughCoil": "Current Through Coil",
-            "magnitudeOfHeatFlux": "Magnitude of the Heat Flux",
-            "resistivity": "Resistivity",
-            "derivativeOfRhoWithRespectToJ": "dRho-dJ",
-            "magneticEnergy": "Magnetic Energy",
-        }
-
-        values["fileName"] = f"{values['quantity']}(TimeSeriesPlot)"
-        values["getdpQuantityName"] = quantityNames[values["quantity"]]
-        values["units"] = units[values["quantity"]]
-        values["quantityProperName"] = properNames[values["quantity"]]
-
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def check_position(cls, values):
-        positionRequiredFor = [
-            "magnitudeOfMagneticField",
-            "temperature",
-            "magnitudeOfCurrentDensity",
-            "resistiveHeating",
-            "axialComponentOfTheMagneticField",
-            "magnitudeOfHeatFlux",
-            "resistivity",
-            "derivativeOfRhoWithRespectToJ",
-        ]
-        if (
-            values["position"].x is None
-            and values["position"].y is None
-            and values["position"].z is None
-            and values["position"].turnNumber is None
-            and values["position"].whichPancakeCoil is None
-        ):
-            if values["quantity"] in positionRequiredFor:
-                raise ValueError(
-                    "Position must be specified for time series plot of"
-                    f" {values['quantity']}!"
-                )
-        else:
-            if values["quantity"] not in positionRequiredFor:
-                logger.warning(
-                    "Position must not be specified for time series plot of"
-                    f" {values['quantity']}, because it's a global scalar quantity!"
-                )
 
-        return values
+Pancake3DPostprocessTimeSeriesPlot = Annotated[
+    Pancake3DPostprocessTimeSeriesPlotPositionRequired
+    | Pancake3DPostprocessTimeSeriesPlotPositionNotRequired,
+    Field(discriminator="quantity"),
+]
 
 
 class Pancake3DPostprocessMagneticFieldOnPlane(BaseModel):
+    # Optional:
     colormap: str = Field(
         default="viridis",
         title="Colormap",
         description="Colormap for the plot.",
     )
     streamLines: bool = Field(
         default=True,
@@ -2017,65 +2346,248 @@
             " vector. Therefore, for smooth 2D plots, interpolation can be"
             " used.\nTypes:\nnearest: it will plot the nearest magnetic field value to"
             " the plotting point.\nlinear: it will do linear interpolation to the"
             " magnetic field values.\ncubic: it will do cubic interpolation to the"
             " magnetic field values."
         ),
     )
-    timesToBePlotted: List[float] = Field(
+    timesToBePlotted: Optional[list[float]] = Field(
         default=None,
         title="Times to be Plotted",
         description=(
             "List of times that wanted to be plotted. If not given, all the time steps"
             " will be plotted."
         ),
     )
-    planeNormal: List[float] = Field(
+    planeNormal: Annotated[list[float], Len(min_length=3, max_length=3)] = Field(
         default=[1, 0, 0],
         title="Plane Normal",
         description="Normal vector of the plane. The default is YZ-plane (1, 0, 0).",
     )
-    planeXAxisUnitVector: List[float] = Field(
-        default=[0, 1, 0],
-        title="Plane X Axis",
-        description=(
-            "If an arbitrary plane is wanted to be plotted, the arbitrary plane's X"
-            " axis unit vector must be specified. The dot product of the plane's X axis"
-            " and the plane's normal vector must be zero."
-        ),
+    planeXAxisUnitVector: Annotated[list[float], Len(min_length=3, max_length=3)] = (
+        Field(
+            default=[0, 1, 0],
+            title="Plane X Axis",
+            description=(
+                "If an arbitrary plane is wanted to be plotted, the arbitrary plane's X"
+                " axis unit vector must be specified. The dot product of the plane's X"
+                " axis and the plane's normal vector must be zero."
+            ),
+        )
     )
 
-    onSection: List[List[float]] = Field(
-        default=None,
-        description="Three corner points of the plane (calculated by FiQuS).",
-    )
+    @field_validator("timesToBePlotted")
+    @classmethod
+    def updateGlobalBreakPointsList(cls, timesToBePlotted):
+        all_break_points.extend(timesToBePlotted)
+        return timesToBePlotted
 
-    @validator("colormap", allow_reuse=True)
+    @field_validator("colormap")
     @classmethod
-    def check_colormap(cls, value):
+    def check_color_map(cls, colorMap):
         """
         Check if the colormap exists.
         """
-        if value not in matplotlib.pyplot.colormaps():
+        if colorMap not in matplotlib.pyplot.colormaps():
             raise ValueError(
-                f"{value} is not a valid colormap! Please see"
+                f"{colorMap} is not a valid colormap! Please see"
                 " https://matplotlib.org/stable/gallery/color/colormap_reference.html"
                 " for available colormaps."
             )
 
-        return value
+        return colorMap
+
+    @computed_field
+    @cached_property
+    def onSection(self) -> list[list[float]]:
+        """Return the three corner points of the plane."""
+
+        class unitVector:
+            def __init__(self, u, v, w) -> None:
+                length = math.sqrt(u**2 + v**2 + w**2)
+                self.u = u / length
+                self.v = v / length
+                self.w = w / length
+
+            def rotate(self, theta, withRespectTo):
+                # Rotate with respect to the withRespectTo vector by theta degrees:
+                # https://en.wikipedia.org/wiki/Rotation_matrix#Rotation_matrix_from_axis_and_angle
+                a = withRespectTo.u
+                b = withRespectTo.v
+                c = withRespectTo.w
+
+                rotationMatrix = np.array(
+                    [
+                        [
+                            math.cos(theta) + a**2 * (1 - math.cos(theta)),
+                            a * b * (1 - math.cos(theta)) - c * math.sin(theta),
+                            a * c * (1 - math.cos(theta)) + b * math.sin(theta),
+                        ],
+                        [
+                            b * a * (1 - math.cos(theta)) + c * math.sin(theta),
+                            math.cos(theta) + b**2 * (1 - math.cos(theta)),
+                            b * c * (1 - math.cos(theta)) - a * math.sin(theta),
+                        ],
+                        [
+                            c * a * (1 - math.cos(theta)) - b * math.sin(theta),
+                            c * b * (1 - math.cos(theta)) + a * math.sin(theta),
+                            math.cos(theta) + c**2 * (1 - math.cos(theta)),
+                        ],
+                    ]
+                )
+                vector = np.array([[self.u], [self.v], [self.w]])
+                rotatedVector = rotationMatrix @ vector
+                return unitVector(
+                    rotatedVector[0][0],
+                    rotatedVector[1][0],
+                    rotatedVector[2][0],
+                )
+
+            def __pow__(self, otherUnitVector):
+                # Cross product:
+                u = self.v * otherUnitVector.w - self.w * otherUnitVector.v
+                v = self.w * otherUnitVector.u - self.u * otherUnitVector.w
+                w = self.u * otherUnitVector.v - self.v * otherUnitVector.u
+                return unitVector(u, v, w)
+
+            def __mul__(self, otherUnitVector) -> float:
+                # Dot product:
+                return (
+                    self.u * otherUnitVector.u
+                    + self.v * otherUnitVector.v
+                    + self.w * otherUnitVector.w
+                )
+
+        planeNormal = unitVector(
+            self.planeNormal[0], self.planeNormal[1], self.planeNormal[2]
+        )
+        planeXAxis = unitVector(
+            self.planeXAxis[0], self.planeXAxis[1], self.planeXAxis[2]
+        )
+
+        if not math.isclose(planeNormal * planeXAxis, 0, abs_tol=1e-8):
+            raise ValueError(
+                "planeNormal and planeXAxis must be perpendicular to each"
+                " other! If planeNormal is chosen arbitrarily, planeXAxis must"
+                " be specified."
+            )
+
+        # A plane that passes through the origin with the normal vector planeNormal
+        # can be defined as:
+        # a*x + b*y + c*z = 0
+        a = planeNormal.u
+        b = planeNormal.v
+        c = planeNormal.w
+
+        # Pick three points on the plane to define a rectangle. The points will
+        # be the corners of the rectangle.
+
+        # To do that, change coordinate system:
+
+        # Find a vector that is perpendicular to planeNormal:
+        randomVector = unitVector(c, a, b)
+        perpendicularVector1 = planeNormal**randomVector
+
+        # Rotate perperndicular vector with respect to the plane's normal vector
+        # by 90 degrees to find the second perpendicular vector:
+        perpendicularVector2 = perpendicularVector1.rotate(math.pi / 2, planeNormal)
+
+        # Build the transformation matrix to change from the plane's coordinate
+        # system to the global coordinate system:
+        transformationMatrix = np.array(
+            [
+                [
+                    perpendicularVector1.u,
+                    perpendicularVector1.v,
+                    perpendicularVector1.w,
+                ],
+                [
+                    perpendicularVector2.u,
+                    perpendicularVector2.v,
+                    perpendicularVector2.w,
+                ],
+                [planeNormal.u, planeNormal.v, planeNormal.w],
+            ]
+        )
+        transformationMatrix = np.linalg.inv(transformationMatrix)
+
+        # Select three points to define the rectangle. Pick large points because
+        # only the intersection of the rectangle and the mesh will be used.
+        geometry = geometry_input.get()
+        if geometry["air"]["type"] == "cuboid":
+            sideLength = geometry["air"]["sideLength"]
+            airMaxWidth = 2 * math.sqrt((sideLength / 2) ** 2 + (sideLength / 2) ** 2)
+        if geometry["air"]["type"] == "cylinder":
+            airMaxWidth = geometry["air"]["radius"]
+
+        airHeight = getAirHeight()
+
+        point1InPlaneCoordinates = np.array(
+            [5 * max(airMaxWidth, airHeight), 5 * max(airMaxWidth, airHeight), 0]
+        )
+        point1 = transformationMatrix @ point1InPlaneCoordinates
+
+        point2InPlaneCoordinates = np.array(
+            [-5 * max(airMaxWidth, airHeight), 5 * max(airMaxWidth, airHeight), 0]
+        )
+        point2 = transformationMatrix @ point2InPlaneCoordinates
+
+        point3InPlaneCoordinates = np.array(
+            [
+                -5 * max(airMaxWidth, airHeight),
+                -5 * max(airMaxWidth, airHeight),
+                0,
+            ]
+        )
+        point3 = transformationMatrix @ point3InPlaneCoordinates
+
+        # Round the point coordinates to the nearest multiple of the dimTol:
+        if "dimTol" in geometry:
+            dimTol = geometry["dimTol"]
+        else:
+            dimTol = 1e-8
+
+        point1[0] = round(point1[0] / dimTol) * dimTol
+        point1[1] = round(point1[1] / dimTol) * dimTol
+        point1[2] = round(point1[2] / dimTol) * dimTol
+        point2[0] = round(point2[0] / dimTol) * dimTol
+        point2[1] = round(point2[1] / dimTol) * dimTol
+        point2[2] = round(point2[2] / dimTol) * dimTol
+        point3[0] = round(point3[0] / dimTol) * dimTol
+        point3[1] = round(point3[1] / dimTol) * dimTol
+        point3[2] = round(point3[2] / dimTol) * dimTol
+
+        onSection = [
+            [float(point1[0]), float(point1[1]), float(point1[2])],
+            [float(point2[0]), float(point2[1]), float(point2[2])],
+            [float(point3[0]), float(point3[1]), float(point3[2])],
+        ]
+
+        return onSection
 
 
 # ======================================================================================
-# POSTPROCESS CLASSES ENDS ================================================================
+# POSTPROCESS CLASSES ENDS =============================================================
 # ======================================================================================
 
 
 class Pancake3DGeometry(BaseModel):
-    # 1) User inputs:
+    # Mandatory:
+    N: PositiveInt = Field(
+        ge=1,
+        alias="numberOfPancakes",
+        title="Number of Pancakes",
+        description="Number of pancake coils stacked on top of each other.",
+    )
+
+    gap: PositiveFloat = Field(
+        alias="gapBetweenPancakes",
+        title="Gap Between Pancakes",
+        description="Gap distance between the pancake coils.",
+    )
 
     wi: Pancake3DGeometryWinding = Field(
         alias="winding",
         title="Winding Geometry",
         description="This dictionary contains the winding geometry information.",
     )
 
@@ -2093,28 +2605,14 @@
 
     ai: Pancake3DGeometryAir = Field(
         alias="air",
         title="Air Geometry",
         description="This dictionary contains the air geometry information.",
     )
 
-    # Mandatory:
-
-    N: PositiveInt = Field(
-        alias="numberOfPancakes",
-        title="Number of Pancakes",
-        description="Number of pancake coils stacked on top of each other.",
-    )
-
-    gap: PositiveFloat = Field(
-        alias="gapBetweenPancakes",
-        title="Gap Between Pancakes",
-        description="Gap distance between the pancake coils.",
-    )
-
     # Optionals:
     dimTol: PositiveFloat = Field(
         default=1e-8,
         alias="dimensionTolerance",
         description="dimension tolerance (CAD related, not physical)",
     )
     pancakeBoundaryName: str = Field(
@@ -2127,62 +2625,29 @@
         default="contactLayerBoundary",
         description=(
             "name of the contact layers's curves that touches the air to be used in the"
             " mesh (only for TSA)"
         ),
     )
 
-    @validator("N", allow_reuse=True)
-    @classmethod
-    def check_N(cls, value):
-        """
-        Checks if the number of pancakes is at least 1.
-
-        :param cls: class
-        :type cls: class
-        :param value: number of pancakes
-        :type value: int
-        :return: number of pancakes
-        :rtype: int
-        """
-        if value < 1:
-            raise ValueError("Number of pancakes must be at least 1!")
-        return value
-
-    @validator("dimTol", allow_reuse=True)
-    @classmethod
-    def check_dimTol(cls, value):
-        """
-        Checks if the dimension tolerance is smaller than 1e-5.
-
-        :param cls: class
-        :type cls: class
-        :param value: dimension tolerance
-        :type value: float
-        :return: dimension tolerance
-        :rtype: float
-        """
-        if value > 1e-5:
-            raise ValueError("Dimension tolerance must be smaller than 1e-5!")
-
-        return value
-
 
 class Pancake3DMesh(BaseModel):
-    # 1) User inputs:
+    # Mandatory:
     wi: Pancake3DMeshWinding = Field(
         alias="winding",
         title="Winding Mesh",
         description="This dictionary contains the winding mesh information.",
     )
     ii: Pancake3DMeshContactLayer = Field(
         alias="contactLayer",
         title="Contact Layer Mesh",
         description="This dictionary contains the contact layer mesh information.",
     )
+
+    # Optionals:
     ti: Pancake3DMeshAirAndTerminals = Field(
         default=Pancake3DMeshAirAndTerminals(),
         alias="terminals",
         title="Terminal Mesh",
         description="This dictionary contains the terminal mesh information.",
     )
     ai: Pancake3DMeshAirAndTerminals = Field(
@@ -2210,87 +2675,146 @@
             "The maximum mesh element size in terms of the largest mesh size in the"
             " winding. This mesh size will be used in the regions close the the"
             " winding, and then the mesh size will increate to maximum mesh element"
             " size as it gets away from the winding."
         ),
     )
 
-    # 2) To be calculated:
-    sizeMin: PositiveFloat = Field(
-        default=None,
-        description=(
-            "minimum mesh element size in real dimensions (calculated by FiQuS)"
-        ),
-    )
-    sizeMax: PositiveFloat = Field(
-        default=None,
-        description=(
-            "maximum mesh element size in real dimensions (calculated by FiQuS)"
-        ),
-    )
-    startGrowingDistance: PositiveFloat = Field(
-        default=None,
-        description=(
-            "distance from the pancake coils to start growing the mesh elements"
-            " (calculated by FiQuS)"
-        ),
-    )
-    stopGrowingDistance: PositiveFloat = Field(
-        default=None,
-        description=(
-            "distance from the pancake coils to stop growing the mesh elements"
-            " (calculated by FiQuS)"
-        ),
-    )
-    theWorstRectangularRatio: PositiveFloat = Field(
-        default=None,
-        description=(
-            "the worst rectangular structured mesh element size ratio (calculated by"
-            " FiQuS)"
-        ),
-    )
-    theWorstTriangularRatio: PositiveFloat = Field(
-        default=None,
-        description=(
-            "the worst triangular structured mesh element size ratio (calculated by"
-            " FiQuS)"
-        ),
-    )
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
+    @field_validator("relSizeMax")
     @classmethod
-    def check_size(cls, values):
-        """
-        Checks if the minimum element size is smaller than the maximum element size.
-
-        :param cls: class
-        :type cls: class
-        :param values: dictionary of mesh
-        :type values: dict
-        :return: dictionary of mesh
-        :rtype: dict
-        """
-        if values["relSizeMin"] > values["relSizeMax"]:
+    def check_rel_size_max(cls, relSizeMax, info: ValidationInfo):
+        if relSizeMax < info.data["relSizeMin"]:
             raise ValueError(
-                "The minimum mesh element size must be smaller than the maximum mesh"
-                " element size!"
+                "Maximum mesh element size (maximumElementSize) cannot be smaller than"
+                " the minimum mesh element size (minimumElementSize)!"
             )
 
-        return values
+        return relSizeMax
+
+    @computed_field
+    @cached_property
+    def sizeMin(self) -> float:
+        """Return the minimum mesh element size in real dimensions."""
+        geometry = geometry_input.get()
+
+        meshLengthsPerElement = []
+
+        # azimuthal elements:
+        for numberOfElements in self.wi.ane:
+            terminalOuterRadius = (
+                getWindingOuterRadius()
+                + 2 * geometry["terminals"]["outer"]["thickness"]
+            )
+            meshLengthsPerElement.append(
+                2 * math.pi * terminalOuterRadius / numberOfElements
+            )
+
+        # radial elements:
+        for numberOfElements in self.wi.rne:
+            meshLengthsPerElement.append(
+                geometry["winding"]["thickness"] / numberOfElements
+            )
+
+        if not geometry["contactLayer"]["thinShellApproximation"]:
+            # radial elements:
+            for numberOfElements in self.ii.rne:
+                meshLengthsPerElement.append(
+                    geometry["contactLayer"]["thickness"] / numberOfElements
+                )
+
+        # axial elements:
+        for numberOfElements in self.wi.axne:
+            meshLengthsPerElement.append(
+                geometry["winding"]["height"] / numberOfElements
+            )
+
+        return max(meshLengthsPerElement) * self.relSizeMin
+
+    @computed_field
+    @cached_property
+    def sizeMax(self) -> float:
+        """Return the minimum mesh element size in real dimensions."""
+        geometry = geometry_input.get()
+
+        meshLengthsPerElement = []
+
+        # azimuthal elements:
+        for numberOfElements in self.wi.ane:
+            terminalOuterRadius = (
+                getWindingOuterRadius()
+                + 2 * geometry["terminals"]["outer"]["thickness"]
+            )
+            meshLengthsPerElement.append(
+                2 * math.pi * terminalOuterRadius / numberOfElements
+            )
+
+        # radial elements:
+        for numberOfElements in self.wi.rne:
+            meshLengthsPerElement.append(
+                geometry["winding"]["thickness"] / numberOfElements
+            )
+
+        if not geometry["contactLayer"]["thinShellApproximation"]:
+            # radial elements:
+            for numberOfElements in self.ii.rne:
+                meshLengthsPerElement.append(
+                    geometry["contactLayer"]["thickness"] / numberOfElements
+                )
+
+        # axial elements:
+        for numberOfElements in self.wi.axne:
+            meshLengthsPerElement.append(
+                geometry["winding"]["height"] / numberOfElements
+            )
+
+        return max(meshLengthsPerElement) * self.relSizeMax
+
+    @computed_field
+    @cached_property
+    def stopGrowingDistance(self) -> float:
+        """Return the distance from the pancake coils to start growing the mesh elements."""
+        geometry = geometry_input.get()
+        terminalOuterRadius = (
+            getWindingOuterRadius() + 2 * geometry["terminals"]["outer"]["thickness"]
+        )
+
+        if geometry["air"]["type"] == "cuboid":
+            sideLength = geometry["air"]["sideLength"]
+            stopGrowingDistance = sideLength / 2 - terminalOuterRadius
+        if geometry["air"]["type"] == "cylinder":
+            stopGrowingDistance = geometry["air"]["radius"] - terminalOuterRadius
+
+        return stopGrowingDistance
+
+    @computed_field
+    @cached_property
+    def startGrowingDistance(self) -> float:
+        geometry = geometry_input.get()
+        terminalOuterRadius = (
+            getWindingOuterRadius() + 2 * geometry["terminals"]["outer"]["thickness"]
+        )
+        terminalInnerRadius = (
+            geometry["winding"]["innerRadius"]
+            - 2 * geometry["terminals"]["inner"]["thickness"]
+        )
+
+        startGrowingDistance = (terminalOuterRadius - terminalInnerRadius) / 2
+
+        return startGrowingDistance
 
 
 class Pancake3DSolve(BaseModel):
     # 1) User inputs:
     t: Pancake3DSolveTime = Field(
         alias="time",
         title="Time Settings",
         description="All the time related settings for transient analysis.",
     )
 
-    nls: Pancake3DSolveNonlinearSolverSettings = Field(
+    nls: Optional[Pancake3DSolveNonlinearSolverSettings] = Field(
         alias="nonlinearSolver",
         title="Nonlinear Solver Settings",
         description="All the nonlinear solver related settings.",
     )
 
     wi: Pancake3DSolveWindingMaterial = Field(
         alias="winding",
@@ -2318,33 +2842,33 @@
 
     ic: Pancake3DSolveInitialConditions = Field(
         alias="initialConditions",
         title="Initial Conditions",
         description="Initial conditions of the problem.",
     )
 
-    save: List[Pancake3DSolveSaveQuantity] = Field(
+    save: list[Pancake3DSolveSaveQuantity] = Field(
         alias="quantitiesToBeSaved",
         default=None,
         title="Quantities to be Saved",
         description="List of quantities to be saved.",
     )
 
     # Mandatory:
-    type: Literal[
-        "electromagnetic", "thermal", "weaklyCoupled", "stronglyCoupled"
-    ] = Field(
-        title="Simulation Type",
-        description=(
-            "FiQuS/Pancake3D can solve only electromagnetics and thermal or"
-            " electromagnetic and thermal coupled. In the weaklyCoupled setting,"
-            " thermal and electromagnetics systems will be put into different"
-            " matrices, whereas in the stronglyCoupled setting, they all will be"
-            " combined into the same matrix. The solution should remain the same."
-        ),
+    type: Literal["electromagnetic", "thermal", "weaklyCoupled", "stronglyCoupled"] = (
+        Field(
+            title="Simulation Type",
+            description=(
+                "FiQuS/Pancake3D can solve only electromagnetics and thermal or"
+                " electromagnetic and thermal coupled. In the weaklyCoupled setting,"
+                " thermal and electromagnetics systems will be put into different"
+                " matrices, whereas in the stronglyCoupled setting, they all will be"
+                " combined into the same matrix. The solution should remain the same."
+            ),
+        )
     )
 
     # Optionals:
     proTemplate: str = Field(
         default="Pancake3D_template.pro",
         description="file name of the .pro template file",
     )
@@ -2375,262 +2899,66 @@
         description=(
             "If True, the DoF along the axial direction will be equated. This means"
             " that the temperature will be the same along the axial direction reducing"
             " the number of DoF. This is only valid for the thermal analysis."
         ),
     )
 
-    # 2) To be calculated:
-    systemsOfEquationsType: Literal["linear", "nonlinear"] = Field(
-        default=None, description="(calculated by FiQuS)"
-    )
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def find_system_type(cls, values):
-        values["systemsOfEquationsType"] = "linear"
-        listOfGeometryParts = ["wi", "ii", "ti"]
-
-        for geometryPart in listOfGeometryParts:
-            if values["type"] == "electromagnetic":
-                if (
-                    not isinstance(values[geometryPart].resistivity, float)
-                    and values[geometryPart].resistivity != "perfectlyInsulating"
-                ):
-                    values["systemsOfEquationsType"] = "nonlinear"
-
-                    if values["ic"].T is None:
-                        raise ValueError(
-                            "Initial temperature must be specified if nonlinear"
-                            " materials are used because of the temperature dependency"
-                            " of the resistivity!"
-                        )
-            elif values["type"] == "thermal":
-                if not isinstance(
-                    values[geometryPart].thermalConductivity, float
-                ) or not isinstance(values[geometryPart].specificHeatCapacity, float):
-                    values["systemsOfEquationsType"] = "nonlinear"
-
-                    if values["ic"].T is None:
-                        raise ValueError(
-                            "Initial temperature must be specified if nonlinear"
-                            " materials are used because of the temperature dependency"
-                            " of the thermal conductivity and specific heat capacity!"
-                        )
-
-            else:
-                if (
-                    (
-                        not isinstance(values[geometryPart].resistivity, float)
-                        and values[geometryPart].resistivity != "perfectlyInsulating"
-                    )
-                    or not isinstance(values[geometryPart].thermalConductivity, float)
-                    or not isinstance(values[geometryPart].specificHeatCapacity, float)
-                ):
-                    values["systemsOfEquationsType"] = "nonlinear"
-
-                    if values["ic"].T is None:
-                        raise ValueError(
-                            "Initial temperature must be specified if nonlinear"
-                            " materials are used because of the temperature dependency"
-                            " of the resistivity, thermal conductivity and specific"
-                            " heat capacity!"
-                        )
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def check_tolerances(cls, values):
-        electromagneticRequiredTolerances = [
-            "totalResistiveHeating",
-            "voltageBetweenTerminals",
-            "resistiveHeating",
-            "currentDensity",
-            "magnitudeOfMagneticField",
-            "axialComponentOfTheMagneticField",
-            "magneticEnergy",
-        ]
-        thermalRequiredTolerances = ["temperature", "magnitudeOfHeatFlux"]
-
-        allTolerances = []
-        allTolerances.extend(values["nls"].tolerances)
-        allTolerances.extend(values["t"].adaptive.tolerances)
-
-        if values["type"] == "thermal":
-            # Then totalResistiveHeating is not a valid tolerance:
-            for tolerance in allTolerances:
-                if tolerance.quantity in electromagneticRequiredTolerances:
-                    raise ValueError(
-                        f"{tolerance.quantity} is not a valid tolerance if the type"
-                        " is thermal!"
-                    )
-        elif values["type"] == "electromagnetic":
-            for tolerance in allTolerances:
-                if tolerance.quantity in thermalRequiredTolerances:
-                    raise ValueError(
-                        f"{tolerance.quantity} is not a valid tolerance if the type"
-                        " is electromagnetic!"
-                    )
-
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def check_times_to_be_saved(cls, values):
-        """ """
-
-        # Check if the times to be saved are between start and end times:
-        allTimesToBeSaved = set()
-        if values["save"]:
-            for saveQuantity in values["save"]:
-                if saveQuantity.timesToBeSaved:
-                    for time in saveQuantity.timesToBeSaved:
-                        if time < values["t"].start or time > values["t"].end:
-                            raise ValueError(
-                                f"Time {time:.5f} in the timesToBeSaved list is not"
-                                " between start and end times!"
-                            )
-
-                        allTimesToBeSaved.add(time)
-
-        if values["localDefects"]:
-            if values["localDefects"].jCritical:
-                if values["localDefects"].jCritical.startTime:
-                    if (
-                        values["localDefects"].jCritical.startTime > values["t"].start
-                        and values["localDefects"].jCritical.startTime < values["t"].end
-                    ):
-                        allTimesToBeSaved.add(
-                            values["localDefects"].jCritical.startTime
-                        )
-
-            allTimesToBeSaved = list(allTimesToBeSaved)
-
-        if values["t"].timeSteppingType == "adaptive":
-            # Add all times to be saved to the break points list:
-            for timeToBeSaved in allTimesToBeSaved:
-                values["t"].adaptive.breakPoints.append(timeToBeSaved)
-
-            values["t"].adaptive.breakPoints = list(
-                set(values["t"].adaptive.breakPoints)
-            )
-            values["t"].adaptive.breakPoints.sort()
-
-            if len(values["t"].adaptive.breakPoints) == 1:
-                values["t"].adaptive.breakPoints = []
-
-        elif values["t"].timeSteppingType == "fixed":
-            # Check if all times to be saved are multiples of the time step:
-            for timeToBeSaved in allTimesToBeSaved:
-                for interval in values["t"].fixed:
-                    if (
-                        timeToBeSaved >= interval.startTime
-                        and timeToBeSaved <= interval.endTime
-                    ):
-                        startTime = interval.startTime
-                        timeStep = interval.step
-                if (
-                    math.fmod(timeToBeSaved - startTime, timeStep) > 1e-8
-                    and math.fmod(timeToBeSaved - startTime, timeStep) - timeStep
-                    < -1e-8
-                ):
-                    raise ValueError(
-                        f"A time value ({timeToBeSaved}) in the timesToBeSaved list is"
-                        " not multiples of the time step!"
-                    )
-
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def check_local_defects(cls, values):
-        """ """
-        if not values["wi"].superConductor or values["wi"].resistivity:
-            if values["localDefects"].jCritical.value is not None:
-                raise ValueError(
-                    "Critical current density local defect cannot be defined if"
-                    " winding does not have superconductivity!"
-                )
-
-        if values["type"] in "thermal":
-            if values["localDefects"].jCritical.value:
-                raise ValueError(
-                    "Critical current density local defect cannot be defined if the"
-                    " simulation type is thermal!"
-                )
-
-        return values
+    @computed_field
+    @cached_property
+    def systemsOfEquationsType(self) -> str:
+
+        windingMaterialIsGiven = self.wi.material is not None
+        contactLayerMaterialIsGiven = self.ii.material is not None
+        terminalMaterialIsGiven = self.ti.material is not None
+        notchMaterialIsGiven = self.ti.transitionNotch.material is not None
+        terminalContactLayerMaterialIsGiven = self.ti.terminalContactLayer.material is not None
 
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def check_quantities_to_be_saved(cls, values):
-        """ """
-        if values["save"]:
-            for saveQuantity in values["save"]:
-                if saveQuantity.quantity == "criticalCurrentDensity":
-                    if not values["wi"].superConductor or values["wi"].resistivity:
-                        raise ValueError(
-                            "Critical current density cannot be saved if winding does"
-                            " not have superconductivity!"
-                        )
-
-            if values["type"] == "electromagnetic":
-                for saveQuantity in values["save"]:
-                    if saveQuantity.quantity in ["temperature", "heatFlux"]:
-                        raise ValueError(
-                            "Temperature cannot be saved if the type is electromagnetic"
-                            " because it is not calculated!"
-                        )
-            elif values["type"] == "thermal":
-                for saveQuantity in values["save"]:
-                    if saveQuantity.quantity in [
-                        "magneticField",
-                        "magnitudeOfMagneticField",
-                        "currentDensity",
-                        "magnitudeOfCurrentDensity",
-                        "resistiveHeating",
-                        "criticalCurrentDensity",
-                    ]:
-                        raise ValueError(
-                            "Magnetic field, current density and resistive heating"
-                            " cannot be saved if the type is thermal because they are"
-                            " not calculated!"
-                        )
+        if (
+            windingMaterialIsGiven
+            or contactLayerMaterialIsGiven
+            or terminalMaterialIsGiven
+            or notchMaterialIsGiven
+            or terminalContactLayerMaterialIsGiven
+        ):
+            systemsOfEquationsType = "nonlinear"
+        else:
+            systemsOfEquationsType = "linear"
 
-        return values
+        return systemsOfEquationsType
 
 
 class Pancake3DPostprocess(BaseModel):
     """
     TO BE UPDATED
     """
 
     # 1) User inputs:
-    timeSeriesPlots: List[Pancake3DPostprocessTimeSeriesPlot] = Field(
+    timeSeriesPlots: list[Pancake3DPostprocessTimeSeriesPlot] = Field(
         default=None,
         title="Time Series Plots",
         description="Values can be plotted with respect to time.",
     )
 
-    magneticFieldOnCutPlane: Pancake3DPostprocessMagneticFieldOnPlane = Field(
+    magneticFieldOnCutPlane: Optional[Pancake3DPostprocessMagneticFieldOnPlane] = Field(
         default=None,
         title="Magnetic Field on a Cut Plane",
         description=(
             "Color map of the magnetic field on the YZ plane can be plotted with"
             " streamlines."
         ),
     )
 
 
 class Pancake3D(BaseModel):
     """
     Level 1: Class for FiQuS Pancake3D
     """
 
-    type: Literal["Pancake3D"] = "Pancake3D"
+    type: Literal["Pancake3D"]
     geometry: Pancake3DGeometry = Field(
         default=None,
         title="Geometry",
         description="This dictionary contains the geometry information.",
     )
     mesh: Pancake3DMesh = Field(
         default=None,
@@ -2649,1300 +2977,49 @@
     )
     input_file_path: str = Field(
         default=None,
         description="path of the input file (calculated by FiQuS)",
         exclude=True,
     )
 
-    # skip_on_failure = True is used to make sure the submodels are validated.
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def geometry_calculations_and_checks(cls, values):
-        """
-        This function calculates the geometry parameters and checks if the user inputs
-        are valid.
-
-        :param cls: class
-        :type cls: class
-        :param values: dictionary of PC3D
-        :type values: dict
-        :return: dictionary of PC3D
-        :rtype: dict
-        """
-        # ==============================================================================
-        # CALCULATIONS STARTS ==========================================================
-        # ==============================================================================
-        geo = values["geometry"]
-        mesh = values["mesh"]
-
-        # Calculate outer radius of the coil:
-        geo.wi.r_o = geo.wi.r_i + geo.wi.t + geo.wi.N * (geo.wi.t + geo.ii.t)
-
-        # Calculate the total tape length of the coil:
-
-        # The same angle can be subtracted from both theta_1 and theta_2 to simplify the
-        # calculations:
-        theta2 = geo.wi.N * 2 * math.pi
-        theta1 = 0
-
-        # Since r = a * theta + b, r_1 = b since theta_1 = 0:
-        b = geo.wi.r_i
-
-        # Since r = a * theta + b, r_2 = a * theta2 + b:
-        a = (geo.wi.r_o - b) / theta2
-
-        def integrand(t):
-            return math.sqrt(a**2 + (a * t + b) ** 2)
-
-        geo.wi.totalTapeLength = abs(scipy.integrate.quad(integrand, theta1, theta2)[0])
-
-        # Calculate the turn tolerance required due to the geometry input:
-        # Turn tolerance is the smallest turn angle (in turns) that is allowed.
-        turnTol = geo.wi.N % 1
-        if math.isclose(turnTol, 0, abs_tol=geo.dimTol):
-            turnTol = 0.5
-
-        # Calculate the minimum turn tolerance possible due to the mesh input:
-        if not isinstance(mesh.wi.ane, list):
-            mesh.wi.ane = [mesh.wi.ane] * geo.N
-
-        minimumTurnTol = 1 / min(mesh.wi.ane)
-
-        if turnTol < minimumTurnTol:
-            numberOfTurns = geo.wi.N
-
-            raise ValueError(
-                "The azimuthal number of elements per turn for one of the pancakes is"
-                f" {min(mesh.wi.ane)}, and the number of turns is {numberOfTurns:.5f}."
-                " The number of turns must always be divisible by the (1/(the"
-                " azimuthal number of elements per turn)) to ensure conformality."
-                " Please change the number of turns or the azimuthal number of"
-                " elemenets per turn. The closest possible number of turns value is"
-                f" {round(numberOfTurns * min(mesh.wi.ane))/min(mesh.wi.ane):.5f}"
-            )
-        else:
-            # Minimum possible sections per turn is 16 (otherwise splines might collide
-            # into each other). But it should be greater than the number of volumes per
-            # turn and it should be divisible by both 1/turnTol and the number of
-            # volumes per turn.
-            sectionsPerTurn = 16
-            while (
-                (
-                    math.fmod(sectionsPerTurn, (1 / turnTol)) > 1e-8
-                    and math.fmod(sectionsPerTurn, (1 / turnTol)) - (1 / turnTol)
-                    < -1e-8
-                )
-                or sectionsPerTurn % geo.wi.NofVolPerTurn != 0
-                or sectionsPerTurn < geo.wi.NofVolPerTurn
-            ):
-                sectionsPerTurn += 1
-
-            geo.wi.spt = sectionsPerTurn
-
-            # Sections per turn will set the turn tolerance value as well.
-            geo.wi.turnTol = 1 / sectionsPerTurn
-
-        # Check if the NofVolPerTurn is compatible swith the azimuthal number of elements
-        # per turn:
-        if not isinstance(mesh.wi.ane, list):
-            mesh.wi.ane = [mesh.wi.ane] * geo.N
-
-        for i, ane in enumerate(mesh.wi.ane):
-            if ane % geo.wi.NofVolPerTurn != 0:
-                raise ValueError(
-                    "The azimuthal number of elements per turn for the pancake coil"
-                    f" number {i+1} is ({ane}), but it must be divisible by the number"
-                    f" of volumes per turn ({geo.wi.NofVolPerTurn})! So it needs to be"
-                    " rounded to"
-                    f" {math.ceil(ane/geo.wi.NofVolPerTurn)*geo.wi.NofVolPerTurn:.5f} or"
-                    f" {math.floor(ane/geo.wi.NofVolPerTurn)*geo.wi.NofVolPerTurn:.5f}."
-                )
-
-        # Calculate terminal radiuses:
-        geo.ti.i.r = geo.wi.r_i - 2 * geo.ti.i.t
-        if geo.ti.i.r < 0:
-            raise ValueError(
-                "Inner terminal's radius is smaller than 0! Please decrease the inner"
-                " terminal's thickness or increase the winding's inner radius."
-            )
-
-        geo.ti.o.r = geo.wi.r_o + 2 * geo.ti.o.t
-
-        # Calculate the total height of air:
-        geo.ai.h = geo.N * (geo.wi.h + geo.gap) - geo.gap + geo.ai.margin * 2
-
-        # ==============================================================================
-        # CALCULATIONS ENDS ============================================================
-        # ==============================================================================
-
-        # =============================================================================
-        # CHECKING TERMINALS STARTS ===================================================
-        # =============================================================================
-
-        if geo.ti.i.t < geo.wi.t / 2:
-            raise ValueError(
-                f"Inner terminal's thickness ({geo.ti.i.t:.5f}) is"
-                " smaller than half of the winding's thickness"
-                f" ({geo.wi.t/2:.5f}). Please increase the inner"
-                " terminal's thickness."
-            )
-        if geo.ti.o.t < geo.wi.t / 2:
-            raise ValueError(
-                f"Outer terminal's thickness ({geo.ti.o.t:.5f}) is"
-                " smaller than half of the winding's thickness"
-                f" ({geo.wi.t/2:.5f}). Please increase the outer"
-                " terminal's thickness."
-            )
-
-        if geo.ti.i.t != geo.ti.o.t:
-            raise ValueError(
-                f"Inner terminal's thickness ({geo.ti.i.t:.5f}) is"
-                " not equal to the outer terminal's thickness"
-                f" ({geo.ti.o.t:.5f}). Please make them equal. If"
-                " you want to have different thicknesses, please comment out this"
-                " error."
-            )
-
-        # =============================================================================
-        # CHECKING TERMINALS ENDS =====================================================
-        # =============================================================================
-
-        # =============================================================================
-        # CHECKING AIR STARTS =========================================================
-        # =============================================================================
-
-        if geo.ai.margin < geo.wi.h / 2:
-            raise ValueError(
-                f"Air margin ({geo.ai.margin:.5f}) is smaller than the"
-                f" winding's half height ({geo.wi.h/2:.5f}). To avoid"
-                " numerical errors, please increase the air margin."
-            )
-
-        if geo.ai.type == "cuboid":
-            if geo.ti.o.r * 1.5 > geo.ai.a / 2:
-                raise ValueError(
-                    f"Side length of the air ({geo.ai.a:.5f}) must be at least 1.5"
-                    " times larger than the outer terminal's diameter"
-                    f" ({geo.ti.o.r*2:.5f}). Please increase the air side length."
-                )
-
-        elif geo.ai.type == "cylinder":
-            if geo.ti.o.r * 1.5 > geo.ai.r:
-                raise ValueError(
-                    f"Radius of the air ({geo.ai.r:.5f}) must be at least 1.5 times"
-                    f" larger than the outer terminal's radius ({geo.ti.o.r:.5f})."
-                    " Please increase the air radius."
-                )
-
-        # =============================================================================
-        # CHECKING AIR ENDS ===========================================================
-        # =============================================================================
-
-        values["mesh"] = mesh
-        values["geometry"] = geo
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def read_IcVSLength_CSV_file(cls, values):
-        """
-        Some fields are names of other files like CSVs. Users are asked to put those
-        files in the same folder as the input file. This function appends the input
-        file path to those file names and checks if the files exist.
-        """
-        geo = values["geometry"]
-        solve = values["solve"]
-
-        if solve.wi.superConductor is not None:
-            if not isinstance(solve.wi.superConductor.IcAtTinit, float):
-                IcVStapeLengthCSVFileName = solve.wi.superConductor.IcAtTinit
-                if isinstance(IcVStapeLengthCSVFileName, str):
-                    solve.wi.superConductor.IcAtTinit = os.path.join(
-                        os.path.dirname(values["input_file_path"]),
-                        IcVStapeLengthCSVFileName,
-                    )
-                    if not os.path.isfile(solve.wi.superConductor.IcAtTinit):
-                        raise ValueError(
-                            f"{solve.wi.superConductor.IcAtTinit} does not exist!"
-                        )
-
-                    with open(solve.wi.superConductor.IcAtTinit, newline="") as csvFile:
-                        reader = csv.reader(csvFile, delimiter=",")
-
-                        solve.wi.superConductor.lengthValues = []
-                        solve.wi.superConductor.IcValues = []
-                        for row in reader:
-                            if len(row) != 2:
-                                raise ValueError(
-                                    f"{solve.wi.superConductor.IcAtTinit} needs to have"
-                                    " 2 columns!"
-                                )
-                            try:
-                                length = float(row[0])
-                            except:
-                                raise ValueError(
-                                    f"{solve.wi.superConductor.IcAtTinit} has a"
-                                    " non-numerical value!"
-                                )
-
-                            try:
-                                Ic = float(row[1])
-                            except:
-                                raise ValueError(
-                                    f"{solve.wi.superConductor.IcAtTinit} has a"
-                                    " non-numerical value!"
-                                )
-
-                            if length >= 0:
-                                solve.wi.superConductor.lengthValues.append(length)
-                            else:
-                                raise ValueError(
-                                    f"{solve.wi.superConductor.IcAtTinit} cannot have"
-                                    " negative length values!"
-                                )
-
-                            if Ic >= 0:
-                                solve.wi.superConductor.IcValues.append(Ic)
-                            else:
-                                raise ValueError(
-                                    f"{solve.wi.superConductor.IcAtTinit} cannot have"
-                                    " negative critical current values!"
-                                )
-
-                        if len(solve.wi.superConductor.lengthValues) == 0:
-                            raise ValueError(
-                                f"{solve.wi.superConductor.IcAtTinit} is empty!"
-                            )
-
-                elif isinstance(IcVStapeLengthCSVFileName, Pancake3DSolveIcVsLength):
-                    solve.wi.superConductor.lengthValues = (
-                        solve.wi.superConductor.IcAtTinit.lengthValues
-                    )
-                    solve.wi.superConductor.IcValues = (
-                        solve.wi.superConductor.IcAtTinit.criticalCurrentValues
-                    )
-
-                # check if the length values are exceeding the winding's length:
-                if max(solve.wi.superConductor.lengthValues) > geo.wi.totalTapeLength:
-                    raise ValueError(
-                        "The length values in the criticalCurrentAtInitialTemperature"
-                        " cannot be greater than the winding's total tape length"
-                        f" ({geo.wi.totalTapeLength})!"
-                    )
-
-                if len(solve.wi.superConductor.lengthValues) != len(
-                    solve.wi.superConductor.IcValues
-                ):
-                    raise ValueError(
-                        "There needs to be the same number of length values and"
-                        " critical current values for"
-                        " criticalCurrentAtInitialTemperature!"
-                    )
-
-                # add Ic for start and end points of the tape:
-                if solve.wi.superConductor.lengthValues[0] != 0:
-                    solve.wi.superConductor.lengthValues.insert(0, 0)
-                    solve.wi.superConductor.IcValues.insert(
-                        0, solve.wi.superConductor.IcValues[0]
-                    )
-
-                if solve.wi.superConductor.lengthValues[-1] != geo.wi.totalTapeLength:
-                    solve.wi.superConductor.lengthValues.append(geo.wi.totalTapeLength)
-                    solve.wi.superConductor.IcValues.append(
-                        solve.wi.superConductor.IcValues[-1]
-                    )
-
-                values["solve"] = solve
-
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
+    @model_validator(mode="before")
     @classmethod
-    def mesh_calculations_and_checks(cls, values):
-        """
-        Checks if the length of the mesh lists are equal to the number of pancakes. If
-        the length of the mesh lists are all one, then it means that the user wants to
-        use the same mesh settings for all the pancakes. In this case, the length of
-        the mesh lists are set to the number of pancakes. If all the settings' lengths
-        are not one, and not equal to the number of pancakes, then the function raises
-        an error.
-
-        :param cls: class
-        :type cls: class
-        :param values: dictionary of PC3D
-        :type values: dict
-        :return: dictionary of PC3D
-        :rtype: dict
+    def set_context_variables(cls, model: "Pancake3D"):
+        """Set the context variables (geometry data model, mesh data model, solve data
+        model) of the Pancake3D model. They will be used in the submodel validators.
         """
-        geo = values["geometry"]
-        mesh = values["mesh"]
-
-        # ==============================================================================
-        # MESH CHECKING STARTS =========================================================
-        # ==============================================================================
-        def check_mesh_input(meshInput, inputName):
-            if not isinstance(meshInput, list):
-                meshInput = [meshInput]
-
-            length = len(meshInput)
-            if length == 1:
-                meshInput = meshInput * geo.N
-            elif length != geo.N:
-                raise ValueError(
-                    "The list length of "
-                    + inputName
-                    + " must be either one (same mesh settings for all the pancakes) or"
-                    " equal to the number of pancakes."
-                )
-
-            return meshInput
-
-        mesh.wi.axne = check_mesh_input(mesh.wi.axne, inputName="axialNumberOfElements")
-        mesh.wi.ane = check_mesh_input(
-            mesh.wi.ane, inputName="azimuthalNumberOfElementsPerTurn"
-        )
-        mesh.wi.rne = check_mesh_input(
-            mesh.wi.rne, inputName="radialNumberOfElementsPerTurn"
-        )
-        mesh.wi.axbc = check_mesh_input(
-            mesh.wi.axbc, inputName="axialDistributionCoefficient"
-        )
-        if not geo.ii.tsa:
-            if mesh.ii.rne is None:
-                mesh.ii.rne = [1] * geo.N
-            else:
-                mesh.ii.rne = check_mesh_input(
-                    mesh.ii.rne, inputName="radialNumberOfElementsPerTurn"
-                )
-        mesh.wi.elementType = check_mesh_input(
-            mesh.wi.elementType, inputName="elementType"
-        )
-
-        for bumpCoefficient in mesh.wi.axbc:
-            if bumpCoefficient > 1:
-                raise ValueError(
-                    "Axial bump coefficient must be smaller than or equal to 1!"
-                )
-
-        for ane in mesh.wi.ane:
-            if ane < 7:
-                raise ValueError(
-                    "Azimuthal number of elements per turn must be greater than or"
-                    " equal to 7!"
-                )
-
-        if True in mesh.wi.elementType == "hexahedron" and geo.N > 1:
-            raise ValueError(
-                "Hexahedron elements is not recommended for multiple pancakes due to"
-                " the possible ill-shaped meshes at the gap between pancakes. If you"
-                " still want to do it, please comment this error."
-            )
-
-        if not geo.ii.tsa and True in mesh.wi.elementType == "prism":
-            raise ValueError(
-                "Prism elements is not recommended for volume contact layer due to the"
-                " possible ill-shaped meshes at the terminal's edges. If you still want"
-                " to do it, please comment this error."
-            )
-
-        if not geo.ii.tsa and True in mesh.wi.elementType == "hexahedron":
-            raise ValueError(
-                "Hexahedron elements is not recommended for volume contact layer due to"
-                " the possible ill-shaped meshes at the terminal's edges. If you still"
-                " want to do it, please comment this error."
-            )
-
-        theWorstRectangularRatios = []
-        theWorstTriangularRatios = []
-        for i in range(geo.N):
-            meshLengthPerElement = {}
-            meshLengthPerElement["azimuthal elements"] = (
-                2 * math.pi * geo.ti.o.r / mesh.wi.ane[i]
-            )
-            meshLengthPerElement["winding's radial elements"] = (
-                geo.wi.t / mesh.wi.rne[i]
-            )
-            meshLengthPerElement["axial elements"] = geo.wi.h / mesh.wi.axne[i]
-            if not geo.ii.tsa:
-                meshLengthPerElement["contact layer's radial elements"] = (
-                    geo.ii.t / mesh.ii.rne[i]
-                )
-
-            if mesh.wi.elementType[i] == "hexahedron":
-                maxRectName = max(meshLengthPerElement, key=meshLengthPerElement.get)
-                maxRectLengthPerElement = meshLengthPerElement[maxRectName]
-                minRectName = min(meshLengthPerElement, key=meshLengthPerElement.get)
-                minRectLengthPerElement = meshLengthPerElement[minRectName]
-
-                maxTriLengthPerElement = 1
-                minTriLengthPerElement = 1
-                maxTriName = "dummy"
-                minTriName = "dummy"
-
-                theWorstRectangularRatio = (
-                    maxRectLengthPerElement / minRectLengthPerElement
-                )
-                theWorstTriangularRatio = 1
-
-            elif mesh.wi.elementType[i] == "tetrahedron":
-                maxTriName = max(meshLengthPerElement, key=meshLengthPerElement.get)
-                maxTriLengthPerElement = meshLengthPerElement[maxTriName]
-                minTriName = min(meshLengthPerElement, key=meshLengthPerElement.get)
-                minTriLengthPerElement = meshLengthPerElement[minTriName]
-
-                maxRectLengthPerElement = 1
-                minRectLengthPerElement = 1
-                maxRectName = "dummy"
-                minRectName = "dummy"
-
-                theWorstRectangularRatio = 1
-                theWorstTriangularRatio = (
-                    maxTriLengthPerElement / minTriLengthPerElement
-                )
-
-            elif mesh.wi.elementType[i] == "prism":
-                if geo.ii.tsa:
-                    rectangularRatios = [
-                        meshLengthPerElement["winding's radial elements"]
-                        / meshLengthPerElement["axial elements"],
-                        meshLengthPerElement["axial elements"]
-                        / meshLengthPerElement["winding's radial elements"],
-                        meshLengthPerElement["azimuthal elements"]
-                        / meshLengthPerElement["axial elements"],
-                        meshLengthPerElement["azimuthal elements"]
-                        / meshLengthPerElement["axial elements"],
-                    ]
-
-                    triangularRatios = [
-                        meshLengthPerElement["azimuthal elements"]
-                        / meshLengthPerElement["winding's radial elements"],
-                        meshLengthPerElement["winding's radial elements"]
-                        / meshLengthPerElement["azimuthal elements"],
-                    ]
-
-                else:
-                    rectangularRatios = [
-                        meshLengthPerElement["winding's radial elements"]
-                        / meshLengthPerElement["axial elements"],
-                        meshLengthPerElement["axial elements"]
-                        / meshLengthPerElement["winding's radial elements"],
-                        meshLengthPerElement["azimuthal elements"]
-                        / meshLengthPerElement["axial elements"],
-                        meshLengthPerElement["azimuthal elements"]
-                        / meshLengthPerElement["axial elements"],
-                        meshLengthPerElement["contact layer's radial elements"]
-                        / meshLengthPerElement["axial elements"],
-                        meshLengthPerElement["axial elements"]
-                        / meshLengthPerElement["contact layer's radial elements"],
-                    ]
-
-                    triangularRatios = [
-                        meshLengthPerElement["azimuthal elements"]
-                        / meshLengthPerElement["winding's radial elements"],
-                        meshLengthPerElement["winding's radial elements"]
-                        / meshLengthPerElement["azimuthal elements"],
-                        meshLengthPerElement["azimuthal elements"]
-                        / meshLengthPerElement["contact layer's radial elements"],
-                        meshLengthPerElement["contact layer's radial elements"]
-                        / meshLengthPerElement["azimuthal elements"],
-                    ]
-
-                theWorstRectangularRatio = max(rectangularRatios)
-                indexRectangular = rectangularRatios.index(theWorstRectangularRatio)
-
-                if indexRectangular == 0:
-                    maxRectName = "winding's radial elements"
-                    minRectName = "axial elements"
-                elif indexRectangular == 1:
-                    maxRectName = "axial elements"
-                    minRectName = "winding's radial elements"
-                elif indexRectangular == 2:
-                    maxRectName = "azimuthal elements"
-                    minRectName = "axial elements"
-                elif indexRectangular == 3:
-                    maxRectName = "azimuthal elements"
-                    minRectName = "axial elements"
-                elif indexRectangular == 4:
-                    maxRectName = "contact layer's radial elements"
-                    minRectName = "axial elements"
-                elif indexRectangular == 5:
-                    maxRectName = "axial elements"
-                    minRectName = "contact layer's radial elements"
-
-                theWorstTriangularRatio = max(triangularRatios)
-                indexTriangular = triangularRatios.index(theWorstTriangularRatio)
-
-                if indexTriangular == 0:
-                    maxTriName = "azimuthal elements"
-                    minTriName = "winding's radial elements"
-                elif indexTriangular == 1:
-                    maxTriName = "winding's radial elements"
-                    minTriName = "azimuthal elements"
-                elif indexTriangular == 2:
-                    maxTriName = "azimuthal elements"
-                    minTriName = "contact layer's radial elements"
-                elif indexTriangular == 3:
-                    maxTriName = "contact layer's radial elements"
-                    minTriName = "azimuthal elements"
-
-            numOfElements = {
-                "azimuthal elements": mesh.wi.ane[i],
-                "axial elements": mesh.wi.axne[i],
-                "winding's radial elements": mesh.wi.rne[i],
-            }
-            if not geo.ii.tsa:
-                numOfElements["contact layer's radial elements"] = mesh.ii.rne[i]
-
-            lengths = {
-                "azimuthal elements": 2 * math.pi * geo.ti.o.r,
-                "axial elements": geo.wi.h,
-                "winding's radial elements": geo.wi.t,
-            }
-            if not geo.ii.tsa:
-                lengths["contact layer's radial elements"] = geo.ii.t
-
-            allowedTriangularRatio = 120
-            allowedRectangularRatio = 115
-
-            allowedTriangularRatio = 999999
-            allowedRectangularRatio = 999999
-
-            theWorstRectangularRatios.append(theWorstRectangularRatio)
-            theWorstTriangularRatios.append(theWorstTriangularRatio)
-            for theWorstRatio, maxName, minName, allowedRatio in zip(
-                [theWorstTriangularRatio, theWorstRectangularRatio],
-                [maxTriName, maxRectName],
-                [minTriName, minRectName],
-                [allowedTriangularRatio, allowedRectangularRatio],
-            ):
-                if theWorstRatio > allowedRatio:
-                    if numOfElements[minName] == 1:
-                        # If the number of elements is 1, then the user cannot decrease the
-                        # number of elements. So the only option is to increase the number
-                        # of elements.
-                        newMaxLengthPerElement = (
-                            meshLengthPerElement[minName] * allowedRatio
-                        )
-                        newNumberOfElements = math.ceil(
-                            lengths[maxName] / newMaxLengthPerElement
-                        )
-                        raise ValueError(
-                            "The structred mesh inputs for pancake coil number"
-                            f" {i+1} might cause ill-shaped meshes. Please increase the"
-                            f" {maxName} per turn up to {newNumberOfElements}."
-                        )
-                    else:
-                        newMaxLengthPerElement = (
-                            meshLengthPerElement[minName] * allowedRatio
-                        )
-                        newNumberOfElementsToIncrease = math.ceil(
-                            lengths[maxName] / newMaxLengthPerElement
-                        )
-
-                        newMinLengthPerElement = (
-                            meshLengthPerElement[maxName] / allowedRatio
-                        )
-                        newNumberOfElementsToDecrease = math.floor(
-                            lengths[minName] / newMinLengthPerElement
-                        )
-                        raise ValueError(
-                            "The structred mesh inputs might cause ill-shaped meshes."
-                            f" Please either increase the {maxName} per turn up"
-                            f" to {newNumberOfElementsToIncrease} or decrease the"
-                            f" {minName} per turn down to"
-                            f" {newNumberOfElementsToDecrease}."
-                        )
-
-        mesh.theWorstRectangularRatio = max(theWorstRectangularRatios)
-        mesh.theWorstTriangularRatio = max(theWorstTriangularRatios)
-
-        # Structured air and terminals checks:
-        if mesh.ai.structured == True:
-            # Air type cannot be cuboid!
-            if geo.ai.type == "cuboid":
-                raise ValueError(
-                    "Structured air cannot be used if the air type is cuboid!"
-                )
-
-            # Element type cannot be hexahedron!
-            if mesh.wi.elementType[0] == "hexahedron":
-                raise ValueError(
-                    "Structured air cannot be used if the element type is hexahedron!"
-                    " Only tetrahedron and prism are allowed."
-                )
-
-        if mesh.ai.structured == True or mesh.ti.structured == True:
-            # Every winding and contact layer mesh settings must be the same:
-            if len(set(mesh.wi.axne)) != 1:
-                raise ValueError(
-                    "The axial number of elements per turn must be the same for all the"
-                    " windings if structured air or structured terminals meshes are"
-                    " used!"
-                )
-            if len(set(mesh.wi.ane)) != 1:
-                raise ValueError(
-                    "The azimuthal number of elements per turn must be the same for all"
-                    " the windings if structured air or structured terminals meshes are"
-                    " used!"
-                )
-            if len(set(mesh.wi.rne)) != 1:
-                raise ValueError(
-                    "The radial number of elements per turn must be the same for all"
-                    " the windings if structured air or structured terminals meshes are"
-                    " used!"
-                )
-            if not geo.ii.tsa:
-                if len(set(mesh.ii.rne)) != 1:
-                    raise ValueError(
-                        "The radial number of elements per turn must be the same for"
-                        " all the contact layers if structured air or structured"
-                        " terminals meshes are used!"
-                    )
-
-            # Start angle must be 0:
-            if math.isclose(geo.wi.theta_i, 0, abs_tol=geo.dimTol) == False:
-                raise ValueError(
-                    "The start angle of the winding must be 0 if structured air or"
-                    " structured terminals meshes are used!"
-                )
-
-            # The number of volumes per turn must be 4:
-            if geo.wi.NofVolPerTurn != 4:
-                logger.warning(
-                    "The number of volumes per turn will be set to 4 since"
-                    " structured air or structured terminals meshes are used."
-                )
-
-            geo.wi.NofVolPerTurn = 4
-
-            # The number of azimuthal elements per turn must be divisible by 4:
-            if mesh.wi.ane[0] % 4 != 0:
-                raise ValueError(
-                    "The number of azimuthal elements per turn must be divisible by 4"
-                    " if structured air or structured terminals meshes are used!"
-                )
 
-        # ==============================================================================
-        # MESH CHECKING ENDS ===========================================================
-        # ==============================================================================
-
-        # ==============================================================================
-        # MESH CALCULATIONS STARTS =====================================================
-        # ==============================================================================
-        mesh.sizeMin = max(meshLengthPerElement.values()) * mesh.relSizeMin
-        mesh.sizeMax = max(meshLengthPerElement.values()) * mesh.relSizeMax
-
-        mesh.startGrowingDistance = (geo.ti.o.r - geo.ti.i.r) / 2
-        if geo.ai.type == "cylinder":
-            mesh.stopGrowingDistance = geo.ai.r - geo.ti.o.r
-        elif geo.ai.type == "cuboid":
-            mesh.stopGrowingDistance = geo.ai.a / 2 - geo.ti.o.r
-
-        def getSizeAtTopAndBottom(sizeMax, airMargin):
-            if airMargin > mesh.stopGrowingDistance:
-                sizeAtTopAndBottom = mesh.sizeMax
-            elif airMargin < mesh.startGrowingDistance:
-                sizeAtTopAndBottom = mesh.sizeMin
-            else:
-                sizeAtTopAndBottom = mesh.sizeMin + (sizeMax - mesh.sizeMin) * (
-                    (airMargin - mesh.startGrowingDistance)
-                    / (mesh.stopGrowingDistance - mesh.startGrowingDistance)
-                )
-
-            return sizeAtTopAndBottom
-
-        def getSizeMax(sizeAtTopAndBottom, airMargin):
-            if airMargin > mesh.stopGrowingDistance:
-                sizeMax = sizeAtTopAndBottom
-            elif airMargin < mesh.startGrowingDistance:
-                # any sizeMax value will work here
-                sizeMax = -1
-            else:
-                sizeMax = (sizeAtTopAndBottom - mesh.sizeMin) * (
-                    (mesh.stopGrowingDistance - mesh.startGrowingDistance)
-                    / (airMargin - mesh.startGrowingDistance)
-                ) + mesh.sizeMin
-
-            return sizeMax
-
-        def getAirMargin(sizeAtTopAndBottom, sizeMax):
-            airMargin = (sizeAtTopAndBottom - mesh.sizeMin) * (
-                (mesh.stopGrowingDistance - mesh.startGrowingDistance)
-                / (sizeMax - mesh.sizeMin)
-            ) + mesh.startGrowingDistance
-
-            return airMargin
-
-        sizeAtTopAndBottom = getSizeAtTopAndBottom(mesh.sizeMax, geo.ai.margin)
-
-        # tolerance = 10.7
-        tolerance = 999999
-        if sizeAtTopAndBottom / min(geo.ti.i.t, geo.ti.o.t) > tolerance:
-            desiredSizeAtTopAndBottom = min(geo.ti.i.t, geo.ti.o.t) * tolerance
-            desiredTerminalRadius = sizeAtTopAndBottom / tolerance
-            desiredAirMargin = getAirMargin(desiredSizeAtTopAndBottom, mesh.sizeMax)
-            desiredRelSizeMax = math.floor(
-                getSizeMax(desiredSizeAtTopAndBottom, geo.ai.margin)
-                / max(meshLengthPerElement.values())
-            )
-            raise ValueError(
-                "Terminals are too thin for the given maximum mesh element size."
-                f" Please either decrease the air margin to {desiredAirMargin:.5f},"
-                f" decrease the maximum mesh element size to {desiredRelSizeMax}, or"
-                f" increase the terminal radius to {desiredTerminalRadius:.5f}."
-            )
-
-        # ==============================================================================
-        # MESH CALCULATIONS ENDS =======================================================
-        # ==============================================================================
-
-        values["mesh"] = mesh
-        values["geometry"] = geo
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def check_contact_layer_materials(cls, values):
-        if values["geometry"].ii.tsa:
-            if values["solve"].ii.resistivity is None:
-                if not (
-                    values["solve"].ii.material.getdpTSAMassResistivityFunction
-                    and values["solve"].ii.material.getdpTSAStiffnessResistivityFunction
-                    and values["solve"].ii.material.getdpTSARHSFunction
-                    and values["solve"].ii.material.getdpTSATripleFunction
-                ):
-                    raise ValueError(
-                        "Thin-shell resistivity properties for"
-                        f" {values['solve'].ii.material.name} are not"
-                        " defined! Please define custom constant resistivity value or"
-                        " use a different material."
-                    )
-            if values["solve"].ii.thermalConductivity is None:
-                if not (
-                    values["solve"].ii.material.getdpTSAMassThermalConductivityFunction
-                    and values[
-                        "solve"
-                    ].ii.material.getdpTSAStiffnessThermalConductivityFunction
-                ):
-                    raise ValueError(
-                        "Thin-shell thermal conductivity properties for"
-                        f" {values['solve'].ii.material.name} are not"
-                        " defined! Please define custom constant thermal conductivity"
-                        " value or use a different material."
-                    )
-            if values["solve"].ii.specificHeatCapacity is None:
-                if not values["solve"].ii.material.getdpTSAMassHeatCapacityFunction:
-                    raise ValueError(
-                        "Thin-shell specific heat capacity properties for"
-                        f" {values['solve'].ii.material.name} are not"
-                        " defined! Please define custom constant specific heat capacity"
-                        " value or use a different material."
-                    )
-
-        if values["solve"].ii.resistivity is not None:
-            if values["solve"].ii.resistivity == "perfectlyInsulating":
-                if values["geometry"].N > 1:
-                    raise ValueError(
-                        "perfectlyInsulating cannot be used if there are multiple"
-                        " pancakes!"
-                    )
-
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def check_and_calculate_postprocessing_quantities(cls, values):
-        """ """
-        solve = values["solve"]
-        postproc = values["postproc"]
-
-        if postproc is None:
-            return values
-
-        if postproc.timeSeriesPlots is not None:
-            electromagneticRequiredQuantities = [
-                "magnitudeOfMagneticField",
-                "magnitudeOfCurrentDensity",
-                "resistiveHeating",
-                "axialComponentOfTheMagneticField",
-                "totalResistiveHeating",
-                "voltageBetweenTerminals",
-                "currentThroughCoil",
-                "resistivity",
-                "derivativeOfRhoWithRespectToJ",
-                "magneticEnergy",
-            ]
-            thermalRequiredQuantities = [
-                "temperature",
-                "magnitudeOfHeatFlux",
-            ]
-            for timeSeriesPlot in postproc.timeSeriesPlots:
-                if (
-                    timeSeriesPlot.quantity in thermalRequiredQuantities
-                    and solve.type == "electromagnetic"
-                ):
-                    raise ValueError(
-                        f'"{timeSeriesPlot.quantity}" cannot be plotted with'
-                        " timeSeriesPlots if the type is electromagnetic because"
-                        " it is not calculated!"
-                    )
-
-                if (
-                    timeSeriesPlot.quantity in electromagneticRequiredQuantities
-                    and solve.type == "thermal"
-                ):
-                    raise ValueError(
-                        f'"{timeSeriesPlot.quantity}" cannot be plotted with'
-                        " timeSeriesPlots if the type is thermal because it is not"
-                        " calculated!"
-                    )
-                if (
-                    timeSeriesPlot.quantity == "derivativeOfRhoWithRespectToJ"
-                    and solve.wi.resistivity is not None
-                ):
-                    raise ValueError(
-                        "derivativeOfRhoWithRespectToJ cannot be plotted with"
-                        " timeSeriesPlots if the winding resistivity is linear!"
-                    )
-
-        if postproc.magneticFieldOnCutPlane is not None:
-            if solve.type == "thermal":
-                raise ValueError(
-                    "magneticFieldOnCutPlane cannot be plotted if the type is thermal!"
-                )
-
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def calculate_positions(cls, values):
-        """"""
-        geo: Pancake3DGeometry = values["geometry"]
-        mesh: Pancake3DMesh = values["mesh"]
-        solve: Pancake3DSolve = values["solve"]
-        postproc: Pancake3DPostprocess = values["postproc"]
-
-        def calculate_position(position):
-            coordinatesAreGiven = False
-            if (
-                position.x is not None
-                and position.y is not None
-                and position.z is not None
-            ):
-                coordinatesAreGiven = True
-
-            turnNumberIsGiven = False
-            if position.turnNumber is not None:
-                turnNumberIsGiven = True
-                if position.turnNumber < 0:
-                    raise ValueError("Turn number for the position cannot be negative!")
-
-                if position.turnNumber > geo.wi.N:
-                    raise ValueError(
-                        "Turn number for the position must be smaller than"
-                        " the number of turns of the winding!"
-                    )
-
-                if geo.N == 1:
-                    position.whichPancakeCoil = 1
-                else:
-                    if position.whichPancakeCoil is None:
-                        raise ValueError(
-                            "whichPancakeCoil entry must be specified if the position"
-                            " is specified with turnNumber!"
-                        )
-                    if position.whichPancakeCoil > geo.N:
-                        raise ValueError(
-                            "whichPancakeCoil entry must be smaller than or equal to"
-                            " the number of pancakes!"
-                        )
-
-            if turnNumberIsGiven:
-                if position.x or position.y or position.z:
-                    raise ValueError(
-                        "Either turn number or x, y, and z coordinates can be"
-                        " specified!"
-                    )
-                if geo.N == 1:
-                    position.whichPancakeCoil = 1
-                elif geo.N > 1:
-                    if position.whichPancakeCoil is None:
-                        raise ValueError(
-                            "whichPancakeCoil entry must be specified if the"
-                            " position is specified with turnNumber!"
-                        )
-                if position.turnNumber > geo.wi.N:
-                    raise ValueError(
-                        "Turn number for the position must be smaller than"
-                        " the number of turns of the winding!"
-                    )
-                # Calculate x, y, and z coordinates from turn number:
-                if geo.ii.tsa:
-                    windingThickness = geo.wi.t + geo.ii.t * (geo.wi.N - 1) / geo.wi.N
-                    gapThickness = 0
-                else:
-                    windingThickness = geo.wi.t
-                    gapThickness = geo.ii.t
-
-                innerRadius = geo.wi.r_i
-                initialTheta = geo.wi.theta_i
-                ane = mesh.wi.ane[0]
-                numberOfPancakes = geo.N
-                gapBetweenPancakes = geo.gap
-                windingHeight = geo.wi.h
-
-                turnNumber = position.turnNumber
-                whichPancake = position.whichPancakeCoil
-
-                elementStartTurnNumber = math.floor(turnNumber / (1 / ane)) * (1 / ane)
-                elementEndTurnNumber = elementStartTurnNumber + 1 / ane
-
-                class point:
-                    def __init__(self, x, y, z):
-                        self.x = x
-                        self.y = y
-                        self.z = z
-
-                    def __add__(self, other):
-                        return point(
-                            self.x + other.x, self.y + other.y, self.z + other.z
-                        )
-
-                    def __sub__(self, other):
-                        return point(
-                            self.x - other.x, self.y - other.y, self.z - other.z
-                        )
-
-                    def __mul__(self, scalar):
-                        return point(self.x * scalar, self.y * scalar, self.z * scalar)
-
-                    def __truediv__(self, scalar):
-                        return point(self.x / scalar, self.y / scalar, self.z / scalar)
-
-                    def rotate(self, degrees):
-                        return point(
-                            self.x * math.cos(degrees) - self.y * math.sin(degrees),
-                            self.x * math.sin(degrees) + self.y * math.cos(degrees),
-                            self.z,
-                        )
-
-                    def normalize(self):
-                        return self / math.sqrt(self.x**2 + self.y**2 + self.z**2)
-
-                if whichPancake % 2 == 1:
-                    # If the spiral is counter-clockwise, the initial theta angle decreases,
-                    # and r increases as the theta angle decreases.
-                    multiplier = 1
-                elif whichPancake % 2 == 0:
-                    # If the spiral is clockwise, the initial theta angle increases, and r
-                    # increases as the theta angle increases.
-                    multiplier = -1
-
-                # Mesh element's starting point:
-                elementStartTheta = 2 * math.pi * elementStartTurnNumber * multiplier
-                elementStartRadius = (
-                    innerRadius
-                    + elementStartTheta
-                    / (2 * math.pi)
-                    * (gapThickness + windingThickness)
-                    * multiplier
-                )
-                elementStartPointX = elementStartRadius * math.cos(
-                    initialTheta + elementStartTheta
-                )
-                elementStartPointY = elementStartRadius * math.sin(
-                    initialTheta + elementStartTheta
-                )
-                elementStartPointZ = (
-                    -(
-                        numberOfPancakes * windingHeight
-                        + (numberOfPancakes - 1) * gapBetweenPancakes
-                    )
-                    / 2
-                    + windingHeight / 2
-                    + (whichPancake - 1) * (windingHeight + gapBetweenPancakes)
-                )
-                elementStartPoint = point(
-                    elementStartPointX, elementStartPointY, elementStartPointZ
-                )
-
-                # Mesh element's ending point:
-                elementEndTheta = 2 * math.pi * elementEndTurnNumber * multiplier
-                elementEndRadius = (
-                    innerRadius
-                    + elementEndTheta
-                    / (2 * math.pi)
-                    * (gapThickness + windingThickness)
-                    * multiplier
-                )
-                elementEndPointX = elementEndRadius * math.cos(
-                    initialTheta + elementEndTheta
-                )
-                elementEndPointY = elementEndRadius * math.sin(
-                    initialTheta + elementEndTheta
-                )
-                elementEndPointZ = elementStartPointZ
-                elementEndPoint = point(
-                    elementEndPointX, elementEndPointY, elementEndPointZ
-                )
-
-                turnNumberFraction = (turnNumber - elementStartTurnNumber) / (
-                    elementEndTurnNumber - elementStartTurnNumber
-                )
-                location = (
-                    elementStartPoint
-                    + (elementEndPoint - elementStartPoint) * turnNumberFraction
-                ) + (elementEndPoint - elementStartPoint).rotate(
-                    -math.pi / 2
-                ).normalize() * windingThickness / 2 * multiplier
-
-                position.x = location.x
-                position.y = location.y
-                position.z = location.z
-
-            return position
-
-        # Calculate positons for time series plots:
-        if postproc is not None:
-            if postproc.timeSeriesPlots is not None:
-                for timeSeriesPlot in postproc.timeSeriesPlots:
-                    timeSeriesPlot.position = calculate_position(
-                        timeSeriesPlot.position
-                    )
-
-        if solve is not None:
-            # Calculate positions for tolerances:
-            for tolerance in solve.t.adaptive.tolerances:
-                if tolerance.position is not None:
-                    tolerance.position = calculate_position(tolerance.position)
-
-            for tolerance in solve.nls.tolerances:
-                if tolerance.position is not None:
-                    tolerance.position = calculate_position(tolerance.position)
-
-        # Calculate z-position for local defect:
-        if solve.localDefects is not None:
-            if (
-                solve.localDefects.jCritical is not None
-                and solve.localDefects.jCritical.startTurn is not None
-            ):
-                localDefect: Pancake3DSolveLocalDefect = solve.localDefects.jCritical
-                if geo.N == 1:
-                    localDefect.whichPancakeCoil = 1
-                elif geo.N > 1:
-                    if localDefect.whichPancakeCoil is None:
-                        raise ValueError(
-                            "whichPancakeCoil entry must be specified if the"
-                            " position is specified with turnNumber!"
-                        )
-                if localDefect.endTurn > geo.wi.N or localDefect.startTurn > geo.wi.N:
-                    raise ValueError(
-                        "Turn number for the position must be smaller than"
-                        " the number of turns of the winding! (jCritical local defect)"
-                    )
-
-                bottomZ = -(geo.N * geo.wi.h + (geo.N - 1) * geo.gap) / 2 + (
-                    localDefect.whichPancakeCoil - 1
-                ) * (geo.wi.h + geo.gap)
-                topZ = bottomZ + geo.wi.h
-
-                localDefect.zTop = topZ
-                localDefect.zBottom = bottomZ
-
-        return values
-
-    @root_validator(pre=False, allow_reuse=True, skip_on_failure=True)
-    @classmethod
-    def calculate_onSection(cls, values):
-        """ """
-        geo: Pancake3DGeometry = values["geometry"]
-        solve: Pancake3DSolve = values["solve"]
-        postproc: Pancake3DPostprocess = values["postproc"]
-
-        import numpy as np
-
-        if postproc is not None:
-            if postproc.magneticFieldOnCutPlane is not None:
-
-                class unitVector:
-                    def __init__(self, u, v, w) -> None:
-                        length = math.sqrt(u**2 + v**2 + w**2)
-                        self.u = u / length
-                        self.v = v / length
-                        self.w = w / length
-
-                    def rotate(self, theta, withRespectTo):
-                        # Rotate with respect to the withRespectTo vector by theta degrees:
-                        # https://en.wikipedia.org/wiki/Rotation_matrix#Rotation_matrix_from_axis_and_angle
-                        a = withRespectTo.u
-                        b = withRespectTo.v
-                        c = withRespectTo.w
-
-                        rotationMatrix = np.array(
-                            [
-                                [
-                                    math.cos(theta) + a**2 * (1 - math.cos(theta)),
-                                    a * b * (1 - math.cos(theta)) - c * math.sin(theta),
-                                    a * c * (1 - math.cos(theta)) + b * math.sin(theta),
-                                ],
-                                [
-                                    b * a * (1 - math.cos(theta)) + c * math.sin(theta),
-                                    math.cos(theta) + b**2 * (1 - math.cos(theta)),
-                                    b * c * (1 - math.cos(theta)) - a * math.sin(theta),
-                                ],
-                                [
-                                    c * a * (1 - math.cos(theta)) - b * math.sin(theta),
-                                    c * b * (1 - math.cos(theta)) + a * math.sin(theta),
-                                    math.cos(theta) + c**2 * (1 - math.cos(theta)),
-                                ],
-                            ]
-                        )
-                        vector = np.array([[self.u], [self.v], [self.w]])
-                        rotatedVector = rotationMatrix @ vector
-                        return unitVector(
-                            rotatedVector[0][0],
-                            rotatedVector[1][0],
-                            rotatedVector[2][0],
-                        )
-
-                    def __pow__(self, otherUnitVector):
-                        # Cross product:
-                        u = self.v * otherUnitVector.w - self.w * otherUnitVector.v
-                        v = self.w * otherUnitVector.u - self.u * otherUnitVector.w
-                        w = self.u * otherUnitVector.v - self.v * otherUnitVector.u
-                        return unitVector(u, v, w)
-
-                    def __mul__(self, otherUnitVector) -> float:
-                        # Dot product:
-                        return (
-                            self.u * otherUnitVector.u
-                            + self.v * otherUnitVector.v
-                            + self.w * otherUnitVector.w
-                        )
-
-                planeNormal = postproc.magneticFieldOnCutPlane.planeNormal
-                if len(planeNormal) != 3:
-                    raise ValueError(
-                        "planeNormal for magneticFieldOnCutPlane must be a list of"
-                        " three numbers!"
-                    )
-
-                planeNormal = unitVector(planeNormal[0], planeNormal[1], planeNormal[2])
-
-                # planeXAxis = postproc.magneticFieldOnCutPlane.planeXAxis
-                # if len(planeXAxis) != 3:
-                #     raise ValueError(
-                #         "planeXAxis for magneticFieldOnCutPlane must be a list of"
-                #         " three numbers!"
-                #     )
-
-                # planeXAxis = unitVector(planeXAxis[0], planeXAxis[1], planeXAxis[2])
-
-                # if (
-                #     math.isclose(planeNormal * planeXAxis, 0, abs_tol=geo.dimTol)
-                #     == False
-                # ):
-                #     raise ValueError(
-                #         "planeNormal and planeXAxis must be perpendicular to each"
-                #         " other! If planeNormal is chosen arbitrarily, planeXAxis must"
-                #         " be specified."
-                #     )
-
-                # A plane that passes through the origin with the normal vector planeNormal
-                # can be defined as:
-                # a*x + b*y + c*z = 0
-                a = planeNormal.u
-                b = planeNormal.v
-                c = planeNormal.w
-
-                # Pick three points on the plane to define a rectangle. The points will
-                # be the corners of the rectangle.
-
-                # To do that, change coordinate system:
-
-                # Find a vector that is perpendicular to planeNormal:
-                randomVector = unitVector(c, a, b)
-                perpendicularVector1 = planeNormal**randomVector
-
-                # Rotate perperndicular vector with respect to the plane's normal vector
-                # by 90 degrees to find the second perpendicular vector:
-                perpendicularVector2 = perpendicularVector1.rotate(
-                    math.pi / 2, planeNormal
-                )
-
-                # Build the transformation matrix to change from the plane's coordinate
-                # system to the global coordinate system:
-                transformationMatrix = np.array(
-                    [
-                        [
-                            perpendicularVector1.u,
-                            perpendicularVector1.v,
-                            perpendicularVector1.w,
-                        ],
-                        [
-                            perpendicularVector2.u,
-                            perpendicularVector2.v,
-                            perpendicularVector2.w,
-                        ],
-                        [planeNormal.u, planeNormal.v, planeNormal.w],
-                    ]
-                )
-                transformationMatrix = np.linalg.inv(transformationMatrix)
-
-                # Select three points to define the rectangle. Pick large points because
-                # only the intersection of the rectangle and the mesh will be used.
-                if geo.ai.type == "cuboid":
-                    airMaxWidth = 2 * math.sqrt(
-                        (geo.ai.a / 2) ** 2 + (geo.ai.a / 2) ** 2
-                    )
-                if geo.ai.type == "cylinder":
-                    airMaxWidth = geo.ai.r
-
-                point1InPlaneCoordinates = np.array(
-                    [5 * max(airMaxWidth, geo.ai.h), 5 * max(airMaxWidth, geo.ai.h), 0]
-                )
-                point1 = transformationMatrix @ point1InPlaneCoordinates
-
-                point2InPlaneCoordinates = np.array(
-                    [-5 * max(airMaxWidth, geo.ai.h), 5 * max(airMaxWidth, geo.ai.h), 0]
-                )
-                point2 = transformationMatrix @ point2InPlaneCoordinates
-
-                point3InPlaneCoordinates = np.array(
-                    [
-                        -5 * max(airMaxWidth, geo.ai.h),
-                        -5 * max(airMaxWidth, geo.ai.h),
-                        0,
-                    ]
-                )
-                point3 = transformationMatrix @ point3InPlaneCoordinates
-
-                # Round the point coordinates to the nearest multiple of the dimTol:
-                point1[0] = round(point1[0] / geo.dimTol) * geo.dimTol
-                point1[1] = round(point1[1] / geo.dimTol) * geo.dimTol
-                point1[2] = round(point1[2] / geo.dimTol) * geo.dimTol
-                point2[0] = round(point2[0] / geo.dimTol) * geo.dimTol
-                point2[1] = round(point2[1] / geo.dimTol) * geo.dimTol
-                point2[2] = round(point2[2] / geo.dimTol) * geo.dimTol
-                point3[0] = round(point3[0] / geo.dimTol) * geo.dimTol
-                point3[1] = round(point3[1] / geo.dimTol) * geo.dimTol
-                point3[2] = round(point3[2] / geo.dimTol) * geo.dimTol
-
-                postproc.magneticFieldOnCutPlane.onSection = [
-                    [float(point1[0]), float(point1[1]), float(point1[2])],
-                    [float(point2[0]), float(point2[1]), float(point2[2])],
-                    [float(point3[0]), float(point3[1]), float(point3[2])],
-                ]
-
-                # Add break points:
-                if postproc.magneticFieldOnCutPlane.timesToBePlotted is not None:
-                    solve.t.adaptive.breakPoints.extend(
-                        postproc.magneticFieldOnCutPlane.timesToBePlotted
-                    )
-                    solve.t.adaptive.breakPoints = list(
-                        set(solve.t.adaptive.breakPoints)
-                    )
-                    solve.t.adaptive.breakPoints.sort()
+        if isinstance(
+            model["mesh"]["winding"]["azimuthalNumberOfElementsPerTurn"], int
+        ):
+            model["mesh"]["winding"]["azimuthalNumberOfElementsPerTurn"] = [
+                model["mesh"]["winding"]["azimuthalNumberOfElementsPerTurn"]
+            ] * model["geometry"]["numberOfPancakes"]
+
+        if isinstance(model["mesh"]["winding"]["radialNumberOfElementsPerTurn"], int):
+            model["mesh"]["winding"]["radialNumberOfElementsPerTurn"] = [
+                model["mesh"]["winding"]["radialNumberOfElementsPerTurn"]
+            ] * model["geometry"]["numberOfPancakes"]
+
+        if isinstance(model["mesh"]["winding"]["axialNumberOfElements"], int):
+            model["mesh"]["winding"]["axialNumberOfElements"] = [
+                model["mesh"]["winding"]["axialNumberOfElements"]
+            ] * model["geometry"]["numberOfPancakes"]
+
+        if isinstance(model["mesh"]["winding"]["elementType"], str):
+            model["mesh"]["winding"]["elementType"] = [
+                model["mesh"]["winding"]["elementType"]
+            ] * model["geometry"]["numberOfPancakes"]
 
-        values["postproc"] = postproc
+        if isinstance(
+            model["mesh"]["contactLayer"]["radialNumberOfElementsPerTurn"], int
+        ):
+            model["mesh"]["contactLayer"]["radialNumberOfElementsPerTurn"] = [
+                model["mesh"]["contactLayer"]["radialNumberOfElementsPerTurn"]
+            ] * model["geometry"]["numberOfPancakes"]
+
+        geometry_input.set(model["geometry"])
+        mesh_input.set(model["mesh"])
+        solve_input.set(model["solve"])
+        input_file_path.set(model["input_file_path"])
 
-        return values
+        return model
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fiqus-2024.1.1/fiqus/data/DataMultipole.py` & `fiqus-2024.4.0/fiqus/data/DataMultipole.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from pydantic import BaseModel
-from typing import (Dict, List)
+from typing import (Dict, List, Optional)
 
 
 class Coord(BaseModel):
-    x: float = None
-    y: float = None
+    x: Optional[float] = None
+    y: Optional[float] = None
 
 
 class Area(BaseModel):
-    loop: int = None
-    surface: int = None
+    loop: Optional[int] = None
+    surface: Optional[int] = None
 
 
 class Region(BaseModel):
-    points: Dict[str, int] = {}
-    lines: Dict[str, int] = {}
-    areas: Dict[str, Area] = {}
+    points: Dict[str | int, int] = {}
+    lines: Dict[str | int, int] = {}
+    areas: Dict[str | int, Area] = {}
 
 
 class BlockData(BaseModel):
     half_turns: Region = Region()
-    current_sign: int = None
+    current_sign: Optional[int] = None
 
 
 class Block(BaseModel):
     blocks: Dict[int, BlockData] = {}
-    conductor_name: str = None
-    conductors_number: int = None
+    conductor_name: Optional[str] = None
+    conductors_number: Optional[int] = None
 
 
 class Winding(BaseModel):
     windings: Dict[int, Block] = {}
 
 
 class Layer(BaseModel):
@@ -44,19 +44,19 @@
 
 class Iron(BaseModel):
     quadrants: Dict[int, Region] = {}
     max_radius: float = 0.
 
 
 class Order(BaseModel):
-    coil: int = None
-    pole: int = None
-    layer: int = None
-    winding: int = None
-    block: int = None
+    coil: Optional[int] = None
+    pole: Optional[int] = None
+    layer: Optional[int] = None
+    winding: Optional[int] = None
+    block: Optional[int] = None
 
 
 class Coil(BaseModel):
     coils: Dict[int, Pole] = {}
     electrical_order: List[Order] = []
```

### Comparing `fiqus-2024.1.1/fiqus/data/RegionsModelFiQuS.py` & `fiqus-2024.4.0/fiqus/data/RegionsModelFiQuS.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 from pydantic import BaseModel
-from typing import (List, Dict)
+from typing import (List, Dict, Optional)
 
 
 class Region(BaseModel):
-    name: str = None
-    number: int = None
+    name: Optional[str] = None
+    number: Optional[int] = None
 
 
 class Regions(BaseModel):
-    names: List[str] = None
-    numbers: List[int] = None
+    names: Optional[List[str]] = None
+    numbers: Optional[List[int]] = None
 
 
 class TwoParBoundaryRegions(BaseModel):
-    names: List[List[str]] = None
-    numbers: List[List[int]] = None
-    values: List[List[float]] = None
+    names: Optional[List[List[str]]] = None
+    numbers: Optional[List[List[int]]] = None
+    values: Optional[List[List[float]]] = None
 
 
 class OneParBoundaryRegions(BaseModel):
-    names: List[List[str]] = None
-    numbers: List[List[int]] = None
-    value: List[float] = None
+    names: Optional[List[List[str]]] = None
+    numbers: Optional[List[List[int]]] = None
+    value: Optional[List[float]] = None
 
 
 class PoweredRegions(BaseModel):
-    names: List[str] = None
-    numbers: List[int] = None
-    currents: List[float] = None
-    sigmas: List[float] = None
-    mu_rs: List[float] = None
+    names: Optional[List[str]] = None
+    numbers: Optional[List[int]] = None
+    currents: Optional[List[float]] = None
+    sigmas: Optional[List[float]] = None
+    mu_rs: Optional[List[float]] = None
 
 
 class InducedRegions(BaseModel):
-    names: List[str] = None
-    numbers: List[int] = None
-    sigmas: List[float] = None
-    mu_rs: List[float] = None
+    names: Optional[List[str]] = None
+    numbers: Optional[List[int]] = None
+    sigmas: Optional[List[float]] = None
+    mu_rs: Optional[List[float]] = None
 
 
 class InsulatorRegions(BaseModel):
-    names: List[str] = None
-    numbers: List[int] = None
-    sigmas: List[float] = None
-    mu_rs: List[float] = None
+    names: Optional[List[str]] = None
+    numbers: Optional[List[int]] = None
+    sigmas: Optional[List[float]] = None
+    mu_rs: Optional[List[float]] = None
 
 
 class IronRegions(BaseModel):
-    names: List[str] = None
-    numbers: List[int] = None
-    sigmas: List[float] = None
-    mu_rs: List[float] = None
+    names: Optional[List[str]] = None
+    numbers: Optional[List[int]] = None
+    sigmas: Optional[List[float]] = None
+    mu_rs: Optional[List[float]] = None
 
 
 class AirRegion(BaseModel):
-    name: str = None
-    number: int = None
-    sigma: float = None
-    mu_r: float = None
+    name: Optional[str] = None
+    number: Optional[int] = None
+    sigma: Optional[float] = None
+    mu_r: Optional[float] = None
 
 
 class AirFarFieldRegions(BaseModel):
-    names: List[str] = None
-    numbers: List[int] = None
-    radius_in: float = None
-    radius_out: float = None
+    names: Optional[List[str]] = None
+    numbers: Optional[List[int]] = None
+    radius_in: Optional[float] = None
+    radius_out: Optional[float] = None
 
 
 class NonPermeableSourceRegion(BaseModel):
-    name: str = None
-    number: int = None
-    sigma: float = None
-    mu_r: float = None
+    name: Optional[str] = None
+    number: Optional[int] = None
+    sigma: Optional[float] = None
+    mu_r: Optional[float] = None
 
 
 class SourceFreeRegion(BaseModel):
-    name: str = None
-    number: int = None
-    sigma: float = None
-    mu_r: float = None
+    name: Optional[str] = None
+    number: Optional[int] = None
+    sigma: Optional[float] = None
+    mu_r: Optional[float] = None
 
 
 class Powered(BaseModel):
     vol: PoweredRegions = PoweredRegions()  # volume region
     vol_in: Region = Region()  # input terminal volume region
     vol_out: Region = Region()  # input terminal volume region
     conductors: Dict[str, List[str]] = {}  # conductor types
@@ -171,15 +171,15 @@
     thin_shells: List[List[int]] = []
     layers_material: List[List[str]] = []
     thicknesses: List[List[float]] = []
 
 
 class ThinShell(BaseModel):
     groups: Dict[str, List[int]] = {}
-    mid_turns_layers_poles: List[int] = None
+    mid_turns_layers_poles: Optional[List[int]] = None
     second_group_is_next: Dict[str, List[int]] = {}
     normals_directed: Dict[str, List[int]] = {}
     insulation_types: InsulationType = InsulationType()
     quench_heaters: InsulationType = InsulationType()
 
 
 class RegionsModel(BaseModel):
```

### Comparing `fiqus-2024.1.1/fiqus/geom_generators/GeometryCCT.py` & `fiqus-2024.4.0/fiqus/geom_generators/GeometryCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/geom_generators/GeometryMultipole.py` & `fiqus-2024.4.0/fiqus/geom_generators/GeometryMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/geom_generators/GeometryPancake3D.py` & `fiqus-2024.4.0/fiqus/geom_generators/GeometryPancake3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -551,21 +551,21 @@
                         )
                     else:
                         dictionary[dimTagsObject.parentName].extend(
                             dimTagsObject.getDimTags()
                         )
                 else:
                     if forPhysicalGroups:
-                        dictionary[
-                            dimTagsObject.parentName
-                        ] = dimTagsObject.getDimTagsForPG()
+                        dictionary[dimTagsObject.parentName] = (
+                            dimTagsObject.getDimTagsForPG()
+                        )
                     else:
-                        dictionary[
-                            dimTagsObject.parentName
-                        ] = dimTagsObject.getDimTags()
+                        dictionary[dimTagsObject.parentName] = (
+                            dimTagsObject.getDimTags()
+                        )
             if forPhysicalGroups:
                 dictionary[name] = dimTagsObject.getDimTagsForPG()
             else:
                 dictionary[name] = dimTagsObject.getDimTags()
 
         return dictionary
 
@@ -739,14 +739,15 @@
     def __init__(
         self,
         innerRadius,
         gap,
         turns,
         z,
         initialTheta,
+        transitionNotchAngle,
         direction=direction.ccw,
         cutPlaneNormal=Tuple[float, float, float],
     ) -> None:
         spt = self.sectionsPerTurn  # just to make the code shorter
         self.turnRes = 1 / spt  # turn resolution
         cpt = self.curvesPerTurn  # just to make the code shorter
         self.turns = turns
@@ -806,40 +807,56 @@
                     and breakPoint2 < initialTheta + 2 * math.pi * self.turns
                 ):
                     listOfBreakPoints.append(breakPoint2)
 
             thetaArrays.append(np.array(listOfBreakPoints))
 
         theta = np.concatenate(thetaArrays)
+        theta = np.round(theta, 10)
         theta = np.unique(theta)
         theta = np.sort(theta)
         theta = theta[::multiplier]
 
         r = innerRadius + (theta - initialTheta) / (2 * math.pi) * (gap) * multiplier
         z = np.ones(theta.shape) * z
 
         # Create the points and store their tags:
         points = []  # point objects
         pointTags = []  # point tags
         breakPointObjectsDueToCutPlane = []  # only used if cutPlaneNormal is not None
         breakPointTagsDueToCutPlane = []  # only used if cutPlaneNormal is not None
         pointObjectsWithoutBreakPoints = []  # only used if cutPlaneNormal is not None
         pointTagsWithoutBreakPoints = []  # only used if cutPlaneNormal is not None
+        breakPointObjectsDueToTransition = []
+        breakPointTagsDueToTransition = []
+
         for j in range(len(theta)):
             pointObject = point(r[j], theta[j], z[j], coordinate.cylindrical)
             points.append(pointObject)
             pointTags.append(pointObject.tag)
             if cutPlaneNormal is not None:
                 if theta[j] in listOfBreakPoints:
                     breakPointObjectsDueToCutPlane.append(pointObject)
                     breakPointTagsDueToCutPlane.append(pointObject.tag)
                 else:
                     pointObjectsWithoutBreakPoints.append(pointObject)
                     pointTagsWithoutBreakPoints.append(pointObject.tag)
 
+            # identify if the point is a break point due to the layer transition:
+            angle1 = initialTheta + (2 * math.pi - transitionNotchAngle) * multiplier
+            angle2 = (
+                initialTheta
+                + ((self.turns % 1) * 2 * math.pi + transitionNotchAngle) * multiplier
+            )
+            if math.isclose(
+                math.fmod(theta[j], 2 * math.pi), angle1, abs_tol=1e-6
+            ) or math.isclose(math.fmod(theta[j], 2 * math.pi), angle2, abs_tol=1e-6):
+                breakPointObjectsDueToTransition.append(pointObject)
+                breakPointTagsDueToTransition.append(pointObject.tag)
+
         # =============================================================================
         # GENERATING POINTS ENDS ======================================================
         # =============================================================================
 
         # =============================================================================
         # GENERATING SPLINES STARTS ===================================================
         # =============================================================================
@@ -860,24 +877,26 @@
             pointObjectsWithoutBreakPoints = points
             pointTagsWithoutBreakPoints = pointTags
 
         splitPointTags = list(
             set(pointTagsWithoutBreakPoints[:-1:sectionsPerCurve])
             | set(pointTagsWithoutBreakPoints[-spt - 1 :: -spt])
             | set(breakPointTagsDueToCutPlane)
+            | set(breakPointTagsDueToTransition)
         )
         splitPointTags = sorted(splitPointTags)
         # Remove the first element of the list (starting point):
         _, *splitPointTags = splitPointTags
 
         # Also create a list of corresponding point objects:
         splitPoints = list(
             set(pointObjectsWithoutBreakPoints[:-1:sectionsPerCurve])
             | set(pointObjectsWithoutBreakPoints[-spt - 1 :: -spt])
             | set(breakPointObjectsDueToCutPlane)
+            | set(breakPointObjectsDueToTransition)
         )
         splitPoints = sorted(splitPoints, key=lambda x: x.tag)
         # Remove the first element of the list (starting point):
         _, *splitPoints = splitPoints
 
         # Split the spline:
         dims = [0] * len(splitPointTags)
@@ -1044,27 +1063,30 @@
         self,
         innerRadius,
         thickness,
         contactLayerThickness,
         turns,
         z,
         initialTheta,
+        transitionNotchAngle,
         spiralDirection=direction.ccw,
         thinShellApproximation=False,
         cutPlaneNormal=None,
     ) -> None:
         r_i = innerRadius
         t = thickness
         theta_i = initialTheta
         self.theta_i = theta_i
 
         self.surfaceTags = []
         self.contactLayerSurfaceTags = []
 
         self.direction = spiralDirection
+        self.tsa = thinShellApproximation
+        self.transitionNotchAngle = transitionNotchAngle
         # =============================================================================
         # GENERATING SPIRAL CURVES STARTS =============================================
         # =============================================================================
         if thinShellApproximation:
             # Create only one spiral curve because the thin shell approximation is used:
             # Winding thickness is increased slightly to ensure that the outer radius
             # would be the same without the thin shell approximation.
@@ -1073,38 +1095,41 @@
             )  # for TSA, spiral has (n+1) turns but spiral surface has n
             spiral = spiralCurve(
                 r_i,
                 t + contactLayerThickness * (turns - 1) / (turns),
                 turns,
                 z,
                 theta_i,
+                transitionNotchAngle,
                 spiralDirection,
                 cutPlaneNormal=cutPlaneNormal,
             )
 
             # These are created to be able to use the same code with TSA and without TSA:
             innerSpiral = spiral
             outerSpiral = spiral
         else:
             # Create two spiral curves because the thin shell approximation is not used:
             innerSpiral = spiralCurve(
-                r_i,
+                r_i - contactLayerThickness,
                 t + contactLayerThickness,
-                turns,
+                turns + 1,
                 z,
                 theta_i,
+                transitionNotchAngle,
                 spiralDirection,
                 cutPlaneNormal=cutPlaneNormal,
             )
             outerSpiral = spiralCurve(
-                r_i + t,
+                r_i,
                 t + contactLayerThickness,
-                turns,
+                turns + 1,
                 z,
                 theta_i,
+                transitionNotchAngle,
                 spiralDirection,
                 cutPlaneNormal=cutPlaneNormal,
             )
 
         self.innerSpiral = innerSpiral
         self.outerSpiral = outerSpiral
         self.turns = turns
@@ -1135,24 +1160,24 @@
 
                 if startTurn + 1 + 1e-4 > turns:
                     # If the current spline is on the outer surface, break the loop,
                     # because the whole surface is finished:
                     break
 
                 # Find the outer spline tag:
-                isItBroken = False
+                isItBroken = True
                 for j, turnTuple in enumerate(spiral.splineTurns):
                     # Equality can not be checked with == because of the floating point
                     # errors:
                     if abs(turnTuple[0] - 1 - startTurn) < 1e-4:
                         outerSplineTag = spiral.splineTags[j]
-                        isItBroken = True
+                        isItBroken = False
                         break
 
-                if not isItBroken:
+                if isItBroken:
                     raise RuntimeError(
                         "Something went wrong while creating the spiral surface. Outer"
                         f" spline tag of {innerSplineTag} could not be found for TSA."
                     )
 
             else:
                 # Store the tags of the current splines:
@@ -1165,15 +1190,15 @@
 
                 # Find the spline tag of the contact layer's outer spline by finding the
                 # spline tag of the spline that is exactly on the next turn:
 
                 # Note the turn number of the current spline's start point:
                 startTurn = outerSpiral.splineTurns[i][0]
 
-                if startTurn + 1 + 1e-4 > turns:
+                if startTurn + 1 + 1e-4 > turns + 1:
                     # If the current spline is on the outer surface, note that all the
                     # contact layers are finished:
                     allContactLayersAreFinished = True
 
                 # Find the contact layer's outer spline tag:
                 for j, turnTuple in enumerate(innerSpiral.splineTurns):
                     if math.isclose(turnTuple[0], 1 + startTurn, abs_tol=1e-6):
@@ -1301,46 +1326,139 @@
         # 3- How you put the curves in the curve loops is very important! The same curve
         #     loop with the same lines might cause problems if the user puts them in a
         #     different order. For example, to create a plane surface with two curve
         #     loops, the direction of the curve loops should be the same. That's why the
         #     code has both innerCurveLoopTag and innerOppositeCurveLoopTag (the same
         #     thing for the outer curve loop).
 
+        # create the transition layer (notch):
         # Inner curve loop:
-        lines = innerSpiral.getSplineTags(0, 1)  # The first turn of the spline
+        notchStartPoint = innerSpiral.getPointTag(
+            1 - transitionNotchAngle / (2 * math.pi)
+        )
+        notchLeftPoint = innerSpiral.getPointTag(0)
+        notchLeftLine = gmsh.model.occ.addLine(notchStartPoint, notchLeftPoint)
+        notchRightLine = innerSpiral.getSplineTag(
+            1 - transitionNotchAngle / (2 * math.pi)
+        )
+
         if thinShellApproximation:
             innerStartCurves = [firstStartLine]
         else:
             innerStartCurves = [firstInsStartLine, firstStartLine]
 
-        innerCurves = lines + innerStartCurves
+        if thinShellApproximation:
+
+            notchCurveLoop = gmsh.model.occ.addCurveLoop(
+                [notchLeftLine, notchRightLine] + innerStartCurves
+            )
+            self.innerNotchSurfaceTags = [
+                gmsh.model.occ.addPlaneSurface([notchCurveLoop])
+            ]
+        else:
+            notchMiddlePoint = outerSpiral.getPointTag(0)
+            notchMiddleLine = gmsh.model.occ.addLine(notchStartPoint, notchMiddlePoint)
+
+            notchCurveLoop1 = gmsh.model.occ.addCurveLoop(
+                [notchLeftLine, notchMiddleLine, firstStartLine]
+            )
+            notchCurveLoop2 = gmsh.model.occ.addCurveLoop(
+                [notchMiddleLine, notchRightLine, firstInsStartLine]
+            )
+            self.innerNotchSurfaceTags = [
+                gmsh.model.occ.addPlaneSurface([notchCurveLoop1]),
+                gmsh.model.occ.addPlaneSurface([notchCurveLoop2]),
+            ]
+
+        lines = innerSpiral.getSplineTags(
+            0, 1 - transitionNotchAngle / (2 * math.pi)
+        )  # The first turn of the spline
+        innerCurves = lines + [notchLeftLine]
+        self.innerNotchLeftLine = notchLeftLine
 
         self.innerStartCurves = innerStartCurves
 
         self.innerCurveLoopTag = gmsh.model.occ.addCurveLoop(innerCurves)
         self.innerOppositeCurveLoopTag = gmsh.model.occ.addCurveLoop(innerCurves[::-1])
 
         # Outer curve loop:
         # The last turn of the spline:
-        lines = outerSpiral.getSplineTags(turns - 1, turns)
+        if thinShellApproximation:
+            notchStartPoint = innerSpiral.getPointTag(
+                self.turns + transitionNotchAngle / (2 * math.pi) - 1
+            )
+            notchLeftPoint = innerSpiral.getPointTag(self.turns)
+            notchLeftLine = gmsh.model.occ.addLine(notchStartPoint, notchLeftPoint)
+            notchRightLine = innerSpiral.getSplineTag(
+                self.turns - 1 + transitionNotchAngle / (2 * math.pi), endPoint=True
+            )
+        else:
+            notchStartPoint = outerSpiral.getPointTag(
+                self.turns + transitionNotchAngle / (2 * math.pi)
+            )
+            notchMiddlePoint = innerSpiral.getPointTag(self.turns + 1)
+            notchLeftPoint = outerSpiral.getPointTag(self.turns + 1)
+            notchLeftLine = gmsh.model.occ.addLine(notchStartPoint, notchLeftPoint)
+            notchMiddleLine = gmsh.model.occ.addLine(notchStartPoint, notchMiddlePoint)
+            notchRightLine = outerSpiral.getSplineTag(
+                self.turns + transitionNotchAngle / (2 * math.pi), self.turns
+            )
+        if thinShellApproximation:
+            lines = outerSpiral.getSplineTags(turns - 1, turns)
+        else:
+            lines = outerSpiral.getSplineTags(turns, turns + 1)
+
         if thinShellApproximation:
             outerEndCurves = [endLines[-1]]
         else:
             outerEndCurves = [endInsLines[-1], endLines[-1]]
 
-        outerCurves = lines + outerEndCurves
+        if thinShellApproximation:
+            notchCurveLoop1 = gmsh.model.occ.addCurveLoop(
+                [notchLeftLine, notchRightLine, endLines[-1]]
+            )
+            self.outerNotchSurfaceTags = [
+                gmsh.model.occ.addPlaneSurface([notchCurveLoop1]),
+            ]
+        else:
+            notchCurveLoop1 = gmsh.model.occ.addCurveLoop(
+                [notchLeftLine, notchMiddleLine, endLines[-1]]
+            )
+            notchCurveLoop2 = gmsh.model.occ.addCurveLoop(
+                [notchMiddleLine, notchRightLine, endInsLines[-1]]
+            )
+            self.outerNotchSurfaceTags = [
+                gmsh.model.occ.addPlaneSurface([notchCurveLoop1]),
+                gmsh.model.occ.addPlaneSurface([notchCurveLoop2]),
+            ]
+
+        if thinShellApproximation:
+            lines = innerSpiral.getSplineTags(
+                self.turns - 1 + transitionNotchAngle / (2 * math.pi), self.turns
+            )  # The first turn of the spline
+        else:
+            lines = outerSpiral.getSplineTags(
+                self.turns + transitionNotchAngle / (2 * math.pi), self.turns + 1
+            )
+        outerCurves = lines + [notchLeftLine]
+        self.outerNotchLeftLine = notchLeftLine
 
         self.outerEndCurves = outerEndCurves
 
         self.outerCurveLoopTag = gmsh.model.occ.addCurveLoop(outerCurves)
         self.outerOppositeCurveLoopTag = gmsh.model.occ.addCurveLoop(outerCurves[::-1])
         # =============================================================================
         # GENERATING CURVE LOOPS ENDS =================================================
         # =============================================================================
 
+        if not thinShellApproximation:
+            surfaceTags = self.surfaceTags
+            self.surfaceTags = self.contactLayerSurfaceTags
+            self.contactLayerSurfaceTags = surfaceTags
+
     def getInnerRightPointTag(self):
         """
         Returns the point tag of the inner left point.
 
         :return: point tag
         :rtype: int
         """
@@ -1382,165 +1500,225 @@
     def getOuterRightPointTag(self):
         """
         Returns the point tag of the outer left point.
 
         :return: point tag
         :rtype: int
         """
-        return self.outerSpiral.getPointTag(self.turns, endPoint=False)
+        if self.tsa:
+            turns = self.turns
+        else:
+            turns = self.turns + 1
+        return self.outerSpiral.getPointTag(turns, endPoint=False)
 
     def getOuterLowerPointTag(self):
         """
         Returns the point tag of the outer right point.
 
         :return: point tag
         :rtype: int
         """
+        if self.tsa:
+            turns = self.turns
+        else:
+            turns = self.turns + 1
         if self.direction is direction.ccw:
-            return self.outerSpiral.getPointTag(self.turns - 0.25, endPoint=False)
+            return self.outerSpiral.getPointTag(turns - 0.25, endPoint=False)
         else:
-            return self.outerSpiral.getPointTag(self.turns - 0.75, endPoint=False)
+            return self.outerSpiral.getPointTag(turns - 0.75, endPoint=False)
 
     def getOuterLeftPointTag(self):
         """
         Returns the point tag of the outer upper point.
 
         :return: point tag
         :rtype: int
         """
-        return self.outerSpiral.getPointTag(self.turns - 0.5, endPoint=False)
+        if self.tsa:
+            turns = self.turns
+        else:
+            turns = self.turns + 1
+        return self.outerSpiral.getPointTag(turns - 0.5, endPoint=False)
 
     def getOuterUpperPointTag(self):
         """
         Returns the point tag of the outer lower point.
 
         :return: point tag
         :rtype: int
         """
+        if self.tsa:
+            turns = self.turns
+        else:
+            turns = self.turns + 1
         if self.direction is direction.ccw:
-            return self.outerSpiral.getPointTag(self.turns - 0.75, endPoint=False)
+            return self.outerSpiral.getPointTag(turns - 0.75, endPoint=False)
         else:
-            return self.outerSpiral.getPointTag(self.turns - 0.25, endPoint=False)
+            return self.outerSpiral.getPointTag(turns - 0.25, endPoint=False)
 
     def getInnerUpperRightCurves(self):
         """
         Returns the curve tags of the upper right curves.
 
         :return: curve tags
         :rtype: list[int]
         """
-
         if self.direction is direction.ccw:
             curves = self.innerSpiral.getSplineTags(0, 0.25)
         else:
-            curves = self.innerSpiral.getSplineTags(0.75, 1)
+            lines = self.innerSpiral.getSplineTags(
+                0.75, 1 - self.transitionNotchAngle / (2 * math.pi)
+            )  # The first turn of the spline
+            lines = lines + [self.innerNotchLeftLine]
+
+            return lines
 
         return curves
 
     def getInnerUpperLeftCurves(self):
         """
         Returns the curve tags of the upper left curves.
 
         :return: curve tags
         :rtype: list[int]
         """
-
         if self.direction is direction.ccw:
             curves = self.innerSpiral.getSplineTags(0.25, 0.5)
         else:
             curves = self.innerSpiral.getSplineTags(0.5, 0.75)
 
         return curves
 
     def getInnerLowerLeftCurves(self):
         """
         Returns the curve tags of the lower left curves.
 
         :return: curve tags
         :rtype: list[int]
         """
-
         if self.direction is direction.ccw:
             curves = self.innerSpiral.getSplineTags(0.5, 0.75)
         else:
             curves = self.innerSpiral.getSplineTags(0.25, 0.5)
 
         return curves
 
     def getInnerLowerRightCurves(self):
         """
         Returns the curve tags of the lower right curves.
 
         :return: curve tags
         :rtype: list[int]
         """
-
         if self.direction is direction.ccw:
-            curves = self.innerSpiral.getSplineTags(0.75, 1)
+            lines = self.innerSpiral.getSplineTags(
+                0.75, 1 - self.transitionNotchAngle / (2 * math.pi)
+            )  # The first turn of the spline
+            lines = lines + [self.innerNotchLeftLine]
+
+            return lines
         else:
             curves = self.innerSpiral.getSplineTags(0, 0.25)
 
         return curves
 
     def getOuterUpperRightCurves(self):
         """
         Returns the curve tags of the upper right curves.
 
         :return: curve tags
         :rtype: list[int]
         """
+        if self.tsa:
+            turns = self.turns
+        else:
+            turns = self.turns + 1
 
         if self.direction is direction.ccw:
-            curves = self.outerSpiral.getSplineTags(self.turns - 1, self.turns - 0.75)
+            if self.tsa:
+                lines = self.innerSpiral.getSplineTags(
+                    self.turns - 1 + self.transitionNotchAngle / (2 * math.pi),
+                    self.turns - 0.75,
+                )  # The first turn of the spline
+            else:
+                lines = self.outerSpiral.getSplineTags(
+                    self.turns + self.transitionNotchAngle / (2 * math.pi),
+                    self.turns + 1 - 0.75,
+                )
+            lines = lines + [self.outerNotchLeftLine]
+
+            return lines
         else:
-            curves = self.outerSpiral.getSplineTags(self.turns - 0.25, self.turns)
+            curves = self.outerSpiral.getSplineTags(turns - 0.25, turns)
 
         return curves
 
     def getOuterUpperLeftCurves(self):
         """
         Returns the curve tags of the lower right curves.
 
         :return: curve tags
         :rtype: list[int]
         """
-
+        if self.tsa:
+            turns = self.turns
+        else:
+            turns = self.turns + 1
         if self.direction is direction.ccw:
-            curves = self.outerSpiral.getSplineTags(self.turns - 0.75, self.turns - 0.5)
+            curves = self.outerSpiral.getSplineTags(turns - 0.75, turns - 0.5)
         else:
-            curves = self.outerSpiral.getSplineTags(self.turns - 0.5, self.turns - 0.25)
+            curves = self.outerSpiral.getSplineTags(turns - 0.5, turns - 0.25)
 
         return curves
 
     def getOuterLowerLeftCurves(self):
         """
         Returns the curve tags of the lower left curves.
 
         :return: curve tags
         :rtype: list[int]
         """
+        if self.tsa:
+            turns = self.turns
+        else:
+            turns = self.turns + 1
         if self.direction is direction.ccw:
-            curves = self.outerSpiral.getSplineTags(self.turns - 0.5, self.turns - 0.25)
+            curves = self.outerSpiral.getSplineTags(turns - 0.5, turns - 0.25)
         else:
-            curves = self.outerSpiral.getSplineTags(self.turns - 0.75, self.turns - 0.5)
+            curves = self.outerSpiral.getSplineTags(turns - 0.75, turns - 0.5)
 
         return curves
 
     def getOuterLowerRightCurves(self):
         """
         Returns the curve tags of the upper left curves.
 
         :return: curve tags
         :rtype: list[int]
         """
-
+        if self.tsa:
+            turns = self.turns
+        else:
+            turns = self.turns + 1
         if self.direction is direction.ccw:
-            curves = self.outerSpiral.getSplineTags(self.turns - 0.25, self.turns)
+            curves = self.outerSpiral.getSplineTags(turns - 0.25, turns)
         else:
-            curves = self.outerSpiral.getSplineTags(self.turns - 1, self.turns - 0.75)
+            if self.tsa:
+                lines = self.innerSpiral.getSplineTags(
+                    self.turns - 1 + self.transitionNotchAngle / (2 * math.pi),
+                    self.turns - 0.75,
+                )  # The first turn of the spline
+            else:
+                lines = self.outerSpiral.getSplineTags(
+                    self.turns + self.transitionNotchAngle / (2 * math.pi),
+                    self.turns + 1 - 0.75,
+                )
+            lines = lines + [self.outerNotchLeftLine]
+
+            return lines
 
         return curves
 
     def getInnerStartCurves(self):
         """
         Returns the curve tags of the start curves.
 
@@ -2061,15 +2239,15 @@
             middleCircle.lowerPointTag, winding.getOuterLowerPointTag()
         )
 
         # Create surfaces for the nontube part:
         if winding.direction is direction.ccw:
             upperRightCurveLoop = gmsh.model.occ.addCurveLoop(
                 winding.getOuterUpperRightCurves()
-                + winding.getOuterEndCurves()
+                # + winding.getOuterEndCurves()
                 + [rightLineTag, middleCircle.upperRightTag, upperLineTag]
             )
         else:
             upperRightCurveLoop = gmsh.model.occ.addCurveLoop(
                 winding.getOuterUpperRightCurves()
                 + [rightLineTag, middleCircle.upperRightTag, upperLineTag]
             )
@@ -2094,15 +2272,15 @@
             lowerRightCurveLoop = gmsh.model.occ.addCurveLoop(
                 winding.getOuterLowerRightCurves()
                 + [rightLineTag, middleCircle.lowerRightTag, lowerLineTag]
             )
         else:
             lowerRightCurveLoop = gmsh.model.occ.addCurveLoop(
                 winding.getOuterLowerRightCurves()
-                + winding.getOuterEndCurves()
+                # + winding.getOuterEndCurves()
                 + [rightLineTag, middleCircle.lowerRightTag, lowerLineTag]
             )
         self.lowerRightTag = gmsh.model.occ.addPlaneSurface([lowerRightCurveLoop])
         self.nontubeSurfaceTags.append(self.lowerRightTag)
 
     def createWithOuterAirAndWinding(
         self, outerAir: outerAirSurface, winding: spiralSurface, pancakeIndex
@@ -2457,15 +2635,15 @@
             upperRightCurveLoop = gmsh.model.occ.addCurveLoop(
                 winding.getInnerUpperRightCurves()
                 + [
                     upperLineTag,
                     middleCircle.upperRightTag,
                     rightLineTag,
                 ]
-                + winding.getInnerStartCurves()
+                # + winding.getInnerStartCurves()
             )
         self.upperRightTag = gmsh.model.occ.addPlaneSurface([upperRightCurveLoop])
         self.nontubeSurfaceTags.append(self.upperRightTag)
 
         upperLeftCurveLoop = gmsh.model.occ.addCurveLoop(
             winding.getInnerUpperLeftCurves()
             + [
@@ -2492,15 +2670,15 @@
             lowerRightCurveLoop = gmsh.model.occ.addCurveLoop(
                 winding.getInnerLowerRightCurves()
                 + [
                     lowerLineTag,
                     middleCircle.lowerRightTag,
                     rightLineTag,
                 ]
-                + winding.getInnerStartCurves()
+                # + winding.getInnerStartCurves()
             )
         else:
             lowerRightCurveLoop = gmsh.model.occ.addCurveLoop(
                 winding.getInnerLowerRightCurves()
                 + [
                     lowerLineTag,
                     middleCircle.lowerRightTag,
@@ -2793,14 +2971,24 @@
         )
 
         # Inner terminal's inner tube part:
         self.innerTerminalTubeVolume = dimTags(
             name=self.geo.ti.i.name + "-Tube", save=True, parentName=self.geo.ti.i.name
         )
 
+        # Transition layers:
+        self.innerTransitionNotchVolume = dimTags(
+            name="innerTransitionNotch",
+            save=True,
+        )
+        self.outerTransitionNotchVolume = dimTags(
+            name="outerTransitionNotch",
+            save=True,
+        )
+
         # Inner air cylinder volume:
         self.centerAirCylinderVolume = dimTags(
             name=self.geo.ai.name + "-InnerCylinder",
             save=True,
             parentName=self.geo.ai.name,
         )
 
@@ -2909,24 +3097,28 @@
                 bottomSurfacesDimTags = []
                 for key, value in topSurfaces.items():
                     if (
                         key is self.individualWinding[self.pancakeIndex - 1]
                         or key is self.individualContactLayer[self.pancakeIndex - 1]
                         or key is self.outerTerminalTouchingVolume
                         or key is self.innerTerminalTouchingVolume
+                        or key is self.innerTransitionNotchVolume
+                        or key is self.outerTransitionNotchVolume
                     ):
                         bottomSurfacesDimTags.extend(value)
 
                 topSurfacesDimTags = []
                 for key, value in self.fundamentalSurfaces.items():
                     if (
                         key is self.individualWinding[self.pancakeIndex]
                         or key is self.individualContactLayer[self.pancakeIndex]
                         or key is self.outerTerminalTouchingVolume
                         or key is self.innerTerminalTouchingVolume
+                        or key is self.innerTransitionNotchVolume
+                        or key is self.outerTransitionNotchVolume
                     ):
                         topSurfacesDimTags.extend(value)
 
                 sideSurfacesDimTags = []
                 if i % 2 == 1:
                     # Touches it tube and air tube
                     bottomSurfacesDimTags.extend(
@@ -3130,14 +3322,15 @@
         surface = spiralSurface(
             self.geo.wi.r_i,
             self.geo.wi.t,
             self.geo.ii.t,
             self.geo.wi.N,
             z,
             self.geo.wi.theta_i,
+            self.geo.ti.transitionNotchAngle,
             spiralDirection,
             thinShellApproximation=self.geo.ii.tsa,
         )
 
         # Save the surface tags (if TSA, contactLayerSurfaceTags will be empty):
         fundamentalSurfaces[self.individualWinding[self.pancakeIndex]] = [
             (2, tag) for tag in surface.surfaceTags
@@ -3311,14 +3504,20 @@
 
         fundamentalSurfaces[self.innerTerminalTubeVolume] = [
             (2, tag) for tag in innerTerminalSurf.tubeSurfaceTags
         ]
         fundamentalSurfaces[self.innerTerminalTouchingVolume] = [
             (2, tag) for tag in innerTerminalSurf.nontubeSurfaceTags
         ]
+        fundamentalSurfaces[self.innerTransitionNotchVolume] = [
+            (2, tag) for tag in surface.innerNotchSurfaceTags
+        ]
+        fundamentalSurfaces[self.outerTransitionNotchVolume] = [
+            (2, tag) for tag in surface.outerNotchSurfaceTags
+        ]
 
         if self.geo.ai.shellTransformation:
             if self.geo.ai.type == "cuboid":
                 fundamentalSurfaces[self.airShellVolumePart1] = [
                     (2, tag) for tag in outerAirSurf.shellTagsPart1
                 ]
                 fundamentalSurfaces[self.airShellVolumePart2] = [
```

### Comparing `fiqus-2024.1.1/fiqus/getdp_runners/RunGetdpCCT.py` & `fiqus-2024.4.0/fiqus/getdp_runners/RunGetdpCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/getdp_runners/RunGetdpMultipole.py` & `fiqus-2024.4.0/fiqus/getdp_runners/RunGetdpMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/getdp_runners/RunGetdpPancake3D.py` & `fiqus-2024.4.0/fiqus/getdp_runners/RunGetdpPancake3D.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/mains/MainCCT.py` & `fiqus-2024.4.0/fiqus/mains/MainCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/mains/MainMultipole.py` & `fiqus-2024.4.0/fiqus/mains/MainMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/mesh_generators/MeshCCT.py` & `fiqus-2024.4.0/fiqus/mesh_generators/MeshCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/mesh_generators/MeshMultipole.py` & `fiqus-2024.4.0/fiqus/mesh_generators/MeshMultipole.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/mesh_generators/MeshPancake3D.py` & `fiqus-2024.4.0/fiqus/mesh_generators/MeshPancake3D.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from enum import Enum
 import operator
 import itertools
 import re
 
 import gmsh
 import scipy.integrate
+import numpy as np
 
 from fiqus.data import RegionsModelFiQuS
 from fiqus.utils.Utils import GmshUtils
 from fiqus.data.RegionsModelFiQuS import RegionsModel
 from fiqus.mains.MainPancake3D import Base
 from fiqus.utils.Utils import FilesAndFolders
 from fiqus.data.DataFiQuSPancake3D import Pancake3DGeometry, Pancake3DMesh
@@ -37,14 +38,15 @@
     A class to specify entity type easily in the regions class.
     """
 
     vol = "vol"
     vol_in = "vol_in"
     vol_out = "vol_out"
     surf = "surf"
+    surf_th = "surf_th"
     surf_in = "surf_in"
     surf_out = "surf_out"
     surf_ext = "surf_ext"
     cochain = "cochain"
     curve = "curve"
     point = "point"
 
@@ -62,14 +64,15 @@
         # The keys are the FiQuS region categories, and the values are the corresponding
         # GMSH entity type.
         self.entityMainType = {
             "vol": "vol",
             "vol_in": "vol",
             "vol_out": "vol",
             "surf": "surf",
+            "surf_th": "surf",
             "surf_in": "surf",
             "surf_out": "surf",
             "surf_ext": "surf",
             "cochain": "curve",
             "curve": "curve",
             "point": "point",
         }
@@ -80,14 +83,15 @@
         # Keys for regions file. The keys are appended to the name of the regions
         # accordingly.
         self.entityKey = {
             "vol": "",
             "vol_in": "",
             "vol_out": "",
             "surf": "_bd",
+            "surf_th": "_bd",
             "surf_in": "_in",
             "surf_out": "_out",
             "surf_ext": "_ext",
             "cochain": "_cut",
             "curve": "_curve",
             "point": "_point",
         }
@@ -109,18 +113,22 @@
 
         # Initializing the required variables (air and powered.vol_in and
         # powered.vol_out are not initialized because they are not lists but numbers):
         self.rm.powered.vol.names = []
         self.rm.powered.vol.numbers = []
         self.rm.powered.surf.names = []
         self.rm.powered.surf.numbers = []
+        self.rm.powered.surf_th.names = []
+        self.rm.powered.surf_th.numbers = []
         self.rm.powered.surf_in.names = []
         self.rm.powered.surf_in.numbers = []
         self.rm.powered.surf_out.names = []
         self.rm.powered.surf_out.numbers = []
+        self.rm.powered.curve.names = []
+        self.rm.powered.curve.numbers = []
 
         self.rm.insulator.vol.names = []
         self.rm.insulator.vol.numbers = []
         self.rm.insulator.surf.names = []
         self.rm.insulator.surf.numbers = []
         self.rm.insulator.curve.names = []
         self.rm.insulator.curve.numbers = []
@@ -160,15 +168,17 @@
         if regionType is regionType.powered:
             if entityType is entityType.vol_in or entityType is entityType.vol_out:
                 getattr(self.rm.powered, entityType).name = name
                 getattr(self.rm.powered, entityType).number = regionTag
 
             else:
                 getattr(self.rm.powered, entityType).names.append(name)
-                getattr(self.rm.powered, entityType).numbers.append(regionTag)
+                getattr(self.rm.powered, entityType).numbers.append(
+                    regionTag
+                )
         elif regionType is regionType.insulator:
             getattr(self.rm.insulator, entityType).names.append(name)
             getattr(self.rm.insulator, entityType).numbers.append(regionTag)
         elif regionType is regionType.air:
             if entityType is entityType.cochain or entityType is entityType.point:
                 getattr(self.rm.air, entityType).names.append(name)
                 getattr(self.rm.air, entityType).numbers.append(regionTag)
@@ -413,14 +423,17 @@
 
         def integrand(t):
             return math.sqrt(a**2 + (a * t + b) ** 2)
 
         return abs(scipy.integrate.quad(integrand, theta1, theta2)[0])
 
 
+alreadyMeshedSurfaceTags = []
+
+
 class Mesh(Base):
     """
     Main mesh class for Pancake3D.
 
     :param fdm: FiQuS data model
     :param geom_folder: folder where the geometry files are saved
     :type geom_folder: str
@@ -461,39 +474,74 @@
         logger.info("Generating Pancake3D mesh has been started.")
 
         start_time = timeit.default_timer()
 
         # =============================================================================
         # MESHING WINDING AND CONTACT LAYER STARTS =======================================
         # =============================================================================
+        allWindingAndCLSurfaceTags = []
+        allWindingAndCLLineTags = []
         for i in range(self.geo.N):
             # Get the volume tags:
             windingVolumeDimTags = self.dimTags[self.geo.wi.name + str(i + 1)]
             windingVolumeTags = [dimTag[1] for dimTag in windingVolumeDimTags]
 
             contactLayerVolumeDimTags = self.dimTags[self.geo.ii.name + str(i + 1)]
             contactLayerVolumeTags = [dimTag[1] for dimTag in contactLayerVolumeDimTags]
 
             # Get the surface and line tags:
             windingSurfaceTags, windingLineTags = self.get_boundaries(
                 windingVolumeDimTags, returnTags=True
             )
+            allWindingAndCLSurfaceTags.extend(windingSurfaceTags)
+            allWindingAndCLLineTags.extend(windingLineTags)
             contactLayerSurfaceTags, contactLayerLineTags = self.get_boundaries(
                 contactLayerVolumeDimTags, returnTags=True
             )
+            allWindingAndCLSurfaceTags.extend(contactLayerSurfaceTags)
+            allWindingAndCLLineTags.extend(contactLayerLineTags)
 
             self.structure_mesh(
                 windingVolumeTags,
                 windingSurfaceTags,
                 windingLineTags,
                 contactLayerVolumeTags,
                 contactLayerSurfaceTags,
                 contactLayerLineTags,
                 meshSettingIndex=i,
             )
+
+        notchVolumesDimTags = (
+            self.dimTags["innerTransitionNotch"] + self.dimTags["outerTransitionNotch"]
+        )
+        notchVolumeTags = [dimTag[1] for dimTag in notchVolumesDimTags]
+
+        notchSurfaceTags, notchLineTags = self.get_boundaries(
+            notchVolumesDimTags, returnTags=True
+        )
+
+        for lineTag in notchLineTags:
+            if lineTag not in allWindingAndCLLineTags:
+                gmsh.model.mesh.setTransfiniteCurve(lineTag, 1)
+
+        recombine = self.mesh.wi.elementType[0] in ["hexahedron", "prism"]
+        for surfaceTag in notchSurfaceTags:
+            if surfaceTag not in allWindingAndCLSurfaceTags:
+                gmsh.model.mesh.setTransfiniteSurface(surfaceTag)
+                if recombine:
+                    normal = gmsh.model.getNormal(surfaceTag, [0.5, 0.5])
+                    if abs(normal[2]) > 1e-4:
+                        pass
+                    else:
+                        gmsh.model.mesh.setRecombine(2, surfaceTag)
+                    
+
+        for volumeTag in notchVolumeTags:
+            gmsh.model.mesh.setTransfiniteVolume(volumeTag)
+
         # =============================================================================
         # MESHING WINDING AND CONTACT LAYER ENDS =========================================
         # =============================================================================
 
         # =============================================================================
         # MESHING AIR STARTS ==========================================================
         # =============================================================================
@@ -538,15 +586,17 @@
             ]
             airBottomContactLayerExtrusionVolumeTags = [
                 dimTag[1] for dimTag in airBottomContactLayerExtrusionVolumeDimTags
             ]
 
             # Calcualte axial number of elements for air:
             axialElementsPerLengthForWinding = min(self.mesh.wi.axne) / self.geo.wi.h
-            axneForAir = round(axialElementsPerLengthForWinding * self.geo.ai.margin)
+            axneForAir = round(
+                axialElementsPerLengthForWinding * self.geo.ai.margin + 1e-6
+            )
 
             # Get the surface and line tags:
             (
                 airTopWindingExtrusionSurfaceTags,
                 airTopWindingExtrusionLineTags,
             ) = self.get_boundaries(
                 airTopWindingExtrusionVolumeDimTags, returnTags=True
@@ -939,14 +989,16 @@
                 elif line.startswith("Warning"):
                     logger.warning(re.sub(r"Warning:\s+", "", line))
                 elif line.startswith("Error"):
                     logger.error(re.sub(r"Error:\s+", "", line))
 
             gmsh.logger.stop()
 
+            self.generate_regions()
+
             logger.error(
                 "Meshing Pancake3D magnet has failed. Try to change"
                 " minimumElementSize and maximumElementSize parameters."
             )
             raise
 
         # SICN not implemented in 1D!
@@ -965,20 +1017,19 @@
 
         logger.info(
             f"The lowest quality among the elements is {lowestQuality:.4f} (SICN). The"
             " number of elements with quality lower than 0.01 is"
             f" {NofLowQualityElements}."
         )
 
-        # if NofIllElemets > 0:
-        #     self.generate_regions()
-        #     raise RuntimeError(
-        #         f"There are {NofIllElemets} elements with quality lower than 0.001. Try"
-        #         " to change minimumElementSize and maximumElementSize parameters."
-        #     )
+        if NofIllElemets > 0:
+            logger.warning(
+                f"There are {NofIllElemets} elements with quality lower than 0.001. Try"
+                " to change minimumElementSize and maximumElementSize parameters."
+            )
 
         # Create cuts:
         # This is required to make the air a simply connected domain. This is required
         # for the solution part. You can read more about Homology in GMSH documentation.
         airTags = [dimTag[1] for dimTag in self.dimTags[self.geo.ai.name]]
 
         if self.geo.ai.shellTransformation:
@@ -1030,30 +1081,62 @@
             realContactLayerTags = []
             for contactLayerTag in contactLayerTags:
                 surfaceNormal = list(gmsh.model.getNormal(contactLayerTag, [0.5, 0.5]))
                 centerOfMass = gmsh.model.occ.getCenterOfMass(2, contactLayerTag)
 
                 if (
                     abs(
-                        surfaceNormal[1] * centerOfMass[1]
-                        + surfaceNormal[2] * centerOfMass[2]
+                        surfaceNormal[0] * centerOfMass[0]
+                        + surfaceNormal[1] * centerOfMass[1]
                     )
-                    > 1e-5
+                    > 1e-6
                 ):
                     realContactLayerTags.append(contactLayerTag)
 
+            # Get rid of surfaces that touch terminals:
+            terminalSurfaces = gmsh.model.getBoundary(
+                self.dimTags[self.geo.ti.o.name] + self.dimTags[self.geo.ti.i.name],
+                combined=False,
+                oriented=False,
+            )
+            terminalSurfaces = [dimTag[1] for dimTag in terminalSurfaces]
+            finalContactLayerTags = [
+                tag for tag in realContactLayerTags if tag not in terminalSurfaces
+            ]
+
             dummyContactLayerRegion = gmsh.model.addPhysicalGroup(
-                dim=2, tags=realContactLayerTags
+                dim=2, tags=finalContactLayerTags
             )
             dummyContactLayerRegionDimTag = (2, dummyContactLayerRegion)
 
         else:
             contactLayerTags = [dimTag[1] for dimTag in self.dimTags[self.geo.ii.name]]
+
+            # get rid of volumes that touch terminals:
+            terminalSurfaces = gmsh.model.getBoundary(
+                self.dimTags[self.geo.ti.o.name] + self.dimTags[self.geo.ti.i.name],
+                combined=False,
+                oriented=False,
+            )
+            finalContactLayerTags = []
+            for contactLayerTag in contactLayerTags:
+                insulatorSurfaces = gmsh.model.getBoundary(
+                    [(3, contactLayerTag)], combined=False, oriented=False
+                )
+                itTouchesTerminals = False
+                for insulatorSurface in insulatorSurfaces:
+                    if insulatorSurface in terminalSurfaces:
+                        itTouchesTerminals = True
+                        break
+
+                if not itTouchesTerminals:
+                    finalContactLayerTags.append(contactLayerTag)
+
             dummyContactLayerRegion = gmsh.model.addPhysicalGroup(
-                dim=3, tags=contactLayerTags
+                dim=3, tags=finalContactLayerTags
             )
             dummyContactLayerRegionDimTag = (3, dummyContactLayerRegion)
 
         # First cohomology request (normal cut for NI coils):
         gmsh.model.mesh.addHomologyRequest(
             "Cohomology",
             domainTags=[dummyAirRegion],
@@ -1071,23 +1154,30 @@
                 ],
                 subdomainTags=[],
                 dims=[1],
             )
         else:
             gmsh.model.mesh.addHomologyRequest(
                 "Cohomology",
-                domainTags=[dummyAirRegion, dummyContactLayerRegion],
+                domainTags=[
+                    dummyAirRegion,
+                    dummyContactLayerRegion,
+                ],
                 subdomainTags=[],
                 dims=[1],
             )
 
         # Third cohomology request (for cuts between pancake coils):
         gmsh.model.mesh.addHomologyRequest(
             "Cohomology",
-            domainTags=[dummyAirRegion, dummyContactLayerRegion, dummyWindingRegion],
+            domainTags=[
+                dummyAirRegion,
+                dummyContactLayerRegion,
+                dummyWindingRegion,
+            ],
             subdomainTags=[],
             dims=[1],
         )
 
         # Start logger:
         gmsh.logger.start()
 
@@ -1232,15 +1322,14 @@
                     if axialNumberOfElements is None:
                         numNodes = self.mesh.wi.axne[meshSettingIndex] + 1
                     else:
                         numNodes = axialNumberOfElements + 1
 
                     if bumpCoefficient is None:
                         bumpCoefficient = self.mesh.wi.axbc[meshSettingIndex]
-
                     gmsh.model.mesh.setTransfiniteCurve(
                         lineTag, numNodes, meshType="Bump", coef=bumpCoefficient
                     )
 
                 else:
                     # The line is an arc, so the previously calculated arcNumElementsPerTurn
                     # is used. All the number of elements per turn must be the same
@@ -1284,16 +1373,15 @@
             # Make all the volumes transfinite:
             gmsh.model.mesh.setTransfiniteVolume(volTag)
 
     def structure_tubes_and_cylinders(
         self, volumeTags, terminalNonTubeParts=False, radialElementMultiplier=1
     ):
         # Number of azimuthal elements per quarter:
-        arcNumElementsPerQuarter = int(self.mesh.wi.ane[0] / 4) + 1
-        axialNumberOfElementsPerLength = self.mesh.wi.axne[0] / self.geo.wi.h
+        arcNumElementsPerQuarter = int(self.mesh.wi.ane[0] / 4)
         radialNumberOfElementsPerLength = (
             self.mesh.wi.rne[0] / self.geo.wi.t * radialElementMultiplier
         )
 
         surfacesDimTags = gmsh.model.getBoundary(
             [(3, tag) for tag in volumeTags], combined=False, oriented=False
         )
@@ -1309,59 +1397,131 @@
         for curveTag in curvesTags:
             curveObject = curve(curveTag, self.geo)
 
             if curveObject.type is curveType.horizontal:
                 # The curve is horizontal, so radialNumberOfElementsPerTurn entry is
                 # used.
 
-                if terminalNonTubeParts:
-                    if curveTag not in self.contactLayerAndWindingRadialLines:
+                # But, the curve might be a part of the transitionNotch.
+                isTransitionNotch = False
+                point2 = curveObject.points[1]
+                point1 = curveObject.points[0]
+                if (
+                    abs(point2[0] - point1[0]) > 1e-5
+                    and abs(point2[1] - point1[1]) > 1e-5
+                ):
+                    isTransitionNotch = True
+
+                if isTransitionNotch:
+                    gmsh.model.mesh.setTransfiniteCurve(curveTag, 2)
+                else:
+                    if terminalNonTubeParts:
+                        if curveTag not in self.contactLayerAndWindingRadialLines:
+                            numNodes = (
+                                round(radialNumberOfElementsPerLength * self.geo.ti.i.t)
+                                + 1
+                            )
+                            # Set transfinite curve:
+                            gmsh.model.mesh.setTransfiniteCurve(curveTag, numNodes)
+                    else:
                         numNodes = (
-                            round(radialNumberOfElementsPerLength * self.geo.ti.i.t) + 1
+                            round(radialNumberOfElementsPerLength * curveObject.length)
+                            + 1
                         )
                         # Set transfinite curve:
                         gmsh.model.mesh.setTransfiniteCurve(curveTag, numNodes)
-                else:
-                    numNodes = (
-                        round(radialNumberOfElementsPerLength * curveObject.length) + 1
-                    )
-                    # Set transfinite curve:
-                    gmsh.model.mesh.setTransfiniteCurve(curveTag, numNodes)
 
             elif curveObject.type is curveType.axial:
                 # The curve is axial, so axialNumberOfElements entry is used.
-                numNodes = (
-                    round(axialNumberOfElementsPerLength * curveObject.length) + 1
-                )
+                if math.isclose(curveObject.length, self.geo.wi.h, rel_tol=1e-7):
+                    numNodes = min(self.mesh.wi.axne) + 1
+                else:
+                    axialElementsPerLength = min(self.mesh.wi.axne) / self.geo.wi.h
+                    numNodes = (
+                        round(axialElementsPerLength * curveObject.length + 1e-6) + 1
+                    )
 
                 gmsh.model.mesh.setTransfiniteCurve(curveTag, numNodes)
 
             else:
                 # The line is an arc
-                gmsh.model.mesh.setTransfiniteCurve(curveTag, arcNumElementsPerQuarter)
+                lengthInTurns = abs(curveObject.n2 - curveObject.n1)
+                if lengthInTurns > 0.5:
+                    # The arc can never be longer than half a turn.
+                    lengthInTurns = 1 - lengthInTurns
+
+                lengthInTurns = (
+                    round(lengthInTurns / self.geo.wi.turnTol) * self.geo.wi.turnTol
+                )
+
+                arcNumEl = round(arcNumElementsPerQuarter * 4 * lengthInTurns)
+
+                arcNumNodes = int(arcNumEl + 1)
+
+                # Set transfinite curve:
+
+                gmsh.model.mesh.setTransfiniteCurve(curveTag, arcNumNodes)
 
         for surfaceTag in surfacesTags:
             # Make all the surfaces transfinite:
 
             if self.mesh.wi.elementType[0] == "hexahedron":
                 # If the element type is hexahedron, recombine all the surfaces:
                 gmsh.model.mesh.setRecombine(2, surfaceTag)
             elif self.mesh.wi.elementType[0] == "prism":
                 # If the element type is prism, recombine only the side surfaces:
                 surfaceNormal = list(gmsh.model.getNormal(surfaceTag, [0.5, 0.5]))
-                if abs(surfaceNormal[2]) < 1e-6:
+                if abs(surfaceNormal[2]) < 1e-5:
                     gmsh.model.mesh.setRecombine(2, surfaceTag)
 
             curves = gmsh.model.getBoundary(
                 [(2, surfaceTag)], combined=False, oriented=False
             )
             numberOfCurves = len(curves)
             if terminalNonTubeParts:
                 if numberOfCurves == 4:
-                    gmsh.model.mesh.setTransfiniteSurface(surfaceTag)
+                    numberOfHorizontalCurves = 0
+                    for curveTag in curves:
+                        curveObject = curve(curveTag[1], self.geo)
+                        if curveObject.type is curveType.horizontal:
+                            numberOfHorizontalCurves += 1
+
+                    if numberOfHorizontalCurves == 3:
+                        pass
+                    else:
+                        gmsh.model.mesh.setTransfiniteSurface(surfaceTag)
+
+                elif numberOfCurves == 3:
+                    pass
+                else:
+                    curves = gmsh.model.getBoundary(
+                        [(2, surfaceTag)], combined=False, oriented=False
+                    )
+                    curveObjects = [curve(line[1], self.geo) for line in curves]
+
+                    divisionCurves = []
+                    for curveObject in curveObjects:
+                        if curveObject.type is curveType.horizontal:
+                            point1 = curveObject.points[0]
+                            point2 = curveObject.points[1]
+                            if not (
+                                abs(point2[0] - point1[0]) > 1e-5
+                                and abs(point2[1] - point1[1]) > 1e-5
+                            ):
+                                divisionCurves.append(curveObject)
+
+                    cornerPoints = (
+                        divisionCurves[0].pointTags + divisionCurves[1].pointTags
+                    )
+
+                    if surfaceTag not in alreadyMeshedSurfaceTags:
+                        alreadyMeshedSurfaceTags.append(surfaceTag)
+                        gmsh.model.mesh.setTransfiniteSurface(
+                            surfaceTag, cornerTags=cornerPoints
+                        )
             else:
                 if numberOfCurves == 3:
                     # Then it is a pie, corner points should be adjusted:
                     originPointTag = None
                     curveObject1 = curve(curves[0][1], self.geo)
                     for point, tag in zip(curveObject1.points, curveObject1.pointTags):
                         if math.sqrt(point[0] ** 2 + point[1] ** 2) < 1e-6:
@@ -1397,15 +1557,45 @@
                 )
                 curves = gmsh.model.getBoundary(
                     surfaces, combined=False, oriented=False
                 )
                 curves = list(set(curves))
 
                 if len(curves) == 12:
-                    gmsh.model.mesh.setTransfiniteVolume(volumeTag)
+                    numberOfArcs = 0
+                    for curveTag in curves:
+                        curveObject = curve(curveTag[1], self.geo)
+                        if curveObject.type is curveType.spiralArc:
+                            numberOfArcs += 1
+                    if numberOfArcs == 2:
+                        pass
+                    else:
+                        gmsh.model.mesh.setTransfiniteVolume(volumeTag)
+                # elif len(curves) == 15:
+                #     divisionCurves = []
+                #     for curveTag in curves:
+                #         curveObject = curve(curveTag[1], self.geo)
+                #         if curveObject.type is curveType.horizontal:
+                #             point1 = curveObject.points[0]
+                #             point2 = curveObject.points[1]
+                #             if not (
+                #                 abs(point2[0] - point1[0]) > 1e-5
+                #                 and abs(point2[1] - point1[1]) > 1e-5
+                #             ):
+                #                 divisionCurves.append(curveObject)
+
+                #     cornerPoints = (
+                #         divisionCurves[0].pointTags
+                #         + divisionCurves[1].pointTags
+                #         + divisionCurves[2].pointTags
+                #         + divisionCurves[3].pointTags
+                #     )
+                #     gmsh.model.mesh.setTransfiniteVolume(
+                #         volumeTag, cornerTags=cornerPoints
+                #     )
             else:
                 # Make all the volumes transfinite:
                 gmsh.model.mesh.setTransfiniteVolume(volumeTag)
 
     @staticmethod
     def get_boundaries(volumeDimTags, returnTags=False):
         """
@@ -1955,108 +2145,312 @@
         if not self.geo.ii.tsa:
             windingTags = [dimTag[1] for dimTag in self.dimTags[self.geo.wi.name]]
             self.regions.addEntities(
                 self.geo.wi.name, windingTags, regionType.powered, entityType.vol
             )
 
             insulatorTags = [dimTag[1] for dimTag in self.dimTags[self.geo.ii.name]]
+
+            terminalDimTags = (
+                self.dimTags[self.geo.ti.i.name] + self.dimTags[self.geo.ti.o.name]
+            )
+            terminalAndNotchSurfaces = gmsh.model.getBoundary(
+                terminalDimTags, combined=False, oriented=False
+            )
+            transitionNotchSurfaces = gmsh.model.getBoundary(
+                self.dimTags["innerTransitionNotch"]
+                + self.dimTags["outerTransitionNotch"],
+                combined=False,
+                oriented=False,
+            )
+
+            contactLayer = []
+            contactLayerBetweenTerminalsAndWinding = []
+            for insulatorTag in insulatorTags:
+                insulatorSurfaces = gmsh.model.getBoundary(
+                    [(3, insulatorTag)], combined=False, oriented=False
+                )
+                itTouchesTerminals = False
+                for insulatorSurface in insulatorSurfaces:
+                    if (
+                        insulatorSurface
+                        in terminalAndNotchSurfaces + transitionNotchSurfaces
+                    ):
+                        contactLayerBetweenTerminalsAndWinding.append(insulatorTag)
+                        itTouchesTerminals = True
+                        break
+
+                if not itTouchesTerminals:
+                    contactLayer.append(insulatorTag)
+
+            self.regions.addEntities(
+                self.geo.ii.name, contactLayer, regionType.insulator, entityType.vol
+            )
+
             self.regions.addEntities(
-                self.geo.ii.name, insulatorTags, regionType.insulator, entityType.vol
+                "WindingAndTerminalContactLayer",
+                contactLayerBetweenTerminalsAndWinding,
+                regionType.insulator,
+                entityType.vol,
             )
         else:
-            insulatorBoundaryTags = []
-            windings = []
-            insulators = []
+            # Calculate the number of stacks for each individual winding. Number of
+            # stacks is the number of volumes per turn. It affects how the regions
+            # are created because of the TSA's pro file formulation.
+
+            # find the smallest prime number that divides NofVolumes:
+            windingDimTags = self.dimTags[self.geo.wi.name + "1"]
+            windingTags = [dimTag[1] for dimTag in windingDimTags]
+            NofVolumes = self.geo.wi.NofVolPerTurn
+            smallest_prime_divisor = 2
+            while NofVolumes % smallest_prime_divisor != 0:
+                smallest_prime_divisor += 1
+
+            # the number of stacks is the region divison per turn:
+            NofStacks = smallest_prime_divisor
+
+            # the number of sets are the total number of regions for all windings and
+            # contact layers:
+            NofSets = 2 * NofStacks
+
+            allInnerTerminalSurfaces = gmsh.model.getBoundary(
+                self.dimTags[self.geo.ti.i.name] + self.dimTags["innerTransitionNotch"],
+                combined=False,
+                oriented=False,
+            )
+            allInnerTerminalContactLayerSurfaces = []
+            for innerTerminalSurface in allInnerTerminalSurfaces:
+                normal = gmsh.model.getNormal(innerTerminalSurface[1], [0.5, 0.5])
+                if abs(normal[2]) < 1e-5:
+                    curves = gmsh.model.getBoundary(
+                        [innerTerminalSurface], combined=False, oriented=False
+                    )
+                    curveTags = [dimTag[1] for dimTag in curves]
+                    for curveTag in curveTags:
+                        curveObject = curve(curveTag, self.geo)
+                        if curveObject.type is curveType.spiralArc:
+                            allInnerTerminalContactLayerSurfaces.append(
+                                innerTerminalSurface[1]
+                            )
+
+            finalWindingSets = []
+            finalContactLayerSets = []
+            for i in range(NofSets):
+                finalWindingSets.append([])
+                finalContactLayerSets.append([])
+
             for i in range(self.geo.N):
                 windingDimTags = self.dimTags[self.geo.wi.name + str(i + 1)]
                 windingTags = [dimTag[1] for dimTag in windingDimTags]
 
-                # Calculate the number of stacks for each individual winding. Number of
-                # stacks is the number of volumes per turn. It affects how the regions
-                # are created because of the TSA's pro file formulation.
                 NofVolumes = len(windingDimTags)
-                roundedNofTurns = math.floor(self.geo.wi.N)
-                NofStacks = math.ceil(NofVolumes / roundedNofTurns)
 
-                # Windings are divided into 2 times NofStacks parts because of the TSA's
-                # pro file formulation.
+                windings = []
+                for windingTag in windingTags:
+                    surfaces = gmsh.model.getBoundary(
+                        [(3, windingTag)], combined=False, oriented=False
+                    )
+                    curves = gmsh.model.getBoundary(
+                        surfaces, combined=False, oriented=False
+                    )
+                    curveTags = list(set([dimTag[1] for dimTag in curves]))
+                    for curveTag in curveTags:
+                        curveObject = curve(curveTag, self.geo)
+                        if curveObject.type is curveType.spiralArc:
+                            windingVolumeLengthInTurns = abs(
+                                curveObject.n2 - curveObject.n1
+                            )
+                            if windingVolumeLengthInTurns > 0.5:
+                                # The arc can never be longer than half a turn.
+                                windingVolumeLengthInTurns = (
+                                    1 - windingVolumeLengthInTurns
+                                )
 
-                # The number of stacks practically means the number of volumes per turn.
-                # The number of sets means how many physical groups will be created for
-                # all windings and contact layers due to TSA formulation.
-                NofSets = 2 * NofStacks
+                    windings.append((windingTag, windingVolumeLengthInTurns))
 
-                for j in range(NofSets):
-                    windings.append(windingTags[j::NofSets])
+                windingStacks = []
+                while len(windings) > 0:
+                    stack = []
+                    stackLength = 0
+                    for windingTag, windingVolumeLengthInTurns in windings:
+                        if stackLength < 1 / NofStacks - 1e-6:
+                            stack.append(windingTag)
+                            stackLength += windingVolumeLengthInTurns
+                        else:
+                            break
+                    # remove all the windings that are already added to the stack:
+                    windings = [
+                        (windingTag, windingVolumeLengthInTurns)
+                        for windingTag, windingVolumeLengthInTurns in windings
+                        if windingTag not in stack
+                    ]
+
+                    # find spiral surfaces of the stack:
+                    stackDimTags = [(3, windingTag) for windingTag in stack]
+                    stackSurfacesDimTags = gmsh.model.getBoundary(
+                        stackDimTags, combined=True, oriented=False
+                    )
+                    stackCurvesDimTags = gmsh.model.getBoundary(
+                        stackSurfacesDimTags, combined=False, oriented=False
+                    )
+                    # find the curve furthest from the origin:
+                    curveObjects = []
+                    for curveDimTag in stackCurvesDimTags:
+                        curveObject = curve(curveDimTag[1], self.geo)
+                        if curveObject.type is curveType.spiralArc:
+                            curveObjectDistanceFromOrigin = math.sqrt(
+                                curveObject.points[0][0] ** 2
+                                + curveObject.points[0][1] ** 2
+                            )
+                            curveObjects.append(
+                                (curveObject, curveObjectDistanceFromOrigin)
+                            )
 
-                # Find all the contact layers:
-                windingBoundary = gmsh.model.getBoundary(
-                    windingDimTags, combined=False, oriented=False
-                )
-                innerBoundary = windingBoundary[1::6]
-                outerBoundary = windingBoundary[3::6]
-                allSideSurfaces = innerBoundary + outerBoundary
-                contactLayerSurfaces = []
-
-                numberOfOccurances = {}
-                for surfTag in allSideSurfaces:
-                    if surfTag not in numberOfOccurances:
-                        numberOfOccurances[surfTag] = 1
+                    # sort the curves based on their distance from the origin (furthest first)
+                    curveObjects.sort(key=lambda x: x[1], reverse=True)
 
-                    else:
-                        if numberOfOccurances[surfTag] == 1:
-                            contactLayerSurfaces.append(surfTag)
+                    curveTags = [curveObject[0].tag for curveObject in curveObjects]
 
-                        numberOfOccurances[surfTag] += 1
+                    # only keep half of the curveTags:
+                    furthestCurveTags = curveTags[: len(curveTags) // 2]
+
+                    stackSpiralSurfaces = []
+                    for surfaceDimTag in stackSurfacesDimTags:
+                        normal = gmsh.model.getNormal(surfaceDimTag[1], [0.5, 0.5])
+                        if abs(normal[2]) < 1e-5:
+                            curves = gmsh.model.getBoundary(
+                                [surfaceDimTag], combined=False, oriented=False
+                            )
+                            curveTags = [dimTag[1] for dimTag in curves]
+                            for curveTag in curveTags:
+                                if curveTag in furthestCurveTags:
+                                    stackSpiralSurfaces.append(surfaceDimTag[1])
+                                    break
+
+                    # add inner terminal surfaces too:
+                    if len(windingStacks) >= NofStacks:
+                        correspondingWindingStack = windingStacks[
+                            len(windingStacks) - NofStacks
+                        ]
+                        correspondingWindings = correspondingWindingStack[0]
+                        correspondingSurfaces = gmsh.model.getBoundary(
+                            [(3, windingTag) for windingTag in correspondingWindings],
+                            combined=True,
+                            oriented=False,
+                        )
+                        correspondingSurfaceTags = [
+                            dimTag[1] for dimTag in correspondingSurfaces
+                        ]
+                        for surface in allInnerTerminalContactLayerSurfaces:
+                            if surface in correspondingSurfaceTags:
+                                stackSpiralSurfaces.append(surface)
 
-                insulatorTags = [dimTag[1] for dimTag in contactLayerSurfaces]
+                    windingStacks.append((stack, stackSpiralSurfaces))
 
-                # Divide insulator surfaces into 4 corresponding parts:
+                windingSets = []
+                contactLayerSets = []
                 for j in range(NofSets):
-                    insulators.append(insulatorTags[j::NofSets])
+                    windingTags = [
+                        windingTags for windingTags, _ in windingStacks[j::NofSets]
+                    ]
+                    windingTags = list(itertools.chain.from_iterable(windingTags))
 
-                # Get insulator's boundary line that touches the air (required for the
-                # pro file formulation):
-                insulatorBoundary = gmsh.model.getBoundary(
-                    contactLayerSurfaces, combined=True, oriented=False
-                )
-                insulatorBoundaryTags.extend(
-                    [dimTag[1] for dimTag in insulatorBoundary]
-                )
+                    surfaceTags = [
+                        surfaceTags for _, surfaceTags in windingStacks[j::NofSets]
+                    ]
+                    surfaceTags = list(itertools.chain.from_iterable(surfaceTags))
+
+                    windingSets.append(windingTags)
+                    contactLayerSets.append(surfaceTags)
+
+                # windingSets is a list with a length of NofSets.
+                # finalWindingSets is also a list with a length of NofSets.
+                for j, (windingSet, contactLayerSet) in enumerate(
+                    zip(windingSets, contactLayerSets)
+                ):
+                    finalWindingSets[j].extend(windingSet)
+                    finalContactLayerSets[j].extend(contactLayerSet)
+
+            # Seperate transition layer:
+            terminalAndNotchSurfaces = gmsh.model.getBoundary(
+                self.dimTags[self.geo.ti.i.name]
+                + self.dimTags[self.geo.ti.o.name]
+                + self.dimTags["innerTransitionNotch"]
+                + self.dimTags["outerTransitionNotch"],
+                combined=False,
+                oriented=False,
+            )
+            terminalAndNotchSurfaceTags = set(
+                [dimTag[1] for dimTag in terminalAndNotchSurfaces]
+            )
 
-            # Add winding and contact layer stacks:
-            windingsFinal = []
-            insulatorsFinal = []
+            contactLayerSets = []
+            terminalWindingContactLayerSets = []
             for j in range(NofSets):
-                listOfWindingLists = windings[j::NofSets]
-                windingsFinal.append(
-                    list(itertools.chain.from_iterable(listOfWindingLists))
-                )
+                contactLayerSets.append([])
+                terminalWindingContactLayerSets.append([])
 
-                listOfContactLayerLists = insulators[j::NofSets]
-                insulatorsFinal.append(
-                    list(itertools.chain.from_iterable(listOfContactLayerLists))
-                )
+            for j in range(NofSets):
+                allContactLayersInTheSet = finalContactLayerSets[j]
+
+                insulatorList = []
+                windingTerminalInsulatorList = []
+                for contactLayer in allContactLayersInTheSet:
+                    if contactLayer in terminalAndNotchSurfaceTags:
+                        windingTerminalInsulatorList.append(contactLayer)
+                    else:
+                        insulatorList.append(contactLayer)
+
+                contactLayerSets[j].extend(set(insulatorList))
+                terminalWindingContactLayerSets[j].extend(set(windingTerminalInsulatorList))
 
+            allContactLayerSurfacesForAllPancakes = []
             for j in range(NofSets):
                 # Add winding volumes:
                 self.regions.addEntities(
                     self.geo.wi.name + "-" + str(j + 1),
-                    windingsFinal[j],
+                    finalWindingSets[j],
                     regionType.powered,
                     entityType.vol,
                 )
 
                 # Add insulator surfaces:
                 self.regions.addEntities(
                     self.geo.ii.name + "-" + str(j + 1),
-                    insulatorsFinal[j],
+                    contactLayerSets[j],
                     regionType.insulator,
                     entityType.surf,
                 )
+                allContactLayerSurfacesForAllPancakes.extend(contactLayerSets[j])
+
+                # Add terminal and winding contact layer:
+                self.regions.addEntities(
+                    "WindingAndTerminalContactLayer" + "-" + str(j + 1),
+                    terminalWindingContactLayerSets[j],
+                    regionType.insulator,
+                    entityType.surf,
+                )
+                allContactLayerSurfacesForAllPancakes.extend(
+                    terminalWindingContactLayerSets[j]
+                )
+
+            allContactLayerSurfacesForAllPancakes = list(
+                set(allContactLayerSurfacesForAllPancakes)
+            )
+            # Get insulator's boundary line that touches the air (required for the
+            # pro file formulation):
+            allContactLayerSurfacesForAllPancakesDimTags = [
+                (2, surfaceTag) for surfaceTag in allContactLayerSurfacesForAllPancakes
+            ]
+            insulatorBoundary = gmsh.model.getBoundary(
+                allContactLayerSurfacesForAllPancakesDimTags,
+                combined=True,
+                oriented=False,
+            )
+            insulatorBoundaryTags = [dimTag[1] for dimTag in insulatorBoundary]
 
             # Add insulator boundary lines:
             # Vertical lines should be removed from the insulator boundary because
             # they touch the terminals, not the air:
             verticalInsulatorBoundaryTags = []
             insulatorBoundaryTagsCopy = insulatorBoundaryTags.copy()
             for lineTag in insulatorBoundaryTagsCopy:
@@ -2074,21 +2468,41 @@
             )
             self.regions.addEntities(
                 self.geo.contactLayerBoundaryName + "-TouchingTerminal",
                 verticalInsulatorBoundaryTags,
                 regionType.insulator,
                 entityType.curve,
             )
+
+        innerTransitionNotchTags = [
+            dimTag[1] for dimTag in self.dimTags["innerTransitionNotch"]
+        ]
+        outerTransitionNotchTags = [
+            dimTag[1] for dimTag in self.dimTags["outerTransitionNotch"]
+        ]
+        self.regions.addEntities(
+            "innerTransitionNotch",
+            innerTransitionNotchTags,
+            regionType.powered,
+            entityType.vol,
+        )
+        self.regions.addEntities(
+            "outerTransitionNotch",
+            outerTransitionNotchTags,
+            regionType.powered,
+            entityType.vol,
+        )
         # ==============================================================================
         # WINDING AND CONTACT LAYER REGIONS ENDS =======================================
         # ==============================================================================
 
         # ==============================================================================
         # TERMINAL REGIONS START =======================================================
         # ==============================================================================
+
         innerTerminalTags = [dimTag[1] for dimTag in self.dimTags[self.geo.ti.i.name]]
         self.regions.addEntities(
             self.geo.ti.i.name, innerTerminalTags, regionType.powered, entityType.vol_in
         )
         outerTerminalTags = [dimTag[1] for dimTag in self.dimTags[self.geo.ti.o.name]]
         self.regions.addEntities(
             self.geo.ti.o.name,
@@ -2138,14 +2552,45 @@
         self.regions.addEntities(
             "BottomSurface",
             bottomSurfaceTags,
             regionType.powered,
             entityType.surf_in,
         )
 
+        # if self.geo.ii.tsa:
+        #     outerTerminalSurfaces = gmsh.model.getBoundary(
+        #         self.dimTags[self.geo.ti.o.name], combined=True, oriented=False
+        #     )
+        #     outerTerminalSurfaces = [dimTag[1] for dimTag in outerTerminalSurfaces]
+        #     innerTerminalSurfaces = gmsh.model.getBoundary(
+        #         self.dimTags[self.geo.ti.i.name], combined=True, oriented=False
+        #     )
+        #     innerTerminalSurfaces = [dimTag[1] for dimTag in innerTerminalSurfaces]
+        #     windingSurfaces = gmsh.model.getBoundary(
+        #         self.dimTags[self.geo.wi.name] + self.dimTags[self.geo.ii.name],
+        #         combined=True,
+        #         oriented=False,
+        #     )
+        #     windingSurfaces = [dimTag[1] for dimTag in windingSurfaces]
+
+        #     windingAndOuterTerminalCommonSurfaces = list(
+        #         set(windingSurfaces).intersection(set(outerTerminalSurfaces))
+        #     )
+        #     windingAndInnerTerminalCommonSurfaces = list(
+        #         set(windingSurfaces).intersection(set(innerTerminalSurfaces))
+        #     )
+
+        #     self.regions.addEntities(
+        #         "WindingAndTerminalContactLayer",
+        #         windingAndOuterTerminalCommonSurfaces
+        #         + windingAndInnerTerminalCommonSurfaces,
+        #         regionType.insulator,
+        #         entityType.surf,
+        #     )
+
         # ==============================================================================
         # TERMINAL REGIONS ENDS ========================================================
         # ==============================================================================
 
         # ==============================================================================
         # AIR AND AIR SHELL REGIONS STARTS =============================================
         # ==============================================================================
@@ -2172,15 +2617,15 @@
             "OuterAirPoint",
             [outerAirPointTag],
             regionType.air,
             entityType.point,
         )
 
         innerAirSurfaces = gmsh.model.getBoundary(
-            self.dimTags[self.geo.ai.name],
+            self.dimTags[self.geo.ai.name + "-InnerCylinder"],
             combined=True,
             oriented=False,
         )
         innerAirSurface = innerAirSurfaces[0]
         innerAirCurves = gmsh.model.getBoundary(
             [innerAirSurface], combined=True, oriented=False
         )
@@ -2263,14 +2708,16 @@
         # ==============================================================================
         # Pancake3D Boundary Surface:
         allPancakeVolumes = (
             self.dimTags[self.geo.wi.name]
             + self.dimTags[self.geo.ti.i.name]
             + self.dimTags[self.geo.ti.o.name]
             + self.dimTags[self.geo.ii.name]
+            + self.dimTags["innerTransitionNotch"]
+            + self.dimTags["outerTransitionNotch"]
         )
         Pancake3DAllBoundary = gmsh.model.getBoundary(
             allPancakeVolumes, combined=True, oriented=False
         )
         Pancake3DBoundaryDimTags = list(
             set(Pancake3DAllBoundary)
             - set(topSurfaceDimTags)
@@ -2286,14 +2733,17 @@
 
         if not self.geo.ii.tsa:
             # Pancake3D Boundary Surface with only winding and terminals:
             allPancakeVolumes = (
                 self.dimTags[self.geo.wi.name]
                 + self.dimTags[self.geo.ti.i.name]
                 + self.dimTags[self.geo.ti.o.name]
+                + self.dimTags["innerTransitionNotch"]
+                + self.dimTags["outerTransitionNotch"]
+                + [(3, tag) for tag in contactLayerBetweenTerminalsAndWinding]
             )
             Pancake3DAllBoundary = gmsh.model.getBoundary(
                 allPancakeVolumes, combined=True, oriented=False
             )
             Pancake3DBoundaryDimTags = list(
                 set(Pancake3DAllBoundary)
                 - set(topSurfaceDimTags)
```

### Comparing `fiqus-2024.1.1/fiqus/parsers/ParserDAT.py` & `fiqus-2024.4.0/fiqus/parsers/ParserDAT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/parsers/ParserGetDPOnSection.py` & `fiqus-2024.4.0/fiqus/parsers/ParserGetDPOnSection.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/parsers/ParserGetDPTimeTable.py` & `fiqus-2024.4.0/fiqus/parsers/ParserGetDPTimeTable.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/parsers/ParserMSH.py` & `fiqus-2024.4.0/fiqus/parsers/ParserMSH.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/parsers/ParserPOS.py` & `fiqus-2024.4.0/fiqus/parsers/ParserPOS.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/parsers/ParserRES.py` & `fiqus-2024.4.0/fiqus/parsers/ParserRES.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/plotters/PlotPythonCCT.py` & `fiqus-2024.4.0/fiqus/plotters/PlotPythonCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/post_processors/PostProcessCCT.py` & `fiqus-2024.4.0/fiqus/post_processors/PostProcessCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/post_processors/PostProcessMultipole.py` & `fiqus-2024.4.0/fiqus/post_processors/PostProcessMultipole.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         if self.data.magnet.postproc.compare_to_ROXIE:
             self.postprocess_parameters['overall_error'] = np.linalg.norm(self.BB_err_mean)
             self.postprocess_parameters['minimum_diff'] = np.min(self.BB_err_mean)
             self.postprocess_parameters['maximum_diff'] = np.max(self.BB_err_mean)
 
         print(f"Info    : {self.data.general.magnet_name} - E n d   I n t e r p o l a t i n g")
 
-        if self.data.magnet.postproc.plot_all != 'False':
+        if self.data.magnet.postproc.plot_all != 'False' and self.data.magnet.postproc.plot_all != False:
             self.plotHalfTurnGeometry()
             if self.data.magnet.postproc.compare_to_ROXIE:
                 cax4 = self.fig4.add_axes([self.ax4.get_position().x1 + 0.02, self.ax4.get_position().y0,
                                            0.02, self.ax4.get_position().height])
                 cbar = plt.colorbar(self.ax4.get_children()[2], cax=cax4)
                 cbar.ax.set_ylabel('Absolute error [mT]', rotation=270)
                 self.ax3.legend([scatter3D_pos, scatter3D_pos_roxie], ['FiQuS', 'ROXIE'], numpoints=1)
```

### Comparing `fiqus-2024.1.1/fiqus/post_processors/PostProcessPancake3D.py` & `fiqus-2024.4.0/fiqus/post_processors/PostProcessPancake3D.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import matplotlib.patches as patches
 import numpy as np
 from scipy.interpolate import griddata
 import matplotlib
 import matplotlib.pyplot as plt
 
 from fiqus.mains.MainPancake3D import Base
+import fiqus.data.DataFiQuSPancake3D as dm
 from fiqus.utils.Utils import GmshUtils
 from fiqus.parsers.ParserGetDPTimeTable import ParserGetDPTimeTable
 from fiqus.parsers.ParserGetDPOnSection import ParserGetDPOnSection
 
 logger = logging.getLogger(__name__)
 
 
@@ -210,27 +211,33 @@
 
     def plotTimeSeriesPlots(self):
         start_time = timeit.default_timer()
         logger.info("Plotting time series plots has been started.")
 
         for timeSeriesPlot in self.pp.timeSeriesPlots:
             filePath = os.path.join(
-                self.solution_folder, timeSeriesPlot.fileName + "-TimeTableFormat.txt"
+                self.solution_folder, timeSeriesPlot.fileName + "-TimeTableFormat.csv"
             )
-            if timeSeriesPlot.position.turnNumber is not None:
-                title = (
-                    f"{timeSeriesPlot.quantityProperName} at turn"
-                    f" {timeSeriesPlot.position.turnNumber}"
-                )
-            elif timeSeriesPlot.position.x is not None:
-                title = (
-                    f"{timeSeriesPlot.quantityProperName} at"
-                    f" ({timeSeriesPlot.position.x}, {timeSeriesPlot.position.y},"
-                    f" {timeSeriesPlot.position.z})"
-                )
+            # check if this is Pancake3DPositionInCoordinates or not:
+            if isinstance(
+                timeSeriesPlot, dm.Pancake3DPostprocessTimeSeriesPlotPositionRequired
+            ):
+                if isinstance(
+                    timeSeriesPlot.position, dm.Pancake3DPositionInCoordinates
+                ):
+                    title = (
+                        f"{timeSeriesPlot.quantityProperName} at"
+                        f" ({timeSeriesPlot.position.x}, {timeSeriesPlot.position.y},"
+                        f" {timeSeriesPlot.position.z})"
+                    )
+                else:
+                    title = (
+                        f"{timeSeriesPlot.quantityProperName} at turn"
+                        f" {timeSeriesPlot.position.turnNumber}"
+                    )
             else:
                 title = f"{timeSeriesPlot.quantityProperName}"
 
             # Parse data:
             parser = ParserGetDPTimeTable(filePath)
             timeValues = parser.time_values
             scalarvalues = parser.get_equivalent_scalar_values()
```

### Comparing `fiqus-2024.1.1/fiqus/pre_processors/PreProcessCCT.py` & `fiqus-2024.4.0/fiqus/pre_processors/PreProcessCCT.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/pro_assemblers/ProAssembler.py` & `fiqus-2024.4.0/fiqus/pro_assemblers/ProAssembler.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/pro_material_functions/ironBHcurves.pro` & `fiqus-2024.4.0/fiqus/pro_material_functions/ironBHcurves.pro`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/pro_templates/combined/CCT_template.pro` & `fiqus-2024.4.0/fiqus/pro_templates/combined/CCT_template.pro`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/pro_templates/combined/Multipole_template.pro` & `fiqus-2024.4.0/fiqus/pro_templates/combined/Multipole_template.pro`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/pro_templates/combined/Pancake3D_template.pro` & `fiqus-2024.4.0/fiqus/pro_templates/combined/Pancake3D_template.pro`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,12 @@
 {% import "materials.pro" as materials %}
 {# ================================================================================== #}
 {# ================================================================================== #}
 {# ================================================================================== #}
 {# ================================================================================== #}
-{% macro FUNCTIONSPACE_TSAFunctionSpaces(type) %}
-// TSA function spaces starts ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-For i In {1:INPUT_NumOfTSAElements - 1}
-{% if type == "electromagnetic" %}
-    {
-        Name SPACE_hPhiThinShell~{i};
-        Type Form1;
-        BasisFunction{
-            {
-                Name se;
-                NameOfCoef he~{i};
-                Function BF_Edge;
-                Support DOM_insulationSurface;
-                Entity EdgesOf[ All ];
-            }
-        }
-    }
-{% elif type == "thermal" %}
-    {
-        Name SPACE_temperatureThinShell~{i};
-        Type Form0;
-        BasisFunction{
-            {
-                Name se;
-                NameOfCoef te~{i};
-                Function BF_Node;
-                Support DOM_insulationSurface;
-                Entity NodesOf[ All ];
-            }
-        }
-        Constraint{
-            {
-                NameOfCoef te~{i};
-                EntityType NodesOf;
-                NameOfConstraint CONSTRAINT_initialTemperature;
-            }
-        }
-    }
-{% endif %}
-EndFor
-// TSA function spaces ends ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-{% endmacro %}
-{# ================================================================================== #}
-{# ================================================================================== #}
-{# ================================================================================== #}
-{# ================================================================================== #}
 {% macro FUNCTIONSPACE_TSABasisFunctions(type) %}
 // TSA basis functions starts ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 // TSA contributions following special indexing to restrict them to one side of the thin
 // layer split in plus and minus side.
 {% for i in range(1, NofSets+1) %}
 {
@@ -60,60 +14,78 @@
     NameOfCoef BASISFUN_snMinus_coeff_<<i>>;
     {% if type == "electromagnetic" %}
     Function BF_Edge;
     {% elif type == "thermal" %}
     Function BF_Node;
     {% endif %}
     Support Region[
-                {
-                    DOM_insulationSurface_<<i>>,
-                    DOM_insulationSurface_<<i+1>>,
+                {   
+                    {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" and type == "electromagnetic" %}
+                    DOM_terminalContactLayerSurface_<<i>>,
+                    DOM_terminalContactLayerSurface_<<i+1>>,
+                    {% else %}
+                    DOM_allInsulationSurface_<<i>>,
+                    DOM_allInsulationSurface_<<i+1>>,
+                    {% endif %}
                     DOM_windingMinus_<<i>>,
                     DOM_windingMinus_<<i+1>>
                 }
             ];
     {% if type == "electromagnetic" %}
     Entity EdgesOf[
-                DOM_insulationSurface_<<i>>,
-                Not {DOM_insulationBoundaryCurvesAir, DOM_insulationBoundaryCurvesTerminal, DOM_insulationSurface_<<i-1>>}
-                ];
+        {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %}
+        DOM_terminalContactLayerSurface_<<i>>,
+        {% else %}
+        DOM_allInsulationSurface_<<i>>,
+        {% endif %}
+        Not {DOM_insulationBoundaryCurvesAir, DOM_insulationBoundaryCurvesTerminal, {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %} DOM_terminalContactLayerSurface_<<i-1>>, DOM_insulationSurface {% else %} DOM_allInsulationSurface_<<i-1>> {% endif %}}
+        ];
     {% elif type == "thermal" %}
     Entity NodesOf[
-                DOM_insulationSurface_<<i>>,
-                Not { DOM_insulationSurface_<<i-1>>, DOM_insulationBoundaryCurvesTerminal }
+                DOM_allInsulationSurface_<<i>>,
+                Not { DOM_allInsulationSurface_<<i-1>>, DOM_insulationBoundaryCurvesTerminal }
                 ];
     {% endif %}
 }
 
 {
     Name BASISFUN_snPlus_<<i>>;
     NameOfCoef BASISFUN_snPlus_coeff_<<i>>;
     {% if type == "electromagnetic" %}
     Function BF_Edge;
     {% elif type == "thermal" %}
     Function BF_Node;
     {% endif %}
     Support Region[
-                {
-                    DOM_insulationSurface_<<i>>,
-                    DOM_insulationSurface_<<i+1>>,
+                {   
+                    {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" and type == "electromagnetic" %}
+                    DOM_terminalContactLayerSurface_<<i>>,
+                    DOM_terminalContactLayerSurface_<<i+1>>,
+                    {% else %}
+                    DOM_allInsulationSurface_<<i>>,
+                    DOM_allInsulationSurface_<<i+1>>,
+                    {% endif %}
                     DOM_windingPlus_<<i>>,
                     DOM_windingPlus_<<i+1>>
                 }
             ];
     {% if type == "electromagnetic" %}
     Entity EdgesOf[
-                DOM_insulationSurface_<<i>>,
-                Not {DOM_insulationBoundaryCurvesAir, DOM_insulationBoundaryCurvesTerminal, DOM_insulationSurface_<<i-1>>}
-                ];
+        {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %}
+        DOM_terminalContactLayerSurface_<<i>>,
+        {% else %}
+        DOM_allInsulationSurface_<<i>>,
+        {% endif %}
+        Not {DOM_insulationBoundaryCurvesAir, DOM_insulationBoundaryCurvesTerminal, {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %} DOM_terminalContactLayerSurface_<<i-1>>, DOM_insulationSurface {% else %} DOM_allInsulationSurface_<<i-1>> {% endif %}}
+        ];
     {% elif type == "thermal" %}
     Entity NodesOf[
-                DOM_insulationSurface_<<i>>,
-                Not { DOM_insulationSurface_<<i-1>>, DOM_insulationBoundaryCurvesTerminal }
-                ];
+        DOM_allInsulationSurface_<<i>>,
+        Not { DOM_allInsulationSurface_<<i-1>>, DOM_insulationBoundaryCurvesTerminal }
+        ];
     {% endif %}
 }
 {% endfor %}
 
 // TSA basis functions ends ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 {% endmacro %}
 {# ================================================================================== #}
@@ -159,14 +131,34 @@
         {% else %}
         <<bf>>,
         {% endif %}
 {% endfor %}
     };
 }
 
+For i In {1:INPUT_NumOfTSAElements - 1}
+    {
+        Name SUBSPACE_tsa~{i}; 
+        NameOfBasisFunction {
+{% if len(aditionalBasisFunctions)==0 %}
+            BASISFUN_sn~{i}
+{% else %}
+            BASISFUN_sn~{i},
+{% endif %}
+{% for bf in aditionalBasisFunctions %}
+        {% if loop.last %}
+            <<bf>>
+        {% else %}
+            <<bf>>,
+        {% endif %}
+{% endfor %}
+        };
+    }
+EndFor
+
 // TSA subspaces ends ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 {% endmacro %}
 {# ================================================================================== #}
 {# ================================================================================== #}
 {# ================================================================================== #}
 {# ================================================================================== #}
 {% macro FORMULATION_VolumetricQuantities(type) %}
@@ -219,15 +211,15 @@
     NameOfSpace SPACE_hPhi[SUBSPACE_insulationSurface_down];
 }
 
 For i In {1:INPUT_NumOfTSAElements-1}
     {
         Name LOCALQUANT_hThinShell~{i};
         Type Local;
-        NameOfSpace SPACE_hPhiThinShell~{i};
+        NameOfSpace SPACE_hPhi[SUBSPACE_tsa~{i}];
     }
 EndFor
 
 {
     Name LOCALQUANT_hThinShell~{INPUT_NumOfTSAElements};
     Type Local;
     NameOfSpace SPACE_hPhi[SUBSPACE_insulationSurface_up];
@@ -239,15 +231,15 @@
     NameOfSpace SPACE_temperature[SUBSPACE_insulationSurface_up];
 }
 
 For i In{1 : INPUT_NumOfTSAElements - 1}
     {
         Name LOCALQUANT_TThinShell~{i};
         Type Local;
-        NameOfSpace SPACE_temperatureThinShell~{i};
+        NameOfSpace SPACE_temperature[SUBSPACE_tsa~{i}];
     }
 EndFor
 
 {
     Name LOCALQUANT_TThinShell~{INPUT_NumOfTSAElements};
     Type Local;
     NameOfSpace SPACE_temperature[SUBSPACE_insulationSurface_down];
@@ -291,21 +283,21 @@
 GlobalTerm{
     [ Dof{GLOBALQUANT_V}, {GLOBALQUANT_I} ];
     In DOM_airCuts;
 }
 {% elif type == "thermal" %}
 Integral {
     [ kappa[<<kappaArguments>>] * Dof{d LOCALQUANT_T}, {d LOCALQUANT_T} ];
-    In DOM_allConducting;
+    In DOM_thermal;
     Jacobian JAC_vol;
     Integration Int;
 }
 Integral {
     DtDof[ Cv[<<CvArguments>>] * Dof{LOCALQUANT_T}, {LOCALQUANT_T} ];
-    In DOM_allConducting;
+    In DOM_thermal;
     Jacobian JAC_vol;
     Integration Int;
 }
 {% if dm.magnet.solve.ti.cooling == "cryocooler" %}
 Integral {
     // Division by area to compute Watts per meter squared
     // SurfaceArea function does not allow DOM_*** as argument, so we need to use
@@ -316,32 +308,43 @@
     Integration Int;
 }
 {% endif %}
 
 {% elif type == "resistiveHeating" %}
 Integral {
     [ -(rho[<<rhoArguments>>] * {d LOCALQUANT_h}) * {d LOCALQUANT_h}, {LOCALQUANT_T} ];
-    In DOM_allConducting;
+    In DOM_resistiveHeating;
     Jacobian JAC_vol;
     Integration Int;
 }
 {% endif %}
 {% endmacro %}
 {# ================================================================================== #}
 {# ================================================================================== #}
 {# ================================================================================== #}
 {# ================================================================================== #}
 {% macro FORMULATION_TSAIntegrals(type) %}
 {% if type == "electromagnetic" %}
     {% set quantityName = "LOCALQUANT_hThinShell" %}
     {% set functionKey = "electromagnetic" %}
+    {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %}
+        {% set integrationDomain = "DOM_terminalContactLayerSurface" %}
+    {% else %}
+        {% set integrationDomain = "DOM_allInsulationSurface" %}
+    {% endif %}
 {% elif  type == "thermal" %}
     {% set quantityName = "LOCALQUANT_TThinShell" %}
     {% set functionKey = "thermal" %}
+    {% set integrationDomain = "DOM_allInsulationSurface" %}
 {% elif type == "resistiveHeating" %}
+    {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %}
+    {% set integrationDomain = "DOM_terminalContactLayerSurface" %}
+    {% else %}
+    {% set integrationDomain = "DOM_allInsulationSurface" %}
+    {% endif %}
 {% else %}
     <<0/0>>
     // ERROR: wrong type for FORMULATION_TSAIntegrals!
 {% endif %}
 
 {% if dm.magnet.solve.type in ["weaklyCoupled", "stronglyCoupled", "thermal"] %}
     {% set temperatureArgument1 = "{LOCALQUANT_TThinShell~{i}}" %}
@@ -351,52 +354,52 @@
     {% set temperatureArgument2 = "INPUT_initialTemperature" %}
 {% endif %}
 
 {% if type == "electromagnetic" or type == "thermal" %}
 For i In {0:INPUT_NumOfTSAElements-1}
     {% for a in range(1,3) %}
         {% for b in range(1,3) %}
-    Integral {
-        [
-            <<functionKey>>MassFunctionNoDta<<a>>b<<b>>[
-                <<temperatureArgument1>>,
-                <<temperatureArgument2>>
-            ] * Dof{d <<quantityName>>~{i + <<a>> - 1}},
-            {d <<quantityName>>~{i + <<b>> - 1}}
-        ];
-        In DOM_insulationSurface;
-        Integration Int;
-        Jacobian JAC_sur;
-    }
+        Integral {
+            [
+                <<functionKey>>MassFunctionNoDta<<a>>b<<b>>[
+                    <<temperatureArgument1>>,
+                    <<temperatureArgument2>>
+                ] * Dof{d <<quantityName>>~{i + <<a>> - 1}},
+                {d <<quantityName>>~{i + <<b>> - 1}}
+            ];
+            In <<integrationDomain>>;
+            Integration Int;
+            Jacobian JAC_sur;
+        }
 
-    Integral {
-        [
-            <<functionKey>>StiffnessFunctiona<<a>>b<<b>>[
-                <<temperatureArgument1>>,
-                <<temperatureArgument2>>
-            ] * Dof{<<quantityName>>~{i + <<a>> - 1}},
-            {<<quantityName>>~{i + <<b>> - 1}}
-        ];
-        In DOM_insulationSurface;
-        Integration Int;
-        Jacobian JAC_sur;
-    }
+        Integral {
+            [
+                <<functionKey>>StiffnessFunctiona<<a>>b<<b>>[
+                    <<temperatureArgument1>>,
+                    <<temperatureArgument2>>
+                ] * Dof{<<quantityName>>~{i + <<a>> - 1}},
+                {<<quantityName>>~{i + <<b>> - 1}}
+            ];
+            In <<integrationDomain>>;
+            Integration Int;
+            Jacobian JAC_sur;
+        }
 
-    Integral {
-        DtDof[
-            <<functionKey>>MassFunctionDta<<a>>b<<b>>[
-                <<temperatureArgument1>>,
-                <<temperatureArgument2>>
-            ] * Dof{<<quantityName>>~{i + <<a>> - 1}},
-            {<<quantityName>>~{i + <<b>> - 1}}
-        ];
-        In DOM_insulationSurface;
-        Integration Int;
-        Jacobian JAC_sur;
-    }
+        Integral {
+            DtDof[
+                <<functionKey>>MassFunctionDta<<a>>b<<b>>[
+                    <<temperatureArgument1>>,
+                    <<temperatureArgument2>>
+                ] * Dof{<<quantityName>>~{i + <<a>> - 1}},
+                {<<quantityName>>~{i + <<b>> - 1}}
+            ];
+            In <<integrationDomain>>;
+            Integration Int;
+            Jacobian JAC_sur;
+        }
         {% endfor %}
     {% endfor %}
 EndFor
 {% elif type == "resistiveHeating" %}
 For i In {0:INPUT_NumOfTSAElements-1}
     {% for k in range(1,3) %} // row of the 1D FE matrix
     Integral {
@@ -405,30 +408,30 @@
                 <<temperatureArgument1>>,
                 <<temperatureArgument2>>
             ] * SquNorm[
                 ({LOCALQUANT_hThinShell~{i + 1}} - {LOCALQUANT_hThinShell~{i}})/th_ins_k
             ],
             {LOCALQUANT_TThinShell~{i + <<k>> - 1}}
         ];
-        In DOM_insulationSurface;
+        In <<integrationDomain>>;
         Integration Int;
         Jacobian JAC_sur;
     } 
 
         {% for a in range(1,3) %}
             {% for b in range(1,3) %}
     Integral {
         [
             -electromagneticTripleFunctionk<<k>>a<<a>>b<<b>>[
                 <<temperatureArgument1>>,
                 <<temperatureArgument2>>
             ] * {d LOCALQUANT_hThinShell~{i + <<a>> - 1}} * {d LOCALQUANT_hThinShell~{i + <<b>> - 1}},
             {LOCALQUANT_TThinShell~{i + <<k>> - 1}}
         ];
-        In DOM_insulationSurface;
+        In <<integrationDomain>>;
         Integration Int;
         Jacobian JAC_sur;
     }
             {% endfor %}
         {% endfor %}
     {% endfor %}
 EndFor
@@ -507,43 +510,42 @@
     GenerateJac <<systemName>>;
     // Print[<<systemName>>];
     SolveJac <<systemName>>;
 
     GetNormSolution[<<systemName>>, $normOfTheSolutionVector];
     Print[{$normOfTheSolutionVector}, Format "Critical: Solution vector norm: %.3g"];
 
-    PostOperation[POSTOP_CONV_temperature];
-    Print[{ $test }, Format "Critical: Temperature: %.3g"];
+    // PostOperation[POSTOP_CONV_temperature];
+    // Print[{ $test }, Format "Critical: Temperature at tolerance point: %.3g"];
 
         {% else %}
     Test[$Time >= <<solveAfterThisTime>>]{
         GenerateJac <<systemName>>;
         SolveJac <<systemName>>;
         PostOperation[POSTOP_CONV_temperature];
         Print[{$test}];
     }
         {% endif %}
     {% endfor %}
 
-    PostOperation[POSTOP_Ic];
-    Print[{ #1 }, Format "Critical: Lowest Ic: %.3g"];
+    // PostOperation[POSTOP_Ic];
+    // Print[{ #1 }, Format "Critical: Lowest Ic: %.3g"];
 
     PostOperation[POSTOP_I];
     Print[{ $I }, Format "Critical: I: %.3g"];
 
-    Test[$I > #1]{
-        Print[{10}, Format "Critical: Quench started! %.1g"];
-    }
+    // Test[$I > #1]{
+    //     Print[{10}, Format "Critical: Quench started! %.1g"];
+    // }
 }
 // Nonlinear solver ends +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 {% elif type == "linear" %}
 // Linear solver starts ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
     {% for systemName in systemNames %}
 Generate <<systemName>>;
-Evaluate[$initializationDone = 1];
 Solve <<systemName>>;
     {% endfor %}
 // Linear solver ends ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 {% else %}
 <<0/0>>
 // ERROR: wrong for RESOLUTION_systemsOfEquationsSolver!
 {% endif %}
@@ -705,15 +707,16 @@
     onPoint="None",
     onRegion="None",
     onGlobal="None",
     onSection="None",
     depth="None",
     format="Default",
     name="None",
-    fileName="None") %}
+    fileName="None",
+    lastTimeStepOnly=False) %}
 Print[
     <<quantity>>,
 {% if onElementsOf != "None" %}
     OnElementsOf <<onElementsOf>>,
 {% elif onPoint != "None" %}
     OnPoint {<<onPoint[0]>>, <<onPoint[1]>>, <<onPoint[2]>>},
 {% elif onRegion != "None" %}
@@ -730,39 +733,49 @@
     {# <<0/0>> #}
     // ERROR: No print region specified!
 {% endif %}
 {% if depth != "None" %}
     Depth <<depth>>,
 {% endif %}
 {% if fileName != "None" %}
-    {% if format != "Default" %}
+    {% if format == "TimeTable" %}
+    File "<<fileName>>-<<format>>Format.csv",
+    {% elif format != "Default" %}
     File "<<fileName>>-<<format>>Format.txt",
     {% else %}
     File "<<fileName>>-<<format>>Format.pos",
     {% endif %}
 {% else %}
-    {% if format != "Default" %}
+    {% if format == "TimeTable" %}
+    File "<<quantity>>-<<format>>Format.csv",
+    {% elif format != "Default" %}
     File "<<quantity>>-<<format>>Format.txt",
     {% else %}
     File "<<quantity>>-<<format>>Format.pos",
     {% endif %}
 {% endif %}
-{% if format != "Default" %}
+{% if format == "TimeTable" %}
+    Format <<format>>,
+    Comma,
+{% elif format != "Default" %}
     Format <<format>>,
 {% endif %}
 {% if dm.magnet.solve.save is not none %}
     {% for quantityDict in dm.magnet.solve.save %}
         {% if quantityDict.getdpQuantityName == quantity %}
             {% if quantityDict.timesToBeSaved %}
     AppendToExistingFile 1,
     LastTimeStepOnly 1,
             {% endif %}
         {% endif %}
     {% endfor %}
 {% endif %}
+{% if lastTimeStepOnly == True %}
+    LastTimeStepOnly 1,
+{% endif %}
 {% if name != "None" %}
     Name "<<name>>"
 {% elif fileName != "None" %}
     Name "<<fileName>>"
 {% else %}
     Name "<<quantity>>"
 {% endif %}
@@ -773,72 +786,105 @@
 {# ================================================================================== #}
 {# ================================================================================== #}
 //======================================================================================
 // Physical regions: ===================================================================
 //======================================================================================
 Group{
 {% if dm.magnet.geometry.ii.tsa %}
-    {% set NofSets = len(rm.insulator.surf.numbers) %}
-    {% set HalfNofSets = (len(rm.insulator.surf.numbers)/2)|int %}
-
-    DOM_insulationSurface_0 = Region[{ <<rm.insulator.surf.numbers[-1]>> }];
+    {% set NofSets = (len(rm.insulator.surf.numbers)/2)|int %}
+    {% set HalfNofSets = (NofSets/2)|int %}
+    DOM_allInsulationSurface_0 = Region[{ <<rm.insulator.surf.numbers[-2]>> }];
+    DOM_allInsulationSurface_0 += Region[{ <<rm.insulator.surf.numbers[-1]>> }];
+    DOM_terminalContactLayerSurface_0 = Region[{ <<rm.insulator.surf.numbers[-1]>> }];
+
+    {% for i in range(1, NofSets+2) %}
+    DOM_windingMinus_<<i>> = Region[{ <<rm.powered.vol.numbers[:-2][(i-1)%NofSets]>> }];
+    DOM_windingPlus_<<i>> = Region[{ <<rm.powered.vol.numbers[:-2][(i-1+HalfNofSets)%NofSets]>> }];
 
-    {% for i in range(1, NofSets+1+1) %}
-    DOM_windingMinus_<<i>> = Region[{ <<rm.powered.vol.numbers[(i-1)%NofSets]>> }];
+    DOM_allInsulationSurface_<<i>> = Region[{ <<rm.insulator.surf.numbers[(2 * (i-1))%(2 * NofSets)]>> }];
+    DOM_allInsulationSurface_<<i>> += Region[{ <<rm.insulator.surf.numbers[(2 * (i-1))%(2 * NofSets) + 1]>> }];
 
-    DOM_windingPlus_<<i>> = Region[{ <<rm.powered.vol.numbers[(i-1+HalfNofSets)%NofSets]>> }];
+    {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %}
+    DOM_terminalContactLayerSurface_<<i>> = Region[{ <<rm.insulator.surf.numbers[(2 * (i-1))%(2 * NofSets) + 1]>> }];
+    {% endif %}
 
-    DOM_insulationSurface_<<i>> = Region[{ <<rm.insulator.surf.numbers[(i-1)%NofSets]>> }];
     {% endfor %}
 
     // Add terminals to winding region logic:
     // <<rm.powered.vol_in.number>>: inner terminal
     // <<rm.powered.vol_out.number>>: outer terminal
-    /*{% for i in range(1, HalfNofSets+1) %}
+    // <<rm.powered.vol.numbers[-2]>>: inner layer transition angle
+    // <<rm.powered.vol.numbers[-1]>>: outer layer transition angle
+    {% for i in range(1, NofSets+2) %}
     DOM_windingMinus_<<i>> += Region[{ <<rm.powered.vol_in.number>> }];
+    DOM_windingMinus_<<i>> += Region[{ <<rm.powered.vol.numbers[-2]>> }];
     {% endfor %}
 
-    {% for i in range(HalfNofSets+1, NofSets+1) %}
-    DOM_windingMinus_<<i>> += Region[{ <<rm.powered.vol_out.number>> }];
-    {% endfor %}*/
+    {% for i in range(1, NofSets+1) %}
+    DOM_windingPlus_<<i>> += Region[{ <<rm.powered.vol_out.number>> }];
+    DOM_windingPlus_<<i>> += Region[{ <<rm.powered.vol.numbers[-1]>> }];
+    {% endfor %}
 
-    DOM_insulationSurface = Region[{ <<rm.insulator.surf.numbers|join(', ')>> }];
+    DOM_allInsulationSurface = Region[{ <<rm.insulator.surf.numbers|join(', ')>> }];
+    DOM_insulationSurface = Region[{ <<rm.insulator.surf.numbers[::2]|join(', ')>> }];
+    DOM_terminalContactLayerSurface = Region[{ <<rm.insulator.surf.numbers[1::2]|join(', ')>> }];
 
     DOM_insulationBoundaryCurvesAir = Region[{ <<rm.insulator.curve.numbers[0]>> }];
     DOM_insulationBoundaryCurvesTerminal = Region[{ <<rm.insulator.curve.numbers[1]>> }];
 {% else %}
-    DOM_insulations = Region[{ <<rm.insulator.vol.numbers|join(', ')>> }];
+    DOM_insulation = Region[ <<rm.insulator.vol.numbers[0]>> ];
+    DOM_terminalContactLayer = Region[ <<rm.insulator.vol.numbers[1]>> ];
+    DOM_allInsulations = Region[{ <<rm.insulator.vol.numbers|join(', ')>> }];
 {% endif %}
 
-
     // create windings region:
-    DOM_allWindings = Region[{ <<rm.powered.vol.numbers|join(', ')>> }];
+    DOM_allWindings = Region[{ <<rm.powered.vol.numbers[:-2]|join(', ')>> }];
 
     // create terminals region:
-    DOM_terminals = Region[{ <<rm.powered.vol_in.number>>, <<rm.powered.vol_out.number>> }];
+    DOM_terminals = Region[{ <<rm.powered.vol_in.number>>, <<rm.powered.vol_out.number>>}];
+
+    // create layer transition angle region:
+    DOM_transitionNotchVolumes = Region[{<<rm.powered.vol.numbers[-2]>>, <<rm.powered.vol.numbers[-1]>>}];
 
     // create powered region:
-    DOM_powered = Region[{ DOM_allWindings, DOM_terminals }];
+    DOM_powered = Region[{ DOM_allWindings, DOM_terminals, DOM_transitionNotchVolumes }];
 
     // support of edge-based magnetic field strength, i.e., all conducting doms:
-{% if dm.magnet.geometry.ii.tsa or dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %}
-    DOM_allConducting = Region[{ DOM_powered }];
+{% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %}
+    {% if  dm.magnet.geometry.ii.tsa %}
+    DOM_allConducting = Region[{ DOM_powered}];
+    DOM_resistiveHeating = Region[{ DOM_allWindings, DOM_terminals }];
+    DOM_thermal = Region[{ DOM_powered}];
+    {% else %}
+    DOM_thermal = Region[{ DOM_powered, DOM_allInsulations}];
+    DOM_allConducting = Region[{ DOM_powered, DOM_terminalContactLayer}];
+    DOM_resistiveHeating = Region[{ DOM_allWindings, DOM_terminals, DOM_terminalContactLayer }];
+    {% endif %}
 {% else %}
-    DOM_allConducting = Region[{ DOM_powered, DOM_insulations }];
+    {% if  dm.magnet.geometry.ii.tsa %}
+    DOM_thermal = Region[{ DOM_powered}];
+    DOM_allConducting = Region[{ DOM_powered }];
+    DOM_resistiveHeating = Region[{ DOM_allWindings, DOM_terminals }];
+    {% else %}
+    DOM_thermal = Region[{ DOM_powered, DOM_allInsulations}];
+    DOM_allConducting = Region[{ DOM_powered, DOM_allInsulations }];
+    DOM_resistiveHeating = Region[{ DOM_allWindings, DOM_terminals, DOM_allInsulations }];
+    {% endif %}
 {% endif %}
     DOM_air = Region[{ <<rm.air.vol.number>> }];
 {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %}
-    DOM_airPoints = Region[{ <<rm.air.point.numbers[1]>> }];
+    DOM_airPoints = Region[{ <<rm.air.point.numbers[0]>> }];
 {% else %}
     DOM_airPoints = Region[{ <<rm.air.point.numbers|join(', ')>> }];
 {% endif %}
 
+
 {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" and
     not dm.magnet.geometry.ii.tsa %}
-    DOM_air += Region[{ <<rm.insulator.vol.numbers|join(', ')>> }];
+    DOM_air += Region[ DOM_insulation ];
 {% endif %}
 
 {% if dm.magnet.geometry.ai.shellTransformation %}
     {% if dm.magnet.geometry.ai.type == "cylinder" %}
     // add shell volume for shell transformation:
     DOM_air += Region[{ <<rm.air_far_field.vol.numbers|join(", ")>> }];
     DOM_airInf = Region[{ <<rm.air_far_field.vol.numbers|join(", ")>> }];
@@ -1033,15 +1079,15 @@
     // Winding material combination parameters start ===================================
     {% for material in dm.magnet.solve.wi.normalConductors %}
     INPUT_relativeThickness<<material.name>> = <<material.relativeThickness>>;
     {% endfor %}
 
     INPUT_relativeThicknessOfSuperConductor = <<dm.magnet.solve.wi.relativeThicknessOfSuperConductor>>;
     INPUT_relativeThicknessOfNormalConductor = <<dm.magnet.solve.wi.relativeThicknessOfNormalConductor>>;
-    INPUT_relativeWidthOfPlating = <<dm.magnet.solve.wi.plating.relativeWidth>>;
+    INPUT_relativeWidthOfPlating = <<dm.magnet.solve.wi.shuntLayer.material.relativeHeight>>;
     // Factor 1.0/<<scalingFactor>> is used equate the scaling applied to Jcritical in the parallel direction 
     INPUT_jCriticalScalingNormalToWinding = 1.0/<<scalingFactor>> * <<dm.magnet.solve.wi.superConductor.jCriticalScalingNormalToWinding>>;
     // Winding material combination parameters end =====================================
 {% endif %}
 
 {% if dm.magnet.geometry.ii.tsa %}
     // TSA parameters start ============================================================
@@ -1054,14 +1100,102 @@
 {% if dm.magnet.solve.type in ["electromagnetic", "weaklyCoupled", "stronglyCoupled"] %}
     // Winding resistivity starts ======================================================
     {% if dm.magnet.solve.wi.resistivity %}
     // Linear:
     INPUT_coilResistivity = <<dm.magnet.solve.wi.resistivity>>; // resistivity of the coil, [Ohm*m]
     rho[DOM_allWindings] = INPUT_coilResistivity;
     {% else %}
+    
+        {% set use_cpp_materials = True %}
+        {% if use_cpp_materials %}
+
+            {% if dm.magnet.solve.wi.superConductor.lengthValues is not none %}
+                {% set numberOfIcValues = len(dm.magnet.solve.wi.superConductor.lengthValues) %}
+                {% set listOfLengthValues = dm.magnet.solve.wi.superConductor.lengthValues %}
+                {% set listOfIcValues = dm.magnet.solve.wi.superConductor.IcValues %}
+            {% else %}
+                {% set numberOfIcValues = 1 %}
+                {% set listOfLengthValues = [1] %}
+                {% set listOfIcValues = [dm.magnet.solve.wi.superConductor.IcAtTinit] %}
+            {% endif %}
+    {% set materialCodes = {
+        "Copper": 0,
+        "Hastelloy": 1,
+        "Silver": 2,
+        "Indium": 3,
+        "StainlessSteel": 4,
+        "HTSSuperPower": 5
+    } %}
+    rhoWindingAndDerivative[] = WindingWithSuperConductorRhoAndDerivativeV1[
+        $Time,
+        XYZ[],
+        $3,
+        $2,
+        $1
+    ]{
+        <<numberOfIcValues>>, // N of Ic Values
+        {% for lengthValue in listOfLengthValues %}
+        <<lengthValue>>,
+        {% endfor %}
+        {% for IcValue in listOfIcValues %}
+        <<IcValue>>,
+        {% endfor %}
+        <<len(dm.magnet.solve.wi.normalConductors)>>, // N of materials,
+        {% for material in dm.magnet.solve.wi.normalConductors %}
+        <<materialCodes[material.name]>>,
+        {% endfor %}
+        {% for material in dm.magnet.solve.wi.normalConductors %}
+        <<material.relativeThickness>>,
+        {% endfor %}
+        {% for material in dm.magnet.solve.wi.normalConductors %}
+        <<material.rrr>>,
+        {% endfor %}
+        {% for material in dm.magnet.solve.wi.normalConductors %}
+        <<material.rrrRefT>>,
+        {% endfor %}
+        <<materialCodes[dm.magnet.solve.wi.shuntLayer.material.name]>>,
+        <<dm.magnet.solve.wi.shuntLayer.material.relativeHeight>>,
+        <<dm.magnet.solve.wi.shuntLayer.material.rrr>>,
+        <<dm.magnet.solve.wi.shuntLayer.material.rrrRefT>>,
+        5, // material integer: HTSSuperPower
+        <<dm.magnet.solve.wi.relativeThicknessOfSuperConductor>>, // relative thickness of HTSSuperPower
+        <<dm.magnet.solve.wi.superConductor.electricFieldCriterion>>, // electric field criterion of HTSSuperPower
+        <<dm.magnet.solve.wi.superConductor.nValue>>, // n value of HTSSuperPower
+        <<dm.magnet.solve.wi.superConductor.minimumPossibleResistivity>>, // winding minimum possible resistivity (or superconductor minimum? bug)
+        <<dm.magnet.solve.wi.superConductor.maximumPossibleResistivity>>, // winding maximum possible resistivity (or superconductor maximum? bug)
+        <<dm.magnet.solve.localDefects.jCritical.startTurn if dm.magnet.solve.localDefects.jCritical is not none else "0">>, // local defect start turn
+        <<dm.magnet.solve.localDefects.jCritical.endTurn if dm.magnet.solve.localDefects.jCritical is not none else "0">>, // local defect end turn
+        <<dm.magnet.solve.localDefects.jCritical.whichPancakeCoil if dm.magnet.solve.localDefects.jCritical is not none else "1">>, // local defect which pancake coil
+        <<dm.magnet.solve.localDefects.jCritical.value if dm.magnet.solve.localDefects.jCritical is not none else "0">>, // local defect value
+        <<dm.magnet.solve.localDefects.jCritical.startTime if dm.magnet.solve.localDefects.jCritical is not none else "99999999">>, // local defect start time
+        <<dm.magnet.geometry.wi.r_i>>,
+        <<windingThickness>>,
+        <<gapThickness>>,
+        <<dm.magnet.geometry.wi.theta_i>>,
+        <<dm.magnet.mesh.wi.ane[0]>>,
+        <<dm.magnet.geometry.N>>,
+        <<dm.magnet.geometry.wi.h>>,
+        <<dm.magnet.geometry.gap>>,
+        <<scalingFactor>>,
+        1 // arbitrary jCritical scaling normal to winding
+    };
+    rho[DOM_allWindings] = GetFirstTensor[
+        SetVariable[
+            rhoWindingAndDerivative[$1, $2, $3],
+            ElementNum[],
+            QuadraturePointIndex[],
+            $NLIteration
+        ]{
+            $rhoWindingAndDerivative
+        }
+    ];
+    d_of_rho_wrt_j_TIMES_j[DOM_allWindings] = GetSecondTensor[
+        GetVariable[ElementNum[], QuadraturePointIndex[], $NLIteration]{$rhoWindingAndDerivative}
+    ];
+        {% else %}
     // Nonlinear:
 
     // Generally, tapes consist of more than one material. They are modeled as one
     // material (including the superconductor), and their effective homogenized
     // resistivity, thermal conductivity, and specific heat capacity are calculated
     // below.
 
@@ -1107,15 +1241,15 @@
                 INPUT_relativeThickness<<material.name>>,
                     {% endif %}
                 {% endfor %}
             };
     
     // In normal direction, we consider the plating of the tape, typcially copper as a 
     // parallel connection between the series connection of all layers and the plating.
-    rhoPlatingNormalToWinding[] = rho<<dm.magnet.solve.wi.plating.name>>[$1, $2];
+    rhoPlatingNormalToWinding[] = rho<<dm.magnet.solve.wi.shuntLayer.material.name>>[$1, $2];
 
         {% if dm.magnet.solve.wi.superConductor %}
     // There is a superconductor in the winding.
 
     // To make it easier for the linear solver, a lower bound for the resistivity in the
     // superconductor is defined:
     winding_minimumPossibleRho = <<dm.magnet.solve.wi.minimumPossibleResistivity>>;
@@ -1489,126 +1623,266 @@
         rhoNormalConductorParallelToWinding[$1, $2],
         rhoNormalConductorParallelToWinding[$1, $2]
     ];
 
     // Homogenized resistivity tensor of the winding in XYZ coordinate system:
     // rho($1 = T, $2 = b, $3 = jinWindingCoordinates)
     rho[DOM_allWindings] = TransformationTensor[] * rhoTensorInWindingCoordinates[$1, $2, $3] * Transpose[TransformationTensor[]];
-
+        {% endif %}
         {% endif %}
     {% endif %}
     // Winding resistivity ends ========================================================
 
     // Terminals resistivity starts ====================================================
+    {% if dm.magnet.solve.ti.transitionNotch.resistivity %}
+    rho[DOM_transitionNotchVolumes] = <<dm.magnet.solve.ti.transitionNotch.resistivity>>;
+    {% else %}
+    rho[DOM_transitionNotchVolumes] = <<materials[dm.magnet.solve.ti.transitionNotch.material.resistivityMacroName](RRR=dm.magnet.solve.ti.transitionNotch.material.rrr, rrrRefT=dm.magnet.solve.ti.transitionNotch.material.rrrRefT)>>;
+    {% endif %}
+
     {% if dm.magnet.solve.ti.resistivity %}
     // Linear:
     INPUT_terminalResistivity = <<dm.magnet.solve.ti.resistivity>>; // resistivity of the terminals, [Ohm*m]
     rho[DOM_terminals] = INPUT_terminalResistivity;
     {% else %}
     // Nonlinear:
     rho[DOM_terminals] = <<materials[dm.magnet.solve.ti.material.resistivityMacroName](RRR=dm.magnet.solve.ti.material.rrr, rrrRefT=dm.magnet.solve.ti.material.rrrRefT)>>;
     
     {% endif %}
     // Terminals resistivity ends ======================================================
 
     // Insulation resistivity starts ===================================================
-    {% if dm.magnet.solve.ii.resistivity and dm.magnet.solve.ii.resistivity != "perfectlyInsulating" %}
+    {% if dm.magnet.solve.ii.resistivity != "perfectlyInsulating" %}
+    {% if dm.magnet.solve.ii.resistivity %}
     // Linear:
-    INPUT_insulationResistivity = <<dm.magnet.solve.ii.resistivity>>; // resistivity of the insulation, [Ohm*m]
+    INPUT_insulationResistivity =<<dm.magnet.solve.ii.resistivity>>; // resistivity of the insulation, [Ohm*m]
 
         {% if dm.magnet.geometry.ii.tsa %}
+        electromagneticOnlyFunction[DOM_insulationSurface] = TSA_constantMaterial_constantThickness_fct_only[]{
+            th_ins_k, INPUT_insulationResistivity
+        };
     // Thin-shell insulation:
             {% for a in range(1,3) %}
                 {% for b in range(1,3) %}
-    electromagneticMassFunctionNoDta<<a>>b<<b>>[] = TSA_constantMaterial_constantThickness_mass[]{
+    electromagneticMassFunctionNoDta<<a>>b<<b>>[DOM_insulationSurface] = TSA_constantMaterial_constantThickness_mass[]{
             th_ins_k, INPUT_insulationResistivity, <<a>>, <<b>>
         };
     
-    electromagneticStiffnessFunctiona<<a>>b<<b>>[] = TSA_constantMaterial_constantThickness_stiffness[]{
+    electromagneticStiffnessFunctiona<<a>>b<<b>>[DOM_insulationSurface] = TSA_constantMaterial_constantThickness_stiffness[]{
             th_ins_k, INPUT_insulationResistivity, <<a>>, <<b>>
         };
 
-    electromagneticMassFunctionDta<<a>>b<<b>>[] = TSA_constantMaterial_constantThickness_mass[]{
+    electromagneticMassFunctionDta<<a>>b<<b>>[DOM_insulationSurface] = TSA_constantMaterial_constantThickness_mass[]{
             th_ins_k, INPUT_airMagneticPermeability, <<a>>, <<b>>
         };
 
                 {% endfor %}
         {% endfor %}
         
             {% for k in range(1,3) %}
-    electromagneticRHSFunctionk<<k>>[] = TSA_constantMaterial_constantThickness_rhs[]{
+    electromagneticRHSFunctionk<<k>>[DOM_insulationSurface] = TSA_constantMaterial_constantThickness_rhs[]{
             th_ins_k, INPUT_insulationResistivity
         };
 
                 {% for a in range(1,3) %}
                     {% for b in range(1,3) %}
-    electromagneticTripleFunctionk<<k>>a<<a>>b<<b>>[] = TSA_constantMaterial_constantThickness_triple[]{
+    electromagneticTripleFunctionk<<k>>a<<a>>b<<b>>[DOM_insulationSurface] = TSA_constantMaterial_constantThickness_triple[]{
             th_ins_k, INPUT_insulationResistivity, <<k>>, <<a>>, <<b>>
         };
 
                     {% endfor %}
                 {% endfor %}
             {% endfor %}
 
         {% else %}
     // Volume insulation:
-    rho[DOM_insulations] = INPUT_insulationResistivity;
+    rho[DOM_insulation] = INPUT_insulationResistivity;
         {% endif %}
     {% elif not dm.magnet.solve.ii.resistivity %}
     // Nonlinear:
         {% if dm.magnet.geometry.ii.tsa %}
+        electromagneticOnlyFunction[DOM_insulationSurface] = <<dm.magnet.solve.ii.material.getdpTSAOnlyResistivityFunction>>[$1, $2]{
+            oneDGaussianOrder, th_ins_k
+        };
     // Thin-shell insulation:
             {% for a in range(1,3) %}   
                 {% for b in range(1,3) %}
-    electromagneticMassFunctionNoDta<<a>>b<<b>>[] = <<dm.magnet.solve.ii.material.getdpTSAMassResistivityFunction>>[$1, $2]{
+    electromagneticMassFunctionNoDta<<a>>b<<b>>[DOM_insulationSurface] = <<dm.magnet.solve.ii.material.getdpTSAMassResistivityFunction>>[$1, $2]{
             <<a>>, <<b>>, oneDGaussianOrder, th_ins_k
         };
     
-    electromagneticStiffnessFunctiona<<a>>b<<b>>[] = <<dm.magnet.solve.ii.material.getdpTSAStiffnessResistivityFunction>>[$1, $2]{
+    electromagneticStiffnessFunctiona<<a>>b<<b>>[DOM_insulationSurface] = <<dm.magnet.solve.ii.material.getdpTSAStiffnessResistivityFunction>>[$1, $2]{
             <<a>>, <<b>>, oneDGaussianOrder, th_ins_k
         };
 
-    electromagneticMassFunctionDta<<a>>b<<b>>[] = TSA_constantMaterial_constantThickness_mass[]{
+    electromagneticMassFunctionDta<<a>>b<<b>>[DOM_insulationSurface] = TSA_constantMaterial_constantThickness_mass[]{
             th_ins_k, INPUT_airMagneticPermeability, <<a>>, <<b>>
         };
 
                 {% endfor %}
             {% endfor %}
     
             {% for k in range(1,3) %}
-    electromagneticRHSFunctionk<<k>>[] = <<dm.magnet.solve.ii.material.getdpTSARHSFunction>>[$1, $2]{
+    electromagneticRHSFunctionk<<k>>[DOM_insulationSurface] = <<dm.magnet.solve.ii.material.getdpTSARHSFunction>>[$1, $2]{
             <<k>>, oneDGaussianOrder, th_ins_k
         };
 
                 {% for a in range(1,3) %}
                     {% for b in range(1,3) %}
-    electromagneticTripleFunctionk<<k>>a<<a>>b<<b>>[] = <<dm.magnet.solve.ii.material.getdpTSATripleFunction>>[$1, $2]{
+    electromagneticTripleFunctionk<<k>>a<<a>>b<<b>>[DOM_insulationSurface] = <<dm.magnet.solve.ii.material.getdpTSATripleFunction>>[$1, $2]{
             <<k>>, <<a>>, <<b>>, oneDGaussianOrder, th_ins_k
         };
 
                     {% endfor %}
                 {% endfor %}
             {% endfor %}
         {% else %}
     // Volume insulation:
-    rho[DOM_insulations] = <<materials[dm.magnet.solve.ii.material.resistivityMacroName](RRR=dm.magnet.solve.ii.material.rrr, rrrRefT=dm.magnet.solve.ii.material.rrrRefT)>>;
+    rho[DOM_insulation] = <<materials[dm.magnet.solve.ii.material.resistivityMacroName](RRR=dm.magnet.solve.ii.material.rrr, rrrRefT=dm.magnet.solve.ii.material.rrrRefT)>>;
 
         {% endif %}
     {% endif %}
+    {% endif %}
     // Insulation resistivity ends =====================================================
+
+    // Transition layer resistivity starts =============================================
+    {% if dm.magnet.solve.ti.terminalContactLayer.resistivity %}
+    // Linear:
+    INPUT_terminalContactLayerResistivity = <<dm.magnet.solve.ti.terminalContactLayer.resistivity>>; // resistivity of the insulation, [Ohm*m]
+
+    {% if dm.magnet.geometry.ii.tsa %}
+    electromagneticOnlyFunction[DOM_terminalContactLayerSurface] = TSA_constantMaterial_constantThickness_fct_only[]{
+        th_ins_k, INPUT_terminalContactLayerResistivity
+    };
+    // Thin-shell insulation:
+        {% for a in range(1,3) %}
+            {% for b in range(1,3) %}
+    electromagneticMassFunctionNoDta<<a>>b<<b>>[DOM_terminalContactLayerSurface] = TSA_constantMaterial_constantThickness_mass[]{
+            th_ins_k, INPUT_terminalContactLayerResistivity, <<a>>, <<b>>
+        };
+
+    electromagneticStiffnessFunctiona<<a>>b<<b>>[DOM_terminalContactLayerSurface] = TSA_constantMaterial_constantThickness_stiffness[]{
+            th_ins_k, INPUT_terminalContactLayerResistivity, <<a>>, <<b>>
+        };
+
+    electromagneticMassFunctionDta<<a>>b<<b>>[DOM_terminalContactLayerSurface] = TSA_constantMaterial_constantThickness_mass[]{
+            th_ins_k, INPUT_airMagneticPermeability, <<a>>, <<b>>
+        };
+
+                {% endfor %}
+        {% endfor %}
+        
+            {% for k in range(1,3) %}
+    electromagneticRHSFunctionk<<k>>[DOM_terminalContactLayerSurface] = TSA_constantMaterial_constantThickness_rhs[]{
+            th_ins_k, INPUT_terminalContactLayerResistivity
+        };
+
+                {% for a in range(1,3) %}
+                    {% for b in range(1,3) %}
+    electromagneticTripleFunctionk<<k>>a<<a>>b<<b>>[DOM_terminalContactLayerSurface] = TSA_constantMaterial_constantThickness_triple[]{
+            th_ins_k, INPUT_terminalContactLayerResistivity, <<k>>, <<a>>, <<b>>
+        };
+
+                    {% endfor %}
+                {% endfor %}
+            {% endfor %}
+
+        {% else %}
+    rho[DOM_terminalContactLayer] = INPUT_terminalContactLayerResistivity;
+        {% endif %}
+    {% elif not dm.magnet.solve.ti.terminalContactLayer.resistivity %}
+    // Nonlinear:
+        {% if dm.magnet.geometry.ii.tsa %}
+        electromagneticOnlyFunction[DOM_terminalContactLayerSurface] = <<dm.magnet.solve.ti.terminalContactLayer.material.getdpTSAOnlyResistivityFunction>>[$1, $2]{
+            oneDGaussianOrder, th_ins_k
+        };
+    // Thin-shell insulation:
+            {% for a in range(1,3) %}   
+                {% for b in range(1,3) %}
+    electromagneticMassFunctionNoDta<<a>>b<<b>>[DOM_terminalContactLayerSurface] = <<dm.magnet.solve.ti.terminalContactLayer.material.getdpTSAMassResistivityFunction>>[$1, $2]{
+            <<a>>, <<b>>, oneDGaussianOrder, th_ins_k
+        };
+    
+    electromagneticStiffnessFunctiona<<a>>b<<b>>[DOM_terminalContactLayerSurface] = <<dm.magnet.solve.ti.terminalContactLayer.material.getdpTSAStiffnessResistivityFunction>>[$1, $2]{
+            <<a>>, <<b>>, oneDGaussianOrder, th_ins_k
+        };
+
+    electromagneticMassFunctionDta<<a>>b<<b>>[DOM_terminalContactLayerSurface] = TSA_constantMaterial_constantThickness_mass[]{
+            th_ins_k, INPUT_airMagneticPermeability, <<a>>, <<b>>
+        };
+
+                {% endfor %}
+            {% endfor %}
+    
+            {% for k in range(1,3) %}
+    electromagneticRHSFunctionk<<k>>[DOM_terminalContactLayerSurface] = <<dm.magnet.solve.ti.terminalContactLayer.material.getdpTSARHSFunction>>[$1, $2]{
+            <<k>>, oneDGaussianOrder, th_ins_k
+        };
+
+                {% for a in range(1,3) %}
+                    {% for b in range(1,3) %}
+    electromagneticTripleFunctionk<<k>>a<<a>>b<<b>>[DOM_terminalContactLayerSurface] = <<dm.magnet.solve.ti.terminalContactLayer.material.getdpTSATripleFunction>>[$1, $2]{
+            <<k>>, <<a>>, <<b>>, oneDGaussianOrder, th_ins_k
+        };
+
+                    {% endfor %}
+                {% endfor %}
+            {% endfor %}
+        {% else %}
+    // Volume insulation:
+    rho[DOM_terminalContactLayer] = <<materials[dm.magnet.solve.ti.terminalContactLayer.material.resistivityMacroName](RRR=dm.magnet.solve.ti.terminalContactLayer.material.rrr, rrrRefT=dm.magnet.solve.ti.terminalContactLayer.material.rrrRefT)>>;
+
+        {% endif %}
+    {% endif %}
+    // Transition layer resistivity ends ===============================================
 {% endif %}
 
 {% if dm.magnet.solve.type in ["thermal", "weaklyCoupled", "stronglyCoupled"] %}
     // Winding thermal conductivity starts =============================================
     {% if dm.magnet.solve.wi.thermalConductivity %}
     // Linear:
     INPUT_windingThermalConductivity = <<dm.magnet.solve.wi.thermalConductivity>>; // thermal conductivity of the winding, [W/*(m*K)]
     kappa[DOM_allWindings] = INPUT_windingThermalConductivity;
     {% else %}
     // Nonlinear:
+    {% if use_cpp_materials %}
+    kappa[DOM_allWindings] = WindingThermalConductivityV1[
+        XYZ[],
+        $2,
+        $1
+    ]{
+        <<len(dm.magnet.solve.wi.normalConductors)>>, // N of materials,
+        {% for material in dm.magnet.solve.wi.normalConductors %}
+        <<materialCodes[material.name]>>,
+        {% endfor %}
+        {% for material in dm.magnet.solve.wi.normalConductors %}
+        <<material.relativeThickness>>,
+        {% endfor %}
+        {% for material in dm.magnet.solve.wi.normalConductors %}
+        <<material.rrr>>,
+        {% endfor %}
+        {% for material in dm.magnet.solve.wi.normalConductors %}
+        <<material.rrrRefT>>,
+        {% endfor %}
+        <<materialCodes[dm.magnet.solve.wi.shuntLayer.material.name]>>,
+        <<dm.magnet.solve.wi.shuntLayer.material.relativeHeight>>,
+        <<dm.magnet.solve.wi.shuntLayer.material.rrr>>,
+        <<dm.magnet.solve.wi.shuntLayer.material.rrrRefT>>,
+        <<dm.magnet.geometry.wi.r_i>>,
+        <<windingThickness>>,
+        <<gapThickness>>,
+        <<dm.magnet.geometry.wi.theta_i>>,
+        <<dm.magnet.mesh.wi.ane[0]>>,
+        <<dm.magnet.geometry.N>>,
+        <<dm.magnet.geometry.wi.h>>,
+        <<dm.magnet.geometry.gap>>,
+        <<scalingFactor>>,
+        1 // arbitrary jCritical scaling normal to winding
+    };
+    {% else %}
         {% for material in dm.magnet.solve.wi.normalConductors %}
     kappa<<material.name>>[] = <<materials[material.thermalConductivityMacroName](RRR=material.rrr, rrrRefT=material.rrrRefT)>>;
         {% endfor %}
 
     // The effective thermal conductivity parallel to the winding (parallel connection
     // of materials):
     kappaParallelToWinding[DOM_allWindings] = RuleOfMixtures[
@@ -1645,34 +1919,40 @@
                 {% if loop.last %}
             INPUT_relativeThickness<<material.name>>
                 {% else %}
             INPUT_relativeThickness<<material.name>>,
                 {% endif %}
             {% endfor %}
         }, 
-        kappa<<dm.magnet.solve.wi.plating.name>>[$1, $2]
+        kappa<<dm.magnet.solve.wi.shuntLayer.material.name>>[$1, $2]
     ]{
         1.0 - INPUT_relativeWidthOfPlating, 
         INPUT_relativeWidthOfPlating
     };
 
     kappaTensorInWindingCoordinates[] = TensorDiag[
         1.0/<<scalingFactor>> * kappaNormalToWinding[$1, $2],
         <<scalingFactor>> * kappaParallelToWinding[$1, $2],
         <<scalingFactor>> * kappaParallelToWinding[$1, $2]
     ];
 
     // Homogenized thermal conductivity tensor of the winding in XYZ coordinate system:
     // rho($1 = T, $2 = b, $3 = jMagnitude)
     kappa[DOM_allWindings] = TransformationTensor[] * kappaTensorInWindingCoordinates[$1, $2] * Transpose[TransformationTensor[]];
-
+    {% endif %}
     {% endif %}
     // Winding thermal conductivity ends ===============================================
 
     // Terminals thermal conductivity starts ===========================================
+    {% if dm.magnet.solve.ti.transitionNotch.thermalConductivity %}
+    kappa[DOM_transitionNotchVolumes] = <<dm.magnet.solve.ti.transitionNotch.thermalConductivity>>;
+    {% else %}
+    kappa[DOM_transitionNotchVolumes] = <<materials[dm.magnet.solve.ti.transitionNotch.material.thermalConductivityMacroName](RRR=dm.magnet.solve.ti.transitionNotch.material.rrr, rrrRefT=dm.magnet.solve.ti.transitionNotch.material.rrrRefT)>>;
+    {% endif %}
+
     {% if dm.magnet.solve.ti.thermalConductivity %}
     // Linear:
     INPUT_terminalThermalConductivity = <<dm.magnet.solve.ti.thermalConductivity>>; // thermal conductivity of the terminal, [W/*(m*K)]
     kappa[DOM_terminals] = INPUT_terminalThermalConductivity;
     kappa[DOM_topTerminalSurface] = INPUT_terminalThermalConductivity;
     kappa[DOM_bottomTerminalSurface] = INPUT_terminalThermalConductivity;
     {% else %}
@@ -1688,50 +1968,95 @@
     // Linear:
     INPUT_insulationThermalConductivity = <<dm.magnet.solve.ii.thermalConductivity>>; // thermal conductivity of the insulation, [W/*(m*K)]
 
         {% if dm.magnet.geometry.ii.tsa %}
     // Thin-shell insulation:
             {% for a in range(1,3) %}
                 {% for b in range(1,3) %}
-    thermalMassFunctionNoDta<<a>>b<<b>>[] = TSA_constantMaterial_constantThickness_mass[]{
+    thermalMassFunctionNoDta<<a>>b<<b>>[DOM_insulationSurface] = TSA_constantMaterial_constantThickness_mass[]{
             th_ins_k, INPUT_insulationThermalConductivity, <<a>>, <<b>>
         };
 
-    thermalStiffnessFunctiona<<a>>b<<b>>[] = TSA_constantMaterial_constantThickness_stiffness[]{
+    thermalStiffnessFunctiona<<a>>b<<b>>[DOM_insulationSurface] = TSA_constantMaterial_constantThickness_stiffness[]{
             th_ins_k, INPUT_insulationThermalConductivity, <<a>>, <<b>>
         };
 
                 {% endfor %}
             {% endfor %}
         {% else %}
     // Volume insulation:
-    kappa[DOM_insulations] = INPUT_insulationThermalConductivity;
+    kappa[DOM_insulation] = INPUT_insulationThermalConductivity;
         {% endif %}
     {% else %}
     // Nonlinear:
         {% if dm.magnet.geometry.ii.tsa %}
     // Thin-shell insulation:
             {% for a in range(1,3) %}
                 {% for b in range(1,3) %}
-    thermalMassFunctionNoDta<<a>>b<<b>>[] = <<dm.magnet.solve.ii.material.getdpTSAMassThermalConductivityFunction>>[$1, $2]{
+    thermalMassFunctionNoDta<<a>>b<<b>>[DOM_insulationSurface] = <<dm.magnet.solve.ii.material.getdpTSAMassThermalConductivityFunction>>[$1, $2]{
             <<a>>, <<b>>, oneDGaussianOrder, th_ins_k
         };
 
-    thermalStiffnessFunctiona<<a>>b<<b>>[] = <<dm.magnet.solve.ii.material.getdpTSAStiffnessThermalConductivityFunction>>[$1, $2]{
+    thermalStiffnessFunctiona<<a>>b<<b>>[DOM_insulationSurface] = <<dm.magnet.solve.ii.material.getdpTSAStiffnessThermalConductivityFunction>>[$1, $2]{
             <<a>>, <<b>>, oneDGaussianOrder, th_ins_k
         };
                 {% endfor %}
             {% endfor %}
         {% else %}
     // Volume insulation:
-    kappa[DOM_insulations] = <<materials[dm.magnet.solve.ii.material.thermalConductivityMacroName](RRR=dm.magnet.solve.ii.material.rrr, rrrRefT=dm.magnet.solve.ii.material.rrrRefT)>>;
+    kappa[DOM_insulation] = <<materials[dm.magnet.solve.ii.material.thermalConductivityMacroName](RRR=dm.magnet.solve.ii.material.rrr, rrrRefT=dm.magnet.solve.ii.material.rrrRefT)>>;
         {% endif %}
     {% endif %}
     // Insulation thermal conductivity ends ============================================
 
+    // Transition layer thermal conductivity starts ====================================
+    {% if dm.magnet.solve.ti.terminalContactLayer.thermalConductivity %}
+    // Linear:
+    INPUT_terminalContactLayerThermalConductivity = <<dm.magnet.solve.ti.terminalContactLayer.thermalConductivity>>; // thermal conductivity of the insulation, [W/*(m*K)]
+
+        {% if dm.magnet.geometry.ii.tsa %}
+    // Thin-shell insulation:
+            {% for a in range(1,3) %}
+                {% for b in range(1,3) %}
+    thermalMassFunctionNoDta<<a>>b<<b>>[DOM_terminalContactLayerSurface] = TSA_constantMaterial_constantThickness_mass[]{
+            th_ins_k, INPUT_terminalContactLayerThermalConductivity, <<a>>, <<b>>
+        };
+
+    thermalStiffnessFunctiona<<a>>b<<b>>[DOM_terminalContactLayerSurface] = TSA_constantMaterial_constantThickness_stiffness[]{
+            th_ins_k, INPUT_terminalContactLayerThermalConductivity, <<a>>, <<b>>
+        };
+
+                {% endfor %}
+            {% endfor %}
+        {% else %}
+    // Volume insulation:
+    kappa[DOM_terminalContactLayer] = INPUT_terminalContactLayerThermalConductivity;
+        {% endif %}
+    {% else %}
+    // Nonlinear:
+        {% if dm.magnet.geometry.ii.tsa %}
+    // Thin-shell insulation:
+            {% for a in range(1,3) %}
+                {% for b in range(1,3) %}
+    thermalMassFunctionNoDta<<a>>b<<b>>[DOM_terminalContactLayerSurface] = <<dm.magnet.solve.ti.terminalContactLayer.material.getdpTSAMassThermalConductivityFunction>>[$1, $2]{
+            <<a>>, <<b>>, oneDGaussianOrder, th_ins_k
+        };
+
+    thermalStiffnessFunctiona<<a>>b<<b>>[DOM_terminalContactLayerSurface] = <<dm.magnet.solve.ti.terminalContactLayer.material.getdpTSAStiffnessThermalConductivityFunction>>[$1, $2]{
+            <<a>>, <<b>>, oneDGaussianOrder, th_ins_k
+        };
+                {% endfor %}
+            {% endfor %}
+        {% else %}
+    // Volume insulation:
+    kappa[DOM_terminalContactLayer] = <<materials[dm.magnet.solve.ti.terminalContactLayer.material.thermalConductivityMacroName](RRR=dm.magnet.solve.ti.terminalContactLayer.material.rrr, rrrRefT=dm.magnet.solve.ti.terminalContactLayer.material.rrrRefT)>>;
+        {% endif %}
+    {% endif %}
+    // Transition layer thermal conductivity ends ======================================
+
     // Winding specific heat capacity starts ===========================================
     {% if dm.magnet.solve.wi.specificHeatCapacity %}
     // Linear:
     INPUT_coilSpecificHeatCapacity = <<dm.magnet.solve.wi.specificHeatCapacity>>; // specific heat capacity of the coil, [J/(kg*K)]
     Cv[DOM_allWindings] = INPUT_coilSpecificHeatCapacity;
     {% else %}
     // Nonlinear:
@@ -1756,14 +2081,20 @@
             {% endif %}
         {% endfor %}
     };
     {% endif %}
     // Winding specific heat capacity ends =============================================
 
     // Terminals specific heat capacity starts =========================================
+    {% if dm.magnet.solve.ti.transitionNotch.specificHeatCapacity %}
+    Cv[DOM_transitionNotchVolumes] = <<dm.magnet.solve.ti.transitionNotch.specificHeatCapacity>>;
+    {% else %}
+    Cv[DOM_transitionNotchVolumes] = <<materials[dm.magnet.solve.ti.transitionNotch.material.heatCapacityMacroName]()>>;
+    {% endif %}
+
     {% if dm.magnet.solve.ti.specificHeatCapacity %}
     // Linear:
     INPUT_terminalSpecificHeatCapacity = <<dm.magnet.solve.ti.specificHeatCapacity>>; // specific heat capacity of the terminal, [J/(kg*K)]
     Cv[DOM_terminals] = INPUT_terminalSpecificHeatCapacity;
     {% else %}
     // Nonlinear:
     Cv[DOM_terminals] =  <<materials[dm.magnet.solve.ti.material.heatCapacityMacroName]()>>;
@@ -1775,42 +2106,82 @@
     // Linear:
     INPUT_insulationSpecificHeatCapacity = <<dm.magnet.solve.ii.specificHeatCapacity>>; // specific heat capacity of the terminal, [J/(kg*K)]
 
         {% if dm.magnet.geometry.ii.tsa %}
     // Thin-shell insulation:
             {% for a in range(1,3) %}
                 {% for b in range(1,3) %}
-    thermalMassFunctionDta<<a>>b<<b>>[] = TSA_constantMaterial_constantThickness_mass[]{
+    thermalMassFunctionDta<<a>>b<<b>>[DOM_insulationSurface] = TSA_constantMaterial_constantThickness_mass[]{
             th_ins_k, INPUT_insulationSpecificHeatCapacity, <<a>>, <<b>>
         };
 
                 {% endfor %}
             {% endfor %}
         {% else %}
     // Volume insulation:
-    Cv[DOM_insulations] = INPUT_insulationSpecificHeatCapacity;
+    Cv[DOM_insulation] = INPUT_insulationSpecificHeatCapacity;
         {% endif %}
+
     {% else %}
     // Nonlinear:
         {% if dm.magnet.geometry.ii.tsa %}
     // Thin-shell insulation:
             {% for a in range(1,3) %}
                 {% for b in range(1,3) %}
-    thermalMassFunctionDta<<a>>b<<b>>[] = <<dm.magnet.solve.ii.material.getdpTSAMassHeatCapacityFunction>>[$1, $2]{
+    thermalMassFunctionDta<<a>>b<<b>>[DOM_insulationSurface] = <<dm.magnet.solve.ii.material.getdpTSAMassHeatCapacityFunction>>[$1, $2]{
             <<a>>, <<b>>, oneDGaussianOrder, th_ins_k
         };
 
                 {% endfor %}
             {% endfor %}
         {% else %}
     // Volume insulation:
-    Cv[DOM_insulations] = <<materials[dm.magnet.solve.ii.material.heatCapacityMacroName]()>>;
+    Cv[DOM_insulation] = <<materials[dm.magnet.solve.ii.material.heatCapacityMacroName]()>>;
         {% endif %}
     {% endif %}
     // Insulation specific heat capacity ends ==========================================
+
+    // Transition layer specific heat capacity starts ==================================
+    {% if dm.magnet.solve.ti.terminalContactLayer.specificHeatCapacity %}
+    // Linear:
+    INPUT_terminalContactLayerSpecificHeatCapacity = <<dm.magnet.solve.ti.terminalContactLayer.specificHeatCapacity>>; // specific heat capacity of the terminal, [J/(kg*K)]
+
+        {% if dm.magnet.geometry.ii.tsa %}
+    // Thin-shell insulation:
+            {% for a in range(1,3) %}
+                {% for b in range(1,3) %}
+    thermalMassFunctionDta<<a>>b<<b>>[DOM_terminalContactLayerSurface] = TSA_constantMaterial_constantThickness_mass[]{
+            th_ins_k, INPUT_terminalContactLayerSpecificHeatCapacity, <<a>>, <<b>>
+        };
+
+                {% endfor %}
+            {% endfor %}
+        {% else %}
+    // Volume insulation:
+    Cv[DOM_terminalContactLayer] = INPUT_terminalContactLayerSpecificHeatCapacity;
+        {% endif %}
+
+    {% else %}
+    // Nonlinear:
+        {% if dm.magnet.geometry.ii.tsa %}
+    // Thin-shell insulation:
+            {% for a in range(1,3) %}
+                {% for b in range(1,3) %}
+    thermalMassFunctionDta<<a>>b<<b>>[DOM_terminalContactLayerSurface] = <<dm.magnet.solve.ti.terminalContactLayer.material.getdpTSAMassHeatCapacityFunction>>[$1, $2]{
+            <<a>>, <<b>>, oneDGaussianOrder, th_ins_k
+        };
+
+                {% endfor %}
+            {% endfor %}
+        {% else %}
+    // Volume insulation:
+    Cv[DOM_terminalContactLayer] = <<materials[dm.magnet.solve.ti.terminalContactLayer.material.heatCapacityMacroName]()>>;
+        {% endif %}
+    {% endif %}
+    // Transition layer specific heat capacity ends ====================================
 {% endif %}
 {% if dm.magnet.geometry.ai.shellTransformation %}
 
     // Shell transformation parameters:
     {% if dm.magnet.geometry.ai.type == "cylinder" %}
     INPUT_shellInnerRadius = <<dm.magnet.geometry.ai.r>>; // inner radius of the shell, [m]
     INPUT_shellOuterRadius = <<dm.magnet.geometry.ai.shellOuterRadius>>; // outer radius of the shell, [m]
@@ -1821,21 +2192,31 @@
     INPUT_shellOuterDistance = <<shellOuterDistance>>; // outer radius of the shell, [m]
     <<0/0>>
     // ERROR: Shell transformation is not implemented for cuboid type of air yet!
     {% endif %}
 {% endif %}
 {% if dm.magnet.solve.systemsOfEquationsType == "nonlinear" %}
     {% if dm.magnet.solve.type in ["weaklyCoupled", "stronglyCoupled"] %}
-        {% set rhoArguments = "{LOCALQUANT_T}, mu[] * {LOCALQUANT_h}, Transpose[TransformationTensor[]] * {d LOCALQUANT_h}, arcLengthOfWinding[]" %}
-        {% set kappaArguments = "{LOCALQUANT_T}, Norm[mu[] * {LOCALQUANT_h}]" %}
+        {% if use_cpp_materials %}
+            {% set rhoArguments = "{LOCALQUANT_T}, mu[] * {LOCALQUANT_h}, {d LOCALQUANT_h}, arcLengthOfWinding[]" %}
+            {% set kappaArguments = "{LOCALQUANT_T}, mu[] * {LOCALQUANT_h}" %}
+        {% else %}
+            {% set rhoArguments = "{LOCALQUANT_T}, mu[] * {LOCALQUANT_h}, Transpose[TransformationTensor[]] * {d LOCALQUANT_h}, arcLengthOfWinding[]" %}
+            {% set kappaArguments = "{LOCALQUANT_T}, Norm[mu[] * {LOCALQUANT_h}]" %}
+        {% endif %}
         {% set CvArguments = "{LOCALQUANT_T}, Norm[mu[] * {LOCALQUANT_h}]" %}
         {% set JcriticalArguments = rhoArguments %}
     {% elif dm.magnet.solve.type == "electromagnetic" %}
-        {% set rhoArguments = "INPUT_initialTemperature, mu[] * {LOCALQUANT_h}, Transpose[TransformationTensor[]] * {d LOCALQUANT_h}, arcLengthOfWinding[]" %}
-        {% set kappaArguments = "INPUT_initialTemperature, Norm[mu[] * {LOCALQUANT_h}]" %}
+        {% if use_cpp_materials %}
+            {% set rhoArguments = "INPUT_initialTemperature, mu[] * {LOCALQUANT_h}, {d LOCALQUANT_h}, arcLengthOfWinding[]" %}
+            {% set kappaArguments = "INPUT_initialTemperature, mu[] * {LOCALQUANT_h}" %}
+        {% else %}
+            {% set rhoArguments = "INPUT_initialTemperature, mu[] * {LOCALQUANT_h}, Transpose[TransformationTensor[]] * {d LOCALQUANT_h}, arcLengthOfWinding[]" %}
+            {% set kappaArguments = "INPUT_initialTemperature, Norm[mu[] * {LOCALQUANT_h}]" %}
+        {% endif %}
         {% set CvArguments = "INPUT_initialTemperature, Norm[mu[] * {LOCALQUANT_h}]" %}
         {% set JcriticalArguments = rhoArguments %}
     {% elif dm.magnet.solve.type == "thermal" %}
         {% set rhoArguments = "{LOCALQUANT_T}, 0, 0, 0" %}
         {% set kappaArguments = "{LOCALQUANT_T}, 0, 0" %}
         {% set CvArguments = "{LOCALQUANT_T}, 0, 0" %}
         {% set JcriticalArguments = rhoArguments %}
@@ -1987,40 +2368,40 @@
                 Type Assign;
                 Value <<dm.magnet.solve.ic.T>>;
             }
         {% endif %}
         {% if dm.magnet.solve.isothermalInAxialDirection %}
             {% if dm.magnet.geometry.ii.tsa %}
             {
-                Region Region[{DOM_allWindings, DOM_insulationSurface}];
+                Region Region[{DOM_allWindings, DOM_allInsulationSurface}];
                 Type Link;
-                RegionRef Region[{DOM_allWindings, DOM_insulationSurface}];
+                RegionRef Region[{DOM_allWindings, DOM_allInsulationSurface}];
                 Coefficient 1;
                 Function Vector[X[], Y[], <<dm.magnet.geometry.wi.h/2>>];
             }
             {% else %}
             {
-                Region Region[{DOM_allWindings, DOM_insulations}];
+                Region Region[{DOM_allWindings, DOM_allInsulations}];
                 Type Link;
-                RegionRef Region[{DOM_allWindings, DOM_insulations}];
+                RegionRef Region[{DOM_allWindings, DOM_allInsulations}];
                 Coefficient 1;
                 Function Vector[X[], Y[], <<dm.magnet.geometry.wi.h/2>>];
             }
             {% endif %}
         {% endif %}
             {
                 {% if dm.magnet.geometry.ii.tsa %}
                 Region Region[
                             {
                                 DOM_powered, 
-                                DOM_insulationSurface
+                                DOM_allInsulationSurface
                             }
                         ];
                 {% else %}
-                Region Region[{DOM_powered, DOM_insulations}];
+                Region Region[{DOM_powered, DOM_allInsulations}];
                 {% endif %}
                 Type Init;
                 Value <<dm.magnet.solve.ic.T>>;
             }
         }
     }
 }
@@ -2031,86 +2412,106 @@
 FunctionSpace{
     {
         Name SPACE_hPhi;
         Type Form1;
         BasisFunction{
             // gradient of nodal basis functions in DOM_Phi and on DOM_pancakeBoundary
             {
-                Name BASISFUN_gradspin;
+                Name BASISFUN_gradpsin;
                 NameOfCoef phin;
                 Function BF_GradNode;
 {% if dm.magnet.geometry.ii.tsa %}
 {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %}
-                Support Region[{DOM_total, DOM_insulationSurface}];
-                Entity NodesOf[{DOM_Phi, DOM_insulationSurface}];
+                Support Region[{DOM_total, DOM_allInsulationSurface}];
+                Entity NodesOf[{DOM_Phi, DOM_insulationSurface}, Not {DOM_insulationBoundaryCurvesAir}];
 {% else %}
                 Support DOM_total;
                 Entity NodesOf[{DOM_Phi}, Not {DOM_insulationBoundaryCurvesAir, DOM_insulationBoundaryCurvesTerminal}];
 {% endif %}
 {% else %}
                 Support DOM_total;
                 Entity NodesOf[DOM_Phi];
 {% endif %}
             }
-            // edge basis functions in DOM_allConducting, and not on DOM_pancakeBoundary or DOM_insulationSurface
+            // edge basis functions in DOM_allConducting, and not on DOM_pancakeBoundary or DOM_allInsulationSurface
             {
                 Name BASISFUN_psie;
                 NameOfCoef he;
                 Function BF_Edge;
                 Support DOM_allConducting;
 {% if dm.magnet.geometry.ii.tsa %}
-                Entity EdgesOf[All, Not {DOM_pancakeBoundary, DOM_insulationSurface}];
+                Entity EdgesOf[All, Not {DOM_pancakeBoundary, DOM_allInsulationSurface}];
 {% else %}
                 Entity EdgesOf[All, Not DOM_pancakeBoundary];
 {% endif %}
             }
             // edge-based cohomology basis functions on both cuts
             {
                 Name BASISFUN_sc;
                 NameOfCoef Ii;
                 Function BF_GroupOfEdges;
 {% if dm.magnet.geometry.ii.tsa %}
-                Support Region[{DOM_total, DOM_insulationSurface}];
+                Support Region[{DOM_total, DOM_allInsulationSurface}];
 {% else %}
                 Support DOM_total;
 {% endif %}
                 Entity GroupsOfEdgesOf[DOM_airCuts];
             }
-{% if dm.magnet.geometry.ii.tsa and dm.magnet.solve.ii.resistivity != "perfectlyInsulating" %}
+{% if dm.magnet.geometry.ii.tsa  %}
             <<FUNCTIONSPACE_TSABasisFunctions(type="electromagnetic")|indent(12)>>
             // TSA contribution on boundary of the thin layer
             {
                 Name BASISFUN_gradpsinBnd;
                 NameOfCoef phin_bnd;
                 Function BF_GradNode;
                 Support Region[
                             {
                                 DOM_allConducting,
                                 DOM_Phi,
-                                DOM_insulationSurface
+                                DOM_allInsulationSurface
                             }
                         ];
                 Entity NodesOf[DOM_insulationBoundaryCurvesAir];
             }
             {
                 Name BASISFUN_psieBnd;
-                NameOfCoef phie_bnd;
+                NameOfCoef psie_bnd;
                 Function BF_Edge;
                 Support Region[
                             {
                                 DOM_allConducting,
-                                DOM_insulationSurface
+                                DOM_allInsulationSurface
                             }
                         ];
                 Entity EdgesOf[DOM_insulationBoundaryCurvesTerminal];
             }
+            For i In {1:INPUT_NumOfTSAElements - 1}
+                {
+                    Name BASISFUN_sn~{i};
+                    NameOfCoef he~{i};
+                    Function BF_Edge;
+                    {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %}
+                    Support DOM_terminalContactLayerSurface;
+                    {% else %}
+                    Support DOM_allInsulationSurface;
+                    {% endif %}
+                    Entity EdgesOf[ All, Not {DOM_insulationBoundaryCurvesAir, DOM_insulationBoundaryCurvesTerminal{% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %}, DOM_insulationSurface {% endif %}} ];
+                }
+            EndFor
         }
+
+        {% if dm.magnet.solve.ii.resistivity != "perfectlyInsulating" %}
         SubSpace{
             <<FUNCTIONSPACE_TSASubSpaces(["BASISFUN_sc", "BASISFUN_gradpsinBnd", "BASISFUN_psieBnd"])|indent(12)>>
         }
+        {% else %}
+        SubSpace{
+            <<FUNCTIONSPACE_TSASubSpaces(["BASISFUN_sc", "BASISFUN_gradpsinBnd", "BASISFUN_psieBnd", "BASISFUN_gradpsin"])|indent(12)>>
+        }
+        {% endif %}
 {% else %}
         }
 {% endif %}
         // global quantities in order to impose/extract currents or voltages
         GlobalQuantity{
             {
                 Name GLOBALQUANT_I;
@@ -2141,51 +2542,63 @@
             {% endif %}
             {
                 NameOfCoef phin;
                 EntityType NodesOf;
                 NameOfConstraint CONSTRAINT_zeroPhiAtOuterPoint;
             }
             {% if dm.magnet.geometry.ii.tsa and dm.magnet.solve.ii.resistivity != "perfectlyInsulating" %}
-            {
-                NameOfCoef phin_bnd;
-                EntityType NodesOf;
-                NameOfConstraint CONSTRAINT_zeroPhiAtOuterPoint;
-            }
+            // {
+            //     NameOfCoef phin_bnd;
+            //     EntityType NodesOf;
+            //     NameOfConstraint CONSTRAINT_zeroPhiAtOuterPoint;
+            // }
             {% endif %}
         }
     }
     {
         Name SPACE_temperature;
         Type Form0;
         BasisFunction{
             {
                 Name BASISFUN_sn;
                 NameOfCoef Tn;
                 Function BF_Node;
             {% if dm.magnet.solve.ti.cooling == "cryocooler" %}
-                Support Region[{DOM_allConducting, DOM_bottomTerminalSurface, DOM_topTerminalSurface}];
+                Support Region[{DOM_thermal, DOM_bottomTerminalSurface, DOM_topTerminalSurface}];
             {% else %}
-                Support DOM_allConducting;
+                Support DOM_thermal;
             {% endif %}
 {% if dm.magnet.geometry.ii.tsa %}
-                Entity NodesOf[DOM_allConducting, Not DOM_insulationSurface];
+                Entity NodesOf[DOM_thermal, Not DOM_allInsulationSurface];
 {% else %}
-                Entity NodesOf[DOM_allConducting];
+                Entity NodesOf[DOM_thermal];
 {% endif %}
             }
 {% if dm.magnet.geometry.ii.tsa %}
             <<FUNCTIONSPACE_TSABasisFunctions(type="thermal")|indent(12)>>
 
             {
                 Name BASISFUN_snBndTerminal;
                 NameOfCoef Tn_Bnd;
                 Function BF_Node;
-                Support Region[{DOM_allConducting, DOM_insulationSurface}];
+                Support Region[{DOM_thermal, DOM_allInsulationSurface}];
                 Entity NodesOf[DOM_insulationBoundaryCurvesTerminal];
             }
+
+            For i In {1:INPUT_NumOfTSAElements - 1}
+                {
+                    Name BASISFUN_sn~{i};
+                    NameOfCoef sn~{i};
+                    Function BF_Node;
+                    Support DOM_allInsulationSurface;
+                    Entity NodesOf[ All, Not DOM_insulationBoundaryCurvesTerminal ];
+                }
+            EndFor
+
+            
 {% endif %}
         }
 {% if dm.magnet.geometry.ii.tsa %}
         SubSpace {
             <<FUNCTIONSPACE_TSASubSpaces(["BASISFUN_snBndTerminal"])|indent(12)>>
         }
 {% endif %}
@@ -2203,131 +2616,118 @@
                 NameOfConstraint CONSTRAINT_initialTemperature;
             }
             {
                 NameOfCoef BASISFUN_snPlus_coeff_<<i>>;
                 EntityType NodesOf;
                 NameOfConstraint CONSTRAINT_initialTemperature;
             }
+            For i In {1:INPUT_NumOfTSAElements - 1}
+                {
+                    NameOfCoef sn~{i};
+                    EntityType NodesOf;
+                    NameOfConstraint CONSTRAINT_initialTemperature;
+                }
+            EndFor
     {% endfor %}
     {
         NameOfCoef Tn_Bnd;
         EntityType NodesOf;
         NameOfConstraint CONSTRAINT_initialTemperature;
     }
 {% endif %}
         }
     }
-{% if dm.magnet.geometry.ii.tsa %}
-    <<FUNCTIONSPACE_TSAFunctionSpaces("electromagnetic")|indent(4)>>
-    <<FUNCTIONSPACE_TSAFunctionSpaces("thermal")|indent(4)>>
-{% endif %}
 }
 
 //======================================================================================
 // Formulations: =======================================================================
 //======================================================================================
 Formulation{
 {% if dm.magnet.solve.type == "stronglyCoupled" %}
     {
         Name FORMULATION_<<dm.magnet.solve.type>>;
         Type FemEquation;
         Quantity{
             <<FORMULATION_VolumetricQuantities("electromagnetic")|indent(12)>>
             <<FORMULATION_VolumetricQuantities("thermal")|indent(12)>>
     {% if dm.magnet.geometry.ii.tsa %}
-            {% if dm.magnet.solve.ii.resistivity != "perfectlyInsulating" %}
             <<FORMULATION_TSAQuantities("electromagnetic")|indent(12)>>
-            {% endif %}
             <<FORMULATION_TSAQuantities("thermal")|indent(12)>>
     {% endif %}
         }
 
         Equation{
             <<FORMULATION_VolumetricIntegrals("electromagnetic")|indent(12)>>
             <<FORMULATION_VolumetricIntegrals("thermal")|indent(12)>> 
             <<FORMULATION_VolumetricIntegrals("resistiveHeating")|indent(12)>>
     {% if dm.magnet.geometry.ii.tsa %}
-        {% if dm.magnet.solve.ii.resistivity != "perfectlyInsulating" %}
             <<FORMULATION_TSAIntegrals("electromagnetic")|indent(12)>>
             <<FORMULATION_TSAIntegrals("resistiveHeating")|indent(12)>>
-        {% endif %}
             <<FORMULATION_TSAIntegrals("thermal")|indent(12)>>
     {% endif %}
         }
     }
 {% elif dm.magnet.solve.type == "weaklyCoupled" %}
     {
         Name FORMULATION_electromagnetic;
         Type FemEquation;
         Quantity{
             <<FORMULATION_VolumetricQuantities("thermal")|indent(12)>>
             <<FORMULATION_VolumetricQuantities("electromagnetic")|indent(12)>>
     {% if dm.magnet.geometry.ii.tsa %}
             <<FORMULATION_TSAQuantities("thermal")|indent(12)>>
-        {% if dm.magnet.solve.ii.resistivity != "perfectlyInsulating" %}
             <<FORMULATION_TSAQuantities("electromagnetic")|indent(12)>>
-        {% endif %}
     {% endif %}
         }
 
         Equation{
             <<FORMULATION_VolumetricIntegrals("electromagnetic")|indent(12)>>
     {% if dm.magnet.geometry.ii.tsa %}
-        {% if dm.magnet.solve.ii.resistivity != "perfectlyInsulating" %}
             <<FORMULATION_TSAIntegrals("electromagnetic")|indent(12)>>
-        {% endif %} 
     {% endif %}
         }
     }
 
     {
         Name FORMULATION_thermal;
         Type FemEquation;
         Quantity {
             <<FORMULATION_VolumetricQuantities("thermal")|indent(12)>>
             <<FORMULATION_VolumetricQuantities("electromagnetic")|indent(12)>>
     {% if dm.magnet.geometry.ii.tsa %}
             <<FORMULATION_TSAQuantities("thermal")|indent(12)>>
-        {% if dm.magnet.solve.ii.resistivity != "perfectlyInsulating" %}
             <<FORMULATION_TSAQuantities("electromagnetic")|indent(12)>>
-        {% endif %}
     {% endif %}
         }
         
         Equation{
             <<FORMULATION_VolumetricIntegrals("thermal")|indent(12)>>
             <<FORMULATION_VolumetricIntegrals("resistiveHeating")|indent(12)>>
     {% if dm.magnet.geometry.ii.tsa %}
             <<FORMULATION_TSAIntegrals("thermal")|indent(12)>>
-        {% if dm.magnet.solve.ii.resistivity != "perfectlyInsulating" %}
             <<FORMULATION_TSAIntegrals("resistiveHeating")|indent(12)>>
-        {% endif %}
     {% endif %}
         }
     }
 
 {% elif dm.magnet.solve.type == "electromagnetic" %}
     {
         Name FORMULATION_<<dm.magnet.solve.type>>;
         Type FemEquation;
         Quantity{
             <<FORMULATION_VolumetricQuantities("electromagnetic")|indent(12)>>
     {% if dm.magnet.geometry.ii.tsa %}
-        {% if dm.magnet.solve.ii.resistivity != "perfectlyInsulating" %}
             <<FORMULATION_TSAQuantities("electromagnetic")|indent(12)>>
-        {% endif %}
     {% endif %}
         }
 
         Equation{
             <<FORMULATION_VolumetricIntegrals("electromagnetic")|indent(12)>>
     {% if dm.magnet.geometry.ii.tsa %}
-        {% if dm.magnet.solve.ii.resistivity != "perfectlyInsulating" %}
             <<FORMULATION_TSAIntegrals("electromagnetic")|indent(12)>>
-        {% endif %}
     {% endif %}
         }
     }
 {% elif dm.magnet.solve.type == "thermal" %}
     {
         Name FORMULATION_<<dm.magnet.solve.type>>;
         Type FemEquation;
@@ -2369,15 +2769,14 @@
                 Name SYSTEM_<<dm.magnet.solve.type>>;
                 NameOfFormulation FORMULATION_<<dm.magnet.solve.type>>;
             }
 {% endif %}
         }
 
         Operation{
-            Evaluate[$initializationDone = 0];
 {% if dm.magnet.solve.type == "weaklyCoupled" %}
     {% set systemNames = ["SYSTEM_electromagnetic", "SYSTEM_thermal"] %}
     {% set solveAfterThisTimes = [0, 0]%}
 {% else %}
     {% set systemNames = ["SYSTEM_"+dm.magnet.solve.type] %}
     {% set solveAfterThisTimes = [0]%}
 {% endif %}
@@ -2454,92 +2853,81 @@
                         [rho[<<rhoArguments>>]];
                         In Region[{ DOM_allConducting }];
                         Jacobian JAC_vol;
                     }
                 }
             }
 
-    {% if dm.magnet.solve.wi.resistivity is none %}
-            {
-                Name RESULT_derivativeOfRhoWithRespectToJ; // current density magnitude
-                Value{
-                    Local{
-                        // [d_of_lambda_wrt_jFD[<<rhoArguments>>]];
-                        // [d_of_lambda_wrt_j[<<rhoArguments>>]];
-
-                        // [rhoParallelToWindingDerivativeFD[<<rhoArguments>>]];
-                        // [rhoParallelToWindingDerivative[<<rhoArguments>>]];
-
-                        // [rhoNormalToWindingDerivativeFD[<<rhoArguments>>]];
-                        [rhoNormalToWindingDerivative[<<rhoArguments>>]];
-
-                        // [d_of_jHTS_wrt_jFD[<<rhoArguments>>]];
-                        // [d_of_jHTS_wrt_j[<<rhoArguments>>]];
-
-                        In Region[{ DOM_allConducting }];
-                        Jacobian JAC_vol;
-                    }
-                }
-            }
-
-    {% endif %}
     {% if dm.magnet.solve.wi.superConductor and not dm.magnet.solve.wi.resistivity and type != "thermal" %}
-            {
-                Name RESULT_criticalCurrentDensity; // critical current density of the winding
-                Value{
-                    Local{
-                        [Jcritical[<<JcriticalArguments>>]];
-                        In Region[{ DOM_allWindings }];
-                        Jacobian JAC_vol;
-                    }
-                }
-            }
-
-            {
-                Name RESULT_jHTSOverjCritical;
-                Value{
-                    Local{
-                        [(TransformationTensor[]*jHTS[<<JcriticalArguments>>])/Jcritical[<<JcriticalArguments>>]];
-                        In Region[{ DOM_allWindings }];
-                        Jacobian JAC_vol;
-                    }
-                }
-            }
+            // {
+            //     Name RESULT_criticalCurrentDensity; // critical current density of the winding
+            //     Value{
+            //         Local{
+            //             [Jcritical[<<JcriticalArguments>>]];
+            //             In Region[{ DOM_allWindings }];
+            //             Jacobian JAC_vol;
+            //         }
+            //     }
+            // }
+
+            // {
+            //     Name RESULT_jHTSOverjCritical;
+            //     Value{
+            //         Local{
+            //             [(TransformationTensor[]*jHTS[<<JcriticalArguments>>])/Jcritical[<<JcriticalArguments>>]];
+            //             In Region[{ DOM_allWindings }];
+            //             Jacobian JAC_vol;
+            //         }
+            //     }
+            // }
+
+            // {
+            //     Name RESULT_criticalCurrent;
+            //     Value{
+            //         Local{
+            //             [Jcritical[<<JcriticalArguments>>] * INPUT_relativeThicknessOfSuperConductor * 1/<<scalingFactor>> * <<dm.magnet.geometry.wi.t>> * <<dm.magnet.geometry.wi.h>>];
+            //             In Region[{ DOM_allWindings }];
+            //             Jacobian JAC_vol;
+            //         }
+            //     }
+            // }
+    {% endif %}
 
             {
-                Name RESULT_criticalCurrent;
+                Name RESULT_magneticEnergy;
                 Value{
-                    Local{
-                        [Jcritical[<<JcriticalArguments>>] * INPUT_relativeThicknessOfSuperConductor * 1/<<scalingFactor>> * <<dm.magnet.geometry.wi.t>> * <<dm.magnet.geometry.wi.h>>];
-                        In Region[{ DOM_allWindings }];
+                    Integral{
+                        Type Global;
+                        [1/2 * mu[] * {LOCALQUANT_h} * {LOCALQUANT_h}];
+                        In DOM_total;
                         Jacobian JAC_vol;
+                        Integration Int;
                     }
                 }
             }
-    {% endif %}
 
             {
-                Name RESULT_magneticEnergy;
+                Name RESULT_inductance;
                 Value{
                     Integral{
                         Type Global;
-                        [1/2 * mu[] * {LOCALQUANT_h} * {LOCALQUANT_h}];
+                        [mu[] * {LOCALQUANT_h} * {LOCALQUANT_h}];
                         In DOM_total;
                         Jacobian JAC_vol;
                         Integration Int;
                     }
                 }
             }
 
             {
                 Name RESULT_resistiveHeating; // resistive heating
                 Value{
                     Local{
                         [(rho[<<rhoArguments>>] * {d LOCALQUANT_h}) * {d LOCALQUANT_h}];
-                        In Region[{ DOM_allConducting }];
+                        In Region[{ DOM_resistiveHeating }];
                         Jacobian JAC_vol;
                     }
                 }
             }
 
             {
                 Name RESULT_voltageBetweenTerminals; // voltages in cuts
@@ -2574,114 +2962,169 @@
 
             {
                 Name RESULT_totalResistiveHeating; // total resistive heating for convergence
                 Value{
                     Integral{
                         Type Global;
                         [(rho[<<rhoArguments>>] * {d LOCALQUANT_h}) * {d LOCALQUANT_h}];
-                        In DOM_allConducting;
+                        In DOM_resistiveHeating;
                         Jacobian JAC_vol;
                         Integration Int;
                     }
+
+                    {% if dm.magnet.solve.type in ["weaklyCoupled", "stronglyCoupled", "thermal"] %}
+                        {% set temperatureArgument1 = "{LOCALQUANT_TThinShell~{i}}" %}
+                        {% set temperatureArgument2 = "{LOCALQUANT_TThinShell~{i+1}}" %}
+                    {% elif dm.magnet.solve.type == "electromagnetic" %}
+                        {% set temperatureArgument1 = "INPUT_initialTemperature" %}
+                        {% set temperatureArgument2 = "INPUT_initialTemperature" %}
+                    {% endif %}
+                    {% if dm.magnet.geometry.ii.tsa %}
+                        For i In {0:INPUT_NumOfTSAElements-1}
+                            Integral {
+                                Type Global;
+                                [
+                                    electromagneticOnlyFunction[
+                                        <<temperatureArgument1>>,
+                                        <<temperatureArgument2>>
+                                    ] * SquNorm[
+                                        ({LOCALQUANT_hThinShell~{i + 1}} - {LOCALQUANT_hThinShell~{i}})/th_ins_k
+                                    ]
+                                ];
+                                {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %}
+                                In DOM_terminalContactLayerSurface;
+                                {% else %}
+                                In DOM_allInsulationSurface;
+                                {% endif %}
+                                Integration Int;
+                                Jacobian JAC_sur;
+                            } 
+                        
+                                {% for a in range(1,3) %}
+                                    {% for b in range(1,3) %}
+                            Integral {
+                                Type Global;
+                                [
+                                    electromagneticMassFunctionNoDta<<a>>b<<b>>[
+                                        <<temperatureArgument1>>,
+                                        <<temperatureArgument2>>
+                                    ] * {d LOCALQUANT_hThinShell~{i + <<a>> - 1}} * {d LOCALQUANT_hThinShell~{i + <<b>> - 1}}
+                                ];
+                                {% if dm.magnet.solve.ii.resistivity == "perfectlyInsulating" %}
+                                In DOM_terminalContactLayerSurface;
+                                {% else %}
+                                In DOM_allInsulationSurface;
+                                {% endif %}
+                                Integration Int;
+                                Jacobian JAC_sur;
+                            }
+                                    {% endfor %}
+                                {% endfor %}
+                        EndFor
+                    {% endif %} 
                 }
             }
 {% endif %}
 {% if dm.magnet.solve.type in ["weaklyCoupled", "stronglyCoupled", "thermal"]  %}
             {
                 Name RESULT_temperature;
                 Value {
                     Local{
                         [{LOCALQUANT_T}];
-                        In DOM_allConducting;
+                        In DOM_thermal;
                         Jacobian JAC_vol;
                     }
                 }
             }
 
             {
                 Name RESULT_heatFlux;
                 Value {
                     Local{
                         [-kappa[<<kappaArguments>>] * {d LOCALQUANT_T}];
-                        In DOM_allConducting;
+                        In DOM_thermal;
                         Jacobian JAC_vol;
                     }
                 }
             }
 
             {
                 Name RESULT_magnitudeOfHeatFlux;
                 Value {
                     Local{
                         [Norm[-kappa[<<kappaArguments>>] * {d LOCALQUANT_T}]];
-                        In DOM_allConducting;
+                        In DOM_thermal;
                         Jacobian JAC_vol;
                     }
                 }
             }
 
             {
                 Name RESULT_thermalConductivity; // current density magnitude
                 Value{
                     Local{
                         [kappa[<<kappaArguments>>]];
-                        In Region[{ DOM_allConducting }];
+                        In Region[{ DOM_thermal }];
                         Jacobian JAC_vol;
                     }
                 }
             }
 
             {
                 Name RESULT_specificHeatCapacity; // current density magnitude
                 Value{
                     Local{
                         [Cv[<<CvArguments>>]];
-                        In Region[{ DOM_allConducting }];
+                        In Region[{ DOM_thermal }];
                         Jacobian JAC_vol;
                     }
                 }
             }
 {% endif %}
-            {
+{% if dm.magnet.geometry.ii.tsa %} {
                 Name RESULT_debug;
                 Value{
                     Local{
-                        [ TransformationTensor[] ];
-                        In Region[{ DOM_allWindings }];
-                        Jacobian JAC_vol;
+                        [ 
+                           Normal[] /\ ({LOCALQUANT_hThinShell~{1}} - {LOCALQUANT_hThinShell~{0}})/th_ins_k + {d LOCALQUANT_hThinShell~{0}}
+                         ];
+                        In DOM_allInsulationSurface;
+                        Jacobian JAC_sur;
                     }
                 }
             }
+{% endif %}
         }
     }
 }
 
 //======================================================================================
 // Post-operation: =====================================================================
 //======================================================================================
 PostOperation{
     {
         Name POSTOP_dummy;
         NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
         Operation {
         }
     }
-    {
+    {% if dm.magnet.geometry.ii.tsa %} {
         Name POSTOP_debug;
         NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
         Operation{
             // 3D magnetic field vector field:
             <<POSTOPERATION_printResults(
                 quantity="RESULT_debug",
-                onElementsOf="DOM_allWindings",
+                onElementsOf="DOM_allInsulationSurface",
                 name="Debug Variable",
                 fileName="debug"
             )|indent(12)>>
         }
     }
+    {% endif %}
 {% if dm.magnet.solve.type in ["electromagnetic", "weaklyCoupled", "stronglyCoupled"] %}
     {
         Name POSTOP_magneticField;
         NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
         Operation{
             // 3D magnetic field vector field:
             <<POSTOPERATION_printResults(
@@ -2753,66 +3196,95 @@
                 quantity="RESULT_resistivity",
                 onElementsOf="DOM_allConducting",
                 name="Resistivity [Ohm*m]",
                 fileName="Resistivity"
             )|indent(12)>>
         }
     }
-    {% if dm.magnet.solve.wi.superConductor and not dm.magnet.solve.wi.resistivity %}
     {
-        Name POSTOP_criticalCurrentDensity;
+        Name POSTOP_inductance;
         NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
         Operation{
             // Current at the cut:
             <<POSTOPERATION_printResults(
-                quantity="RESULT_criticalCurrentDensity",
-                onElementsOf="DOM_allWindings",
-                name="Critical Current Density [A/m^2]",
-                fileName="CriticalCurrentDensity"
-            )|indent(12)>>
-        }
-    }
-    {
-        Name POSTOP_jHTSOverjCritical;
-        NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
-        Operation{
-            // Current at the cut:
-            <<POSTOPERATION_printResults(
-                quantity="RESULT_jHTSOverjCritical",
-                onElementsOf="DOM_allWindings",
-                name="(HTS Current Density)/(Critical Current Density)",
-                fileName="HTSCurrentDensityOverCriticalCurrentDensity"
+                quantity="RESULT_inductance",
+                onGlobal=True,
+                format="TimeTable",
+                name="Inductance [H]",
+                fileName="Inductance",
+                lastTimeStepOnly=True
             )|indent(12)>>
         }
     }
     {
-        Name POSTOP_criticalCurrent;
+        Name POSTOP_timeConstant;
         NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
         Operation{
             // Current at the cut:
             <<POSTOPERATION_printResults(
-                quantity="RESULT_criticalCurrent",
-                onElementsOf="DOM_allWindings",
-                name="Critical Current [A]",
-                fileName="CriticalCurrent"
+                quantity="RESULT_axialComponentOfTheMagneticField",
+                onPoint=[0, 0, 0],
+                name="The Magnitude of the Magnetic Field [T]",
+                fileName="axialComponentOfTheMagneticFieldForTimeConstant",
+                format="TimeTable"
             )|indent(12)>>
         }
     }
-    {
-        Name POSTOP_Ic;
-        NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
-        LastTimeStepOnly 1;
-        Operation {
-            Print[
-                RESULT_criticalCurrent,
-                OnElementsOf DOM_allWindings,
-                StoreMinInRegister 1
-            ];
-        }
-    }
+    {% if dm.magnet.solve.wi.superConductor and not dm.magnet.solve.wi.resistivity %}
+    // {
+    //     Name POSTOP_criticalCurrentDensity;
+    //     NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
+    //     Operation{
+    //         // Current at the cut:
+    //         {# POSTOPERATION_printResults(
+    //             quantity="RESULT_criticalCurrentDensity",
+    //             onElementsOf="DOM_allWindings",
+    //             name="Critical Current Density [A/m^2]",
+    //             fileName="CriticalCurrentDensity"
+    //         )|indent(12) #}
+    //     }
+    // }
+    // {
+    //     Name POSTOP_jHTSOverjCritical;
+    //     NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
+    //     Operation{
+    //         // Current at the cut:
+    //         {# POSTOPERATION_printResults(
+    //             quantity="RESULT_jHTSOverjCritical",
+    //             onElementsOf="DOM_allWindings",
+    //             name="(HTS Current Density)/(Critical Current Density)",
+    //             fileName="HTSCurrentDensityOverCriticalCurrentDensity"
+    //         )|indent(12) #}
+    //     }
+    // }
+    // {
+    //     Name POSTOP_criticalCurrent;
+    //     NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
+    //     Operation{
+    //         // Current at the cut:
+    //         {# POSTOPERATION_printResults(
+    //             quantity="RESULT_criticalCurrent",
+    //             onElementsOf="DOM_allWindings",
+    //             name="Critical Current [A]",
+    //             fileName="CriticalCurrent"
+    //         )|indent(12) #}
+    //     }
+    // }
+    // {
+    //     Name POSTOP_Ic;
+    //     NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
+    //     LastTimeStepOnly 1;
+    //     Operation {
+    //         Print[
+    //             RESULT_criticalCurrent,
+    //             OnElementsOf DOM_allWindings,
+    //             StoreMinInRegister 1
+    //         ];
+    //     }
+    // }
     {
         Name POSTOP_I;
         NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
         LastTimeStepOnly 1;
         Operation {
             Print[
                 RESULT_currentThroughCoil,
@@ -2855,54 +3327,54 @@
     {
         Name POSTOP_temperature;
         NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
         Operation {
             // 3D temperature scalar field:
             <<POSTOPERATION_printResults(
                 quantity="RESULT_temperature",
-                onElementsOf="DOM_allConducting",
+                onElementsOf="DOM_thermal",
                 name="Temperature [K]",
                 fileName="Temperature"
             )|indent(12)>>
         }
     }
     {
         Name POSTOP_heatFlux;
         NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
         Operation {
             // 3D temperature scalar field:
             <<POSTOPERATION_printResults(
                 quantity="RESULT_heatFlux",
-                onElementsOf="DOM_allConducting",
+                onElementsOf="DOM_thermal",
                 name="Heat Flux [W/m^2]",
                 fileName="HeatFlux"
             )|indent(12)>>
         }
     }
     {
         Name POSTOP_thermalConductivity;
         NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
         Operation{
             // Resistive heating:
             <<POSTOPERATION_printResults(
                 quantity="RESULT_thermalConductivity",
-                onElementsOf="DOM_allConducting",
+                onElementsOf="DOM_thermal",
                 name="Thermal Conductivity [W/(m*K)]",
                 fileName="thermalConductivity"
             )|indent(12)>>
         }
     }
     {
         Name POSTOP_specificHeatCapacity;
         NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
         Operation{
             // Resistive heating:
             <<POSTOPERATION_printResults(
                 quantity="RESULT_specificHeatCapacity",
-                onElementsOf="DOM_allConducting",
+                onElementsOf="DOM_thermal",
                 name="Specific Heat Capacity [J/(kg*K)]",
                 fileName="specificHeatCapacity"
             )|indent(12)>>
         }
     }
 {% endif %}
 {% if dm.magnet.postproc.timeSeriesPlots is not none %}
@@ -2969,15 +3441,15 @@
 {% for tolerance in (dm.magnet.solve.nls.postOperationTolerances + dm.magnet.solve.t.adaptive.postOperationTolerances)|unique(attribute="quantity") %}
     {% if tolerance.quantity == "totalResistiveHeating" %}
     {
         Name POSTOP_CONV_totalResistiveHeating;
         NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
         LastTimeStepOnly 1;
         Operation {
-            Print[RESULT_totalResistiveHeating, OnElementsOf DOM_allConducting];
+            Print[RESULT_totalResistiveHeating, OnGlobal];
         }
     }
     {% elif tolerance.quantity in ["voltageBetweenTerminals", "currentThroughCoil"] %}
     {
         Name POSTOP_CONV_<<tolerance.quantity>>;
         NameOfPostProcessing POSTPRO_<<dm.magnet.solve.type>>;
         LastTimeStepOnly 1;
```

### Comparing `fiqus-2024.1.1/fiqus/pro_templates/combined/materials.pro` & `fiqus-2024.4.0/fiqus/pro_templates/combined/materials.pro`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus/utils/Utils.py` & `fiqus-2024.4.0/fiqus/utils/Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 
 class FilesAndFolders:
     @staticmethod
     def read_data_from_yaml(full_file_path, data_class):
         with open(full_file_path, 'r') as stream:
             yaml = ruamel.yaml.YAML(typ='safe', pure=True)
             yaml_str = yaml.load(stream)
+            if "magnet" in yaml_str:
+                yaml_str["magnet"]["input_file_path"] = str(full_file_path)
+                
         return data_class(**yaml_str)
 
     @staticmethod
     def write_data_to_yaml(full_file_path, dict_of_data_class):
         def my_represent_none(self, data):
             return self.represent_scalar('tag:yaml.org,2002:null', 'null')
```

### Comparing `fiqus-2024.1.1/fiqus.egg-info/SOURCES.txt` & `fiqus-2024.4.0/fiqus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/fiqus.egg-info/requires.txt` & `fiqus-2024.4.0/fiqus.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 gmsh==4.11.1
-matplotlib==3.6.0
-Jinja2==3.1.2
-numpy==1.23.3
-pandas==1.5.0
-pydantic==1.10.8
-ruamel.yaml==0.17.21
-scipy==1.10.1
-typing_extensions==4.5.0
+matplotlib==3.8.3
+Jinja2==3.1.3
+numpy==1.26.4
+pandas==2.2.1
+pydantic==2.6.4
+ruamel.yaml==0.18.6
+scipy==1.12.0
+typing_extensions==4.10.0
 
 [all]
 gmsh==4.11.1
-matplotlib==3.6.0
-Jinja2==3.1.2
-numpy==1.23.3
-pandas==1.5.0
-pydantic==1.10.8
-ruamel.yaml==0.17.21
-scipy==1.10.1
-typing_extensions==4.5.0
+matplotlib==3.8.3
+Jinja2==3.1.3
+numpy==1.26.4
+pandas==2.2.1
+pydantic==2.6.4
+ruamel.yaml==0.18.6
+scipy==1.12.0
+typing_extensions==4.10.0
 markdown==3.3.7
 markdown-include==0.7.0
 mkdocs==1.3.1
 mkdocs-material==8.5.3
 mkdocstrings-python==0.7.1
 mkdocs-include-markdown-plugin==3.8.1
 mkdocs-git-revision-date-localized-plugin==1.1.0
```

### Comparing `fiqus-2024.1.1/setup.py` & `fiqus-2024.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,39 +24,39 @@
     "pytest-cov==3.0.0",
     "coverage==6.4.4",
     "coverage-badge==1.1.0",
     "flake8==5.0.4",
 ]
 
 build_require = [
-    "setuptools==65.3.0",
+    "setuptools==65.3.0"
 ]
 
 all_requirements = required + docs_require + tests_require + build_require
 
 setup(
     name="fiqus",
-    version="2024.1.1",
+    version="2024.4.0",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for STEAM FiQuS tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.cern.ch/steam/fiqus",
     keywords=["STEAM", "FiQuS", "CERN"],
     install_requires=required,
     extras_require={
         "all": all_requirements,
         "docs": docs_require,
         "tests": tests_require,
         "build": build_require,
     },
-    python_requires=">=3.8",
+    python_requires=">=3.11",
     packages=find_packages(),
     package_data={
         "fiqus": [
             "**/*.pro",
         ]
     },
     include_package_data=True,
-    classifiers=["Programming Language :: Python :: 3.8"],
+    classifiers=["Programming Language :: Python :: 3.11"],
 )
```

### Comparing `fiqus-2024.1.1/tests/test_FiQuS.py` & `fiqus-2024.4.0/tests/test_FiQuS.py`

 * *Files identical despite different names*

### Comparing `fiqus-2024.1.1/tests/test_mesh_generators.py` & `fiqus-2024.4.0/tests/test_geometry_generators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 import unittest
-from tests.utils.fiqus_test_classes import FiQuSMeshTests
+from tests.utils.fiqus_test_classes import FiQuSGeometryTests
 
-class TestMeshGenerators(FiQuSMeshTests):
+
+class TestGeometryGenerators(FiQuSGeometryTests):
     def test_Pancake3D(self):
         """
         Checks if Pancake3D geometry generators work correctly by comparing the number
         of entities in the generated geometry file to the reference file that was
         checked manually.
         """
         model_names = [
             "TEST_Pancake3D_REF",
             "TEST_Pancake3D_REFStructured",
             "TEST_Pancake3D_TSA",
             "TEST_Pancake3D_TSAStructured",
+            "TEST_Pancake3D_TSAInsulating"
         ]
 
         for model_name in model_names:
             with self.subTest(model_name=model_name):
                 data_model = self.get_data_model(model_name)
 
                 # data_model can be modified here if necessary
                 # Example:
 
-                # data_model.magnet.mesh.wi.axne = 30
+                # data_model.magnet.geometry.N = 3
 
-                self.generate_mesh(data_model, model_name)
+                self.generate_geometry(data_model, model_name)
 
                 # Compare the number of entities with the reference file:
-                mesh_file = self.get_path_to_generated_file(file_name=model_name, file_extension="msh")
-                reference_file = self.get_path_to_reference_file(model_name, "msh")
-                self.compare_mesh_qualities(mesh_file, reference_file)
-
-                # Compare the regions files:
-                regions_file = self.get_path_to_generated_file(file_name=model_name, file_extension="regions")
-                reference_regions_file = self.get_path_to_reference_file(
-                    model_name, "regions"
+                geometry_file = self.get_path_to_generated_file(
+                    data_model=data_model, file_name=model_name, file_extension="brep"
+                )
+                reference_file = self.get_path_to_reference_file(
+                    data_model=data_model, file_name=model_name, file_extension="brep"
                 )
-                self.compare_json_or_yaml_files(regions_file, reference_regions_file)
+                self.compare_number_of_entities(geometry_file, reference_file)
 
+                # Compare the volume information files:
+                vi_file = self.get_path_to_generated_file(
+                    data_model=data_model, file_name=model_name, file_extension="vi"
+                )
+                reference_vi_file = self.get_path_to_reference_file(
+                    data_model=data_model, file_name=model_name, file_extension="vi"
+                )
+                self.compare_json_or_yaml_files(vi_file, reference_vi_file)
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `fiqus-2024.1.1/tests/test_solvers.py` & `fiqus-2024.4.0/tests/test_mesh_generators.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 import unittest
-from tests.utils.fiqus_test_classes import FiQuSSolverTests
-from fiqus.data.DataFiQuS import FDM
+from tests.utils.fiqus_test_classes import FiQuSMeshTests
 
-
-class TestSolvers(FiQuSSolverTests):
+class TestMeshGenerators(FiQuSMeshTests):
     def test_Pancake3D(self):
         """
-        Checks if Pancake3D solvers work correctly by comparing the results to the
-        reference results that were checked manually.
+        Checks if Pancake3D geometry generators work correctly by comparing the number
+        of entities in the generated geometry file to the reference file that was
+        checked manually.
         """
-        with self.subTest(msg="tsa linear weakly coupled"):
-            model_name = "TEST_Pancake3D_TSA"
-            data_model: FDM = self.get_data_model(model_name)
-
-            data_model.magnet.solve.type = "weaklyCoupled"
-
-            self.solve(data_model, model_name)
-
-            # Compare the pro files:
-            pro_file = self.get_path_to_generated_file(
-                file_name=model_name, file_extension="pro"
-            )
-            reference_pro_file = self.get_path_to_reference_file(
-                file_name=model_name, file_extension="pro"
-            )
-            self.compare_text_files(pro_file, reference_pro_file)
-
-            # Compare the results files:
-            pos_file = self.get_path_to_generated_file(file_name="Temperature-DefaultFormat", file_extension="pos")
-            reference_pos_file = self.get_path_to_reference_file(file_name="Temperature-DefaultFormat", file_extension="pos")
-            self.compare_pos_files(pos_file, reference_pos_file)
-
-        with self.subTest(msg="tsa linear strongly coupled"):
-            model_name = "TEST_Pancake3D_TSA"
-            data_model = self.get_data_model(model_name)
-
-            data_model.magnet.solve.type = "stronglyCoupled"
-            data_model.magnet.solve.ti.cooling = "fixedTemperature"
-
-            self.solve(data_model, model_name)
-
-        with self.subTest(msg="tsa linear electromagnetic"):
-            model_name = "TEST_Pancake3D_TSA"
-            data_model = self.get_data_model(model_name)
-
-            data_model.magnet.solve.type = "electromagnetic"
-            del data_model.magnet.solve.t.adaptive.postOperationTolerances[1]
-
-            self.solve(data_model, model_name)
+        model_names = [
+            "TEST_Pancake3D_REF",
+            "TEST_Pancake3D_REFStructured",
+            "TEST_Pancake3D_TSA",
+            "TEST_Pancake3D_TSAStructured",
+            "TEST_Pancake3D_TSAInsulating"
+        ]
+
+        for model_name in model_names:
+            with self.subTest(model_name=model_name):
+                data_model = self.get_data_model(model_name)
+
+                # data_model can be modified here if necessary
+                # Example:
+
+                # data_model.magnet.mesh.wi.axne = 30
+
+                self.generate_mesh(data_model, model_name)
+
+                # Compare the number of entities with the reference file:
+                mesh_file = self.get_path_to_generated_file(
+                    data_model=data_model, file_name=model_name, file_extension="msh"
+                )
+                reference_file = self.get_path_to_reference_file(
+                    data_model=data_model, file_name=model_name, file_extension="msh"
+                )
+                self.compare_mesh_qualities(mesh_file, reference_file)
+
+                # Compare the regions files:
+                regions_file = self.get_path_to_generated_file(
+                    data_model=data_model,
+                    file_name=model_name,
+                    file_extension="regions",
+                )
+                reference_regions_file = self.get_path_to_reference_file(
+                    data_model=data_model,
+                    file_name=model_name,
+                    file_extension="regions",
+                )
+                self.compare_json_or_yaml_files(regions_file, reference_regions_file)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `fiqus-2024.1.1/tests/utils/fiqus_test_classes.py` & `fiqus-2024.4.0/tests/utils/fiqus_test_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
 import os
+import filecmp
 import gmsh
 import logging
 import shutil
 from typing import Union, Tuple, Literal
 import ruamel.yaml
 import numpy as np
 
@@ -116,35 +117,38 @@
         """
         # Make sure the run type is correct:
         data_model.run.type = run_type
 
         # Make sure the output files are overwritten:
         data_model.run.overwrite = True
 
+        # Disable GUI:
+        data_model.run.launch_gui = False
+
         # Prepare the output folder:
         model_folder = os.path.join(self.outputs_folder, f"{model_name}_{run_type}")
         FFs.prep_folder(model_folder)
 
         # Depending on the run_type, copy the reference files to the model folder:
         if run_type in ["geometry_only", "geometry_and_mesh", "start_from_yaml"]:
             pass
         else:
             # Copy the reference geometry and mesh folders to the model folder:
             reference_geometry_folder = self.get_path_to_specific_reference_folder(
-                model_name, folder="Geometry"
+                data_model, model_name, folder="Geometry"
             )
             reference_mesh_folder = self.get_path_to_specific_reference_folder(
-                model_name, folder="Mesh"
+                data_model, model_name, folder="Mesh"
             )
 
             output_geometry_folder = self.get_path_to_specific_output_folder(
-                model_name, run_type=run_type, folder="Geometry"
+                data_model, model_name, run_type=run_type, folder="Geometry"
             )
             output_mesh_folder = self.get_path_to_specific_output_folder(
-                model_name, run_type=run_type, folder="Mesh"
+                data_model, model_name, run_type=run_type, folder="Mesh"
             )
 
             shutil.copytree(
                 reference_geometry_folder, output_geometry_folder, dirs_exist_ok=True
             )
             shutil.copytree(
                 reference_mesh_folder, output_mesh_folder, dirs_exist_ok=True
@@ -156,14 +160,15 @@
             input_file_path=self.get_input_file_path(model_name),
             fdm=data_model,
             verbose=False,
         )
 
     def get_path_to_generated_file(
         self,
+        data_model: FDM,
         model_name: str,
         file_name: str,
         file_extension: str,
         run_type: Literal[
             "start_from_yaml",
             "mesh_only",
             "geometry_only",
@@ -175,15 +180,15 @@
             "post_process_getdp_only",
             "post_process_python_only",
         ],
     ) -> Union[str, os.PathLike]:
         """
         This method returns the path to the generated file with the given extension
         for the given model name depending on the run type.
-        
+
         :param model_name: name of the model to get the generated file for
         :type model_name: str
         :param file_name: name of the file
         :type file_name: str
         :param file_extension: file extension of the generated file
         :type file_extension: str
         :param run_type: run type to run FiQuS with
@@ -210,15 +215,15 @@
             folder = "Solution"
         else:
             raise ValueError(
                 "The run type must be geometry_only, mesh_only, or solve_only!"
             )
 
         sections_folder = self.get_path_to_specific_output_folder(
-            model_name, run_type, folder
+            data_model, model_name, run_type, folder
         )
 
         generated_file = os.path.join(
             sections_folder,
             f"{file_name}.{file_extension}",
         )
 
@@ -228,14 +233,15 @@
                 f"Could not find the generated file: {generated_file}!"
             )
 
         return generated_file
 
     def get_path_to_specific_reference_folder(
         self,
+        data_model: FDM,
         model_name: str,
         folder: Literal[
             "Geometry",
             "Mesh",
             "Solution",
         ],
     ):
@@ -248,15 +254,15 @@
         :param folder: folder to get the reference folder for
         :type folder: Literal[
                 "Geometry",
                 "Mesh",
                 "Solution",
             ]
         """
-        fdm = self.get_data_model(model_name)
+        fdm = data_model
         geometry_folder_name = f"Geometry_{fdm.run.geometry}"
         mesh_folder_name = f"Mesh_{fdm.run.mesh}"
         solve_folder_name = f"Solution_{fdm.run.solution}"
 
         if folder == "Geometry":
             reference_folder = os.path.join(
                 self.references_folder, model_name, geometry_folder_name
@@ -277,14 +283,15 @@
                 solve_folder_name,
             )
 
         return reference_folder
 
     def get_path_to_specific_output_folder(
         self,
+        data_model: FDM,
         model_name: str,
         run_type: Literal[
             "start_from_yaml",
             "mesh_only",
             "geometry_only",
             "geometry_and_mesh",
             "pre_process_only",
@@ -322,15 +329,15 @@
         :param folder: folder to get the output folder for
         :type folder: Literal[
                 "Geometry",
                 "Mesh",
                 "Solution",
             ]
         """
-        fdm = self.get_data_model(model_name)
+        fdm = data_model
         geometry_folder_name = f"Geometry_{fdm.run.geometry}"
         mesh_folder_name = f"Mesh_{fdm.run.mesh}"
         solve_folder_name = f"Solution_{fdm.run.solution}"
 
         if run_type is None:
             model_folder_name = model_name
         else:
@@ -358,27 +365,28 @@
 
         FFs.prep_folder(output_folder)
 
         return output_folder
 
     def get_path_to_reference_file(
         self,
+        data_model: FDM,
         model_name: str,
         file_name: str,
         file_extension: str,
         folder: Literal[
             "Geometry",
             "Mesh",
             "Solution",
         ],
     ) -> Union[str, os.PathLike]:
         """
         This method returns the path to the reference file with the given extension
         for the given model name from the given folder.
-        
+
         :param model_name: name of the model to get the reference file for
         :type model_name: str
         :param file_name: name of the model to get the reference file for
         :type file_name: str
         :param file_extension: file extension of the reference file
         :type file_extension: str
         :param folder: folder to get the reference file from
@@ -387,15 +395,15 @@
                 "Mesh",
                 "Solution",
             ]
         :return: path to the reference file
         :rtype: Union[str, os.PathLike]
         """
         reference_folder = self.get_path_to_specific_reference_folder(
-            model_name, folder=folder
+            data_model, model_name, folder=folder
         )
         reference_file = os.path.join(
             reference_folder,
             f"{file_name}.{file_extension}",
         )
 
         # Check if the file exists:
@@ -427,39 +435,47 @@
         except:
             raise ValueError("The files must be JSON or YAML files!")
 
         # Compare the dictionaries:
         self.assertDictEqual(
             file_1_dictionary,
             file_2_dictionary,
-            msg=f"{os.path.basename(file_1)} did not match {os.path.basename(file_2)}!",
+            msg=f"{file_1} did not match {file_2}!",
         )
 
-    def compare_text_files(self, file_1, file_2):
+    def compare_pkl_files(self, file_1, file_2):
         """
-        This method compares the contents of two text files. It is used to check that
-        the generated files are the same as the reference.
+        This method compares the contents of two pkl files. It is used to check that the
+        generated files are the same as the reference.
 
         :param file_1: path to the first file
         :type file_1: Union[str, os.PathLike]
         :param file_2: path to the second file
         :type file_2: Union[str, os.PathLike]
         """
-        # Open the files and get the contents:
-        with open(file_1, "r") as file:
-            file_1_contents = file.read()
+        # Compare the pickle files:
+        self.assertTrue(
+            filecmp.cmp(file_1, file_2),
+            msg=f"{file_1} did not match {file_2}!",
+        )
 
-        with open(file_2, "r") as file:
-            file_2_contents = file.read()
+    def compare_text_files(self, file_1, file_2):
+        """
+        This method compares the contents of two files. It is used to check that the
+        generated files are the same as the reference.
 
-        # Compare the contents:
-        self.assertEqual(
-            file_1_contents,
-            file_2_contents,
-            msg=f"{os.path.basename(file_1)} did not match {os.path.basename(file_2)}!",
+        :param file_1: path to the first file
+        :type file_1: Union[str, os.PathLike]
+        :param file_2: path to the second file
+        :type file_2: Union[str, os.PathLike]
+        """
+        # Compare the files:
+        self.assertTrue(
+            filecmp.cmp(file_1, file_2),
+            msg=f"{file_1} did not match {file_2}!",
         )
 
 
 class FiQuSGeometryTests(BaseClassesForTests):
     def generate_geometry(
         self,
         data_model: FDM,
@@ -514,25 +530,29 @@
             self.assertEqual(
                 len(model_entities[geometry_file_1][dim]),
                 len(model_entities[geometry_file_2][dim]),
                 msg=f"{geometry_file_1} and {geometry_file_2} did not match!",
             )
 
     def get_path_to_generated_file(
-        self, file_name: str, file_extension: str
+        self, data_model: FDM, file_name: str, file_extension: str
     ) -> Union[str, os.PathLike]:
         return super().get_path_to_generated_file(
-            self.model_name, file_name, file_extension, run_type="geometry_only"
+            data_model,
+            self.model_name,
+            file_name,
+            file_extension,
+            run_type="geometry_only",
         )
 
     def get_path_to_reference_file(
-        self, file_name: str, file_extension: str
+        self, data_model: FDM, file_name: str, file_extension: str
     ) -> Union[str, os.PathLike]:
         return super().get_path_to_reference_file(
-            self.model_name, file_name, file_extension, folder="Geometry"
+            data_model, self.model_name, file_name, file_extension, folder="Geometry"
         )
 
 
 class FiQuSMeshTests(BaseClassesForTests):
     def generate_mesh(
         self,
         data_model: FDM,
@@ -577,25 +597,25 @@
         self.assertGreater(
             ratio,
             0.9,
             msg=f"{mesh_file_1} and {mesh_file_2} did not match!",
         )
 
     def get_path_to_generated_file(
-        self, file_name: str, file_extension: str
+        self, data_model, file_name: str, file_extension: str
     ) -> Union[str, os.PathLike]:
         return super().get_path_to_generated_file(
-            self.model_name, file_name, file_extension, run_type="mesh_only"
+            data_model, self.model_name, file_name, file_extension, run_type="mesh_only"
         )
 
     def get_path_to_reference_file(
-        self, file_name: str, file_extension: str
+        self, data_model, file_name: str, file_extension: str
     ) -> Union[str, os.PathLike]:
         return super().get_path_to_reference_file(
-            self.model_name, file_name, file_extension, folder="Mesh"
+            data_model, self.model_name, file_name, file_extension, folder="Mesh"
         )
 
 
 class FiQuSSolverTests(BaseClassesForTests):
     def solve(
         self,
         data_model: FDM,
@@ -629,51 +649,60 @@
         gmsh_utils.initialize()
 
         # Open the pos files and get the model data:
         model_datas = []
         for pos_file in [pos_file_1, pos_file_2]:
             # Open the pos file:
             gmsh.open(pos_file)
+            data_all_steps = []
             for time_step in range(1, 100):
-                data_all_steps = []
                 # Save all available time steps up to 100:
                 try:
                     (
                         data_type,
                         tags,
                         data,
                         time,
                         numComponents,
                     ) = gmsh.view.getHomogeneousModelData(tag=0, step=time_step)
-                    data_all_steps.extend(data)
+                    data_all_steps.extend(list(data))
                 except:
                     break
 
             model_datas.append(data_all_steps)
 
         # Make sure the pos files are close enough:
-        with self.subTest(msg=f"{pos_file_1} and {pos_file_2} did not match!"):
-            self.assertEqual(
-                len(model_datas[0]),
-                len(model_datas[1]),
-            )
-
-            # Convert to numppy array:
-            model_data1 = np.array(model_datas[0])
-            model_data2 = np.array(model_datas[1])
+        self.assertEqual(
+            len(model_datas[0]),
+            len(model_datas[1]),
+            msg=f"{pos_file_1} and {pos_file_2} did not match!",
+        )
 
-            # Compare the data:
-            np.testing.assert_allclose(model_data1, model_data2, rtol=1e-05, atol=1e-08)
+        # Convert to numppy array:
+        model_data1 = np.array(model_datas[0])
+        model_data2 = np.array(model_datas[1])
+
+        # Compare the data:
+        np.testing.assert_allclose(
+            model_data1,
+            model_data2,
+            rtol=1e-05,
+            atol=1e-08,
+        )
 
     def get_path_to_generated_file(
-        self, file_name: str, file_extension: str
+        self, data_model, file_name: str, file_extension: str
     ) -> Union[str, os.PathLike]:
         return super().get_path_to_generated_file(
-            self.model_name, file_name, file_extension, run_type="solve_only"
+            data_model,
+            self.model_name,
+            file_name,
+            file_extension,
+            run_type="solve_only",
         )
 
     def get_path_to_reference_file(
-        self, file_name, file_extension
+        self, data_model, file_name, file_extension
     ) -> Union[str, os.PathLike]:
         return super().get_path_to_reference_file(
-            self.model_name, file_name, file_extension, folder="Solution"
+            data_model, self.model_name, file_name, file_extension, folder="Solution"
         )
```

### Comparing `fiqus-2024.1.1/tests/utils/helpers.py` & `fiqus-2024.4.0/tests/utils/helpers.py`

 * *Files identical despite different names*

