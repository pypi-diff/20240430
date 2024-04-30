# Comparing `tmp/housekeeper-4.8.7.tar.gz` & `tmp/housekeeper-4.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "housekeeper-4.8.7.tar", last modified: Fri Oct  6 12:37:20 2023, max compression
+gzip compressed data, was "housekeeper-4.8.8.tar", last modified: Fri Oct  6 13:11:40 2023, max compression
```

## Comparing `housekeeper-4.8.7.tar` & `housekeeper-4.8.8.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.837825 housekeeper-4.8.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-10-06 12:37:12.000000 housekeeper-4.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-10-06 12:37:12.000000 housekeeper-4.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2023-10-06 12:37:20.837825 housekeeper-4.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2023-10-06 12:37:12.000000 housekeeper-4.8.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.833825 housekeeper-4.8.7/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.833825 housekeeper-4.8.7/housekeeper/archive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/archive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.833825 housekeeper-4.8.7/housekeeper/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7096 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/cli/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/cli/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/cli/include.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/cli/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/include.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.833825 housekeeper-4.8.7/housekeeper/store/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.833825 housekeeper-4.8.7/housekeeper/store/api/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/api/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.833825 housekeeper-4.8.7/housekeeper/store/api/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/api/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/api/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/api/handlers/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     9449 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/api/handlers/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/api/handlers/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/api/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.833825 housekeeper-4.8.7/housekeeper/store/filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/filters/archive_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/filters/bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/filters/file_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/filters/tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/filters/version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/filters/version_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2023-10-06 12:37:12.000000 housekeeper-4.8.7/housekeeper/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.833825 housekeeper-4.8.7/housekeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2023-10-06 12:37:20.000000 housekeeper-4.8.7/housekeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2023-10-06 12:37:20.000000 housekeeper-4.8.7/housekeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 12:37:20.000000 housekeeper-4.8.7/housekeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-10-06 12:37:20.000000 housekeeper-4.8.7/housekeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 12:37:20.000000 housekeeper-4.8.7/housekeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-06 12:37:20.000000 housekeeper-4.8.7/housekeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-06 12:37:20.000000 housekeeper-4.8.7/housekeeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-10-06 12:37:12.000000 housekeeper-4.8.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-06 12:37:12.000000 housekeeper-4.8.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-06 12:37:12.000000 housekeeper-4.8.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-06 12:37:20.837825 housekeeper-4.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2023-10-06 12:37:12.000000 housekeeper-4.8.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.833825 housekeeper-4.8.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.833825 housekeeper-4.8.7/tests/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.837825 housekeeper-4.8.7/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/add/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/add/test_cli_add_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/add/test_cli_add_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/add/test_cli_add_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/add/test_cli_add_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.837825 housekeeper-4.8.7/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/delete/test_cli_delete_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/delete/test_cli_delete_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/delete/test_cli_delete_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/delete/test_cli_delete_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.837825 housekeeper-4.8.7/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/get/test_get_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/get/test_get_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/get/test_get_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/get/test_get_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/test_cli_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/cli/test_cli_include.py
--rw-r--r--   0 runner    (1001) docker     (127)    13944 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.837825 housekeeper-4.8.7/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.837825 housekeeper-4.8.7/tests/fixtures/sequencing_files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/fixtures/sequencing_files/lane1.spring
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/fixtures/sequencing_files/lane2.spring
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.837825 housekeeper-4.8.7/tests/fixtures/vcfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/fixtures/vcfs/example.2.vcf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/fixtures/vcfs/example.vcf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/fixtures/vcfs/family.2.vcf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/fixtures/vcfs/family.3.vcf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/fixtures/vcfs/family.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.837825 housekeeper-4.8.7/tests/store/
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.837825 housekeeper-4.8.7/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/store/filters/test_archive_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/store/filters/test_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/store/filters/test_file_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/store/filters/test_tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/store/filters/test_version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/store/filters/test_version_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 12:37:20.837825 housekeeper-4.8.7/tests/store/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/store/handlers/test_createhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/store/handlers/test_readhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/store/handlers/test_updatehandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/store/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-10-06 12:37:12.000000 housekeeper-4.8.7/tests/test_include.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.873644 housekeeper-4.8.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-10-06 13:11:31.000000 housekeeper-4.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2023-10-06 13:11:31.000000 housekeeper-4.8.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2023-10-06 13:11:40.877644 housekeeper-4.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2023-10-06 13:11:31.000000 housekeeper-4.8.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.865644 housekeeper-4.8.8/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.869644 housekeeper-4.8.8/housekeeper/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/archive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.869644 housekeeper-4.8.8/housekeeper/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/cli/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/cli/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/cli/include.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/cli/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/include.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.869644 housekeeper-4.8.8/housekeeper/store/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.869644 housekeeper-4.8.8/housekeeper/store/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/api/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.869644 housekeeper-4.8.8/housekeeper/store/api/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/api/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/api/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/api/handlers/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9449 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/api/handlers/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/api/handlers/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/api/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.869644 housekeeper-4.8.8/housekeeper/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/filters/archive_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/filters/bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/filters/file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/filters/tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/filters/version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/filters/version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2023-10-06 13:11:31.000000 housekeeper-4.8.8/housekeeper/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.869644 housekeeper-4.8.8/housekeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2023-10-06 13:11:40.000000 housekeeper-4.8.8/housekeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2023-10-06 13:11:40.000000 housekeeper-4.8.8/housekeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 13:11:40.000000 housekeeper-4.8.8/housekeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-06 13:11:40.000000 housekeeper-4.8.8/housekeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 13:11:40.000000 housekeeper-4.8.8/housekeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-06 13:11:40.000000 housekeeper-4.8.8/housekeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-06 13:11:40.000000 housekeeper-4.8.8/housekeeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-10-06 13:11:31.000000 housekeeper-4.8.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-06 13:11:31.000000 housekeeper-4.8.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-06 13:11:31.000000 housekeeper-4.8.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-06 13:11:40.877644 housekeeper-4.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2023-10-06 13:11:31.000000 housekeeper-4.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.869644 housekeeper-4.8.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.873644 housekeeper-4.8.8/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.873644 housekeeper-4.8.8/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/add/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/add/test_cli_add_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/add/test_cli_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/add/test_cli_add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/add/test_cli_add_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.873644 housekeeper-4.8.8/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/delete/test_cli_delete_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/delete/test_cli_delete_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/delete/test_cli_delete_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/delete/test_cli_delete_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.873644 housekeeper-4.8.8/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/get/test_get_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/get/test_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/get/test_get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/get/test_get_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/test_cli_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/cli/test_cli_include.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13944 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.873644 housekeeper-4.8.8/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.873644 housekeeper-4.8.8/tests/fixtures/sequencing_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/fixtures/sequencing_files/lane1.spring
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/fixtures/sequencing_files/lane2.spring
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.873644 housekeeper-4.8.8/tests/fixtures/vcfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/fixtures/vcfs/example.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/fixtures/vcfs/example.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/fixtures/vcfs/family.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/fixtures/vcfs/family.3.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/fixtures/vcfs/family.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.873644 housekeeper-4.8.8/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.873644 housekeeper-4.8.8/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/store/filters/test_archive_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/store/filters/test_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/store/filters/test_file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/store/filters/test_tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/store/filters/test_version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/store/filters/test_version_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:11:40.873644 housekeeper-4.8.8/tests/store/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/store/handlers/test_createhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/store/handlers/test_readhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/store/handlers/test_updatehandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/store/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-10-06 13:11:31.000000 housekeeper-4.8.8/tests/test_include.py
```

### Comparing `housekeeper-4.8.7/LICENSE` & `housekeeper-4.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/README.md` & `housekeeper-4.8.8/README.md`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/cli/add.py` & `housekeeper-4.8.8/housekeeper/cli/add.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/cli/core.py` & `housekeeper-4.8.8/housekeeper/cli/core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/cli/delete.py` & `housekeeper-4.8.8/housekeeper/cli/delete.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/cli/get.py` & `housekeeper-4.8.8/housekeeper/cli/get.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/cli/include.py` & `housekeeper-4.8.8/housekeeper/cli/include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/cli/init.py` & `housekeeper-4.8.8/housekeeper/cli/init.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/cli/tables.py` & `housekeeper-4.8.8/housekeeper/cli/tables.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/date.py` & `housekeeper-4.8.8/housekeeper/date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/files.py` & `housekeeper-4.8.8/housekeeper/files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/include.py` & `housekeeper-4.8.8/housekeeper/include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/store/api/core.py` & `housekeeper-4.8.8/housekeeper/store/api/core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/store/api/handlers/base.py` & `housekeeper-4.8.8/housekeeper/store/api/handlers/base.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/store/api/handlers/create.py` & `housekeeper-4.8.8/housekeeper/store/api/handlers/create.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/store/api/handlers/read.py` & `housekeeper-4.8.8/housekeeper/store/api/handlers/read.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/store/api/handlers/update.py` & `housekeeper-4.8.8/housekeeper/store/api/handlers/update.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/store/api/schema.py` & `housekeeper-4.8.8/housekeeper/store/api/schema.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/store/filters/archive_filters.py` & `housekeeper-4.8.8/housekeeper/store/filters/archive_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/store/filters/bundle_filters.py` & `housekeeper-4.8.8/housekeeper/store/filters/bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/store/filters/file_filters.py` & `housekeeper-4.8.8/housekeeper/store/filters/file_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/store/filters/tag_filters.py` & `housekeeper-4.8.8/housekeeper/store/filters/tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/store/filters/version_bundle_filters.py` & `housekeeper-4.8.8/housekeeper/store/filters/version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/store/filters/version_filters.py` & `housekeeper-4.8.8/housekeeper/store/filters/version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper/store/models.py` & `housekeeper-4.8.8/housekeeper/store/models.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/housekeeper.egg-info/SOURCES.txt` & `housekeeper-4.8.8/housekeeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/setup.py` & `housekeeper-4.8.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 setup(
     name=NAME,
     # Versions should comply with PEP440. For a discussion on
     # single-sourcing the version across setup.py and the project code,
     # see http://packaging.python.org/en/latest/tutorial.html#version
-    version="4.8.7",
+    version="4.8.8",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     # What does your project relate to? Separate with spaces.
     keywords="housekeeper development",
     author=AUTHOR,
     author_email=EMAIL,
```

### Comparing `housekeeper-4.8.7/tests/cli/add/test_cli_add_bundle.py` & `housekeeper-4.8.8/tests/cli/add/test_cli_add_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/add/test_cli_add_file.py` & `housekeeper-4.8.8/tests/cli/add/test_cli_add_file.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/add/test_cli_add_tags.py` & `housekeeper-4.8.8/tests/cli/add/test_cli_add_tags.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/add/test_cli_add_version.py` & `housekeeper-4.8.8/tests/cli/add/test_cli_add_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/conftest.py` & `housekeeper-4.8.8/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/delete/test_cli_delete_bundle.py` & `housekeeper-4.8.8/tests/cli/delete/test_cli_delete_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/delete/test_cli_delete_file.py` & `housekeeper-4.8.8/tests/cli/delete/test_cli_delete_file.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/delete/test_cli_delete_files.py` & `housekeeper-4.8.8/tests/cli/delete/test_cli_delete_files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/delete/test_cli_delete_version.py` & `housekeeper-4.8.8/tests/cli/delete/test_cli_delete_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/get/test_get_bundle.py` & `housekeeper-4.8.8/tests/cli/get/test_get_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/get/test_get_files.py` & `housekeeper-4.8.8/tests/cli/get/test_get_files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/get/test_get_tag.py` & `housekeeper-4.8.8/tests/cli/get/test_get_tag.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/get/test_get_version.py` & `housekeeper-4.8.8/tests/cli/get/test_get_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/test_cli_core.py` & `housekeeper-4.8.8/tests/cli/test_cli_core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/cli/test_cli_include.py` & `housekeeper-4.8.8/tests/cli/test_cli_include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/conftest.py` & `housekeeper-4.8.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/helper_functions.py` & `housekeeper-4.8.8/tests/helper_functions.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/store/conftest.py` & `housekeeper-4.8.8/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/store/filters/test_archive_filters.py` & `housekeeper-4.8.8/tests/store/filters/test_archive_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/store/filters/test_bundle_filters.py` & `housekeeper-4.8.8/tests/store/filters/test_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/store/filters/test_file_filters.py` & `housekeeper-4.8.8/tests/store/filters/test_file_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/store/filters/test_tag_filters.py` & `housekeeper-4.8.8/tests/store/filters/test_tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/store/filters/test_version_bundle_filters.py` & `housekeeper-4.8.8/tests/store/filters/test_version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/store/filters/test_version_filters.py` & `housekeeper-4.8.8/tests/store/filters/test_version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/store/handlers/test_createhandler.py` & `housekeeper-4.8.8/tests/store/handlers/test_createhandler.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/store/handlers/test_readhandler.py` & `housekeeper-4.8.8/tests/store/handlers/test_readhandler.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/store/handlers/test_updatehandler.py` & `housekeeper-4.8.8/tests/store/handlers/test_updatehandler.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/store/test_models.py` & `housekeeper-4.8.8/tests/store/test_models.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/test_date.py` & `housekeeper-4.8.8/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.8.7/tests/test_include.py` & `housekeeper-4.8.8/tests/test_include.py`

 * *Files identical despite different names*

