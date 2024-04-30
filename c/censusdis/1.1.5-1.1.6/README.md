# Comparing `tmp/censusdis-1.1.5.tar.gz` & `tmp/censusdis-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censusdis-1.1.5.tar", max compression
+gzip compressed data, was "censusdis-1.1.6.tar", max compression
```

## Comparing `censusdis-1.1.5.tar` & `censusdis-1.1.6.tar`

### file list

```diff
@@ -1,134 +1,134 @@
--rw-r--r--   0        0        0    19938 2023-05-29 16:16:27.244036 censusdis-1.1.5/LICENSE.md
--rw-r--r--   0        0        0     3717 2024-02-27 13:33:21.685281 censusdis-1.1.5/README.md
--rw-r--r--   0        0        0     6148 2023-12-17 16:06:26.749329 censusdis-1.1.5/censusdis/.DS_Store
--rw-r--r--   0        0        0      458 2024-02-15 00:31:57.583171 censusdis-1.1.5/censusdis/__init__.py
--rw-r--r--   0        0        0       92 2023-12-04 23:22:53.481176 censusdis-1.1.5/censusdis/cli/__init__.py
--rw-r--r--   0        0        0     5932 2023-12-05 20:25:11.495292 censusdis-1.1.5/censusdis/cli/cli.py
--rw-r--r--   0        0        0    34433 2024-01-24 14:31:26.141820 censusdis-1.1.5/censusdis/cli/yamlspec.py
--rw-r--r--   0        0        0     1129 2023-12-11 16:55:11.454323 censusdis-1.1.5/censusdis/counties/alabama.py
--rw-r--r--   0        0        0     1013 2023-12-11 16:55:11.455889 censusdis-1.1.5/censusdis/counties/alaska.py
--rw-r--r--   0        0        0      301 2023-12-11 16:55:11.456593 censusdis-1.1.5/censusdis/counties/arizona.py
--rw-r--r--   0        0        0     1261 2023-12-11 16:55:11.459042 censusdis-1.1.5/censusdis/counties/arkansas.py
--rw-r--r--   0        0        0     1029 2023-12-11 16:55:11.460975 censusdis-1.1.5/censusdis/counties/california.py
--rw-r--r--   0        0        0     1091 2023-12-11 16:55:11.463070 censusdis-1.1.5/censusdis/counties/colorado.py
--rw-r--r--   0        0        0     1115 2023-12-11 19:29:35.515569 censusdis-1.1.5/censusdis/counties/connecticut.py
--rw-r--r--   0        0        0      119 2023-12-11 16:55:11.463832 censusdis-1.1.5/censusdis/counties/delaware.py
--rw-r--r--   0        0        0      113 2023-12-11 16:55:11.464049 censusdis-1.1.5/censusdis/counties/district_of_columbia.py
--rw-r--r--   0        0        0     1140 2023-12-11 16:55:11.466050 censusdis-1.1.5/censusdis/counties/florida.py
--rw-r--r--   0        0        0     2539 2023-12-11 16:55:11.470438 censusdis-1.1.5/censusdis/counties/georgia.py
--rw-r--r--   0        0        0      145 2023-12-11 16:55:11.470786 censusdis-1.1.5/censusdis/counties/hawaii.py
--rw-r--r--   0        0        0      756 2023-12-11 16:55:11.472130 censusdis-1.1.5/censusdis/counties/idaho.py
--rw-r--r--   0        0        0     1670 2023-12-11 16:55:11.474786 censusdis-1.1.5/censusdis/counties/illinois.py
--rw-r--r--   0        0        0     1504 2023-12-11 16:55:11.477149 censusdis-1.1.5/censusdis/counties/indiana.py
--rw-r--r--   0        0        0     1627 2023-12-11 16:55:11.479639 censusdis-1.1.5/censusdis/counties/iowa.py
--rw-r--r--   0        0        0     1700 2023-12-11 16:55:11.482454 censusdis-1.1.5/censusdis/counties/kansas.py
--rw-r--r--   0        0        0     1943 2023-12-11 16:55:11.485657 censusdis-1.1.5/censusdis/counties/kentucky.py
--rw-r--r--   0        0        0     1227 2023-12-11 16:55:11.487208 censusdis-1.1.5/censusdis/counties/louisiana.py
--rw-r--r--   0        0        0      340 2023-12-11 16:55:11.487753 censusdis-1.1.5/censusdis/counties/maine.py
--rw-r--r--   0        0        0      492 2023-12-11 16:55:11.488448 censusdis-1.1.5/censusdis/counties/maryland.py
--rw-r--r--   0        0        0      312 2023-12-11 16:55:11.488933 censusdis-1.1.5/censusdis/counties/massachusetts.py
--rw-r--r--   0        0        0     1408 2023-12-11 16:55:11.490783 censusdis-1.1.5/censusdis/counties/michigan.py
--rw-r--r--   0        0        0     1472 2023-12-11 16:55:11.492725 censusdis-1.1.5/censusdis/counties/minnesota.py
--rw-r--r--   0        0        0     1388 2023-12-11 16:55:11.494560 censusdis-1.1.5/censusdis/counties/mississippi.py
--rw-r--r--   0        0        0     1876 2023-12-11 16:55:11.496943 censusdis-1.1.5/censusdis/counties/missouri.py
--rw-r--r--   0        0        0     1012 2023-12-11 16:55:11.498213 censusdis-1.1.5/censusdis/counties/montana.py
--rw-r--r--   0        0        0     1496 2023-12-11 16:55:11.500179 censusdis-1.1.5/censusdis/counties/nebraska.py
--rw-r--r--   0        0        0      339 2023-12-11 16:55:11.500687 censusdis-1.1.5/censusdis/counties/nevada.py
--rw-r--r--   0        0        0      248 2023-12-11 16:55:11.501047 censusdis-1.1.5/censusdis/counties/new_hampshire.py
--rw-r--r--   0        0        0      412 2023-12-11 16:55:11.501613 censusdis-1.1.5/censusdis/counties/new_jersey.py
--rw-r--r--   0        0        0      593 2023-12-11 16:55:11.502420 censusdis-1.1.5/censusdis/counties/new_mexico.py
--rw-r--r--   0        0        0     1083 2023-12-11 16:55:11.503743 censusdis-1.1.5/censusdis/counties/new_york.py
--rw-r--r--   0        0        0     1668 2023-12-11 16:55:11.505932 censusdis-1.1.5/censusdis/counties/north_carolina.py
--rw-r--r--   0        0        0      900 2023-12-11 16:55:11.507102 censusdis-1.1.5/censusdis/counties/north_dakota.py
--rw-r--r--   0        0        0     1446 2023-12-11 16:55:11.508907 censusdis-1.1.5/censusdis/counties/ohio.py
--rw-r--r--   0        0        0     1283 2023-12-11 16:55:11.510477 censusdis-1.1.5/censusdis/counties/oklahoma.py
--rw-r--r--   0        0        0      635 2023-12-11 16:55:11.511295 censusdis-1.1.5/censusdis/counties/oregon.py
--rw-r--r--   0        0        0     1168 2023-12-11 16:55:11.512672 censusdis-1.1.5/censusdis/counties/pennsylvania.py
--rw-r--r--   0        0        0     1381 2023-12-11 16:55:11.532504 censusdis-1.1.5/censusdis/counties/puerto_rico.py
--rw-r--r--   0        0        0      159 2023-12-11 16:55:11.512922 censusdis-1.1.5/censusdis/counties/rhode_island.py
--rw-r--r--   0        0        0      855 2023-12-11 16:55:11.514193 censusdis-1.1.5/censusdis/counties/south_carolina.py
--rw-r--r--   0        0        0     1104 2023-12-11 16:55:11.515784 censusdis-1.1.5/censusdis/counties/south_dakota.py
--rw-r--r--   0        0        0     1568 2023-12-11 16:55:11.517745 censusdis-1.1.5/censusdis/counties/tennessee.py
--rw-r--r--   0        0        0     4049 2023-12-11 16:55:11.522518 censusdis-1.1.5/censusdis/counties/texas.py
--rw-r--r--   0        0        0      506 2023-12-11 16:55:11.523238 censusdis-1.1.5/censusdis/counties/utah.py
--rw-r--r--   0        0        0      308 2023-12-11 16:55:11.523841 censusdis-1.1.5/censusdis/counties/vermont.py
--rw-r--r--   0        0        0     2603 2023-12-11 16:55:11.526648 censusdis-1.1.5/censusdis/counties/virginia.py
--rw-r--r--   0        0        0      705 2023-12-11 16:55:11.527561 censusdis-1.1.5/censusdis/counties/washington.py
--rw-r--r--   0        0        0      938 2023-12-11 16:55:11.528745 censusdis-1.1.5/censusdis/counties/west_virginia.py
--rw-r--r--   0        0        0     1219 2023-12-11 16:55:11.530242 censusdis-1.1.5/censusdis/counties/wisconsin.py
--rw-r--r--   0        0        0      439 2023-12-11 16:55:11.530847 censusdis-1.1.5/censusdis/counties/wyoming.py
--rw-r--r--   0        0        0     7109 2023-12-11 20:36:13.100154 censusdis-1.1.5/censusdis/csa.py
--rw-r--r--   0        0        0    50290 2024-03-23 17:38:35.323344 censusdis-1.1.5/censusdis/data.py
--rw-r--r--   0        0        0    26488 2024-03-21 21:46:41.629759 censusdis-1.1.5/censusdis/datasets.py
--rw-r--r--   0        0        0      332 2023-12-11 20:36:14.332200 censusdis-1.1.5/censusdis/division.py
--rw-r--r--   0        0        0    14425 2024-03-23 17:38:35.323871 censusdis-1.1.5/censusdis/geography.py
--rw-r--r--   0        0        0       98 2023-12-04 23:22:53.473814 censusdis-1.1.5/censusdis/impl/__init__.py
--rw-r--r--   0        0        0      160 2023-12-04 16:32:55.038743 censusdis-1.1.5/censusdis/impl/exceptions.py
--rw-r--r--   0        0        0     7671 2024-03-23 17:38:35.324199 censusdis-1.1.5/censusdis/impl/fetch.py
--rw-r--r--   0        0        0     5096 2024-01-26 21:46:43.129405 censusdis-1.1.5/censusdis/impl/geometry.py
--rw-r--r--   0        0        0    20972 2024-03-14 21:06:25.569684 censusdis-1.1.5/censusdis/impl/us_census_shapefiles.py
--rw-r--r--   0        0        0    22662 2024-03-14 21:06:25.570218 censusdis-1.1.5/censusdis/impl/varcache.py
--rw-r--r--   0        0        0       66 2023-12-04 23:22:53.483682 censusdis-1.1.5/censusdis/impl/varsource/__init__.py
--rw-r--r--   0        0        0     6682 2024-03-14 21:06:25.570849 censusdis-1.1.5/censusdis/impl/varsource/base.py
--rw-r--r--   0        0        0     5672 2024-03-14 21:06:25.571500 censusdis-1.1.5/censusdis/impl/varsource/censusapi.py
--rw-r--r--   0        0        0    40124 2024-03-23 17:38:35.324606 censusdis-1.1.5/censusdis/maps.py
--rw-r--r--   0        0        0    34128 2023-12-11 20:36:12.393854 censusdis-1.1.5/censusdis/msa_msa.py
--rw-r--r--   0        0        0    14558 2023-12-11 19:29:35.515941 censusdis-1.1.5/censusdis/places/alabama.py
--rw-r--r--   0        0        0     8790 2023-12-11 19:29:35.516183 censusdis-1.1.5/censusdis/places/alaska.py
--rw-r--r--   0        0        0    11861 2023-12-11 19:29:35.516445 censusdis-1.1.5/censusdis/places/arizona.py
--rw-r--r--   0        0        0    15048 2023-12-11 19:29:35.516764 censusdis-1.1.5/censusdis/places/arkansas.py
--rw-r--r--   0        0        0    41385 2023-12-11 19:29:35.517121 censusdis-1.1.5/censusdis/places/california.py
--rw-r--r--   0        0        0    11894 2023-12-11 19:29:35.517306 censusdis-1.1.5/censusdis/places/colorado.py
--rw-r--r--   0        0        0     5822 2023-12-11 19:29:35.517517 censusdis-1.1.5/censusdis/places/connecticut.py
--rw-r--r--   0        0        0     2047 2023-12-11 19:29:35.517640 censusdis-1.1.5/censusdis/places/delaware.py
--rw-r--r--   0        0        0      108 2023-12-11 19:29:35.517800 censusdis-1.1.5/censusdis/places/district_of_columbia.py
--rw-r--r--   0        0        0    25466 2023-12-11 19:29:35.518158 censusdis-1.1.5/censusdis/places/florida.py
--rw-r--r--   0        0        0    16652 2023-12-11 19:29:35.518343 censusdis-1.1.5/censusdis/places/georgia.py
--rw-r--r--   0        0        0     4060 2023-12-11 19:29:35.518467 censusdis-1.1.5/censusdis/places/hawaii.py
--rw-r--r--   0        0        0     5685 2023-12-11 19:29:35.518634 censusdis-1.1.5/censusdis/places/idaho.py
--rw-r--r--   0        0        0    38933 2023-12-11 19:29:35.519027 censusdis-1.1.5/censusdis/places/illinois.py
--rw-r--r--   0        0        0    23926 2023-12-11 19:29:35.519320 censusdis-1.1.5/censusdis/places/indiana.py
--rw-r--r--   0        0        0    24633 2023-12-11 19:29:35.519626 censusdis-1.1.5/censusdis/places/iowa.py
--rw-r--r--   0        0        0    17556 2023-12-11 19:29:35.519874 censusdis-1.1.5/censusdis/places/kansas.py
--rw-r--r--   0        0        0    14063 2023-12-11 19:29:35.520117 censusdis-1.1.5/censusdis/places/kentucky.py
--rw-r--r--   0        0        0    12119 2023-12-11 19:29:35.520465 censusdis-1.1.5/censusdis/places/louisiana.py
--rw-r--r--   0        0        0     3818 2023-12-11 19:29:35.520594 censusdis-1.1.5/censusdis/places/maine.py
--rw-r--r--   0        0        0    13853 2023-12-11 19:29:35.520760 censusdis-1.1.5/censusdis/places/maryland.py
--rw-r--r--   0        0        0     6351 2023-12-11 19:29:35.520935 censusdis-1.1.5/censusdis/places/massachusetts.py
--rw-r--r--   0        0        0    19186 2023-12-11 19:29:35.521108 censusdis-1.1.5/censusdis/places/michigan.py
--rw-r--r--   0        0        0    22227 2023-12-11 19:29:35.521432 censusdis-1.1.5/censusdis/places/minnesota.py
--rw-r--r--   0        0        0    10406 2023-12-11 19:29:35.521602 censusdis-1.1.5/censusdis/places/mississippi.py
--rw-r--r--   0        0        0    27499 2023-12-11 19:29:35.521942 censusdis-1.1.5/censusdis/places/missouri.py
--rw-r--r--   0        0        0    12297 2023-12-11 19:29:35.522122 censusdis-1.1.5/censusdis/places/montana.py
--rw-r--r--   0        0        0    14951 2023-12-11 19:29:35.522289 censusdis-1.1.5/censusdis/places/nebraska.py
--rw-r--r--   0        0        0     3341 2023-12-11 19:29:35.522400 censusdis-1.1.5/censusdis/places/nevada.py
--rw-r--r--   0        0        0     2504 2023-12-11 19:29:35.522517 censusdis-1.1.5/censusdis/places/new_hampshire.py
--rw-r--r--   0        0        0    19179 2023-12-11 19:29:35.522722 censusdis-1.1.5/censusdis/places/new_jersey.py
--rw-r--r--   0        0        0    13434 2023-12-11 19:29:35.522891 censusdis-1.1.5/censusdis/places/new_mexico.py
--rw-r--r--   0        0        0    34855 2023-12-11 19:29:35.523211 censusdis-1.1.5/censusdis/places/new_york.py
--rw-r--r--   0        0        0    19432 2023-12-11 19:29:35.523418 censusdis-1.1.5/censusdis/places/north_carolina.py
--rw-r--r--   0        0        0     9524 2023-12-11 19:29:35.523558 censusdis-1.1.5/censusdis/places/north_dakota.py
--rw-r--r--   0        0        0    34277 2023-12-11 19:29:35.523920 censusdis-1.1.5/censusdis/places/ohio.py
--rw-r--r--   0        0        0    19802 2023-12-11 19:29:35.524122 censusdis-1.1.5/censusdis/places/oklahoma.py
--rw-r--r--   0        0        0    10398 2023-12-11 19:29:35.524366 censusdis-1.1.5/censusdis/places/oregon.py
--rw-r--r--   0        0        0    51324 2023-12-11 19:29:35.524811 censusdis-1.1.5/censusdis/places/pennsylvania.py
--rw-r--r--   0        0        0     9391 2023-12-11 19:29:35.524961 censusdis-1.1.5/censusdis/places/puerto_rico.py
--rw-r--r--   0        0        0      985 2023-12-11 19:29:35.525076 censusdis-1.1.5/censusdis/places/rhode_island.py
--rw-r--r--   0        0        0    11708 2023-12-11 19:29:35.525311 censusdis-1.1.5/censusdis/places/south_carolina.py
--rw-r--r--   0        0        0    12094 2023-12-11 19:29:35.525524 censusdis-1.1.5/censusdis/places/south_dakota.py
--rw-r--r--   0        0        0    12647 2023-12-11 19:29:35.525795 censusdis-1.1.5/censusdis/places/tennessee.py
--rw-r--r--   0        0        0    46473 2023-12-11 19:29:35.526090 censusdis-1.1.5/censusdis/places/texas.py
--rw-r--r--   0        0        0     8246 2023-12-11 19:29:35.526224 censusdis-1.1.5/censusdis/places/utah.py
--rw-r--r--   0        0        0     4712 2023-12-11 19:29:35.526351 censusdis-1.1.5/censusdis/places/vermont.py
--rw-r--r--   0        0        0    17023 2023-12-11 19:29:35.526524 censusdis-1.1.5/censusdis/places/virginia.py
--rw-r--r--   0        0        0    15869 2023-12-11 19:29:35.526833 censusdis-1.1.5/censusdis/places/washington.py
--rw-r--r--   0        0        0    10717 2023-12-11 19:29:35.526982 censusdis-1.1.5/censusdis/places/west_virginia.py
--rw-r--r--   0        0        0    20957 2023-12-11 19:29:35.527184 censusdis-1.1.5/censusdis/places/wisconsin.py
--rw-r--r--   0        0        0     5030 2023-12-11 19:29:35.527313 censusdis-1.1.5/censusdis/places/wyoming.py
--rw-r--r--   0        0        0      140 2023-12-11 20:36:13.710754 censusdis-1.1.5/censusdis/region.py
--rw-r--r--   0        0        0       70 2023-12-04 22:25:55.364310 censusdis-1.1.5/censusdis/resources/__init__.py
--rw-r--r--   0        0        0    25951 2023-05-29 16:16:27.245353 censusdis-1.1.5/censusdis/resources/crs_bounds.geojson
--rw-r--r--   0        0        0     7192 2023-12-04 21:03:55.744421 censusdis-1.1.5/censusdis/states.py
--rw-r--r--   0        0        0     2399 2023-05-29 16:16:27.245539 censusdis-1.1.5/censusdis/values.py
--rw-r--r--   0        0        0     2503 2024-03-23 17:38:45.989585 censusdis-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     5882 1970-01-01 00:00:00.000000 censusdis-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    19938 2023-05-29 16:16:27.244036 censusdis-1.1.6/LICENSE.md
+-rw-r--r--   0        0        0     3717 2024-02-27 13:33:21.685281 censusdis-1.1.6/README.md
+-rw-r--r--   0        0        0     6148 2023-12-17 16:06:26.749329 censusdis-1.1.6/censusdis/.DS_Store
+-rw-r--r--   0        0        0      458 2024-02-15 00:31:57.583171 censusdis-1.1.6/censusdis/__init__.py
+-rw-r--r--   0        0        0       92 2023-12-04 23:22:53.481176 censusdis-1.1.6/censusdis/cli/__init__.py
+-rw-r--r--   0        0        0     5932 2023-12-05 20:25:11.495292 censusdis-1.1.6/censusdis/cli/cli.py
+-rw-r--r--   0        0        0    34433 2024-01-24 14:31:26.141820 censusdis-1.1.6/censusdis/cli/yamlspec.py
+-rw-r--r--   0        0        0     1129 2023-12-11 16:55:11.454323 censusdis-1.1.6/censusdis/counties/alabama.py
+-rw-r--r--   0        0        0     1013 2023-12-11 16:55:11.455889 censusdis-1.1.6/censusdis/counties/alaska.py
+-rw-r--r--   0        0        0      301 2023-12-11 16:55:11.456593 censusdis-1.1.6/censusdis/counties/arizona.py
+-rw-r--r--   0        0        0     1261 2023-12-11 16:55:11.459042 censusdis-1.1.6/censusdis/counties/arkansas.py
+-rw-r--r--   0        0        0     1029 2023-12-11 16:55:11.460975 censusdis-1.1.6/censusdis/counties/california.py
+-rw-r--r--   0        0        0     1091 2023-12-11 16:55:11.463070 censusdis-1.1.6/censusdis/counties/colorado.py
+-rw-r--r--   0        0        0     1115 2023-12-11 19:29:35.515569 censusdis-1.1.6/censusdis/counties/connecticut.py
+-rw-r--r--   0        0        0      119 2023-12-11 16:55:11.463832 censusdis-1.1.6/censusdis/counties/delaware.py
+-rw-r--r--   0        0        0      113 2023-12-11 16:55:11.464049 censusdis-1.1.6/censusdis/counties/district_of_columbia.py
+-rw-r--r--   0        0        0     1140 2023-12-11 16:55:11.466050 censusdis-1.1.6/censusdis/counties/florida.py
+-rw-r--r--   0        0        0     2539 2023-12-11 16:55:11.470438 censusdis-1.1.6/censusdis/counties/georgia.py
+-rw-r--r--   0        0        0      145 2023-12-11 16:55:11.470786 censusdis-1.1.6/censusdis/counties/hawaii.py
+-rw-r--r--   0        0        0      756 2023-12-11 16:55:11.472130 censusdis-1.1.6/censusdis/counties/idaho.py
+-rw-r--r--   0        0        0     1670 2023-12-11 16:55:11.474786 censusdis-1.1.6/censusdis/counties/illinois.py
+-rw-r--r--   0        0        0     1504 2023-12-11 16:55:11.477149 censusdis-1.1.6/censusdis/counties/indiana.py
+-rw-r--r--   0        0        0     1627 2023-12-11 16:55:11.479639 censusdis-1.1.6/censusdis/counties/iowa.py
+-rw-r--r--   0        0        0     1700 2023-12-11 16:55:11.482454 censusdis-1.1.6/censusdis/counties/kansas.py
+-rw-r--r--   0        0        0     1943 2023-12-11 16:55:11.485657 censusdis-1.1.6/censusdis/counties/kentucky.py
+-rw-r--r--   0        0        0     1227 2023-12-11 16:55:11.487208 censusdis-1.1.6/censusdis/counties/louisiana.py
+-rw-r--r--   0        0        0      340 2023-12-11 16:55:11.487753 censusdis-1.1.6/censusdis/counties/maine.py
+-rw-r--r--   0        0        0      492 2023-12-11 16:55:11.488448 censusdis-1.1.6/censusdis/counties/maryland.py
+-rw-r--r--   0        0        0      312 2023-12-11 16:55:11.488933 censusdis-1.1.6/censusdis/counties/massachusetts.py
+-rw-r--r--   0        0        0     1408 2023-12-11 16:55:11.490783 censusdis-1.1.6/censusdis/counties/michigan.py
+-rw-r--r--   0        0        0     1472 2023-12-11 16:55:11.492725 censusdis-1.1.6/censusdis/counties/minnesota.py
+-rw-r--r--   0        0        0     1388 2023-12-11 16:55:11.494560 censusdis-1.1.6/censusdis/counties/mississippi.py
+-rw-r--r--   0        0        0     1876 2023-12-11 16:55:11.496943 censusdis-1.1.6/censusdis/counties/missouri.py
+-rw-r--r--   0        0        0     1012 2023-12-11 16:55:11.498213 censusdis-1.1.6/censusdis/counties/montana.py
+-rw-r--r--   0        0        0     1496 2023-12-11 16:55:11.500179 censusdis-1.1.6/censusdis/counties/nebraska.py
+-rw-r--r--   0        0        0      339 2023-12-11 16:55:11.500687 censusdis-1.1.6/censusdis/counties/nevada.py
+-rw-r--r--   0        0        0      248 2023-12-11 16:55:11.501047 censusdis-1.1.6/censusdis/counties/new_hampshire.py
+-rw-r--r--   0        0        0      412 2023-12-11 16:55:11.501613 censusdis-1.1.6/censusdis/counties/new_jersey.py
+-rw-r--r--   0        0        0      593 2023-12-11 16:55:11.502420 censusdis-1.1.6/censusdis/counties/new_mexico.py
+-rw-r--r--   0        0        0     1083 2023-12-11 16:55:11.503743 censusdis-1.1.6/censusdis/counties/new_york.py
+-rw-r--r--   0        0        0     1668 2023-12-11 16:55:11.505932 censusdis-1.1.6/censusdis/counties/north_carolina.py
+-rw-r--r--   0        0        0      900 2023-12-11 16:55:11.507102 censusdis-1.1.6/censusdis/counties/north_dakota.py
+-rw-r--r--   0        0        0     1446 2023-12-11 16:55:11.508907 censusdis-1.1.6/censusdis/counties/ohio.py
+-rw-r--r--   0        0        0     1283 2023-12-11 16:55:11.510477 censusdis-1.1.6/censusdis/counties/oklahoma.py
+-rw-r--r--   0        0        0      635 2023-12-11 16:55:11.511295 censusdis-1.1.6/censusdis/counties/oregon.py
+-rw-r--r--   0        0        0     1168 2023-12-11 16:55:11.512672 censusdis-1.1.6/censusdis/counties/pennsylvania.py
+-rw-r--r--   0        0        0     1381 2023-12-11 16:55:11.532504 censusdis-1.1.6/censusdis/counties/puerto_rico.py
+-rw-r--r--   0        0        0      159 2023-12-11 16:55:11.512922 censusdis-1.1.6/censusdis/counties/rhode_island.py
+-rw-r--r--   0        0        0      855 2023-12-11 16:55:11.514193 censusdis-1.1.6/censusdis/counties/south_carolina.py
+-rw-r--r--   0        0        0     1104 2023-12-11 16:55:11.515784 censusdis-1.1.6/censusdis/counties/south_dakota.py
+-rw-r--r--   0        0        0     1568 2023-12-11 16:55:11.517745 censusdis-1.1.6/censusdis/counties/tennessee.py
+-rw-r--r--   0        0        0     4049 2023-12-11 16:55:11.522518 censusdis-1.1.6/censusdis/counties/texas.py
+-rw-r--r--   0        0        0      506 2023-12-11 16:55:11.523238 censusdis-1.1.6/censusdis/counties/utah.py
+-rw-r--r--   0        0        0      308 2023-12-11 16:55:11.523841 censusdis-1.1.6/censusdis/counties/vermont.py
+-rw-r--r--   0        0        0     2603 2023-12-11 16:55:11.526648 censusdis-1.1.6/censusdis/counties/virginia.py
+-rw-r--r--   0        0        0      705 2023-12-11 16:55:11.527561 censusdis-1.1.6/censusdis/counties/washington.py
+-rw-r--r--   0        0        0      938 2023-12-11 16:55:11.528745 censusdis-1.1.6/censusdis/counties/west_virginia.py
+-rw-r--r--   0        0        0     1219 2023-12-11 16:55:11.530242 censusdis-1.1.6/censusdis/counties/wisconsin.py
+-rw-r--r--   0        0        0      439 2023-12-11 16:55:11.530847 censusdis-1.1.6/censusdis/counties/wyoming.py
+-rw-r--r--   0        0        0     7109 2023-12-11 20:36:13.100154 censusdis-1.1.6/censusdis/csa.py
+-rw-r--r--   0        0        0    50290 2024-03-23 17:38:35.323344 censusdis-1.1.6/censusdis/data.py
+-rw-r--r--   0        0        0    29967 2024-04-29 22:17:32.815725 censusdis-1.1.6/censusdis/datasets.py
+-rw-r--r--   0        0        0      332 2023-12-11 20:36:14.332200 censusdis-1.1.6/censusdis/division.py
+-rw-r--r--   0        0        0    14425 2024-03-23 17:38:35.323871 censusdis-1.1.6/censusdis/geography.py
+-rw-r--r--   0        0        0       98 2023-12-04 23:22:53.473814 censusdis-1.1.6/censusdis/impl/__init__.py
+-rw-r--r--   0        0        0      160 2023-12-04 16:32:55.038743 censusdis-1.1.6/censusdis/impl/exceptions.py
+-rw-r--r--   0        0        0     7671 2024-03-23 17:38:35.324199 censusdis-1.1.6/censusdis/impl/fetch.py
+-rw-r--r--   0        0        0     5096 2024-01-26 21:46:43.129405 censusdis-1.1.6/censusdis/impl/geometry.py
+-rw-r--r--   0        0        0    21273 2024-04-29 21:22:19.307664 censusdis-1.1.6/censusdis/impl/us_census_shapefiles.py
+-rw-r--r--   0        0        0    23248 2024-04-29 21:22:19.307957 censusdis-1.1.6/censusdis/impl/varcache.py
+-rw-r--r--   0        0        0       66 2023-12-04 23:22:53.483682 censusdis-1.1.6/censusdis/impl/varsource/__init__.py
+-rw-r--r--   0        0        0     6682 2024-03-14 21:06:25.570849 censusdis-1.1.6/censusdis/impl/varsource/base.py
+-rw-r--r--   0        0        0     5672 2024-03-14 21:06:25.571500 censusdis-1.1.6/censusdis/impl/varsource/censusapi.py
+-rw-r--r--   0        0        0    40124 2024-03-23 17:38:35.324606 censusdis-1.1.6/censusdis/maps.py
+-rw-r--r--   0        0        0    34128 2023-12-11 20:36:12.393854 censusdis-1.1.6/censusdis/msa_msa.py
+-rw-r--r--   0        0        0    14558 2023-12-11 19:29:35.515941 censusdis-1.1.6/censusdis/places/alabama.py
+-rw-r--r--   0        0        0     8790 2023-12-11 19:29:35.516183 censusdis-1.1.6/censusdis/places/alaska.py
+-rw-r--r--   0        0        0    11861 2023-12-11 19:29:35.516445 censusdis-1.1.6/censusdis/places/arizona.py
+-rw-r--r--   0        0        0    15048 2023-12-11 19:29:35.516764 censusdis-1.1.6/censusdis/places/arkansas.py
+-rw-r--r--   0        0        0    41385 2023-12-11 19:29:35.517121 censusdis-1.1.6/censusdis/places/california.py
+-rw-r--r--   0        0        0    11894 2023-12-11 19:29:35.517306 censusdis-1.1.6/censusdis/places/colorado.py
+-rw-r--r--   0        0        0     5822 2023-12-11 19:29:35.517517 censusdis-1.1.6/censusdis/places/connecticut.py
+-rw-r--r--   0        0        0     2047 2023-12-11 19:29:35.517640 censusdis-1.1.6/censusdis/places/delaware.py
+-rw-r--r--   0        0        0      108 2023-12-11 19:29:35.517800 censusdis-1.1.6/censusdis/places/district_of_columbia.py
+-rw-r--r--   0        0        0    25466 2023-12-11 19:29:35.518158 censusdis-1.1.6/censusdis/places/florida.py
+-rw-r--r--   0        0        0    16652 2023-12-11 19:29:35.518343 censusdis-1.1.6/censusdis/places/georgia.py
+-rw-r--r--   0        0        0     4060 2023-12-11 19:29:35.518467 censusdis-1.1.6/censusdis/places/hawaii.py
+-rw-r--r--   0        0        0     5685 2023-12-11 19:29:35.518634 censusdis-1.1.6/censusdis/places/idaho.py
+-rw-r--r--   0        0        0    38933 2023-12-11 19:29:35.519027 censusdis-1.1.6/censusdis/places/illinois.py
+-rw-r--r--   0        0        0    23926 2023-12-11 19:29:35.519320 censusdis-1.1.6/censusdis/places/indiana.py
+-rw-r--r--   0        0        0    24633 2023-12-11 19:29:35.519626 censusdis-1.1.6/censusdis/places/iowa.py
+-rw-r--r--   0        0        0    17556 2023-12-11 19:29:35.519874 censusdis-1.1.6/censusdis/places/kansas.py
+-rw-r--r--   0        0        0    14063 2023-12-11 19:29:35.520117 censusdis-1.1.6/censusdis/places/kentucky.py
+-rw-r--r--   0        0        0    12119 2023-12-11 19:29:35.520465 censusdis-1.1.6/censusdis/places/louisiana.py
+-rw-r--r--   0        0        0     3818 2023-12-11 19:29:35.520594 censusdis-1.1.6/censusdis/places/maine.py
+-rw-r--r--   0        0        0    13853 2023-12-11 19:29:35.520760 censusdis-1.1.6/censusdis/places/maryland.py
+-rw-r--r--   0        0        0     6351 2023-12-11 19:29:35.520935 censusdis-1.1.6/censusdis/places/massachusetts.py
+-rw-r--r--   0        0        0    19186 2023-12-11 19:29:35.521108 censusdis-1.1.6/censusdis/places/michigan.py
+-rw-r--r--   0        0        0    22227 2023-12-11 19:29:35.521432 censusdis-1.1.6/censusdis/places/minnesota.py
+-rw-r--r--   0        0        0    10406 2023-12-11 19:29:35.521602 censusdis-1.1.6/censusdis/places/mississippi.py
+-rw-r--r--   0        0        0    27499 2023-12-11 19:29:35.521942 censusdis-1.1.6/censusdis/places/missouri.py
+-rw-r--r--   0        0        0    12297 2023-12-11 19:29:35.522122 censusdis-1.1.6/censusdis/places/montana.py
+-rw-r--r--   0        0        0    14951 2023-12-11 19:29:35.522289 censusdis-1.1.6/censusdis/places/nebraska.py
+-rw-r--r--   0        0        0     3341 2023-12-11 19:29:35.522400 censusdis-1.1.6/censusdis/places/nevada.py
+-rw-r--r--   0        0        0     2504 2023-12-11 19:29:35.522517 censusdis-1.1.6/censusdis/places/new_hampshire.py
+-rw-r--r--   0        0        0    19179 2023-12-11 19:29:35.522722 censusdis-1.1.6/censusdis/places/new_jersey.py
+-rw-r--r--   0        0        0    13434 2023-12-11 19:29:35.522891 censusdis-1.1.6/censusdis/places/new_mexico.py
+-rw-r--r--   0        0        0    34855 2023-12-11 19:29:35.523211 censusdis-1.1.6/censusdis/places/new_york.py
+-rw-r--r--   0        0        0    19432 2023-12-11 19:29:35.523418 censusdis-1.1.6/censusdis/places/north_carolina.py
+-rw-r--r--   0        0        0     9524 2023-12-11 19:29:35.523558 censusdis-1.1.6/censusdis/places/north_dakota.py
+-rw-r--r--   0        0        0    34277 2023-12-11 19:29:35.523920 censusdis-1.1.6/censusdis/places/ohio.py
+-rw-r--r--   0        0        0    19802 2023-12-11 19:29:35.524122 censusdis-1.1.6/censusdis/places/oklahoma.py
+-rw-r--r--   0        0        0    10398 2023-12-11 19:29:35.524366 censusdis-1.1.6/censusdis/places/oregon.py
+-rw-r--r--   0        0        0    51324 2023-12-11 19:29:35.524811 censusdis-1.1.6/censusdis/places/pennsylvania.py
+-rw-r--r--   0        0        0     9391 2023-12-11 19:29:35.524961 censusdis-1.1.6/censusdis/places/puerto_rico.py
+-rw-r--r--   0        0        0      985 2023-12-11 19:29:35.525076 censusdis-1.1.6/censusdis/places/rhode_island.py
+-rw-r--r--   0        0        0    11708 2023-12-11 19:29:35.525311 censusdis-1.1.6/censusdis/places/south_carolina.py
+-rw-r--r--   0        0        0    12094 2023-12-11 19:29:35.525524 censusdis-1.1.6/censusdis/places/south_dakota.py
+-rw-r--r--   0        0        0    12647 2023-12-11 19:29:35.525795 censusdis-1.1.6/censusdis/places/tennessee.py
+-rw-r--r--   0        0        0    46473 2023-12-11 19:29:35.526090 censusdis-1.1.6/censusdis/places/texas.py
+-rw-r--r--   0        0        0     8246 2023-12-11 19:29:35.526224 censusdis-1.1.6/censusdis/places/utah.py
+-rw-r--r--   0        0        0     4712 2023-12-11 19:29:35.526351 censusdis-1.1.6/censusdis/places/vermont.py
+-rw-r--r--   0        0        0    17023 2023-12-11 19:29:35.526524 censusdis-1.1.6/censusdis/places/virginia.py
+-rw-r--r--   0        0        0    15869 2023-12-11 19:29:35.526833 censusdis-1.1.6/censusdis/places/washington.py
+-rw-r--r--   0        0        0    10717 2023-12-11 19:29:35.526982 censusdis-1.1.6/censusdis/places/west_virginia.py
+-rw-r--r--   0        0        0    20957 2023-12-11 19:29:35.527184 censusdis-1.1.6/censusdis/places/wisconsin.py
+-rw-r--r--   0        0        0     5030 2023-12-11 19:29:35.527313 censusdis-1.1.6/censusdis/places/wyoming.py
+-rw-r--r--   0        0        0      140 2023-12-11 20:36:13.710754 censusdis-1.1.6/censusdis/region.py
+-rw-r--r--   0        0        0       70 2023-12-04 22:25:55.364310 censusdis-1.1.6/censusdis/resources/__init__.py
+-rw-r--r--   0        0        0    25951 2023-05-29 16:16:27.245353 censusdis-1.1.6/censusdis/resources/crs_bounds.geojson
+-rw-r--r--   0        0        0     7192 2023-12-04 21:03:55.744421 censusdis-1.1.6/censusdis/states.py
+-rw-r--r--   0        0        0     2399 2023-05-29 16:16:27.245539 censusdis-1.1.6/censusdis/values.py
+-rw-r--r--   0        0        0     4053 2024-04-29 21:54:14.552850 censusdis-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5916 1970-01-01 00:00:00.000000 censusdis-1.1.6/PKG-INFO
```

### Comparing `censusdis-1.1.5/LICENSE.md` & `censusdis-1.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/README.md` & `censusdis-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/.DS_Store` & `censusdis-1.1.6/censusdis/.DS_Store`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/cli/cli.py` & `censusdis-1.1.6/censusdis/cli/cli.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/cli/yamlspec.py` & `censusdis-1.1.6/censusdis/cli/yamlspec.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/alabama.py` & `censusdis-1.1.6/censusdis/counties/alabama.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/alaska.py` & `censusdis-1.1.6/censusdis/counties/alaska.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/arkansas.py` & `censusdis-1.1.6/censusdis/counties/arkansas.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/california.py` & `censusdis-1.1.6/censusdis/counties/california.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/colorado.py` & `censusdis-1.1.6/censusdis/counties/colorado.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/connecticut.py` & `censusdis-1.1.6/censusdis/counties/connecticut.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/florida.py` & `censusdis-1.1.6/censusdis/counties/florida.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/georgia.py` & `censusdis-1.1.6/censusdis/counties/georgia.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/idaho.py` & `censusdis-1.1.6/censusdis/counties/idaho.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/illinois.py` & `censusdis-1.1.6/censusdis/counties/illinois.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/indiana.py` & `censusdis-1.1.6/censusdis/counties/indiana.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/iowa.py` & `censusdis-1.1.6/censusdis/counties/iowa.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/kansas.py` & `censusdis-1.1.6/censusdis/counties/kansas.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/kentucky.py` & `censusdis-1.1.6/censusdis/counties/kentucky.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/louisiana.py` & `censusdis-1.1.6/censusdis/counties/louisiana.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/michigan.py` & `censusdis-1.1.6/censusdis/counties/michigan.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/minnesota.py` & `censusdis-1.1.6/censusdis/counties/minnesota.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/mississippi.py` & `censusdis-1.1.6/censusdis/counties/mississippi.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/missouri.py` & `censusdis-1.1.6/censusdis/counties/missouri.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/montana.py` & `censusdis-1.1.6/censusdis/counties/montana.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/nebraska.py` & `censusdis-1.1.6/censusdis/counties/nebraska.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/new_mexico.py` & `censusdis-1.1.6/censusdis/counties/new_mexico.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/new_york.py` & `censusdis-1.1.6/censusdis/counties/new_york.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/north_carolina.py` & `censusdis-1.1.6/censusdis/counties/north_carolina.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/north_dakota.py` & `censusdis-1.1.6/censusdis/counties/north_dakota.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/ohio.py` & `censusdis-1.1.6/censusdis/counties/ohio.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/oklahoma.py` & `censusdis-1.1.6/censusdis/counties/oklahoma.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/oregon.py` & `censusdis-1.1.6/censusdis/counties/oregon.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/pennsylvania.py` & `censusdis-1.1.6/censusdis/counties/pennsylvania.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/puerto_rico.py` & `censusdis-1.1.6/censusdis/counties/puerto_rico.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/south_carolina.py` & `censusdis-1.1.6/censusdis/counties/south_carolina.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/south_dakota.py` & `censusdis-1.1.6/censusdis/counties/south_dakota.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/tennessee.py` & `censusdis-1.1.6/censusdis/counties/tennessee.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/texas.py` & `censusdis-1.1.6/censusdis/counties/texas.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/virginia.py` & `censusdis-1.1.6/censusdis/counties/virginia.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/washington.py` & `censusdis-1.1.6/censusdis/counties/washington.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/west_virginia.py` & `censusdis-1.1.6/censusdis/counties/west_virginia.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/counties/wisconsin.py` & `censusdis-1.1.6/censusdis/counties/wisconsin.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/csa.py` & `censusdis-1.1.6/censusdis/csa.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/data.py` & `censusdis-1.1.6/censusdis/data.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/datasets.py` & `censusdis-1.1.6/censusdis/datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,57 +98,117 @@
 
 CFSHAZMAT = "cfshazmat"
 
 CFSPRELIM = "cfsprelim"
 
 CFSTEMP = "cfstemp"
 
-CPS_ARTS = "cps/arts/feb"
+CPS_ARTS_FEB = "cps/arts/feb"
 
-CPS_ASEC = "cps/asec/mar"
+CPS_ASEC_MAR = "cps/asec/mar"
 
-CPS_BASIC = "cps/basic/jan"
+CPS_BASIC_APR = "cps/basic/apr"
 
-CPS_CIVIC = "cps/civic/nov"
+CPS_BASIC_AUG = "cps/basic/aug"
 
-CPS_CONTWORKER = "cps/contworker/may"
+CPS_BASIC_DEC = "cps/basic/dec"
 
-CPS_DISABILITY = "cps/disability/jul"
+CPS_BASIC_FEB = "cps/basic/feb"
 
-CPS_DWJT = "cps/dwjt/jan"
+CPS_BASIC_JAN = "cps/basic/jan"
 
-CPS_FERTILITY = "cps/fertility/jun"
+CPS_BASIC_JUL = "cps/basic/jul"
 
-CPS_FOODSEC = "cps/foodsec/dec"
+CPS_BASIC_JUN = "cps/basic/jun"
 
-CPS_IMMIGRATION = "cps/immigration/aug"
+CPS_BASIC_MAR = "cps/basic/mar"
 
-CPS_INTERNET = "cps/internet/nov"
+CPS_BASIC_MAY = "cps/basic/may"
 
-CPS_LIBRARY = "cps/library/oct"
+CPS_BASIC_NOV = "cps/basic/nov"
 
-CPS_MARITAL = "cps/marital/jun"
+CPS_BASIC_OCT = "cps/basic/oct"
 
-CPS_PUBARTS = "cps/pubarts/jul"
+CPS_BASIC_SEP = "cps/basic/sep"
 
-CPS_RACE = "cps/race/may"
+CPS_CIVIC_NOV = "cps/civic/nov"
 
-CPS_SCHOOL = "cps/school/oct"
+CPS_CONTWORKER_FEB = "cps/contworker/feb"
 
-CPS_TOBACCO = "cps/tobacco/may"
+CPS_CONTWORKER_MAY = "cps/contworker/may"
 
-CPS_UNBANK = "cps/unbank/jun"
+CPS_DISABILITY_JUL = "cps/disability/jul"
 
-CPS_VETS = "cps/vets/aug"
+CPS_DISABILITY_MAY = "cps/disability/may"
 
-CPS_VOLUNTEER = "cps/volunteer/sep"
+CPS_DWJT_FEB = "cps/dwjt/feb"
 
-CPS_VOTING = "cps/voting/nov"
+CPS_DWJT_JAN = "cps/dwjt/jan"
 
-CPS_WORKSCHED = "cps/worksched/may"
+CPS_FERTILITY_JUN = "cps/fertility/jun"
+
+CPS_FOODSEC_APR = "cps/foodsec/apr"
+
+CPS_FOODSEC_AUG = "cps/foodsec/aug"
+
+CPS_FOODSEC_DEC = "cps/foodsec/dec"
+
+CPS_FOODSEC_SEP = "cps/foodsec/sep"
+
+CPS_IMMIGRATION_AUG = "cps/immigration/aug"
+
+CPS_INTERNET_AUG = "cps/internet/aug"
+
+CPS_INTERNET_DEC = "cps/internet/dec"
+
+CPS_INTERNET_JUL = "cps/internet/jul"
+
+CPS_INTERNET_NOV = "cps/internet/nov"
+
+CPS_INTERNET_OCT = "cps/internet/oct"
+
+CPS_INTERNET_SEP = "cps/internet/sep"
+
+CPS_LIBRARY_OCT = "cps/library/oct"
+
+CPS_MARITAL_JUN = "cps/marital/jun"
+
+CPS_PUBARTS_AUG = "cps/pubarts/aug"
+
+CPS_PUBARTS_JUL = "cps/pubarts/jul"
+
+CPS_RACE_MAY = "cps/race/may"
+
+CPS_SCHOOL_OCT = "cps/school/oct"
+
+CPS_TOBACCO_AUG = "cps/tobacco/aug"
+
+CPS_TOBACCO_JAN = "cps/tobacco/jan"
+
+CPS_TOBACCO_JUL = "cps/tobacco/jul"
+
+CPS_TOBACCO_MAY = "cps/tobacco/may"
+
+CPS_TOBACCO_SEP = "cps/tobacco/sep"
+
+CPS_UNBANK_JAN = "cps/unbank/jan"
+
+CPS_UNBANK_JUN = "cps/unbank/jun"
+
+CPS_VETS_AUG = "cps/vets/aug"
+
+CPS_VETS_JUL = "cps/vets/jul"
+
+CPS_VETS_SEP = "cps/vets/sep"
+
+CPS_VOLUNTEER_SEP = "cps/volunteer/sep"
+
+CPS_VOTING_NOV = "cps/voting/nov"
+
+CPS_WORKSCHED_MAY = "cps/worksched/may"
 
 CRE = "cre"
 
 DECENNIAL_AIAN = "dec/aian"
 
 DECENNIAL_AIANPROFILE = "dec/aianprofile"
 
@@ -496,14 +556,16 @@
 
 SBO_CS = "sbo/cs"
 
 SBO_CSCB = "sbo/cscb"
 
 SBO_CSCBO = "sbo/cscbo"
 
+SIPP_BENEFIT = "sipp/benefit/1991panel"
+
 SIPP_CORE = "sipp/core/2008panel/wave9"
 
 SIPP_TOPICAL = "sipp/topical/2008panel/wave9"
 
 SIPP_TOPICALED = "sipp/topicaled/1993panel/wave8"
 
 SIPP_TOPICALEDEX = "sipp/topicaledex/1993panel/wave8"
@@ -593,36 +655,66 @@
     ASE_CSCBO: "http://api.census.gov/data/2016/ase/cscbo",
     CBP: "http://api.census.gov/data/2021/cbp",
     CFSAREA: "http://api.census.gov/data/2017/cfsarea",
     CFSEXPORT: "http://api.census.gov/data/2017/cfsexport",
     CFSHAZMAT: "http://api.census.gov/data/2017/cfshazmat",
     CFSPRELIM: "http://api.census.gov/data/2017/cfsprelim",
     CFSTEMP: "http://api.census.gov/data/2017/cfstemp",
-    CPS_ARTS: "http://api.census.gov/data/2020/cps/arts/feb",
-    CPS_ASEC: "http://api.census.gov/data/2023/cps/asec/mar",
-    CPS_BASIC: "http://api.census.gov/data/2024/cps/basic/jan",
-    CPS_CIVIC: "http://api.census.gov/data/2013/cps/civic/nov",
-    CPS_CONTWORKER: "http://api.census.gov/data/2017/cps/contworker/may",
-    CPS_DISABILITY: "http://api.census.gov/data/2021/cps/disability/jul",
-    CPS_DWJT: "http://api.census.gov/data/2022/cps/dwjt/jan",
-    CPS_FERTILITY: "http://api.census.gov/data/2022/cps/fertility/jun",
-    CPS_FOODSEC: "http://api.census.gov/data/2022/cps/foodsec/dec",
-    CPS_IMMIGRATION: "http://api.census.gov/data/2008/cps/immigration/aug",
-    CPS_INTERNET: "http://api.census.gov/data/2021/cps/internet/nov",
-    CPS_LIBRARY: "http://api.census.gov/data/2002/cps/library/oct",
-    CPS_MARITAL: "http://api.census.gov/data/1995/cps/marital/jun",
-    CPS_PUBARTS: "http://api.census.gov/data/2022/cps/pubarts/jul",
-    CPS_RACE: "http://api.census.gov/data/1995/cps/race/may",
-    CPS_SCHOOL: "http://api.census.gov/data/2022/cps/school/oct",
-    CPS_TOBACCO: "http://api.census.gov/data/2019/cps/tobacco/may",
-    CPS_UNBANK: "http://api.census.gov/data/2021/cps/unbank/jun",
-    CPS_VETS: "http://api.census.gov/data/2022/cps/vets/aug",
-    CPS_VOLUNTEER: "http://api.census.gov/data/2021/cps/volunteer/sep",
-    CPS_VOTING: "http://api.census.gov/data/2022/cps/voting/nov",
-    CPS_WORKSCHED: "http://api.census.gov/data/2004/cps/worksched/may",
+    CPS_ARTS_FEB: "http://api.census.gov/data/2020/cps/arts/feb",
+    CPS_ASEC_MAR: "http://api.census.gov/data/2023/cps/asec/mar",
+    CPS_BASIC_APR: "http://api.census.gov/data/2023/cps/basic/apr",
+    CPS_BASIC_AUG: "http://api.census.gov/data/2023/cps/basic/aug",
+    CPS_BASIC_DEC: "http://api.census.gov/data/2023/cps/basic/dec",
+    CPS_BASIC_FEB: "http://api.census.gov/data/2024/cps/basic/feb",
+    CPS_BASIC_JAN: "http://api.census.gov/data/2024/cps/basic/jan",
+    CPS_BASIC_JUL: "http://api.census.gov/data/2023/cps/basic/jul",
+    CPS_BASIC_JUN: "http://api.census.gov/data/2023/cps/basic/jun",
+    CPS_BASIC_MAR: "http://api.census.gov/data/2024/cps/basic/mar",
+    CPS_BASIC_MAY: "http://api.census.gov/data/2023/cps/basic/may",
+    CPS_BASIC_NOV: "http://api.census.gov/data/2023/cps/basic/nov",
+    CPS_BASIC_OCT: "http://api.census.gov/data/2023/cps/basic/oct",
+    CPS_BASIC_SEP: "http://api.census.gov/data/2023/cps/basic/sep",
+    CPS_CIVIC_NOV: "http://api.census.gov/data/2013/cps/civic/nov",
+    CPS_CONTWORKER_FEB: "http://api.census.gov/data/2005/cps/contworker/feb",
+    CPS_CONTWORKER_MAY: "http://api.census.gov/data/2017/cps/contworker/may",
+    CPS_DISABILITY_JUL: "http://api.census.gov/data/2021/cps/disability/jul",
+    CPS_DISABILITY_MAY: "http://api.census.gov/data/2012/cps/disability/may",
+    CPS_DWJT_FEB: "http://api.census.gov/data/2000/cps/dwjt/feb",
+    CPS_DWJT_JAN: "http://api.census.gov/data/2022/cps/dwjt/jan",
+    CPS_FERTILITY_JUN: "http://api.census.gov/data/2022/cps/fertility/jun",
+    CPS_FOODSEC_APR: "http://api.census.gov/data/2001/cps/foodsec/apr",
+    CPS_FOODSEC_AUG: "http://api.census.gov/data/1998/cps/foodsec/aug",
+    CPS_FOODSEC_DEC: "http://api.census.gov/data/2022/cps/foodsec/dec",
+    CPS_FOODSEC_SEP: "http://api.census.gov/data/2000/cps/foodsec/sep",
+    CPS_IMMIGRATION_AUG: "http://api.census.gov/data/2008/cps/immigration/aug",
+    CPS_INTERNET_AUG: "http://api.census.gov/data/2000/cps/internet/aug",
+    CPS_INTERNET_DEC: "http://api.census.gov/data/1998/cps/internet/dec",
+    CPS_INTERNET_JUL: "http://api.census.gov/data/2015/cps/internet/jul",
+    CPS_INTERNET_NOV: "http://api.census.gov/data/2021/cps/internet/nov",
+    CPS_INTERNET_OCT: "http://api.census.gov/data/2012/cps/internet/oct",
+    CPS_INTERNET_SEP: "http://api.census.gov/data/2001/cps/internet/sep",
+    CPS_LIBRARY_OCT: "http://api.census.gov/data/2002/cps/library/oct",
+    CPS_MARITAL_JUN: "http://api.census.gov/data/1995/cps/marital/jun",
+    CPS_PUBARTS_AUG: "http://api.census.gov/data/2002/cps/pubarts/aug",
+    CPS_PUBARTS_JUL: "http://api.census.gov/data/2022/cps/pubarts/jul",
+    CPS_RACE_MAY: "http://api.census.gov/data/1995/cps/race/may",
+    CPS_SCHOOL_OCT: "http://api.census.gov/data/2022/cps/school/oct",
+    CPS_TOBACCO_AUG: "http://api.census.gov/data/2010/cps/tobacco/aug",
+    CPS_TOBACCO_JAN: "http://api.census.gov/data/2019/cps/tobacco/jan",
+    CPS_TOBACCO_JUL: "http://api.census.gov/data/2018/cps/tobacco/jul",
+    CPS_TOBACCO_MAY: "http://api.census.gov/data/2019/cps/tobacco/may",
+    CPS_TOBACCO_SEP: "http://api.census.gov/data/2022/cps/tobacco/sep",
+    CPS_UNBANK_JAN: "http://api.census.gov/data/2009/cps/unbank/jan",
+    CPS_UNBANK_JUN: "http://api.census.gov/data/2021/cps/unbank/jun",
+    CPS_VETS_AUG: "http://api.census.gov/data/2023/cps/vets/aug",
+    CPS_VETS_JUL: "http://api.census.gov/data/2010/cps/vets/jul",
+    CPS_VETS_SEP: "http://api.census.gov/data/1999/cps/vets/sep",
+    CPS_VOLUNTEER_SEP: "http://api.census.gov/data/2021/cps/volunteer/sep",
+    CPS_VOTING_NOV: "http://api.census.gov/data/2022/cps/voting/nov",
+    CPS_WORKSCHED_MAY: "http://api.census.gov/data/2004/cps/worksched/may",
     CRE: "http://api.census.gov/data/2022/cre",
     DECENNIAL_AIAN: "http://api.census.gov/data/2010/dec/aian",
     DECENNIAL_AIANPROFILE: "http://api.census.gov/data/2000/dec/aianprofile",
     DECENNIAL_AS: "http://api.census.gov/data/2010/dec/as",
     DECENNIAL_ASYOE: "http://api.census.gov/data/2010/dec/asyoe",
     DECENNIAL_CD110H: "http://api.census.gov/data/2000/dec/cd110h",
     DECENNIAL_CD110HPROFILE: "http://api.census.gov/data/2000/dec/cd110hprofile",
@@ -792,14 +884,15 @@
     POPPROJ_DEATHS: "http://api.census.gov/data/2017/popproj/deaths",
     POPPROJ_NAT: "http://api.census.gov/data/2017/popproj/nat",
     POPPROJ_NIM: "http://api.census.gov/data/2017/popproj/nim",
     PUBLIC_PK12_EDUCATION_FINANCE: "http://api.census.gov/data/2012/pubschlfin",
     SBO_CS: "http://api.census.gov/data/2012/sbo/cs",
     SBO_CSCB: "http://api.census.gov/data/2012/sbo/cscb",
     SBO_CSCBO: "http://api.census.gov/data/2012/sbo/cscbo",
+    SIPP_BENEFIT: "http://api.census.gov/data/1991/sipp/benefit/1991panel",
     SIPP_CORE: "http://api.census.gov/data/2008/sipp/core/2008panel/wave9",
     SIPP_TOPICAL: "http://api.census.gov/data/2008/sipp/topical/2008panel/wave9",
     SIPP_TOPICALED: "http://api.census.gov/data/1993/sipp/topicaled/1993panel/wave8",
     SIPP_TOPICALEDEX: "http://api.census.gov/data/1993/sipp/topicaledex/1993panel/wave8",
     SIPP_TOPICALEX: "http://api.census.gov/data/1993/sipp/topicalex/1993panel/wave3",
     SIPP_TOPICALRES: "http://api.census.gov/data/2001/sipp/topicalres/2001panel/wave8",
     TIMESERIES_ASM: "http://api.census.gov/data/timeseries/asm/value2017",
```

### Comparing `censusdis-1.1.5/censusdis/geography.py` & `censusdis-1.1.6/censusdis/geography.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/impl/fetch.py` & `censusdis-1.1.6/censusdis/impl/fetch.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/impl/geometry.py` & `censusdis-1.1.6/censusdis/impl/geometry.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/impl/us_census_shapefiles.py` & `censusdis-1.1.6/censusdis/impl/us_census_shapefiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 
 _GEO_QUERY_FROM_DATA_QUERY_INNER_GEO: Dict[
     str,
     Callable[[int], Tuple[Optional[str], str, List[str], List[str]]],
 ] = {
     # innermost geo: ( shapefile_scope, shapefile_geo_name, df_on, gdf_on )
+    "us": lambda year: ("us", "nation", ["US"], ["US"]),
     "region": lambda year: ("us", "region", ["REGION"], ["REGIONCE"]),
     "division": lambda year: ("us", "division", ["DIVISION"], ["DIVISIONCE"]),
     "combined statistical area": lambda year: (
         "us",
         "csa",
         ["COMBINED_STATISTICAL_AREA"],
         ["CSAFP"],
@@ -369,17 +370,19 @@
 
     # If the query spec has a hard-coded value then we use it.
     if query_shapefile_scope is not None:
         shapefile_scope = query_shapefile_scope
 
     def individual_shapefile(sub_scope: str, query_year: int) -> gpd.GeoDataFrame:
         """Read the relevant shapefile and add a YEAR column to it."""
+        resolution = "5m" if shapefile_geo_level == "nation" else "500k"
+
         try:
             gdf = __shapefile_reader(query_year).try_cb_tiger_shapefile(
-                sub_scope, shapefile_geo_level
+                sub_scope, shapefile_geo_level, resolution=resolution
             )
             gdf["YEAR"] = query_year
             return gdf
         except cmap.MapException as ex:
             # If there are some years where we can't find a shapefile,
             # skip over it and those rows will not have geometry in the
             # final result.
@@ -392,15 +395,15 @@
             return gpd.GeoDataFrame()
 
     # If there is a single defined year then we can load the single
     # shapefile. If not, then we have to load multiple shapefiles,
     # one per year, and concatenate them.
     #
     # Whether there is a single or multiple years, there could also
-    # me mutliple scopes, e.g. states, for which we have to download
+    # me multiple scopes, e.g. states, for which we have to download
     # shapefiles. If so, by the time we get here, they are encoded in
     # one string with comma separators.
     if isinstance(year, int):
         gdf_shapefile = pd.concat(
             individual_shapefile(sub_scope, year)
             for sub_scope in shapefile_scope.split(",")
         )
@@ -422,14 +425,19 @@
         return gdf
 
     if "TRACT" in df_data.columns:
         df_data["TRACT"] = df_data["TRACT"].str.ljust(
             6, "0"
         )  # Pre 2010 data has inconsistencies in TRACT string length
 
+    # The nation-level shapefile is missing a column
+    # to merge on.
+    if shapefile_geo_level == "nation":
+        gdf_shapefile["US"] = "1"
+
     gdf_data = gdf_shapefile[merge_gdf_on + ["geometry"]].merge(
         df_data, how="right", left_on=merge_gdf_on, right_on=df_on
     )
 
     # Get the columns we want in a reasonable order matching
     # how they are in the data, with geometry at the end.
     gdf_data = gdf_data[list(df_data.columns) + ["geometry"]]
```

### Comparing `censusdis-1.1.5/censusdis/impl/varcache.py` & `censusdis-1.1.6/censusdis/impl/varcache.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 import numpy as np
 import pandas as pd
 
 from censusdis.impl.varsource.base import VariableSource
 from censusdis.impl.varsource.censusapi import CensusApiVariableSource
 
+import censusdis.datasets
+
+
 logger = getLogger(__name__)
 
 
 class VariableCache:
     """
     A cache of variables and groups.
 
@@ -390,14 +393,34 @@
                         if dataset.get("distribution")
                         else None
                     ),
                 }
                 for dataset in datasets
             ]
         )
+
+        symbol_dict_reversed = {
+            value: symbol
+            for symbol, value in censusdis.datasets.__dict__.items()
+            if isinstance(value, str)
+        }
+
+        df_datasets["SYMBOL"] = df_datasets["DATASET"].apply(
+            lambda name: symbol_dict_reversed.get(name, None)
+        )
+
+        df_datasets = df_datasets[
+            ["YEAR", "SYMBOL", "DATASET"]
+            + [
+                col
+                for col in df_datasets.columns
+                if col not in ["YEAR", "SYMBOL", "DATASET"]
+            ]
+        ]
+
         return df_datasets.sort_values(["YEAR", "DATASET"]).reset_index(drop=True)
 
     def all_data_sets(self, *, year: Optional[int] = None) -> pd.DataFrame:
         """
         Retrieve a description of available data sets.
 
         Parameters
```

### Comparing `censusdis-1.1.5/censusdis/impl/varsource/base.py` & `censusdis-1.1.6/censusdis/impl/varsource/base.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/impl/varsource/censusapi.py` & `censusdis-1.1.6/censusdis/impl/varsource/censusapi.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/maps.py` & `censusdis-1.1.6/censusdis/maps.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/msa_msa.py` & `censusdis-1.1.6/censusdis/msa_msa.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/alabama.py` & `censusdis-1.1.6/censusdis/places/alabama.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/alaska.py` & `censusdis-1.1.6/censusdis/places/alaska.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/arizona.py` & `censusdis-1.1.6/censusdis/places/arizona.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/arkansas.py` & `censusdis-1.1.6/censusdis/places/arkansas.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/california.py` & `censusdis-1.1.6/censusdis/places/california.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/colorado.py` & `censusdis-1.1.6/censusdis/places/colorado.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/connecticut.py` & `censusdis-1.1.6/censusdis/places/connecticut.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/delaware.py` & `censusdis-1.1.6/censusdis/places/delaware.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/florida.py` & `censusdis-1.1.6/censusdis/places/florida.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/georgia.py` & `censusdis-1.1.6/censusdis/places/georgia.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/hawaii.py` & `censusdis-1.1.6/censusdis/places/hawaii.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/idaho.py` & `censusdis-1.1.6/censusdis/places/idaho.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/illinois.py` & `censusdis-1.1.6/censusdis/places/illinois.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/indiana.py` & `censusdis-1.1.6/censusdis/places/indiana.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/iowa.py` & `censusdis-1.1.6/censusdis/places/iowa.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/kansas.py` & `censusdis-1.1.6/censusdis/places/kansas.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/kentucky.py` & `censusdis-1.1.6/censusdis/places/kentucky.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/louisiana.py` & `censusdis-1.1.6/censusdis/places/louisiana.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/maine.py` & `censusdis-1.1.6/censusdis/places/maine.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/maryland.py` & `censusdis-1.1.6/censusdis/places/maryland.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/massachusetts.py` & `censusdis-1.1.6/censusdis/places/massachusetts.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/michigan.py` & `censusdis-1.1.6/censusdis/places/michigan.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/minnesota.py` & `censusdis-1.1.6/censusdis/places/minnesota.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/mississippi.py` & `censusdis-1.1.6/censusdis/places/mississippi.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/missouri.py` & `censusdis-1.1.6/censusdis/places/missouri.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/montana.py` & `censusdis-1.1.6/censusdis/places/montana.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/nebraska.py` & `censusdis-1.1.6/censusdis/places/nebraska.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/nevada.py` & `censusdis-1.1.6/censusdis/places/nevada.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/new_hampshire.py` & `censusdis-1.1.6/censusdis/places/new_hampshire.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/new_jersey.py` & `censusdis-1.1.6/censusdis/places/new_jersey.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/new_mexico.py` & `censusdis-1.1.6/censusdis/places/new_mexico.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/new_york.py` & `censusdis-1.1.6/censusdis/places/new_york.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/north_carolina.py` & `censusdis-1.1.6/censusdis/places/north_carolina.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/north_dakota.py` & `censusdis-1.1.6/censusdis/places/north_dakota.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/ohio.py` & `censusdis-1.1.6/censusdis/places/ohio.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/oklahoma.py` & `censusdis-1.1.6/censusdis/places/oklahoma.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/oregon.py` & `censusdis-1.1.6/censusdis/places/oregon.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/pennsylvania.py` & `censusdis-1.1.6/censusdis/places/pennsylvania.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/puerto_rico.py` & `censusdis-1.1.6/censusdis/places/puerto_rico.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/rhode_island.py` & `censusdis-1.1.6/censusdis/places/rhode_island.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/south_carolina.py` & `censusdis-1.1.6/censusdis/places/south_carolina.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/south_dakota.py` & `censusdis-1.1.6/censusdis/places/south_dakota.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/tennessee.py` & `censusdis-1.1.6/censusdis/places/tennessee.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/texas.py` & `censusdis-1.1.6/censusdis/places/texas.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/utah.py` & `censusdis-1.1.6/censusdis/places/utah.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/vermont.py` & `censusdis-1.1.6/censusdis/places/vermont.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/virginia.py` & `censusdis-1.1.6/censusdis/places/virginia.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/washington.py` & `censusdis-1.1.6/censusdis/places/washington.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/west_virginia.py` & `censusdis-1.1.6/censusdis/places/west_virginia.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/wisconsin.py` & `censusdis-1.1.6/censusdis/places/wisconsin.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/places/wyoming.py` & `censusdis-1.1.6/censusdis/places/wyoming.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/resources/crs_bounds.geojson` & `censusdis-1.1.6/censusdis/resources/crs_bounds.geojson`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/states.py` & `censusdis-1.1.6/censusdis/states.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/censusdis/values.py` & `censusdis-1.1.6/censusdis/values.py`

 * *Files identical despite different names*

### Comparing `censusdis-1.1.5/PKG-INFO` & `censusdis-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censusdis
-Version: 1.1.5
+Version: 1.1.6
 Summary: US Census utilities for a variety of data loading, analysis, and mapping purposes.
 Home-page: https://github.com/vengroff/censusdis
 License: HL3-CL-ECO-EXTR-FFD-LAW-MIL-SV
 Keywords: census,demographics
 Author: Darren Vengroff
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -23,25 +23,26 @@
 Requires-Dist: Fiona (>=1.9.0,<2.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: Rtree (>=1.0.0,<2.0.0)
 Requires-Dist: Sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
 Requires-Dist: adjustText (>=0.8,<0.9)
 Requires-Dist: contextily (>=1.3.0,<2.0.0)
 Requires-Dist: divintseg (>=0.6.1,<0.7.0)
-Requires-Dist: folium (>=0.15.1,<0.16.0) ; extra == "explore"
+Requires-Dist: folium (>=0.16.0,<0.17.0) ; extra == "explore"
 Requires-Dist: geopandas (>=0.14.1,<0.15.0)
 Requires-Dist: geopy (>=2.2.0,<3.0.0)
 Requires-Dist: haversine (>=2.8.0,<3.0.0)
-Requires-Dist: ipyleaflet (>=0.18.2,<0.19.0) ; extra == "explore"
+Requires-Dist: ipyleaflet (>=0.19.0,<0.20.0) ; extra == "explore"
 Requires-Dist: logargparser (>=0.1.1,<0.2.0)
 Requires-Dist: mapclassify (>=2.6.1,<3.0.0) ; extra == "explore"
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: nbsphinx (>=0.9.3,<0.10.0)
-Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
+Requires-Dist: pyarrow (>=16.0.0,<17.0.0)
 Requires-Dist: pyogrio (>=0.7.2,<0.8.0)
+Requires-Dist: rasterio (==1.3.9)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: sphinx-copybutton (>=0.5.1,<0.6.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (==2.0.0) ; extra == "docs"
 Requires-Dist: sphinxcontrib-napoleon (==0.7) ; extra == "docs"
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "docs"
 Requires-Dist: usingversion (>=0.1.1,<0.2.0)
 Project-URL: Repository, https://github.com/vengroff/censusdis
```

