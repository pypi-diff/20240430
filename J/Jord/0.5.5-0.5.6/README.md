# Comparing `tmp/jord-0.5.5.tar.gz` & `tmp/jord-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jord-0.5.5.tar", last modified: Thu Apr 25 16:34:30 2024, max compression
+gzip compressed data, was "jord-0.5.6.tar", last modified: Mon Apr 29 11:24:03 2024, max compression
```

## Comparing `jord-0.5.5.tar` & `jord-0.5.6.tar`

### file list

```diff
@@ -1,162 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.569846 jord-0.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.541846 jord-0.5.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-25 16:34:25.000000 jord-0.5.5/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-25 16:34:25.000000 jord-0.5.5/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 16:34:25.000000 jord-0.5.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:25.000000 jord-0.5.5/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.561846 jord-0.5.5/Jord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-25 16:34:30.000000 jord-0.5.5/Jord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-25 16:34:30.000000 jord-0.5.5/Jord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:34:30.000000 jord-0.5.5/Jord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-25 16:34:30.000000 jord-0.5.5/Jord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 16:34:30.000000 jord-0.5.5/Jord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 16:34:25.000000 jord-0.5.5/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-25 16:34:25.000000 jord-0.5.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-25 16:34:25.000000 jord-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-25 16:34:30.569846 jord-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-25 16:34:25.000000 jord-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-25 16:34:25.000000 jord-0.5.5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.545846 jord-0.5.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 16:34:25.000000 jord-0.5.5/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.545846 jord-0.5.5/jord/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 16:34:25.000000 jord-0.5.5/jord/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2024-04-25 16:34:25.000000 jord-0.5.5/jord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.545846 jord-0.5.5/jord/fiona_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:25.000000 jord-0.5.5/jord/fiona_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-04-25 16:34:25.000000 jord-0.5.5/jord/fiona_utilities/deserialise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.545846 jord-0.5.5/jord/gdal_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      672 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/cloning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/context.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2228 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/drivers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/enums.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/error_handling.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/importing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2750 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/persistence.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-25 16:34:25.000000 jord-0.5.5/jord/gdal_utilities/spatial_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.549846 jord-0.5.5/jord/geojson_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geojson_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geojson_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      704 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geojson_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.549846 jord-0.5.5/jord/geometric_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geometric_analysis/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geometric_analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geometric_analysis/center_line.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geometric_analysis/degrees_of_freedom.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geometric_analysis/intersections.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geometric_analysis/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.549846 jord-0.5.5/jord/geopandas_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/geometry_filtering.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.549846 jord-0.5.5/jord/geopandas_utilities/serialisation/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/serialisation/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/serialisation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      673 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/serialisation/well_known_binary.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1401 2024-04-25 16:34:25.000000 jord-0.5.5/jord/geopandas_utilities/serialisation/well_known_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.549846 jord-0.5.5/jord/networkx_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-25 16:34:25.000000 jord-0.5.5/jord/networkx_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-25 16:34:25.000000 jord-0.5.5/jord/networkx_utilities/construction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.549846 jord-0.5.5/jord/pillow_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 16:34:25.000000 jord-0.5.5/jord/pillow_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-04-25 16:34:25.000000 jord-0.5.5/jord/pillow_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      280 2024-04-25 16:34:25.000000 jord-0.5.5/jord/pillow_utilities/exif.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-04-25 16:34:25.000000 jord-0.5.5/jord/pillow_utilities/tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.553846 jord-0.5.5/jord/qgis_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3521 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/categorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.553846 jord-0.5.5/jord/qgis_utilities/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/configuration/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/configuration/plugin_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/configuration/project_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.553846 jord-0.5.5/jord/qgis_utilities/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/conversion/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/conversion/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/conversion/parsing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14840 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/data_provider.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/geo_interface_serialisation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.557846 jord-0.5.5/jord/qgis_utilities/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2484 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/actions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      398 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/copying.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/drawing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/environment.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3357 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/models.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3566 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2877 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/randomize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/sessions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/signals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/helpers/timestamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      460 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/importing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13965 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/layer_creation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2128 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/layer_serialisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.557846 jord-0.5.5/jord/qgis_utilities/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/numpy_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/numpy_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2676 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/numpy_utilities/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/numpy_utilities/data_type.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/numpy_utilities/rasters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/plugin_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/styles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1978 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qgis_utilities/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.557846 jord-0.5.5/jord/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.557846 jord-0.5.5/jord/qlive_utilities/clients/
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/clients/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/clients/arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2865 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/clients/auto.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/clients/batching.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/clients/interfaced.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/pandas_procedures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20181 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/procedures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2566 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/serialisation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qlive_utilities/uri_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.557846 jord-0.5.5/jord/qt_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qt_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23855 2024-04-25 16:34:25.000000 jord-0.5.5/jord/qt_utilities/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.557846 jord-0.5.5/jord/rasterio_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 16:34:25.000000 jord-0.5.5/jord/rasterio_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-25 16:34:25.000000 jord-0.5.5/jord/rasterio_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.561846 jord-0.5.5/jord/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      558 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8327 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/clamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1907 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/geometry_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/grouping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27441 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/lines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/mirroring.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10107 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/morphology.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/points.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12570 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/polygons.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5885 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/projection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/rings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/selection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2902 2024-04-25 16:34:25.000000 jord-0.5.5/jord/shapely_utilities/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.561846 jord-0.5.5/jord/spatialite_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-25 16:34:25.000000 jord-0.5.5/jord/spatialite_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-04-25 16:34:25.000000 jord-0.5.5/jord/spatialite_utilities/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.561846 jord-0.5.5/jord/torch_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:25.000000 jord-0.5.5/jord/torch_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-25 16:34:25.000000 jord-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 16:34:25.000000 jord-0.5.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-25 16:34:30.569846 jord-0.5.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2024-04-25 16:34:25.000000 jord-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.561846 jord-0.5.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:34:30.561846 jord-0.5.5/tests/qgis/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 16:34:25.000000 jord-0.5.5/tests/qgis/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-04-25 16:34:25.000000 jord-0.5.5/tests/test_import.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-04-25 16:34:25.000000 jord-0.5.5/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.436167 jord-0.5.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.408167 jord-0.5.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-29 11:23:54.000000 jord-0.5.6/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-29 11:23:54.000000 jord-0.5.6/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 11:23:54.000000 jord-0.5.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:23:54.000000 jord-0.5.6/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.428167 jord-0.5.6/Jord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-29 11:24:03.000000 jord-0.5.6/Jord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-29 11:24:03.000000 jord-0.5.6/Jord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:24:03.000000 jord-0.5.6/Jord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-29 11:24:03.000000 jord-0.5.6/Jord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 11:24:03.000000 jord-0.5.6/Jord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 11:23:54.000000 jord-0.5.6/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-29 11:23:54.000000 jord-0.5.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-29 11:23:54.000000 jord-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-29 11:24:03.436167 jord-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-29 11:23:54.000000 jord-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-29 11:23:54.000000 jord-0.5.6/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.408167 jord-0.5.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-29 11:23:54.000000 jord-0.5.6/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.408167 jord-0.5.6/jord/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 11:23:55.000000 jord-0.5.6/jord/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2024-04-29 11:23:55.000000 jord-0.5.6/jord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.408167 jord-0.5.6/jord/fiona_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:23:55.000000 jord-0.5.6/jord/fiona_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-04-29 11:23:55.000000 jord-0.5.6/jord/fiona_utilities/deserialise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.408167 jord-0.5.6/jord/gdal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 11:23:55.000000 jord-0.5.6/jord/gdal_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      672 2024-04-29 11:23:55.000000 jord-0.5.6/jord/gdal_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-04-29 11:23:55.000000 jord-0.5.6/jord/gdal_utilities/cloning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-04-29 11:23:55.000000 jord-0.5.6/jord/gdal_utilities/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2228 2024-04-29 11:23:55.000000 jord-0.5.6/jord/gdal_utilities/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-04-29 11:23:55.000000 jord-0.5.6/jord/gdal_utilities/drivers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-04-29 11:23:55.000000 jord-0.5.6/jord/gdal_utilities/enums.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-29 11:23:55.000000 jord-0.5.6/jord/gdal_utilities/error_handling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-04-29 11:23:55.000000 jord-0.5.6/jord/gdal_utilities/importing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2750 2024-04-29 11:23:55.000000 jord-0.5.6/jord/gdal_utilities/persistence.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-29 11:23:55.000000 jord-0.5.6/jord/gdal_utilities/spatial_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.412167 jord-0.5.6/jord/geojson_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geojson_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geojson_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      704 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geojson_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.412167 jord-0.5.6/jord/geometric_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geometric_analysis/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geometric_analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geometric_analysis/center_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geometric_analysis/degrees_of_freedom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geometric_analysis/intersections.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geometric_analysis/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.412167 jord-0.5.6/jord/geopandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geopandas_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geopandas_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geopandas_utilities/geometry_filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geopandas_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.412167 jord-0.5.6/jord/geopandas_utilities/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geopandas_utilities/serialisation/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geopandas_utilities/serialisation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      673 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geopandas_utilities/serialisation/well_known_binary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1401 2024-04-29 11:23:55.000000 jord-0.5.6/jord/geopandas_utilities/serialisation/well_known_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.412167 jord-0.5.6/jord/networkx_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-29 11:23:55.000000 jord-0.5.6/jord/networkx_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-29 11:23:55.000000 jord-0.5.6/jord/networkx_utilities/construction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.412167 jord-0.5.6/jord/pillow_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 11:23:55.000000 jord-0.5.6/jord/pillow_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-04-29 11:23:55.000000 jord-0.5.6/jord/pillow_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      280 2024-04-29 11:23:55.000000 jord-0.5.6/jord/pillow_utilities/exif.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-04-29 11:23:55.000000 jord-0.5.6/jord/pillow_utilities/tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.416167 jord-0.5.6/jord/qgis_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3521 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.416167 jord-0.5.6/jord/qgis_utilities/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/configuration/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/configuration/plugin_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/configuration/project_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.416167 jord-0.5.6/jord/qgis_utilities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/conversion/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/conversion/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/conversion/parsing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14840 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/data_provider.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/geo_interface_serialisation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.420167 jord-0.5.6/jord/qgis_utilities/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2484 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/actions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      398 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/copying.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/drawing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/garbage_collection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3357 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3566 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2877 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/randomize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/sessions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/signals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/helpers/timestamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      460 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/importing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15779 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/layer_creation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2128 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/layer_serialisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.420167 jord-0.5.6/jord/qgis_utilities/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/numpy_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/numpy_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2676 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/numpy_utilities/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/numpy_utilities/data_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/numpy_utilities/rasters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/plugin_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/styles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1978 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qgis_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.420167 jord-0.5.6/jord/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qlive_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qlive_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qlive_utilities/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.424167 jord-0.5.6/jord/qlive_utilities/clients/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qlive_utilities/clients/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qlive_utilities/clients/arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2865 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qlive_utilities/clients/auto.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qlive_utilities/clients/batching.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qlive_utilities/clients/interfaced.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qlive_utilities/pandas_procedures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20181 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qlive_utilities/procedures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2566 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qlive_utilities/serialisation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qlive_utilities/uri_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.424167 jord-0.5.6/jord/qt_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qt_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23855 2024-04-29 11:23:55.000000 jord-0.5.6/jord/qt_utilities/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.424167 jord-0.5.6/jord/rasterio_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 11:23:55.000000 jord-0.5.6/jord/rasterio_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-29 11:23:55.000000 jord-0.5.6/jord/rasterio_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.424167 jord-0.5.6/jord/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      558 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8327 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/clamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1907 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/geometry_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/grouping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27441 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/lines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/mirroring.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10107 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/morphology.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/points.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12570 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/polygons.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5885 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/projection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/rings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/selection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2902 2024-04-29 11:23:55.000000 jord-0.5.6/jord/shapely_utilities/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.424167 jord-0.5.6/jord/spatialite_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-29 11:23:55.000000 jord-0.5.6/jord/spatialite_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-04-29 11:23:55.000000 jord-0.5.6/jord/spatialite_utilities/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.424167 jord-0.5.6/jord/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:23:55.000000 jord-0.5.6/jord/torch_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-29 11:23:55.000000 jord-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-29 11:23:55.000000 jord-0.5.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-29 11:24:03.436167 jord-0.5.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2024-04-29 11:23:55.000000 jord-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.428167 jord-0.5.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:24:03.428167 jord-0.5.6/tests/qgis/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-29 11:23:55.000000 jord-0.5.6/tests/qgis/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-04-29 11:23:55.000000 jord-0.5.6/tests/test_import.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-04-29 11:23:55.000000 jord-0.5.6/tests/test_sanity.py
```

### Comparing `jord-0.5.5/.github/CODE_OF_CONDUCT.md` & `jord-0.5.6/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/.github/CONTRIBUTING.md` & `jord-0.5.6/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/Jord.egg-info/PKG-INFO` & `jord-0.5.6/Jord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.5.5
+Version: 0.5.6
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Lindbjerg
 Author-email: chen@mapspeople.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: chen@mapspeople.dk
 License: Apache License, Version 2.0
@@ -36,87 +36,87 @@
 Provides-Extra: qgis
 Requires-Dist: PySide2; extra == "qgis"
 Provides-Extra: samples
 Provides-Extra: geopandas
 Requires-Dist: geopandas; extra == "geopandas"
 Provides-Extra: extra
 Provides-Extra: docs
-Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
-Requires-Dist: sphinx>=4.0.1; extra == "docs"
 Requires-Dist: furo; extra == "docs"
+Requires-Dist: sphinx>=4.0.1; extra == "docs"
+Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
 Provides-Extra: fiona
 Requires-Dist: fiona>=1.1.1; extra == "fiona"
 Provides-Extra: gdal
 Provides-Extra: tests
-Requires-Dist: mock; extra == "tests"
 Requires-Dist: pytest>=4.4.1; extra == "tests"
+Requires-Dist: mock; extra == "tests"
 Provides-Extra: shapely
-Requires-Dist: pyproj; extra == "shapely"
 Requires-Dist: shapely; extra == "shapely"
+Requires-Dist: pyproj; extra == "shapely"
 Provides-Extra: network
 Requires-Dist: networkx; extra == "network"
 Provides-Extra: dev
-Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
-Requires-Dist: pip>=22.1.2; extra == "dev"
-Requires-Dist: wheel>=0.33.0; extra == "dev"
-Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
+Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: sympy>=1.1.1; extra == "dev"
 Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: mock; extra == "dev"
-Requires-Dist: sphinx>=4.0.1; extra == "dev"
-Requires-Dist: pytest>=4.4.1; extra == "dev"
+Requires-Dist: pyzmq>=1.1.1; extra == "dev"
 Requires-Dist: apppath>=1.0.2; extra == "dev"
+Requires-Dist: numpy>=1.20.0; extra == "dev"
 Requires-Dist: draugr>=1.0.9; extra == "dev"
-Requires-Dist: sympy>=1.1.1; extra == "dev"
-Requires-Dist: pre-commit>=2.17.0; extra == "dev"
+Requires-Dist: mock; extra == "dev"
 Requires-Dist: tqdm>=1.1.1; extra == "dev"
-Requires-Dist: numpy>=1.20.0; extra == "dev"
 Requires-Dist: furo; extra == "dev"
 Requires-Dist: sorcery>=0.2.0; extra == "dev"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
-Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
-Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
+Requires-Dist: pip>=22.1.2; extra == "dev"
+Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
 Requires-Dist: warg>=1.1.6; extra == "dev"
+Requires-Dist: pytest>=4.4.1; extra == "dev"
+Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: wheel>=0.33.0; extra == "dev"
 Provides-Extra: pil
 Requires-Dist: Pillow; extra == "pil"
 Provides-Extra: legacy
-Requires-Dist: importlib-metadata; extra == "legacy"
 Requires-Dist: importlib-resources; extra == "legacy"
+Requires-Dist: importlib-metadata; extra == "legacy"
 Provides-Extra: setup
 Provides-Extra: all
 Requires-Dist: Pillow; extra == "all"
-Requires-Dist: importlib-metadata; extra == "all"
-Requires-Dist: pytest-cov>=2.11.1; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
-Requires-Dist: pip>=22.1.2; extra == "all"
-Requires-Dist: PySide2; extra == "all"
-Requires-Dist: wheel>=0.33.0; extra == "all"
-Requires-Dist: pytest>=4.3.0; extra == "all"
-Requires-Dist: fiona>=1.1.1; extra == "all"
-Requires-Dist: mock; extra == "all"
-Requires-Dist: sphinx>=4.0.1; extra == "all"
-Requires-Dist: geopandas; extra == "all"
+Requires-Dist: shapely; extra == "all"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: sympy>=1.1.1; extra == "all"
 Requires-Dist: coveralls>=1.6.0; extra == "all"
-Requires-Dist: pyproj; extra == "all"
-Requires-Dist: pytest>=4.4.1; extra == "all"
+Requires-Dist: fiona>=1.1.1; extra == "all"
+Requires-Dist: pyzmq>=1.1.1; extra == "all"
 Requires-Dist: apppath>=1.0.2; extra == "all"
+Requires-Dist: numpy>=1.20.0; extra == "all"
 Requires-Dist: draugr>=1.0.9; extra == "all"
-Requires-Dist: sympy>=1.1.1; extra == "all"
-Requires-Dist: pre-commit>=2.17.0; extra == "all"
-Requires-Dist: tqdm>=1.1.1; extra == "all"
-Requires-Dist: importlib-resources; extra == "all"
-Requires-Dist: warg>=1.1.6; extra == "all"
+Requires-Dist: mock; extra == "all"
 Requires-Dist: furo; extra == "all"
+Requires-Dist: importlib-resources; extra == "all"
+Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: importlib-metadata; extra == "all"
 Requires-Dist: sorcery>=0.2.0; extra == "all"
-Requires-Dist: shapely; extra == "all"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
-Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
+Requires-Dist: PySide2; extra == "all"
+Requires-Dist: pip>=22.1.2; extra == "all"
 Requires-Dist: networkx; extra == "all"
-Requires-Dist: pyzmq>=1.1.1; extra == "all"
-Requires-Dist: numpy>=1.20.0; extra == "all"
+Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
+Requires-Dist: pyproj; extra == "all"
+Requires-Dist: warg>=1.1.6; extra == "all"
+Requires-Dist: pytest>=4.4.1; extra == "all"
+Requires-Dist: tqdm>=1.1.1; extra == "all"
+Requires-Dist: wheel>=0.33.0; extra == "all"
+Requires-Dist: geopandas; extra == "all"
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
 </p>
```

### Comparing `jord-0.5.5/Jord.egg-info/SOURCES.txt` & `jord-0.5.6/Jord.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 jord/qgis_utilities/conversion/parsing.py
 jord/qgis_utilities/helpers/README.md
 jord/qgis_utilities/helpers/__init__.py
 jord/qgis_utilities/helpers/actions.py
 jord/qgis_utilities/helpers/copying.py
 jord/qgis_utilities/helpers/drawing.py
 jord/qgis_utilities/helpers/environment.py
+jord/qgis_utilities/helpers/garbage_collection.py
 jord/qgis_utilities/helpers/groups.py
 jord/qgis_utilities/helpers/logging.py
 jord/qgis_utilities/helpers/models.py
 jord/qgis_utilities/helpers/progress_bar.py
 jord/qgis_utilities/helpers/randomize.py
 jord/qgis_utilities/helpers/sessions.py
 jord/qgis_utilities/helpers/signals.py
```

### Comparing `jord-0.5.5/Jord.egg-info/requires.txt` & `jord-0.5.6/Jord.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -5,85 +5,85 @@
 sorcery>=0.2.0
 sympy>=1.1.1
 tqdm>=1.1.1
 warg>=1.1.6
 
 [all]
 Pillow
-importlib-metadata
-pytest-cov>=2.11.1
-twine>=1.13.0
-pip>=22.1.2
-PySide2
-wheel>=0.33.0
-pytest>=4.3.0
-fiona>=1.1.1
-mock
-sphinx>=4.0.1
-geopandas
-coveralls>=1.6.0
-pyproj
-pytest>=4.4.1
-apppath>=1.0.2
-draugr>=1.0.9
-sympy>=1.1.1
-pre-commit>=2.17.0
-tqdm>=1.1.1
-importlib-resources
-warg>=1.1.6
-furo
-sorcery>=0.2.0
 shapely
 black[jupyter]>=21.5b0
 sphinxcontrib-programoutput
-networkx
+sympy>=1.1.1
+coveralls>=1.6.0
+fiona>=1.1.1
 pyzmq>=1.1.1
+apppath>=1.0.2
 numpy>=1.20.0
-
-[dev]
+draugr>=1.0.9
+mock
+furo
+importlib-resources
 pytest-cov>=2.11.1
-twine>=1.13.0
+importlib-metadata
+sorcery>=0.2.0
+pre-commit>=2.17.0
+PySide2
 pip>=22.1.2
-wheel>=0.33.0
-pytest>=4.3.0
-coveralls>=1.6.0
-mock
+networkx
 sphinx>=4.0.1
+pytest>=4.3.0
+twine>=1.13.0
+pyproj
+warg>=1.1.6
 pytest>=4.4.1
+tqdm>=1.1.1
+wheel>=0.33.0
+geopandas
+
+[dev]
+black[jupyter]>=21.5b0
+sphinxcontrib-programoutput
+sympy>=1.1.1
+coveralls>=1.6.0
+pyzmq>=1.1.1
 apppath>=1.0.2
+numpy>=1.20.0
 draugr>=1.0.9
-sympy>=1.1.1
-pre-commit>=2.17.0
+mock
 tqdm>=1.1.1
-numpy>=1.20.0
 furo
 sorcery>=0.2.0
-black[jupyter]>=21.5b0
-sphinxcontrib-programoutput
-pyzmq>=1.1.1
+pre-commit>=2.17.0
+pip>=22.1.2
+sphinx>=4.0.1
+pytest>=4.3.0
+twine>=1.13.0
 warg>=1.1.6
+pytest>=4.4.1
+pytest-cov>=2.11.1
+wheel>=0.33.0
 
 [docs]
-sphinxcontrib-programoutput
-sphinx>=4.0.1
 furo
+sphinx>=4.0.1
+sphinxcontrib-programoutput
 
 [extra]
 
 [fiona]
 fiona>=1.1.1
 
 [gdal]
 
 [geopandas]
 geopandas
 
 [legacy]
-importlib-metadata
 importlib-resources
+importlib-metadata
 
 [network]
 networkx
 
 [pil]
 Pillow
 
@@ -94,13 +94,13 @@
 PySide2
 
 [samples]
 
 [setup]
 
 [shapely]
-pyproj
 shapely
+pyproj
 
 [tests]
-mock
 pytest>=4.4.1
+mock
```

### Comparing `jord-0.5.5/LICENSE.md` & `jord-0.5.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/PKG-INFO` & `jord-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.5.5
+Version: 0.5.6
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Lindbjerg
 Author-email: chen@mapspeople.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: chen@mapspeople.dk
 License: Apache License, Version 2.0
@@ -36,87 +36,87 @@
 Provides-Extra: qgis
 Requires-Dist: PySide2; extra == "qgis"
 Provides-Extra: samples
 Provides-Extra: geopandas
 Requires-Dist: geopandas; extra == "geopandas"
 Provides-Extra: extra
 Provides-Extra: docs
-Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
-Requires-Dist: sphinx>=4.0.1; extra == "docs"
 Requires-Dist: furo; extra == "docs"
+Requires-Dist: sphinx>=4.0.1; extra == "docs"
+Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
 Provides-Extra: fiona
 Requires-Dist: fiona>=1.1.1; extra == "fiona"
 Provides-Extra: gdal
 Provides-Extra: tests
-Requires-Dist: mock; extra == "tests"
 Requires-Dist: pytest>=4.4.1; extra == "tests"
+Requires-Dist: mock; extra == "tests"
 Provides-Extra: shapely
-Requires-Dist: pyproj; extra == "shapely"
 Requires-Dist: shapely; extra == "shapely"
+Requires-Dist: pyproj; extra == "shapely"
 Provides-Extra: network
 Requires-Dist: networkx; extra == "network"
 Provides-Extra: dev
-Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
-Requires-Dist: pip>=22.1.2; extra == "dev"
-Requires-Dist: wheel>=0.33.0; extra == "dev"
-Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
+Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: sympy>=1.1.1; extra == "dev"
 Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: mock; extra == "dev"
-Requires-Dist: sphinx>=4.0.1; extra == "dev"
-Requires-Dist: pytest>=4.4.1; extra == "dev"
+Requires-Dist: pyzmq>=1.1.1; extra == "dev"
 Requires-Dist: apppath>=1.0.2; extra == "dev"
+Requires-Dist: numpy>=1.20.0; extra == "dev"
 Requires-Dist: draugr>=1.0.9; extra == "dev"
-Requires-Dist: sympy>=1.1.1; extra == "dev"
-Requires-Dist: pre-commit>=2.17.0; extra == "dev"
+Requires-Dist: mock; extra == "dev"
 Requires-Dist: tqdm>=1.1.1; extra == "dev"
-Requires-Dist: numpy>=1.20.0; extra == "dev"
 Requires-Dist: furo; extra == "dev"
 Requires-Dist: sorcery>=0.2.0; extra == "dev"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
-Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
-Requires-Dist: pyzmq>=1.1.1; extra == "dev"
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
+Requires-Dist: pip>=22.1.2; extra == "dev"
+Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
 Requires-Dist: warg>=1.1.6; extra == "dev"
+Requires-Dist: pytest>=4.4.1; extra == "dev"
+Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: wheel>=0.33.0; extra == "dev"
 Provides-Extra: pil
 Requires-Dist: Pillow; extra == "pil"
 Provides-Extra: legacy
-Requires-Dist: importlib-metadata; extra == "legacy"
 Requires-Dist: importlib-resources; extra == "legacy"
+Requires-Dist: importlib-metadata; extra == "legacy"
 Provides-Extra: setup
 Provides-Extra: all
 Requires-Dist: Pillow; extra == "all"
-Requires-Dist: importlib-metadata; extra == "all"
-Requires-Dist: pytest-cov>=2.11.1; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
-Requires-Dist: pip>=22.1.2; extra == "all"
-Requires-Dist: PySide2; extra == "all"
-Requires-Dist: wheel>=0.33.0; extra == "all"
-Requires-Dist: pytest>=4.3.0; extra == "all"
-Requires-Dist: fiona>=1.1.1; extra == "all"
-Requires-Dist: mock; extra == "all"
-Requires-Dist: sphinx>=4.0.1; extra == "all"
-Requires-Dist: geopandas; extra == "all"
+Requires-Dist: shapely; extra == "all"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
+Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: sympy>=1.1.1; extra == "all"
 Requires-Dist: coveralls>=1.6.0; extra == "all"
-Requires-Dist: pyproj; extra == "all"
-Requires-Dist: pytest>=4.4.1; extra == "all"
+Requires-Dist: fiona>=1.1.1; extra == "all"
+Requires-Dist: pyzmq>=1.1.1; extra == "all"
 Requires-Dist: apppath>=1.0.2; extra == "all"
+Requires-Dist: numpy>=1.20.0; extra == "all"
 Requires-Dist: draugr>=1.0.9; extra == "all"
-Requires-Dist: sympy>=1.1.1; extra == "all"
-Requires-Dist: pre-commit>=2.17.0; extra == "all"
-Requires-Dist: tqdm>=1.1.1; extra == "all"
-Requires-Dist: importlib-resources; extra == "all"
-Requires-Dist: warg>=1.1.6; extra == "all"
+Requires-Dist: mock; extra == "all"
 Requires-Dist: furo; extra == "all"
+Requires-Dist: importlib-resources; extra == "all"
+Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: importlib-metadata; extra == "all"
 Requires-Dist: sorcery>=0.2.0; extra == "all"
-Requires-Dist: shapely; extra == "all"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
-Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
+Requires-Dist: PySide2; extra == "all"
+Requires-Dist: pip>=22.1.2; extra == "all"
 Requires-Dist: networkx; extra == "all"
-Requires-Dist: pyzmq>=1.1.1; extra == "all"
-Requires-Dist: numpy>=1.20.0; extra == "all"
+Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
+Requires-Dist: pyproj; extra == "all"
+Requires-Dist: warg>=1.1.6; extra == "all"
+Requires-Dist: pytest>=4.4.1; extra == "all"
+Requires-Dist: tqdm>=1.1.1; extra == "all"
+Requires-Dist: wheel>=0.33.0; extra == "all"
+Requires-Dist: geopandas; extra == "all"
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
 </p>
```

### Comparing `jord-0.5.5/README.md` & `jord-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/SECURITY.md` & `jord-0.5.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/__init__.py` & `jord-0.5.6/jord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     from importlib_metadata import PackageNotFoundError
     from importlib_resources import files
 
 from warg import package_is_editable, clean_string, get_version
 
 __project__ = "Jord"
 __author__ = "Christian Heider Lindbjerg"
-__version__ = "0.5.5"
+__version__ = "0.5.6"
 __doc__ = r"""
 .. module:: jord
    :platform: Unix, Windows
    :synopsis: A set of general tools build for geo data.
 
 .. moduleauthor:: Christian Heider Lindbjerg <chen@mapspeople.dk>
```

### Comparing `jord-0.5.5/jord/fiona_utilities/deserialise.py` & `jord-0.5.6/jord/fiona_utilities/deserialise.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/gdal_utilities/__init__.py` & `jord-0.5.6/jord/gdal_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/gdal_utilities/cloning.py` & `jord-0.5.6/jord/gdal_utilities/cloning.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/gdal_utilities/context.py` & `jord-0.5.6/jord/gdal_utilities/context.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/gdal_utilities/conversion.py` & `jord-0.5.6/jord/gdal_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/gdal_utilities/error_handling.py` & `jord-0.5.6/jord/gdal_utilities/error_handling.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/gdal_utilities/importing.py` & `jord-0.5.6/jord/gdal_utilities/importing.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/gdal_utilities/persistence.py` & `jord-0.5.6/jord/gdal_utilities/persistence.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/geojson_utilities/geometry_types.py` & `jord-0.5.6/jord/geojson_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/geometric_analysis/center_line.py` & `jord-0.5.6/jord/geometric_analysis/center_line.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/geometric_analysis/intersections.py` & `jord-0.5.6/jord/geometric_analysis/intersections.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/geopandas_utilities/geometry_filtering.py` & `jord-0.5.6/jord/geopandas_utilities/geometry_filtering.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/geopandas_utilities/serialisation/well_known_binary.py` & `jord-0.5.6/jord/geopandas_utilities/serialisation/well_known_binary.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/geopandas_utilities/serialisation/well_known_text.py` & `jord-0.5.6/jord/geopandas_utilities/serialisation/well_known_text.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/networkx_utilities/construction.py` & `jord-0.5.6/jord/networkx_utilities/construction.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/__init__.py` & `jord-0.5.6/jord/qgis_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/categorisation.py` & `jord-0.5.6/jord/qgis_utilities/categorisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/configuration/plugin_settings.py` & `jord-0.5.6/jord/qgis_utilities/configuration/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/configuration/project_settings.py` & `jord-0.5.6/jord/qgis_utilities/configuration/project_settings.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/data_provider.py` & `jord-0.5.6/jord/qgis_utilities/data_provider.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/enums.py` & `jord-0.5.6/jord/qgis_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/geo_interface_serialisation.py` & `jord-0.5.6/jord/qgis_utilities/geo_interface_serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/geometry_types.py` & `jord-0.5.6/jord/qgis_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/helpers/actions.py` & `jord-0.5.6/jord/qgis_utilities/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/helpers/drawing.py` & `jord-0.5.6/jord/qgis_utilities/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/helpers/environment.py` & `jord-0.5.6/jord/qgis_utilities/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/helpers/groups.py` & `jord-0.5.6/jord/qgis_utilities/helpers/groups.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/helpers/logging.py` & `jord-0.5.6/jord/qgis_utilities/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/helpers/models.py` & `jord-0.5.6/jord/qgis_utilities/helpers/models.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/helpers/progress_bar.py` & `jord-0.5.6/jord/qgis_utilities/helpers/progress_bar.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/helpers/randomize.py` & `jord-0.5.6/jord/qgis_utilities/helpers/randomize.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/helpers/sessions.py` & `jord-0.5.6/jord/qgis_utilities/helpers/sessions.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/helpers/signals.py` & `jord-0.5.6/jord/qgis_utilities/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/helpers/timestamp.py` & `jord-0.5.6/jord/qgis_utilities/helpers/timestamp.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/layer_creation.py` & `jord-0.5.6/jord/qgis_utilities/layer_creation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 import json
+import logging
 import time
 from typing import Any, Iterable, List, Mapping, Optional, Union
 
 from warg import passes_kws_to
 
 from jord.geojson_utilities import GeoJsonGeometryTypesEnum
 
@@ -20,14 +21,16 @@
 
 __all__ = [
     "add_qgis_single_feature_layer",
     "add_qgis_single_geometry_layers",
     "add_qgis_multi_feature_layer",
 ]
 
+logger = logging.getLogger(__name__)
+
 
 def add_qgis_single_feature_layer(
     qgis_instance_handle: Any,
     geom: Any,  #: QgsGeometry,
     name: Optional[str] = None,
     crs: Optional[str] = None,
     columns: Optional[Mapping[str, Any]] = None,
@@ -195,15 +198,24 @@
                     list(to_string_if_not_of_exact_type(columns.values()))
                 )
 
         layer = QgsVectorLayer(uri, layer_name, "memory")
         layer_data_provider = (
             layer.dataProvider()
         )  # DEFAULT DATA PROVIDER, TODO: MAYBE CHANGE THIS
-        layer_data_provider.addFeatures([feat])
+        assert feat.isValid(), f"{feat} was invalid"
+        res, out_feats = layer_data_provider.addFeatures([feat])
+
+        if not res:
+            logger.error(f"{layer_data_provider.lastError()}")
+
+            assert (
+                res
+            ), f"Failure while adding features {res} {layer_data_provider.lastError()}: {[o.isValid() for o in out_feats]}"
+
         layer_data_provider.updateExtents()
 
         if SKIP_MEMORY_LAYER_CHECK_AT_CLOSE:
             layer.setCustomProperty("skipMemoryLayersCheck", 1)
 
         if categorise_by_attribute:
             categorise_layer(layer, categorise_by_attribute)
@@ -287,19 +299,15 @@
     :param index:
     :return:
     """
 
     from .categorisation import categorise_layer
 
     # noinspection PyUnresolvedReferences
-    from qgis.core import (
-        QgsFeature,
-        QgsVectorLayer,
-        QgsProject,
-    )
+    from qgis.core import QgsFeature, QgsVectorLayer, QgsProject, QgsFeatureSink
 
     # noinspection PyUnresolvedReferences
     import qgis
 
     # uri = geom.type()
     # uri = geom.wkbType()
     # uri = geom.wktTypeStr()
@@ -314,15 +322,14 @@
 
     layer_name = f"{name}"
     if APPEND_TIMESTAMP:
         layer_name += f"_{time.time()}"
 
     geom_type = None
     uri = None
-    features = []
 
     sample_row = None
     num_cols = None
     attr_generator = None
     fields = None
 
     if columns and len(columns):
@@ -347,16 +354,18 @@
 
     if categorise_by_attribute and fields:
         assert (
             categorise_by_attribute in fields
         ), f"{categorise_by_attribute} was not found in {fields}"
 
     if not geoms:
+        logger.warning("Found no geometries")
         return  # No geometry
 
+    features = []
     for geom in geoms:
         geom_type_ = json.loads(geom.asJson())["type"]
 
         assert geom_type_ is not None, f"could not read {geom_type_=} as json"
 
         if geom_type_ is None:
             raise Exception(f"Could not load {geom.asJson()} as json")
@@ -391,16 +400,22 @@
                 if row:
                     feat.initAttributes(num_cols)
                     feat.setAttributes(
                         list(to_string_if_not_of_exact_type(row.values()))
                     )
 
             feat.setGeometry(geom)
+
+            assert feat.isValid(), f"{feat} was invalid"
             features.append(feat)
 
+    assert len(list(geoms)) == len(
+        features
+    ), f"Some features where dropped! {len(list(geoms))} != {len(features)}"
+
     if uri is None:
         raise Exception("uri is None")
 
     uri += "?"
 
     if crs:
         uri += f"crs={crs}"
@@ -412,27 +427,59 @@
 
     uri = str(uri).rstrip("&")
     uri += f'&index={"yes" if index else "no"}'
     uri.replace("?&", "?")
 
     layer = QgsVectorLayer(uri, layer_name, "memory")
     layer_data_provider = layer.dataProvider()
-    layer_data_provider.addFeatures(features)
+    # pr.addAttributes([QgsField("name", QVariant.String),QgsField("age", QVariant.Int),QgsField("size", QVariant.Double)])
+
+    (res, out_feats) = layer_data_provider.addFeatures(
+        features
+        # , QgsFeatureSink.RollBackOnErrors
+    )
+
+    if not res:
+        logger.error(f"{layer_data_provider.lastError()}")
+
+        assert (
+            res
+        ), f"Failure while adding features {res} {layer_data_provider.lastError()}: {[o.isValid() for o in out_feats]}"
+
+        assert len(list(geoms)) == len(
+            out_feats
+        ), f"Some features where dropped! return status {res}:  {len(list(geoms))} != {len(out_feats)}"
+
+    if len(list(geoms)) == layer.featureCount():
+        logger.error(f"{features}")
+
+        assert (
+            len(list(geoms)) == layer.featureCount()
+        ), f"Some features where dropped! {len(list(geoms))} != {layer.featureCount()}"
+
     layer_data_provider.updateExtents()
 
     if SKIP_MEMORY_LAYER_CHECK_AT_CLOSE:
         layer.setCustomProperty("skipMemoryLayersCheck", 1)
 
     if categorise_by_attribute:
         categorise_layer(layer, categorise_by_attribute)
 
+        assert (
+            len(list(geoms)) == layer.featureCount()
+        ), f"Some features where dropped! {len(list(geoms))} != {layer.featureCount()}"
+
     layer.commitChanges()
     layer.updateFields()
     layer.updateExtents()
 
+    assert (
+        len(list(geoms)) == layer.featureCount()
+    ), f"Some features where dropped! {len(list(geoms))} != {layer.featureCount()}"
+
     if qgis_instance_handle is None:
         qgis_project = QgsProject.instance()
     elif not isinstance(qgis_instance_handle, QgsProject):
         qgis_project = qgis_instance_handle.qgis_project
     else:
         qgis_project = qgis_instance_handle
 
@@ -448,14 +495,16 @@
 
     actions = qgis.utils.iface.layerTreeView().defaultActions()
     actions.showFeatureCount()  # TODO: Twice?
     actions.showFeatureCount()
 
     return_collection.append(layer)
 
+    assert len(return_collection) > 0, f"Return collection was empty"
+
     return return_collection
 
 
 def to_string_if_not_of_exact_type(
     gen: Iterable, type_: Iterable[type] = (int, float)
 ) -> Union[str, Any]:
     """
```

### Comparing `jord-0.5.5/jord/qgis_utilities/layer_serialisation.py` & `jord-0.5.6/jord/qgis_utilities/layer_serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/numpy_utilities/conversion.py` & `jord-0.5.6/jord/qgis_utilities/numpy_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/numpy_utilities/data_type.py` & `jord-0.5.6/jord/qgis_utilities/numpy_utilities/data_type.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py` & `jord-0.5.6/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/styles.py` & `jord-0.5.6/jord/qgis_utilities/styles.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qgis_utilities/styling.py` & `jord-0.5.6/jord/qgis_utilities/styling.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qlive_utilities/client.py` & `jord-0.5.6/jord/qlive_utilities/client.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qlive_utilities/clients/auto.py` & `jord-0.5.6/jord/qlive_utilities/clients/auto.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qlive_utilities/procedures.py` & `jord-0.5.6/jord/qlive_utilities/procedures.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qlive_utilities/serialisation.py` & `jord-0.5.6/jord/qlive_utilities/serialisation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qlive_utilities/uri_utilities.py` & `jord-0.5.6/jord/qlive_utilities/uri_utilities.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/qt_utilities/enums.py` & `jord-0.5.6/jord/qt_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/__init__.py` & `jord-0.5.6/jord/shapely_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/base.py` & `jord-0.5.6/jord/shapely_utilities/base.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/clamp.py` & `jord-0.5.6/jord/shapely_utilities/clamp.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/geometry_types.py` & `jord-0.5.6/jord/shapely_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/grouping.py` & `jord-0.5.6/jord/shapely_utilities/grouping.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/lines.py` & `jord-0.5.6/jord/shapely_utilities/lines.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/mirroring.py` & `jord-0.5.6/jord/shapely_utilities/mirroring.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/morphology.py` & `jord-0.5.6/jord/shapely_utilities/morphology.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/points.py` & `jord-0.5.6/jord/shapely_utilities/points.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/polygons.py` & `jord-0.5.6/jord/shapely_utilities/polygons.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/projection.py` & `jord-0.5.6/jord/shapely_utilities/projection.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/rings.py` & `jord-0.5.6/jord/shapely_utilities/rings.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/selection.py` & `jord-0.5.6/jord/shapely_utilities/selection.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/jord/shapely_utilities/transformation.py` & `jord-0.5.6/jord/shapely_utilities/transformation.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/setup.py` & `jord-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `jord-0.5.5/tests/test_import.py` & `jord-0.5.6/tests/test_import.py`

 * *Files identical despite different names*

