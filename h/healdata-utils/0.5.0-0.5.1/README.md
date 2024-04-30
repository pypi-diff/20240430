# Comparing `tmp/healdata_utils-0.5.0.tar.gz` & `tmp/healdata_utils-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healdata_utils-0.5.0.tar", last modified: Tue Mar 19 22:33:10 2024, max compression
+gzip compressed data, was "healdata_utils-0.5.1.tar", last modified: Tue Apr 30 18:56:33 2024, max compression
```

## Comparing `healdata_utils-0.5.0.tar` & `healdata_utils-0.5.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.729730 healdata_utils-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-19 22:33:10.729730 healdata_utils-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 22:33:10.729730 healdata_utils-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.717730 healdata_utils-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.721731 healdata_utils-0.5.0/src/healdata_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.721731 healdata_utils-0.5.0/src/healdata_utils/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/mappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/mappings/names.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/mappings/values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/mappings/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.721731 healdata_utils-0.5.0/src/healdata_utils/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23837 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/schemas/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    86519 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/schemas/redcap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.721731 healdata_utils-0.5.0/src/healdata_utils/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.721731 healdata_utils-0.5.0/src/healdata_utils/transforms/csvdata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/csvdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/csvdata/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.721731 healdata_utils-0.5.0/src/healdata_utils/transforms/csvdatadict/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/csvdatadict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/csvdatadict/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.725731 healdata_utils-0.5.0/src/healdata_utils/transforms/excel/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/excel/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.725731 healdata_utils-0.5.0/src/healdata_utils/transforms/frictionless/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/frictionless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/frictionless/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.725731 healdata_utils-0.5.0/src/healdata_utils/transforms/jsontemplate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/jsontemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/jsontemplate/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.725731 healdata_utils-0.5.0/src/healdata_utils/transforms/readstat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/readstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/readstat/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.725731 healdata_utils-0.5.0/src/healdata_utils/transforms/redcapcsv/
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/redcapcsv/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/redcapcsv/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/redcapcsv/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.725731 healdata_utils-0.5.0/src/healdata_utils/transforms/sas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/sas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/sas/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.725731 healdata_utils-0.5.0/src/healdata_utils/transforms/spss/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/spss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/spss/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.725731 healdata_utils-0.5.0/src/healdata_utils/transforms/stata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/stata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/transforms/stata/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.725731 healdata_utils-0.5.0/src/healdata_utils/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/types/typesets.py
--rw-r--r--   0 runner    (1001) docker     (127)    15198 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.725731 healdata_utils-0.5.0/src/healdata_utils/validators/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/validators/frictionless.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/validators/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/src/healdata_utils/validators/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.729730 healdata_utils-0.5.0/src/healdata_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-19 22:33:10.000000 healdata_utils-0.5.0/src/healdata_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-19 22:33:10.000000 healdata_utils-0.5.0/src/healdata_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 22:33:10.000000 healdata_utils-0.5.0/src/healdata_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-19 22:33:10.000000 healdata_utils-0.5.0/src/healdata_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-19 22:33:10.000000 healdata_utils-0.5.0/src/healdata_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-19 22:33:10.000000 healdata_utils-0.5.0/src/healdata_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:33:10.729730 healdata_utils-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/tests/test_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-03-19 22:33:02.000000 healdata_utils-0.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.618081 healdata_utils-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-30 18:56:33.618081 healdata_utils-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:56:33.618081 healdata_utils-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.606081 healdata_utils-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.610081 healdata_utils-0.5.1/src/healdata_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.610081 healdata_utils-0.5.1/src/healdata_utils/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/mappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/mappings/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/mappings/values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/mappings/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.610081 healdata_utils-0.5.1/src/healdata_utils/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23837 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/schemas/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86519 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/schemas/redcap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.610081 healdata_utils-0.5.1/src/healdata_utils/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.614081 healdata_utils-0.5.1/src/healdata_utils/transforms/csvdata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/csvdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/csvdata/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.614081 healdata_utils-0.5.1/src/healdata_utils/transforms/csvdatadict/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/csvdatadict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9390 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/csvdatadict/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.614081 healdata_utils-0.5.1/src/healdata_utils/transforms/excel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/excel/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.614081 healdata_utils-0.5.1/src/healdata_utils/transforms/frictionless/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/frictionless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/frictionless/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.614081 healdata_utils-0.5.1/src/healdata_utils/transforms/jsontemplate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/jsontemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/jsontemplate/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.614081 healdata_utils-0.5.1/src/healdata_utils/transforms/readstat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/readstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/readstat/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.614081 healdata_utils-0.5.1/src/healdata_utils/transforms/redcapcsv/
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/redcapcsv/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/redcapcsv/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/redcapcsv/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.614081 healdata_utils-0.5.1/src/healdata_utils/transforms/sas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/sas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/sas/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.614081 healdata_utils-0.5.1/src/healdata_utils/transforms/spss/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/spss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/spss/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.614081 healdata_utils-0.5.1/src/healdata_utils/transforms/stata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/stata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/transforms/stata/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.614081 healdata_utils-0.5.1/src/healdata_utils/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/types/typesets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.618081 healdata_utils-0.5.1/src/healdata_utils/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/validators/frictionless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/validators/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/src/healdata_utils/validators/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.618081 healdata_utils-0.5.1/src/healdata_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-30 18:56:33.000000 healdata_utils-0.5.1/src/healdata_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-30 18:56:33.000000 healdata_utils-0.5.1/src/healdata_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:56:33.000000 healdata_utils-0.5.1/src/healdata_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 18:56:33.000000 healdata_utils-0.5.1/src/healdata_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-30 18:56:33.000000 healdata_utils-0.5.1/src/healdata_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 18:56:33.000000 healdata_utils-0.5.1/src/healdata_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:56:33.618081 healdata_utils-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/tests/test_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-30 18:56:29.000000 healdata_utils-0.5.1/tests/test_utils.py
```

### Comparing `healdata_utils-0.5.0/PKG-INFO` & `healdata_utils-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: healdata_utils
-Version: 0.5.0
+Version: 0.5.1
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 Requires-Dist: petl==1.7.12
-Requires-Dist: jsonschema==4.17.3
-Requires-Dist: PyYaml==6.0
-Requires-Dist: pandas==1.4
-Requires-Dist: pyreadstat==1.2.0
-Requires-Dist: charset_normalizer==2.1
-Requires-Dist: visions==0.7.5
-Requires-Dist: click==8.1.3
+Requires-Dist: jsonschema>=4.17.3
+Requires-Dist: PyYaml>=6.0
+Requires-Dist: pandas>=1.4
+Requires-Dist: pyreadstat>=1.2.0
+Requires-Dist: charset_normalizer>=2.1
+Requires-Dist: visions>=0.7.5
+Requires-Dist: click>=8.1.3
 Requires-Dist: python-slugify
 Requires-Dist: openpyxl
 
 # HEAL Data Utilities
 
 The HEAL Data Utilities python package provides data packaging tools for the HEAL Data Ecosystem to facilitate data discovery, sharing, and harmonization on the [HEAL Platform](https://healdata.org).
```

### Comparing `healdata_utils-0.5.0/README.md` & `healdata_utils-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/setup.py` & `healdata_utils-0.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,31 +4,29 @@
 
 os.chdir(Path(__file__).parent)
 def generate_long_description():
     return Path("README.md").read_text()
 
 def get_install_requirements():
     return '''petl==1.7.12
-jsonschema==4.17.3
-# requests==2.28.2
-PyYaml==6.0
-#frictionless==4.40.8
-pandas==1.4
-pyreadstat==1.2.0
-charset_normalizer==2.1
-visions== 0.7.5
-click==8.1.3
+jsonschema>=4.17.3
+PyYaml>=6.0
+pandas>=1.4
+pyreadstat>=1.2.0
+charset_normalizer>=2.1
+visions>=0.7.5
+click>=8.1.3
 python-slugify
 openpyxl
 
 '''
 
 setup(
     name='healdata_utils',
-    version='0.5.0',
+    version='0.5.1',
     author='Michael Kranz',
     author_email='kranz-michael@norc.org',
     long_description=generate_long_description(),
     long_description_content_type="text/markdown",    
     description='Data packaging tools for the HEAL data ecosystem',
     #TODO: change url to HEAL once migrated.
     url='https://github.com/norc-heal/healdata-utils',
```

### Comparing `healdata_utils-0.5.0/src/healdata_utils/cli.py` & `healdata_utils-0.5.1/src/healdata_utils/cli.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/conversion.py` & `healdata_utils-0.5.1/src/healdata_utils/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/io.py` & `healdata_utils-0.5.1/src/healdata_utils/io.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/mappings/names.py` & `healdata_utils-0.5.1/src/healdata_utils/mappings/names.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/mappings/values.py` & `healdata_utils-0.5.1/src/healdata_utils/mappings/values.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/mappings/versions.py` & `healdata_utils-0.5.1/src/healdata_utils/mappings/versions.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/schemas/csv.py` & `healdata_utils-0.5.1/src/healdata_utils/schemas/csv.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/schemas/json.py` & `healdata_utils-0.5.1/src/healdata_utils/schemas/json.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/schemas/redcap.py` & `healdata_utils-0.5.1/src/healdata_utils/schemas/redcap.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/transforms/csvdata/conversion.py` & `healdata_utils-0.5.1/src/healdata_utils/transforms/csvdata/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/transforms/csvdatadict/conversion.py` & `healdata_utils-0.5.1/src/healdata_utils/transforms/csvdatadict/conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -124,16 +124,14 @@
         ["fields"]
         ["items"]
         ["properties"]
     )
     
     # init to-be formatted tables
     tbl_csv = template_tbl.copy()
-    tbl_json = template_tbl.copy()
-
     # transform each column with slugified mappings, harmonizing delims (if array, object) 
     for colname in tbl_csv.columns.tolist():
         slugified_col = slugify(colname)
         newcolname = colname
 
         # rename based on slugified names or original col names
         newcolname = renamemap.get(slugified_col) or renamemap.get(colname)
@@ -149,18 +147,22 @@
                 .apply(slugify)
                 .replace(recodemap[newcolname])
             )
 
         if newcolname in droplist:
             del tbl_csv[newcolname]
 
+        # NOTE: the below methodology uses the schema to instruct how to convert to json.
         fieldpropname = utils.find_propname(newcolname,field_properties)
         fieldprop = field_properties.get(fieldpropname)
+        # infer delimiters of stringified lists (note: stringified lists are identified from schema)
 
-        if fieldprop:
+        
+        if fieldpropname:
+            
             if fieldprop["type"] == "integer":
                 tbl_csv[newcolname] = tbl_csv[newcolname].apply(lambda s: int(float(s)) if s else s)
             elif fieldprop["type"] == "number":
                 tbl_csv[newcolname] = tbl_csv[newcolname].astype(float)
             elif fieldprop["type"] == "object":
 
                 possible_keyval = ["=",":"]
@@ -176,27 +178,50 @@
 
             elif fieldprop["type"] == "array":
                 possible_list = [";","|"]
                 item_sep = infer_delim(tbl_csv[newcolname],possible_list,firstmatch=False) or "|"
                 tbl_csv[newcolname] = tbl_csv[newcolname].replace(item_sep,"|")
 
     # parse string objects and array to create the dict (json) instance
-    tbl_json = tbl_csv.copy()
+    tbl_json = tbl_csv.copy()   
     for colname in tbl_json.columns.tolist():
+        # NOTE: the below methodology uses the schema to instruct how to convert to json.
         fieldpropname = utils.find_propname(colname,field_properties)
         fieldprop = field_properties.get(fieldpropname)
         if fieldprop:
             if fieldprop["type"] == "object":
                 tbl_json[colname] = tbl_csv[colname].apply(
                     utils.parse_dictionary_str,
                     item_sep="|",keyval_sep="=")
             
             elif fieldprop["type"] == "array":
                 tbl_json[colname] = tbl_csv[colname].apply(
                     utils.parse_list_str,item_sep="|")
+        # columns not included in schema (custom or other)
+        else:
+            if colname.split(".")[0] == "custom":
+                
+                if not "custom" in tbl_json:
+                    tbl_json["custom"] = [{}] * len(tbl_json)
+
+                for i in range(len(tbl_csv)):
+                    value = tbl_csv[colname].iloc[i]
+                    if value:
+                        custom = {}
+                        parts = colname.split(".")[1:]
+                        
+                        for key in reversed(parts):
+                            result = {key: value}
+
+                        tbl_json["custom"].iloc[i].update(result)
+            else:
+                tbl_json[colname] = tbl_csv[colname]
+
+    # drop all custom columns (as I have nested already)
+    tbl_json.drop(columns=tbl_json.filter(regex="^custom\\.").columns, inplace=True)
 
     # refactor (i.e., cascade, move up to root) properties if present in all records
     refactored_props,tbl_json = utils.refactor_field_props(
         tbl_json,schema=schemas.healjsonschema)
 
     # data dictionary root level properties
     data_dictionary_props_csv = dict(data_dictionary_props)
```

### Comparing `healdata_utils-0.5.0/src/healdata_utils/transforms/excel/conversion.py` & `healdata_utils-0.5.1/src/healdata_utils/transforms/excel/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/transforms/frictionless/conversion.py` & `healdata_utils-0.5.1/src/healdata_utils/transforms/frictionless/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/transforms/jsontemplate/conversion.py` & `healdata_utils-0.5.1/src/healdata_utils/transforms/jsontemplate/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,16 +75,16 @@
             for f in fields_json])
     flattened_data_dictionary_props = pd.Series(utils.flatten_to_jsonpath(data_dictionary_props,schemas.healjsonschema))
 
     flattened_and_embedded = utils.embed_data_dictionary_props(flattened_fields,flattened_data_dictionary_props,schemas.healjsonschema)
     tbl_csv = (
         flattened_and_embedded
         .fillna("")
-        .applymap(lambda v: utils.join_dictitems(v) if isinstance(v,collections.abc.MutableMapping) else v)
-        .applymap(lambda v: utils.join_iter(v) if isinstance(v,collections.abc.MutableSequence) else v)
+        .map(lambda v: utils.join_dictitems(v) if isinstance(v,collections.abc.MutableMapping) else v)
+        .map(lambda v: utils.join_iter(v) if isinstance(v,collections.abc.MutableSequence) else v)
     )
     fields_csv = tbl_csv.to_dict(orient="records")
 
     template_json = {**data_dictionary_props,"fields":fields_json}
     template_csv = {**data_dictionary_props,"fields":fields_csv}
 
     return {"templatejson":template_json,"templatecsv":template_csv}
```

### Comparing `healdata_utils-0.5.0/src/healdata_utils/transforms/readstat/conversion.py` & `healdata_utils-0.5.1/src/healdata_utils/transforms/readstat/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/transforms/redcapcsv/conversion.py` & `healdata_utils-0.5.1/src/healdata_utils/transforms/redcapcsv/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Reads in a path to a redcap csv file
     and outputs and dictionary with cleaned up header (field) names
     """ 
     sourcedf = (
         read_delim(file_path)
         .fillna("")
         .rename(columns=headers.mapping)
-        .applymap(utils.strip_html)
+        .map(utils.strip_html)
     )
 
     #downfill section (if blank -- given we read in with petl, blanks are "" but ffill takes in np.nan)
     sourcedf['section'] = sourcedf.replace({"":np.nan}).groupby('form')['section'].ffill()
 
     sourcedf.fillna("",inplace=True)
```

### Comparing `healdata_utils-0.5.0/src/healdata_utils/transforms/redcapcsv/headers.py` & `healdata_utils-0.5.1/src/healdata_utils/transforms/redcapcsv/headers.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/transforms/redcapcsv/mappings.py` & `healdata_utils-0.5.1/src/healdata_utils/transforms/redcapcsv/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/transforms/sas/conversion.py` & `healdata_utils-0.5.1/src/healdata_utils/transforms/sas/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/types/typesets.py` & `healdata_utils-0.5.1/src/healdata_utils/types/typesets.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/utils.py` & `healdata_utils-0.5.1/src/healdata_utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     """  
     flat_fields_df = pd.DataFrame(flat_fields)
     propnames = _get_propnames_to_rearrange(flat_fields_df.columns.tolist(),schema)
     flat_record = pd.Series(dtype="object")
     for name in propnames:
         in_df = name in flat_fields_df
-        is_one_unique = len(flat_fields_df[name].unique()) == 1 # NOTE: Includes NA values which is desired
+        is_one_unique = len(flat_fields_df[name].map(str).unique()) == 1 # NOTE: Includes NA values which is desired
         if in_df and is_one_unique:
             flat_record[name] = flat_fields_df.pop(name).iloc[0]
             
 
     return flat_record,flat_fields_df
 
 # individual cell utilities
@@ -165,75 +165,61 @@
     return dict(items)
 
 def stringify_keys(dictionary):
     orig_keys = list(dictionary.keys())
     for key in orig_keys:
         dictionary[str(key)] = dictionary.pop(key)
 
-def unflatten_from_jsonpath(field):
+
+def unflatten_from_jsonpath(field,missing_values=[None,""]):
     """
     Converts a flattened dictionary with key names conforming to 
     JSONpath notation to the nested dictionary format.
     """
     field_json = {}
 
     for prop_path, prop in field.items():
+        
+        if prop in missing_values:
+            continue
+
         prop_json = field_json
 
-        # if isinstance(prop,list):
-        #     prop = [v for val in prop if if val != None or val != ""]
-        # elif isinstance(prop,dict):
-        #     # filter falsey  values of "" and None
-        #     prop = {key:val for key,val in prop.items() if val != None or val != ""}
-
-
-        if prop:
-            # Get the necessary info from the JSON path 
-            nested_names = [re.sub("\[\d+\]$", "", prop_name) for prop_name in prop_path.split(".")]
-            nested_indices = [re.findall("\[(\d+)\]$", prop_name)[-1] if re.search("\[(\d+)\]$", prop_name) else None for prop_name in prop_path.split(".")]
-
-            for prop_name, array_index in zip(nested_names, nested_indices):
-                is_last_nested = prop_name == nested_names[-1]
-
-                if array_index is not None:
-                    # Handle array properties
-                    if prop_name not in prop_json:
-                        prop_json[prop_name] = [None] * (int(array_index) + 1)
-
-                    if is_last_nested:
-                        if prop_json[prop_name][int(array_index)] is None:
-                            prop_json[prop_name][int(array_index)] = {}
-                        
-                        if isinstance(prop_json[prop_name][int(array_index)], dict):
-                            prop_json[prop_name][int(array_index)].update({prop_name: prop})
-                        else:
-                            prop_json[prop_name][int(array_index)] = {prop_name: prop}
-                    else:
-                        if prop_json[prop_name][int(array_index)] is None:
-                            prop_json[prop_name][int(array_index)] = {}
-                        
-                        prop_json = prop_json[prop_name][int(array_index)]
-                else:
-                    # Handle non-array properties
-                    if is_last_nested:
-                        if prop_name not in prop_json:
-                            prop_json[prop_name] = prop
-                        else:
-                            if isinstance(prop_json[prop_name], dict):
-                                prop_json[prop_name].update({prop_name: prop})
-                            else:
-                                prop_json[prop_name] = {prop_name: prop}
-                    else:
-                        if prop_name not in prop_json:
-                            prop_json[prop_name] = {}
-                        
-                        prop_json = prop_json[prop_name]
+        nested_names = prop_path.split(".")
+        for prop_name in nested_names[:-1]:
+            if '[' in prop_name:
+                array_name, array_index = prop_name.split('[')
+                array_index = int(array_index[:-1])
+                if array_name not in prop_json:
+                    prop_json[array_name] = [{} for _ in range(array_index + 1)]
+                elif len(prop_json[array_name]) <= array_index:
+                    prop_json[array_name].extend([{} for _ in range(array_index - len(prop_json[array_name]) + 1)])
+                prop_json = prop_json[array_name][array_index]
+            else:
+                if prop_name not in prop_json:
+                    prop_json[prop_name] = {}
+                prop_json = prop_json[prop_name]
+
+        last_prop_name = nested_names[-1]
+        if '[' in last_prop_name:
+            array_name, array_index = last_prop_name.split('[')
+            array_index = int(array_index[:-1])
+            if array_name not in prop_json:
+                prop_json[array_name] = [{} for _ in range(array_index + 1)]
+            elif len(prop_json[array_name]) <= array_index:
+                prop_json[array_name].extend([{} for _ in range(array_index - len(prop_json[array_name]) + 1)])
+            if isinstance(prop_json[array_name][array_index], dict):
+                prop_json[array_name][array_index].update({array_name: prop})
+            else:
+                prop_json[array_name][array_index] = {array_name: prop}
+        else:
+            prop_json[last_prop_name] = prop
 
     return field_json
-
+    
 # json to csv utils
 def join_iter(iterable,sep_list="|"):
     return sep_list.join([str(p) for p in iterable])
 
 def join_dictvals(dictionary:dict,sep:str):
     return sep.join(dictionary.values())
 
@@ -404,17 +390,20 @@
     given a dictionary of json schema object properties OR a list of property names, return the 
     matching property name. 
 
     This function is needed when a schema is flattened according to a json path 
     and converted into a regular expression for list (array) indices.
 
     """ 
-    propmatch = re.findall("|".join("^"+name+"$" for name in list(properties)),colname)
+    propmatch = []
+    for name in list(properties):
+        if re.match("^"+name+"$",colname):
+            propmatch.append(name)
 
     if len(propmatch) == 1:
         return propmatch[0]
     elif len(propmatch) > 1:
         raise Exception(f"Multiple matching properties found for {colname}. Can only have one match")
     elif len(propmatch) == 0:
-        raise Exception(f"No matching properties found for {colname}")
+        return None
     else:
         raise Exception(f"Unknown error when matching properties against {colname}")
```

### Comparing `healdata_utils-0.5.0/src/healdata_utils/validators/jsonschema.py` & `healdata_utils-0.5.1/src/healdata_utils/validators/jsonschema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils/validators/validate.py` & `healdata_utils-0.5.1/src/healdata_utils/validators/validate.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/src/healdata_utils.egg-info/PKG-INFO` & `healdata_utils-0.5.1/src/healdata_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: healdata_utils
-Version: 0.5.0
+Version: 0.5.1
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 Requires-Dist: petl==1.7.12
-Requires-Dist: jsonschema==4.17.3
-Requires-Dist: PyYaml==6.0
-Requires-Dist: pandas==1.4
-Requires-Dist: pyreadstat==1.2.0
-Requires-Dist: charset_normalizer==2.1
-Requires-Dist: visions==0.7.5
-Requires-Dist: click==8.1.3
+Requires-Dist: jsonschema>=4.17.3
+Requires-Dist: PyYaml>=6.0
+Requires-Dist: pandas>=1.4
+Requires-Dist: pyreadstat>=1.2.0
+Requires-Dist: charset_normalizer>=2.1
+Requires-Dist: visions>=0.7.5
+Requires-Dist: click>=8.1.3
 Requires-Dist: python-slugify
 Requires-Dist: openpyxl
 
 # HEAL Data Utilities
 
 The HEAL Data Utilities python package provides data packaging tools for the HEAL Data Ecosystem to facilitate data discovery, sharing, and harmonization on the [HEAL Platform](https://healdata.org).
```

### Comparing `healdata_utils-0.5.0/src/healdata_utils.egg-info/SOURCES.txt` & `healdata_utils-0.5.1/src/healdata_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/tests/test_cli.py` & `healdata_utils-0.5.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/tests/test_conversion.py` & `healdata_utils-0.5.1/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/tests/test_io.py` & `healdata_utils-0.5.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.5.0/tests/test_utils.py` & `healdata_utils-0.5.1/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,16 @@
                     **schema_version,
                     **another_field_to_rearrange,
                 }
             },
         },
     },
 }
+
+
 def test_add_missing_fields():
     # data (note one var not in schema)
     data = [
         {"var2": 2, "var3": 3, "var1": 1},
         {
             "var5": 10,
             "var4": 9,
@@ -58,29 +60,37 @@
 
 
 def test_unflatten_jsonpath():
     input = {
         "module": "Testing",
         "constraints.enum": "1|2|3|4",
         "standardsMappings[1].item.url": "http//:helloitem1",
-        "standardsMappings[0].item.url": "http//:helloitem2",
-        "standardsMappings[1].instrument.url": "http//:helloworld4",
+        "standardsMappings[0].item.url": "http//:helloitem0",
+        "standardsMappings[0].instrument.url": "http//:helloworld0",
+        "standardsMappings[1].instrument.url": "http//:helloworld1",
+        "standardsMappings[2].item.url": "http//:helloitem2",
         "test1.test2.test3[1]": "test3_1",
         "test1.test2.test3[0].test4": "test4_1",
     }
 
     output = {
         "module": "Testing",
         "constraints": {"enum": "1|2|3|4"},
         "standardsMappings": [
-            {"item": {"url": "http//:helloitem2"}},
+            {
+                "item": {"url": "http//:helloitem0"},
+                "instrument": {"url": "http//:helloworld0"},
+            },
             {
                 "item": {"url": "http//:helloitem1"},
-                "instrument": {"url": "http//:helloworld4"},
+                "instrument": {"url": "http//:helloworld1"},
             },
+            {
+                "item":{"url":"http//:helloitem2"}
+            }
         ],
         "test1": {"test2": {"test3": [{"test4": "test4_1"}, {"test3": "test3_1"}]}},
     }
     field_json = utils.unflatten_from_jsonpath(input)
     assert (
         field_json == output
     ), "Problem with converting input dictionary to output dictionary"
@@ -96,15 +106,17 @@
 def test_embed_data_dictionary_props():
 
     flat_root = {
         "schemaVersion": "0.2.0",
         "anotherFieldToEmbed[0].thisone": "helloworld",
     }
     flat_fields_array = [{"justAField": "cool"}, {"justAField": "sad"}]
-    flat_fields = utils.embed_data_dictionary_props(flat_fields_array, flat_root, schema_to_rearrange)
+    flat_fields = utils.embed_data_dictionary_props(
+        flat_fields_array, flat_root, schema_to_rearrange
+    )
 
     assert flat_fields.to_dict(orient="records") == [
         {
             "justAField": "cool",
             "schemaVersion": "0.2.0",
             "anotherFieldToEmbed[0].thisone": "helloworld",
         },
@@ -117,14 +129,16 @@
 
 
 def test_refactor_field_props():
     flat_fields_array = [
         {"justAField": "cool", "anotherFieldToEmbed[0].thisone": "helloworld"},
         {"justAField": "sad", "anotherFieldToEmbed[0].thisone": "helloworld"},
     ]
-    flat_root, flat_fields = utils.refactor_field_props(flat_fields_array, schema_to_rearrange)
+    flat_root, flat_fields = utils.refactor_field_props(
+        flat_fields_array, schema_to_rearrange
+    )
 
     assert flat_root.to_dict() == {"anotherFieldToEmbed[0].thisone": "helloworld"}
     assert flat_fields.to_dict(orient="records") == [
         {"justAField": "cool"},
         {"justAField": "sad"},
     ]
```

