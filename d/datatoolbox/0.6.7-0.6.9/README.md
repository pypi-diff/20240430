# Comparing `tmp/datatoolbox-0.6.7.tar.gz` & `tmp/datatoolbox-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatoolbox-0.6.7.tar", last modified: Mon Apr 22 08:25:38 2024, max compression
+gzip compressed data, was "datatoolbox-0.6.9.tar", last modified: Tue Apr 30 07:55:20 2024, max compression
```

## Comparing `datatoolbox-0.6.7.tar` & `datatoolbox-0.6.9.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.279337 datatoolbox-0.6.7/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      159 2022-05-25 07:15:53.000000 datatoolbox-0.6.7/.gitignore
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      950 2022-10-19 13:17:33.000000 datatoolbox-0.6.7/.gitlab-ci.yml
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      703 2020-10-14 14:04:18.000000 datatoolbox-0.6.7/.travis.yml
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1073 2020-10-14 14:04:18.000000 datatoolbox-0.6.7/LICENSE
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1564 2024-04-22 08:25:38.279006 datatoolbox-0.6.7/PKG-INFO
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1298 2023-09-22 10:59:58.000000 datatoolbox-0.6.7/README.md
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1225 2020-10-14 14:04:18.000000 datatoolbox-0.6.7/appveyor.yml
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.236018 datatoolbox-0.6.7/ci/
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.241741 datatoolbox-0.6.7/ci/appveyor/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3111 2020-10-14 14:04:18.000000 datatoolbox-0.6.7/ci/appveyor/install.ps1
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1842 2020-10-14 14:04:18.000000 datatoolbox-0.6.7/ci/appveyor/run_with_env.cmd
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.250589 datatoolbox-0.6.7/datatoolbox/
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     5681 2023-08-18 10:53:24.000000 datatoolbox-0.6.7/datatoolbox/__init__.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    15513 2023-06-08 08:12:18.000000 datatoolbox-0.6.7/datatoolbox/admin.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3753 2024-04-17 07:49:21.000000 datatoolbox-0.6.7/datatoolbox/aggregator.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     6773 2023-07-25 21:00:35.000000 datatoolbox-0.6.7/datatoolbox/config.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    18681 2023-08-29 12:09:48.000000 datatoolbox-0.6.7/datatoolbox/converters.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    16287 2024-04-17 11:20:09.000000 datatoolbox-0.6.7/datatoolbox/core.py
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.254896 datatoolbox-0.6.7/datatoolbox/data/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    15781 2020-10-14 14:04:18.000000 datatoolbox-0.6.7/datatoolbox/data/GHG_alternative_naming.pkl
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    13482 2023-05-23 13:04:06.000000 datatoolbox-0.6.7/datatoolbox/data/GHG_properties_2019_CA.csv
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.255399 datatoolbox-0.6.7/datatoolbox/data/SANDBOX_datashelf/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      286 2024-04-22 08:23:23.000000 datatoolbox-0.6.7/datatoolbox/data/SANDBOX_datashelf/inventory.csv
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.256140 datatoolbox-0.6.7/datatoolbox/data/SANDBOX_datashelf/mappings/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    10757 2024-04-22 08:23:22.000000 datatoolbox-0.6.7/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     8466 2024-04-22 08:23:22.000000 datatoolbox-0.6.7/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      999 2024-04-22 08:23:22.000000 datatoolbox-0.6.7/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      161 2024-04-22 08:23:23.000000 datatoolbox-0.6.7/datatoolbox/data/SANDBOX_datashelf/sources.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    22865 2020-10-14 14:04:18.000000 datatoolbox-0.6.7/datatoolbox/data/all.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    14615 2020-10-14 14:04:18.000000 datatoolbox-0.6.7/datatoolbox/data/compatible1_5_unfiltered.xlsx
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    10757 2020-04-20 12:32:09.000000 datatoolbox-0.6.7/datatoolbox/data/continent.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     8466 2021-09-15 15:48:16.000000 datatoolbox-0.6.7/datatoolbox/data/country_codes.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1711 2022-05-25 07:15:53.000000 datatoolbox-0.6.7/datatoolbox/data/datashelf_contents.csv
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     2923 2021-12-16 12:32:58.000000 datatoolbox-0.6.7/datatoolbox/data/external_mappings.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      178 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/data/personal_template.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)      999 2019-08-14 10:00:22.000000 datatoolbox-0.6.7/datatoolbox/data/regions.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)   237445 2024-04-03 07:39:56.000000 datatoolbox-0.6.7/datatoolbox/data_readers.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    70580 2024-04-15 09:57:54.000000 datatoolbox-0.6.7/datatoolbox/data_structures.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    65668 2024-03-20 09:16:19.000000 datatoolbox-0.6.7/datatoolbox/database.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     6730 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/greenhouse_gas_database.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3542 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/init_tools.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    21653 2023-08-18 10:29:12.000000 datatoolbox-0.6.7/datatoolbox/interfaces.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    11022 2024-04-04 14:18:18.000000 datatoolbox-0.6.7/datatoolbox/io_tools.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    41818 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/mapping.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     2854 2022-12-01 09:27:15.000000 datatoolbox-0.6.7/datatoolbox/naming_convention.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3305 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/patches.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     2189 2023-08-17 09:12:01.000000 datatoolbox-0.6.7/datatoolbox/pint_definitions.txt
--rw-r--r--   0 andreasgeiges   (501) staff       (20)        0 2020-06-08 07:09:19.000000 datatoolbox-0.6.7/datatoolbox/relations.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    26449 2023-07-17 09:50:44.000000 datatoolbox-0.6.7/datatoolbox/sets.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)        0 2020-06-08 07:09:19.000000 datatoolbox-0.6.7/datatoolbox/storage.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1632 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/templates.py
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.264358 datatoolbox-0.6.7/datatoolbox/tools/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    16351 2021-04-19 11:31:45.000000 datatoolbox-0.6.7/datatoolbox/tools/CRF_extract_CA_2021.xlsx
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    28022 2021-02-02 15:17:26.000000 datatoolbox-0.6.7/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    17445 2021-02-02 12:48:44.000000 datatoolbox-0.6.7/datatoolbox/tools/IEA_B2DS_4.SCEN
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    17375 2019-12-20 11:46:57.000000 datatoolbox-0.6.7/datatoolbox/tools/WEO_2019_test.SCEN
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      587 2023-08-29 11:46:45.000000 datatoolbox-0.6.7/datatoolbox/tools/__init__.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     4320 2022-11-17 09:58:39.000000 datatoolbox-0.6.7/datatoolbox/tools/conversion_to_v0.3.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    48127 2024-04-18 13:35:14.000000 datatoolbox-0.6.7/datatoolbox/tools/excel.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      370 2022-11-17 09:58:39.000000 datatoolbox-0.6.7/datatoolbox/tools/export_all.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     4441 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/tools/for_datatables.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     8132 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/tools/html.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      182 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/tools/install_support.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     7188 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/tools/kaya_idendentiy_decomposition.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     4283 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/tools/magicc6.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     5931 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/tools/matplotlib.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      892 2023-08-04 09:51:33.000000 datatoolbox-0.6.7/datatoolbox/tools/new_SR15_pathway_matching.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3797 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/tools/pandas.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     5533 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/tools/py_magicc_tools.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     7948 2023-08-18 10:42:50.000000 datatoolbox-0.6.7/datatoolbox/tools/pyam.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      965 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/tools/renaming_DB.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    84992 2019-08-14 10:26:08.000000 datatoolbox-0.6.7/datatoolbox/tools/run_MAGICC_startup_simple.xlsx
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1830 2021-02-02 14:03:36.000000 datatoolbox-0.6.7/datatoolbox/tools/run_magicc6.m
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1044 2022-11-17 09:58:40.000000 datatoolbox-0.6.7/datatoolbox/tools/statistics.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    61174 2021-06-03 14:06:07.000000 datatoolbox-0.6.7/datatoolbox/tools/test.docx
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     8625 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/tools/word.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     9597 2023-08-18 10:43:36.000000 datatoolbox-0.6.7/datatoolbox/tools/xarray.py
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.267751 datatoolbox-0.6.7/datatoolbox/tutorials/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     2996 2022-05-25 07:15:53.000000 datatoolbox-0.6.7/datatoolbox/tutorials/00_search_find_and_access_data.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1019 2020-10-14 14:04:18.000000 datatoolbox-0.6.7/datatoolbox/tutorials/01_emission_comparison.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     2096 2022-05-25 07:15:53.000000 datatoolbox-0.6.7/datatoolbox/tutorials/02_unit_conversion.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     5685 2020-10-14 14:04:18.000000 datatoolbox-0.6.7/datatoolbox/tutorials/03_intermediate_example.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1416 2020-10-14 14:04:19.000000 datatoolbox-0.6.7/datatoolbox/tutorials/04_sources.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      382 2020-10-14 14:04:19.000000 datatoolbox-0.6.7/datatoolbox/tutorials/05_plot_source_content.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      734 2020-12-22 15:09:15.000000 datatoolbox-0.6.7/datatoolbox/tutorials/06_xarray_examples.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1142 2021-05-11 13:19:29.000000 datatoolbox-0.6.7/datatoolbox/tutorials/07_renewable_share_compuation.py
--rw-rw-r--   0 andreasgeiges   (501) staff       (20)      793 2021-05-11 12:59:38.000000 datatoolbox-0.6.7/datatoolbox/tutorials/08_low_carbon_fuel_computation.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)   137631 2020-10-14 14:04:19.000000 datatoolbox-0.6.7/datatoolbox/tutorials/introduction_v1.ipynb
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     4631 2022-03-22 14:54:50.000000 datatoolbox-0.6.7/datatoolbox/tutorials/jump_start.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)      417 2023-05-12 14:15:39.000000 datatoolbox-0.6.7/datatoolbox/units.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    43885 2023-08-18 10:28:42.000000 datatoolbox-0.6.7/datatoolbox/util.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      160 2024-04-22 08:25:37.000000 datatoolbox-0.6.7/datatoolbox/version.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      746 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/datatoolbox/workflows.py
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.251968 datatoolbox-0.6.7/datatoolbox.egg-info/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1564 2024-04-22 08:25:38.000000 datatoolbox-0.6.7/datatoolbox.egg-info/PKG-INFO
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3787 2024-04-22 08:25:38.000000 datatoolbox-0.6.7/datatoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 andreasgeiges   (501) staff       (20)        1 2024-04-22 08:25:38.000000 datatoolbox-0.6.7/datatoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      157 2024-04-22 08:25:38.000000 datatoolbox-0.6.7/datatoolbox.egg-info/requires.txt
--rw-r--r--   0 andreasgeiges   (501) staff       (20)       12 2024-04-22 08:25:38.000000 datatoolbox-0.6.7/datatoolbox.egg-info/top_level.txt
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.272972 datatoolbox-0.6.7/doc/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     7755 2024-04-02 13:29:36.000000 datatoolbox-0.6.7/doc/Makefile
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     9684 2024-04-02 12:29:22.000000 datatoolbox-0.6.7/doc/conf.py
--rwxr-x---   0 andreasgeiges   (501) staff       (20)      101 2024-04-02 13:46:58.000000 datatoolbox-0.6.7/doc/core.rst
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      236 2024-04-02 14:07:33.000000 datatoolbox-0.6.7/doc/data_structures.rst
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      122 2021-01-11 16:19:59.000000 datatoolbox-0.6.7/doc/database.rst
--rw-r--r--   0 andreasgeiges   (501) staff       (20)       91 2021-01-11 16:18:53.000000 datatoolbox-0.6.7/doc/database_database.rst
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      130 2021-01-11 16:21:50.000000 datatoolbox-0.6.7/doc/database_gitrepomanager.rst
--rwxr-x---   0 andreasgeiges   (501) staff       (20)       93 2021-01-11 16:03:03.000000 datatoolbox-0.6.7/doc/excel.rst
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.273748 datatoolbox-0.6.7/doc/figures/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    21579 2020-11-09 13:08:35.000000 datatoolbox-0.6.7/doc/figures/ID_meta_data.svg
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    67463 2021-05-17 15:08:58.000000 datatoolbox-0.6.7/doc/figures/config_input.png
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     7008 2023-06-08 10:16:48.000000 datatoolbox-0.6.7/doc/first_steps.md
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      100 2020-12-22 15:09:15.000000 datatoolbox-0.6.7/doc/foo.rst_template
--rw-r--r--   0 andreasgeiges   (501) staff       (20)       77 2020-12-22 15:09:15.000000 datatoolbox-0.6.7/doc/help.rst
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      463 2024-04-02 11:53:11.000000 datatoolbox-0.6.7/doc/index.rst
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1655 2023-06-08 08:19:25.000000 datatoolbox-0.6.7/doc/installation.md
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1080 2020-12-22 15:09:15.000000 datatoolbox-0.6.7/doc/license.rst
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     7353 2020-10-14 14:04:19.000000 datatoolbox-0.6.7/doc/make.bat
--rwxr-x---   0 andreasgeiges   (501) staff       (20)      103 2021-01-11 16:09:22.000000 datatoolbox-0.6.7/doc/matplotlib.rst
--rwxr-x---   0 andreasgeiges   (501) staff       (20)       95 2021-01-11 16:10:43.000000 datatoolbox-0.6.7/doc/pandas.rst
--rwxr-x---   0 andreasgeiges   (501) staff       (20)      243 2024-04-02 12:12:03.000000 datatoolbox-0.6.7/doc/tools.rst
--rwxr-x---   0 andreasgeiges   (501) staff       (20)       95 2021-01-11 16:09:13.000000 datatoolbox-0.6.7/doc/xarray.rst
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.274227 datatoolbox-0.6.7/documentation/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     7761 2020-12-22 15:09:15.000000 datatoolbox-0.6.7/documentation/Datatoolbox - First steps.md
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      396 2023-10-10 10:32:47.000000 datatoolbox-0.6.7/environment.yml
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      418 2020-10-14 14:04:19.000000 datatoolbox-0.6.7/make_proj.sh
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      598 2024-04-02 14:16:29.000000 datatoolbox-0.6.7/readthedocs.yml
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      228 2024-04-02 14:19:55.000000 datatoolbox-0.6.7/requirements.txt
--rw-r--r--   0 andreasgeiges   (501) staff       (20)       38 2024-04-22 08:25:38.279446 datatoolbox-0.6.7/setup.cfg
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1862 2023-09-22 10:49:18.000000 datatoolbox-0.6.7/setup.py
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-22 08:25:38.278525 datatoolbox-0.6.7/tests/
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     7292 2022-12-19 11:29:58.000000 datatoolbox-0.6.7/tests/test_calculations.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      696 2022-11-18 16:16:07.000000 datatoolbox-0.6.7/tests/test_converters.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     3941 2024-04-22 08:16:23.000000 datatoolbox-0.6.7/tests/test_database.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1640 2023-03-30 13:32:13.000000 datatoolbox-0.6.7/tests/test_dataset.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     7741 2022-05-25 07:15:53.000000 datatoolbox-0.6.7/tests/test_datatable.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1063 2022-11-16 11:59:46.000000 datatoolbox-0.6.7/tests/test_io.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      390 2022-11-22 09:54:34.000000 datatoolbox-0.6.7/tests/test_linked_functions.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1563 2023-05-04 07:49:24.000000 datatoolbox-0.6.7/tests/test_pyam.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3570 2022-05-25 07:15:53.000000 datatoolbox-0.6.7/tests/test_tableset.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     2610 2022-05-25 07:15:53.000000 datatoolbox-0.6.7/tests/test_tools.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1768 2023-10-11 06:54:12.000000 datatoolbox-0.6.7/tests/test_units.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      870 2020-10-14 14:04:19.000000 datatoolbox-0.6.7/tests/test_utilities.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     2437 2022-10-19 13:17:33.000000 datatoolbox-0.6.7/tests/test_xarray.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     2959 2022-05-25 07:15:53.000000 datatoolbox-0.6.7/tests/util_for_testing.py
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.321687 datatoolbox-0.6.9/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      159 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/.gitignore
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      950 2022-10-19 13:17:33.000000 datatoolbox-0.6.9/.gitlab-ci.yml
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      703 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/.travis.yml
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1073 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/LICENSE
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1564 2024-04-30 07:55:20.321408 datatoolbox-0.6.9/PKG-INFO
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1298 2023-09-22 10:59:58.000000 datatoolbox-0.6.9/README.md
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1225 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/appveyor.yml
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.273494 datatoolbox-0.6.9/ci/
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.280489 datatoolbox-0.6.9/ci/appveyor/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3111 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/ci/appveyor/install.ps1
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1842 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/ci/appveyor/run_with_env.cmd
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.290595 datatoolbox-0.6.9/datatoolbox/
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     5681 2023-08-18 10:53:24.000000 datatoolbox-0.6.9/datatoolbox/__init__.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    15513 2023-06-08 08:12:18.000000 datatoolbox-0.6.9/datatoolbox/admin.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3753 2024-04-17 07:49:21.000000 datatoolbox-0.6.9/datatoolbox/aggregator.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     6846 2024-04-29 10:25:24.000000 datatoolbox-0.6.9/datatoolbox/config.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    18681 2023-08-29 12:09:48.000000 datatoolbox-0.6.9/datatoolbox/converters.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    17879 2024-04-30 07:21:37.000000 datatoolbox-0.6.9/datatoolbox/core.py
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.295201 datatoolbox-0.6.9/datatoolbox/data/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    15781 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/datatoolbox/data/GHG_alternative_naming.pkl
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    13482 2023-05-23 13:04:06.000000 datatoolbox-0.6.9/datatoolbox/data/GHG_properties_2019_CA.csv
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.295890 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      286 2024-04-30 07:49:57.000000 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/inventory.csv
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.296794 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    10757 2024-04-30 07:49:53.000000 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     8466 2024-04-30 07:49:53.000000 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      999 2024-04-30 07:49:53.000000 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      161 2024-04-30 07:49:57.000000 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/sources.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    22865 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/datatoolbox/data/all.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    14615 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/datatoolbox/data/compatible1_5_unfiltered.xlsx
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    10757 2020-04-20 12:32:09.000000 datatoolbox-0.6.9/datatoolbox/data/continent.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     8466 2021-09-15 15:48:16.000000 datatoolbox-0.6.9/datatoolbox/data/country_codes.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1711 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/datatoolbox/data/datashelf_contents.csv
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     2923 2021-12-16 12:32:58.000000 datatoolbox-0.6.9/datatoolbox/data/external_mappings.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      178 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/data/personal_template.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)      999 2019-08-14 10:00:22.000000 datatoolbox-0.6.9/datatoolbox/data/regions.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)   237445 2024-04-03 07:39:56.000000 datatoolbox-0.6.9/datatoolbox/data_readers.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    70580 2024-04-15 09:57:54.000000 datatoolbox-0.6.9/datatoolbox/data_structures.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    65668 2024-03-20 09:16:19.000000 datatoolbox-0.6.9/datatoolbox/database.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     6730 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/greenhouse_gas_database.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3542 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/init_tools.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    21653 2023-08-18 10:29:12.000000 datatoolbox-0.6.9/datatoolbox/interfaces.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    11022 2024-04-04 14:18:18.000000 datatoolbox-0.6.9/datatoolbox/io_tools.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    41818 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/mapping.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     2854 2022-12-01 09:27:15.000000 datatoolbox-0.6.9/datatoolbox/naming_convention.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3305 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/patches.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     2189 2023-08-17 09:12:01.000000 datatoolbox-0.6.9/datatoolbox/pint_definitions.txt
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)        0 2020-06-08 07:09:19.000000 datatoolbox-0.6.9/datatoolbox/relations.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    26449 2023-07-17 09:50:44.000000 datatoolbox-0.6.9/datatoolbox/sets.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)        0 2020-06-08 07:09:19.000000 datatoolbox-0.6.9/datatoolbox/storage.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1632 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/templates.py
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.306907 datatoolbox-0.6.9/datatoolbox/tools/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    16351 2021-04-19 11:31:45.000000 datatoolbox-0.6.9/datatoolbox/tools/CRF_extract_CA_2021.xlsx
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    28022 2021-02-02 15:17:26.000000 datatoolbox-0.6.9/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    17445 2021-02-02 12:48:44.000000 datatoolbox-0.6.9/datatoolbox/tools/IEA_B2DS_4.SCEN
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    17375 2019-12-20 11:46:57.000000 datatoolbox-0.6.9/datatoolbox/tools/WEO_2019_test.SCEN
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      587 2023-08-29 11:46:45.000000 datatoolbox-0.6.9/datatoolbox/tools/__init__.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     4320 2022-11-17 09:58:39.000000 datatoolbox-0.6.9/datatoolbox/tools/conversion_to_v0.3.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    45928 2024-04-30 07:25:50.000000 datatoolbox-0.6.9/datatoolbox/tools/excel.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      370 2022-11-17 09:58:39.000000 datatoolbox-0.6.9/datatoolbox/tools/export_all.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     4441 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/for_datatables.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     8132 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/html.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      182 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/install_support.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     7188 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/kaya_idendentiy_decomposition.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     4283 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/magicc6.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     5931 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/matplotlib.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      892 2023-08-04 09:51:33.000000 datatoolbox-0.6.9/datatoolbox/tools/new_SR15_pathway_matching.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3797 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/pandas.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     5533 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/py_magicc_tools.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     7948 2023-08-18 10:42:50.000000 datatoolbox-0.6.9/datatoolbox/tools/pyam.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      965 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/renaming_DB.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    84992 2019-08-14 10:26:08.000000 datatoolbox-0.6.9/datatoolbox/tools/run_MAGICC_startup_simple.xlsx
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1830 2021-02-02 14:03:36.000000 datatoolbox-0.6.9/datatoolbox/tools/run_magicc6.m
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1044 2022-11-17 09:58:40.000000 datatoolbox-0.6.9/datatoolbox/tools/statistics.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    61174 2021-06-03 14:06:07.000000 datatoolbox-0.6.9/datatoolbox/tools/test.docx
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     8625 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/word.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     9597 2023-08-18 10:43:36.000000 datatoolbox-0.6.9/datatoolbox/tools/xarray.py
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.310830 datatoolbox-0.6.9/datatoolbox/tutorials/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     2996 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/datatoolbox/tutorials/00_search_find_and_access_data.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1019 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/datatoolbox/tutorials/01_emission_comparison.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     2096 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/datatoolbox/tutorials/02_unit_conversion.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     5685 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/datatoolbox/tutorials/03_intermediate_example.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1416 2020-10-14 14:04:19.000000 datatoolbox-0.6.9/datatoolbox/tutorials/04_sources.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      382 2020-10-14 14:04:19.000000 datatoolbox-0.6.9/datatoolbox/tutorials/05_plot_source_content.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      734 2020-12-22 15:09:15.000000 datatoolbox-0.6.9/datatoolbox/tutorials/06_xarray_examples.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1142 2021-05-11 13:19:29.000000 datatoolbox-0.6.9/datatoolbox/tutorials/07_renewable_share_compuation.py
+-rw-rw-r--   0 andreasgeiges   (501) staff       (20)      793 2021-05-11 12:59:38.000000 datatoolbox-0.6.9/datatoolbox/tutorials/08_low_carbon_fuel_computation.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)   137631 2020-10-14 14:04:19.000000 datatoolbox-0.6.9/datatoolbox/tutorials/introduction_v1.ipynb
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     4631 2022-03-22 14:54:50.000000 datatoolbox-0.6.9/datatoolbox/tutorials/jump_start.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)      417 2023-05-12 14:15:39.000000 datatoolbox-0.6.9/datatoolbox/units.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    43885 2023-08-18 10:28:42.000000 datatoolbox-0.6.9/datatoolbox/util.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      160 2024-04-30 07:55:19.000000 datatoolbox-0.6.9/datatoolbox/version.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      746 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/workflows.py
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.292296 datatoolbox-0.6.9/datatoolbox.egg-info/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1564 2024-04-30 07:55:20.000000 datatoolbox-0.6.9/datatoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3787 2024-04-30 07:55:20.000000 datatoolbox-0.6.9/datatoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)        1 2024-04-30 07:55:20.000000 datatoolbox-0.6.9/datatoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      157 2024-04-30 07:55:20.000000 datatoolbox-0.6.9/datatoolbox.egg-info/requires.txt
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)       12 2024-04-30 07:55:20.000000 datatoolbox-0.6.9/datatoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.316137 datatoolbox-0.6.9/doc/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     7755 2024-04-02 13:29:36.000000 datatoolbox-0.6.9/doc/Makefile
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     9684 2024-04-02 12:29:22.000000 datatoolbox-0.6.9/doc/conf.py
+-rwxr-x---   0 andreasgeiges   (501) staff       (20)      101 2024-04-02 13:46:58.000000 datatoolbox-0.6.9/doc/core.rst
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      236 2024-04-02 14:07:33.000000 datatoolbox-0.6.9/doc/data_structures.rst
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      122 2021-01-11 16:19:59.000000 datatoolbox-0.6.9/doc/database.rst
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)       91 2021-01-11 16:18:53.000000 datatoolbox-0.6.9/doc/database_database.rst
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      130 2021-01-11 16:21:50.000000 datatoolbox-0.6.9/doc/database_gitrepomanager.rst
+-rwxr-x---   0 andreasgeiges   (501) staff       (20)       93 2021-01-11 16:03:03.000000 datatoolbox-0.6.9/doc/excel.rst
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.316704 datatoolbox-0.6.9/doc/figures/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    21579 2020-11-09 13:08:35.000000 datatoolbox-0.6.9/doc/figures/ID_meta_data.svg
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    67463 2021-05-17 15:08:58.000000 datatoolbox-0.6.9/doc/figures/config_input.png
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     7008 2023-06-08 10:16:48.000000 datatoolbox-0.6.9/doc/first_steps.md
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      100 2020-12-22 15:09:15.000000 datatoolbox-0.6.9/doc/foo.rst_template
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)       77 2020-12-22 15:09:15.000000 datatoolbox-0.6.9/doc/help.rst
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      463 2024-04-02 11:53:11.000000 datatoolbox-0.6.9/doc/index.rst
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1655 2023-06-08 08:19:25.000000 datatoolbox-0.6.9/doc/installation.md
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1080 2020-12-22 15:09:15.000000 datatoolbox-0.6.9/doc/license.rst
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     7353 2020-10-14 14:04:19.000000 datatoolbox-0.6.9/doc/make.bat
+-rwxr-x---   0 andreasgeiges   (501) staff       (20)      103 2021-01-11 16:09:22.000000 datatoolbox-0.6.9/doc/matplotlib.rst
+-rwxr-x---   0 andreasgeiges   (501) staff       (20)       95 2021-01-11 16:10:43.000000 datatoolbox-0.6.9/doc/pandas.rst
+-rwxr-x---   0 andreasgeiges   (501) staff       (20)      243 2024-04-02 12:12:03.000000 datatoolbox-0.6.9/doc/tools.rst
+-rwxr-x---   0 andreasgeiges   (501) staff       (20)       95 2021-01-11 16:09:13.000000 datatoolbox-0.6.9/doc/xarray.rst
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.317139 datatoolbox-0.6.9/documentation/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     7761 2020-12-22 15:09:15.000000 datatoolbox-0.6.9/documentation/Datatoolbox - First steps.md
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      396 2023-10-10 10:32:47.000000 datatoolbox-0.6.9/environment.yml
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      418 2020-10-14 14:04:19.000000 datatoolbox-0.6.9/make_proj.sh
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      598 2024-04-02 14:16:29.000000 datatoolbox-0.6.9/readthedocs.yml
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      233 2024-04-29 10:26:45.000000 datatoolbox-0.6.9/requirements.txt
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)       38 2024-04-30 07:55:20.321779 datatoolbox-0.6.9/setup.cfg
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1862 2023-09-22 10:49:18.000000 datatoolbox-0.6.9/setup.py
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.321038 datatoolbox-0.6.9/tests/
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     7292 2022-12-19 11:29:58.000000 datatoolbox-0.6.9/tests/test_calculations.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      696 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/tests/test_converters.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     3941 2024-04-22 08:16:23.000000 datatoolbox-0.6.9/tests/test_database.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1640 2023-03-30 13:32:13.000000 datatoolbox-0.6.9/tests/test_dataset.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     7741 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/tests/test_datatable.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1063 2022-11-16 11:59:46.000000 datatoolbox-0.6.9/tests/test_io.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      390 2022-11-22 09:54:34.000000 datatoolbox-0.6.9/tests/test_linked_functions.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1563 2023-05-04 07:49:24.000000 datatoolbox-0.6.9/tests/test_pyam.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3570 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/tests/test_tableset.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     2610 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/tests/test_tools.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1768 2023-10-11 06:54:12.000000 datatoolbox-0.6.9/tests/test_units.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      870 2020-10-14 14:04:19.000000 datatoolbox-0.6.9/tests/test_utilities.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     2437 2022-10-19 13:17:33.000000 datatoolbox-0.6.9/tests/test_xarray.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     2959 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/tests/util_for_testing.py
```

### Comparing `datatoolbox-0.6.7/.gitlab-ci.yml` & `datatoolbox-0.6.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/.travis.yml` & `datatoolbox-0.6.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/LICENSE` & `datatoolbox-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/PKG-INFO` & `datatoolbox-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatoolbox
-Version: 0.6.7
+Version: 0.6.9
 Summary: The Python Data Toolbox
 Home-page: https://gitlab.com/climateanalytics/datatoolbox
 Author: Andreas Geiges
 Author-email: a.geiges@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `datatoolbox-0.6.7/README.md` & `datatoolbox-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/appveyor.yml` & `datatoolbox-0.6.9/appveyor.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/ci/appveyor/install.ps1` & `datatoolbox-0.6.9/ci/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/ci/appveyor/run_with_env.cmd` & `datatoolbox-0.6.9/ci/appveyor/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/__init__.py` & `datatoolbox-0.6.9/datatoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/admin.py` & `datatoolbox-0.6.9/datatoolbox/admin.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/aggregator.py` & `datatoolbox-0.6.9/datatoolbox/aggregator.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/config.py` & `datatoolbox-0.6.9/datatoolbox/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,32 +107,33 @@
         config_file = os.path.join(CONFIG_DIR, 'personal.py')
         exec(open(config_file).read())
     except:
         raise (Exception(f'Error in config file: {config_file}. Please correct'))
 
     TEST_ENV = False
 
-
-try:
-    import xarray as xr
-
-    AVAILABLE_XARRAY = True
-except:
-
-    AVAILABLE_XARRAY = False
-    if DEBUG:
-        print('xarray not available: Use "pip install xarray" to install')
-try:
-    import docx
-
-    AVAILABLE_DOCX = True
-except:
-    AVAILABLE_DOCX = False
-    if DEBUG:
-        print('python-docx not available: Use "pip install python-docx" to install')
+AVAILABLE_XARRAY = True
+AVAILABLE_DOCX = True
+# try:
+#     import xarray as xr
+
+#     AVAILABLE_XARRAY = True
+# except:
+
+#     AVAILABLE_XARRAY = False
+#     if DEBUG:
+#         print('xarray not available: Use "pip install xarray" to install')
+# try:
+#     import docx
+
+#     AVAILABLE_DOCX = True
+# except:
+#     AVAILABLE_DOCX = False
+#     if DEBUG:
+#         print('python-docx not available: Use "pip install python-docx" to install')
 
 
 META_DECLARATION = '### META ###\n'
 DATA_DECLARATION = '### DATA ###\n'
 
 MODULE_PATH = os.path.dirname(__file__)
 MODULE_DATA_PATH = os.path.join(MODULE_PATH, 'data')
```

### Comparing `datatoolbox-0.6.7/datatoolbox/converters.py` & `datatoolbox-0.6.9/datatoolbox/converters.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/core.py` & `datatoolbox-0.6.9/datatoolbox/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,54 @@
 from datatoolbox import naming_convention
 import pandas_indexing as pix
 
 if config.DEBUG:
     print('Core import in {:2.4f} seconds'.format(time.time() - tt))
 
 
-tt = time.time()
+
 import pint
 
 from copy import copy
 from treelib import Node, Tree
 
+from colorama import init as colorama_init
+from colorama import Fore
+from colorama import Style
+
+colorama_init()
+
+def colored_string(string,color):
+    
+    color_mapping = {
+        'r' : Fore.RED,
+        'y' : Fore.LIGHTYELLOW_EX,
+        'g' : Fore.GREEN
+        }
+    return f"{color_mapping[color]}{string}{Style.RESET_ALL}"
+    
 #%% Aggregator class
 class Aggregator():
     
     def __init__(self):
         
         self.tree = None
         
+        class bc:
+            HEADER = '\033[95m'
+            OKBLUE = '\033[94m'
+            OKCYAN = '\033[96m'
+            OKGREEN = '\033[92m'
+            WARNING = '\033[93m'
+            FAIL = '\033[91m'
+            ENDC = '\033[0m'
+            BOLD = '\033[1m'
+            UNDERLINE = '\033[4m'
+
+        
     def __str__(self):
         return self.tree.__str__()
      
     def _dict2tree(self, relation:dict):
         
         trees = list()
         for source, target in relation.items():
@@ -130,24 +157,47 @@
     def bottom_up_aggregations(self):
         
         root = self.tree.root
         
         mappings = list()
         
         self._leave_to_dict(root, mappings)
-        
+        	
         return mappings
     
+    # def show_availability_data(self, wdf, index_name):
+    #     #%%
+    #     wdf = all_data.copy().loc[pix.isin(entity='Emissions|CO2', region='POL')]
+        
+    #     string_lines = self.__str__()
+    #     new_string_lines = list()
+    #     for line in string_lines.split('\n'):
+    #         sel_str = line.split('──')[-1].strip()
+    #         data = wdf.loc[pix.isin(**{index_name: sel_str})]
+            
+    #         if len(data) == 0 or (data.isnull().all(axis=1).all()):
+    #             new_string_lines.append(colored_string(line, color='r'))
+    #         elif data.isnull().any(axis=1).any():
+    #             new_string_lines.append(colored_string(line, color='y'))
+                
+    #         else:
+    #             new_string_lines.append(colored_string(line, color='g'))
+                
+    #     new_string_lines = '\n'.join(new_string_lines)
+    #     print(new_string_lines)
+                
 #%% Pint unit handling
 gases = {
     "CO2eq": "carbon_dioxide_equivalent",
     # "CO2e": "CO2eq",
     "NO2": "NO2",
     'PM25': 'PM25',
 }
+
+tt_pint = time.time()
 from openscm_units import unit_registry as ur
 
 # self.ur = self_ur
 
 try:
     
    ur._add_gases(gases)
@@ -162,15 +212,15 @@
 except pint.errors.DefinitionSyntaxError:
     # avoid double import of units defintions
     pass
    
 import pint
 
 if config.DEBUG:
-    print('pint unit handling initialised in core in {:2.4f} seconds'.format(time.time() - tt))
+    print('pint unit handling initialised in core in {:2.4f} seconds'.format(time.time() - tt_pint))
 
 
 
 LOG = dict()
 LOG['tableIDs'] = list()
 
 def slim_index(df):
```

### Comparing `datatoolbox-0.6.7/datatoolbox/data/GHG_alternative_naming.pkl` & `datatoolbox-0.6.9/datatoolbox/data/GHG_alternative_naming.pkl`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/data/GHG_properties_2019_CA.csv` & `datatoolbox-0.6.9/datatoolbox/data/GHG_properties_2019_CA.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv` & `datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv` & `datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv` & `datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/data/all.csv` & `datatoolbox-0.6.9/datatoolbox/data/all.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/data/compatible1_5_unfiltered.xlsx` & `datatoolbox-0.6.9/datatoolbox/data/compatible1_5_unfiltered.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/data/continent.csv` & `datatoolbox-0.6.9/datatoolbox/data/continent.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/data/country_codes.csv` & `datatoolbox-0.6.9/datatoolbox/data/country_codes.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/data/datashelf_contents.csv` & `datatoolbox-0.6.9/datatoolbox/data/datashelf_contents.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/data/external_mappings.py` & `datatoolbox-0.6.9/datatoolbox/data/external_mappings.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/data/regions.csv` & `datatoolbox-0.6.9/datatoolbox/data/regions.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/data_readers.py` & `datatoolbox-0.6.9/datatoolbox/data_readers.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/data_structures.py` & `datatoolbox-0.6.9/datatoolbox/data_structures.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/database.py` & `datatoolbox-0.6.9/datatoolbox/database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/greenhouse_gas_database.py` & `datatoolbox-0.6.9/datatoolbox/greenhouse_gas_database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/init_tools.py` & `datatoolbox-0.6.9/datatoolbox/init_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/interfaces.py` & `datatoolbox-0.6.9/datatoolbox/interfaces.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/io_tools.py` & `datatoolbox-0.6.9/datatoolbox/io_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/mapping.py` & `datatoolbox-0.6.9/datatoolbox/mapping.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/naming_convention.py` & `datatoolbox-0.6.9/datatoolbox/naming_convention.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/patches.py` & `datatoolbox-0.6.9/datatoolbox/patches.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/pint_definitions.txt` & `datatoolbox-0.6.9/datatoolbox/pint_definitions.txt`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/sets.py` & `datatoolbox-0.6.9/datatoolbox/sets.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/templates.py` & `datatoolbox-0.6.9/datatoolbox/templates.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/CRF_extract_CA_2021.xlsx` & `datatoolbox-0.6.9/datatoolbox/tools/CRF_extract_CA_2021.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN` & `datatoolbox-0.6.9/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/IEA_B2DS_4.SCEN` & `datatoolbox-0.6.9/datatoolbox/tools/IEA_B2DS_4.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/WEO_2019_test.SCEN` & `datatoolbox-0.6.9/datatoolbox/tools/WEO_2019_test.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/__init__.py` & `datatoolbox-0.6.9/datatoolbox/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/conversion_to_v0.3.py` & `datatoolbox-0.6.9/datatoolbox/tools/conversion_to_v0.3.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/excel.py` & `datatoolbox-0.6.9/datatoolbox/tools/excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -529,57 +529,16 @@
                 ldf = ldf.idx.assign(**{meta_key : meta_value})
         return ldf
     
     def openSourceFile(self):
         if OS == 'Linux':
             os.system('libreoffice ' + self.filename)
         elif OS == 'Darwin':
-            os.system('open -a "Microsoft Excel" ' + filename)
+            os.system('open -a "Microsoft Excel" ' + self.filename)
 #%%
-filename= '/Users/andreasgeiges/Documents/python/ca_data_management/data/UNFCCC_CRF/UNFCCC_CRF_2023/AUT/AUT_2023_1990_07042023_154105.xlsx'
-reader = Excel_Reader(filename)
-
-test_config =    {
-        "xlsx_layout": {  # pandas parameters
-            "sheet_name": "Table1s1",
-            "header": 4,
-            "index_col": 0,
-        },
-        'data_layout': 
-            {'column_names' : ['entity'],
-             'index_names' : ['category']},
-        "column_mapping": {
-            "CO2": "Emissions|CO2(reported)",
-            "CH4": "Emissions|CH4(reported)",
-            "N2O": "Emissions|N2O(reported)",
-        },
-        "index_mapping": {
-            "Total Energy" : "IPC1",
-            "a.  Public electricity and heat production": "IPC1|Fuel_combustion|Energy_industries|Public electricity and heat production",
-            "b.  Petroleum refining": "IPC1|Fuel_combustion|Energy_industries|Petroleum refining",
-            "c.  Manufacture of solid fuels and other energy industries": "IPC1|Fuel_combustion|Energy_industries|Manufacture of solid fuels and other energy industries",
-            "a.  Iron and steel": "IPC1|Fuel_combustion|Manufacturing&construction|Iron and steel",
-            "b.  Non-ferrous metals": "IPC1|Fuel_combustion|Manufacturing&construction|Non-ferrous metals",
-            "c.  Chemicals": "IPC1|Fuel_combustion|Manufacturing&construction|Chemicals",
-            "a.  Domestic aviation": "IPC1|Fuel_combustion|Transport|Domestic aviation",
-            "b.  Road transportation": "IPC1|Fuel_combustion|Transport|Road transportation",
-            "c.  Railways": "IPC1|Fuel_combustion|Transport|Railways",
-            "d.  Domestic navigation": "IPC1|Fuel_combustion|Transport|Domestic navigation",
-            "e.  Other transportation": "IPC1|Fuel_combustion|Transport|Other transportation",
-        },
-        'units' : {
-             "Emissions|CO2(reported)" : "kt CO2",
-             "Emissions|CH4(reported)" : "kt CH4",
-             "Emissions|N2O(reported)" : "kt N2O"
-             },
-        "meta": {
-                 'scenario' : 'Historic|UNFCCC_reported',
-                 'source' : 'UNFCCC_2023'},
-    }
-df = reader.extract_data(**test_config)
 
 
 #%%
 
 # class Excel_Reader:
 #     """
 #     Reader clase that uses an setup information provided in the excel file
```

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/for_datatables.py` & `datatoolbox-0.6.9/datatoolbox/tools/for_datatables.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/html.py` & `datatoolbox-0.6.9/datatoolbox/tools/html.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/kaya_idendentiy_decomposition.py` & `datatoolbox-0.6.9/datatoolbox/tools/kaya_idendentiy_decomposition.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/magicc6.py` & `datatoolbox-0.6.9/datatoolbox/tools/magicc6.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/matplotlib.py` & `datatoolbox-0.6.9/datatoolbox/tools/matplotlib.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/new_SR15_pathway_matching.py` & `datatoolbox-0.6.9/datatoolbox/tools/new_SR15_pathway_matching.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/pandas.py` & `datatoolbox-0.6.9/datatoolbox/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/py_magicc_tools.py` & `datatoolbox-0.6.9/datatoolbox/tools/py_magicc_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/pyam.py` & `datatoolbox-0.6.9/datatoolbox/tools/pyam.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/renaming_DB.py` & `datatoolbox-0.6.9/datatoolbox/tools/renaming_DB.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/run_MAGICC_startup_simple.xlsx` & `datatoolbox-0.6.9/datatoolbox/tools/run_MAGICC_startup_simple.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/run_magicc6.m` & `datatoolbox-0.6.9/datatoolbox/tools/run_magicc6.m`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/statistics.py` & `datatoolbox-0.6.9/datatoolbox/tools/statistics.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/test.docx` & `datatoolbox-0.6.9/datatoolbox/tools/test.docx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/word.py` & `datatoolbox-0.6.9/datatoolbox/tools/word.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tools/xarray.py` & `datatoolbox-0.6.9/datatoolbox/tools/xarray.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tutorials/00_search_find_and_access_data.py` & `datatoolbox-0.6.9/datatoolbox/tutorials/00_search_find_and_access_data.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tutorials/01_emission_comparison.py` & `datatoolbox-0.6.9/datatoolbox/tutorials/01_emission_comparison.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tutorials/02_unit_conversion.py` & `datatoolbox-0.6.9/datatoolbox/tutorials/02_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tutorials/03_intermediate_example.py` & `datatoolbox-0.6.9/datatoolbox/tutorials/03_intermediate_example.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tutorials/04_sources.py` & `datatoolbox-0.6.9/datatoolbox/tutorials/04_sources.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tutorials/06_xarray_examples.py` & `datatoolbox-0.6.9/datatoolbox/tutorials/06_xarray_examples.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tutorials/07_renewable_share_compuation.py` & `datatoolbox-0.6.9/datatoolbox/tutorials/07_renewable_share_compuation.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tutorials/08_low_carbon_fuel_computation.py` & `datatoolbox-0.6.9/datatoolbox/tutorials/08_low_carbon_fuel_computation.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tutorials/introduction_v1.ipynb` & `datatoolbox-0.6.9/datatoolbox/tutorials/introduction_v1.ipynb`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/tutorials/jump_start.py` & `datatoolbox-0.6.9/datatoolbox/tutorials/jump_start.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/util.py` & `datatoolbox-0.6.9/datatoolbox/util.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox/workflows.py` & `datatoolbox-0.6.9/datatoolbox/workflows.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/datatoolbox.egg-info/PKG-INFO` & `datatoolbox-0.6.9/datatoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatoolbox
-Version: 0.6.7
+Version: 0.6.9
 Summary: The Python Data Toolbox
 Home-page: https://gitlab.com/climateanalytics/datatoolbox
 Author: Andreas Geiges
 Author-email: a.geiges@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `datatoolbox-0.6.7/datatoolbox.egg-info/SOURCES.txt` & `datatoolbox-0.6.9/datatoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/doc/Makefile` & `datatoolbox-0.6.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/doc/conf.py` & `datatoolbox-0.6.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/doc/figures/ID_meta_data.svg` & `datatoolbox-0.6.9/doc/figures/ID_meta_data.svg`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/doc/figures/config_input.png` & `datatoolbox-0.6.9/doc/figures/config_input.png`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/doc/first_steps.md` & `datatoolbox-0.6.9/doc/first_steps.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/doc/installation.md` & `datatoolbox-0.6.9/doc/installation.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/doc/license.rst` & `datatoolbox-0.6.9/doc/license.rst`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/doc/make.bat` & `datatoolbox-0.6.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/documentation/Datatoolbox - First steps.md` & `datatoolbox-0.6.9/documentation/Datatoolbox - First steps.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/readthedocs.yml` & `datatoolbox-0.6.9/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/setup.py` & `datatoolbox-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/tests/test_calculations.py` & `datatoolbox-0.6.9/tests/test_calculations.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/tests/test_converters.py` & `datatoolbox-0.6.9/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/tests/test_database.py` & `datatoolbox-0.6.9/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/tests/test_dataset.py` & `datatoolbox-0.6.9/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/tests/test_datatable.py` & `datatoolbox-0.6.9/tests/test_datatable.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/tests/test_io.py` & `datatoolbox-0.6.9/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/tests/test_pyam.py` & `datatoolbox-0.6.9/tests/test_pyam.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/tests/test_tableset.py` & `datatoolbox-0.6.9/tests/test_tableset.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/tests/test_tools.py` & `datatoolbox-0.6.9/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/tests/test_units.py` & `datatoolbox-0.6.9/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/tests/test_utilities.py` & `datatoolbox-0.6.9/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/tests/test_xarray.py` & `datatoolbox-0.6.9/tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.7/tests/util_for_testing.py` & `datatoolbox-0.6.9/tests/util_for_testing.py`

 * *Files identical despite different names*

