# Comparing `tmp/ignition_api_stubs-8.1.39.tar.gz` & `tmp/ignition_api_stubs-8.1.39.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignition_api_stubs-8.1.39.tar", last modified: Fri Apr 12 21:08:48 2024, max compression
+gzip compressed data, was "ignition_api_stubs-8.1.39.post1.tar", last modified: Tue Apr 30 18:35:45 2024, max compression
```

## Comparing `ignition_api_stubs-8.1.39.tar` & `ignition_api_stubs-8.1.39.post1.tar`

### file list

```diff
@@ -1,418 +1,418 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.518378 ignition_api_stubs-8.1.39/
--rw-rw-r--   0 root         (0) root         (0)     4918 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/CHANGELOG.md
--rw-rw-r--   0 root         (0) root         (0)     1070 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       21 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4745 2024-04-12 21:08:48.518378 ignition_api_stubs-8.1.39/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2042 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/README.md
--rw-rw-r--   0 root         (0) root         (0)     1584 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 21:08:48.518378 ignition_api_stubs-8.1.39/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.470378 ignition_api_stubs-8.1.39/stubs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.470378 ignition_api_stubs-8.1.39/stubs/ch/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/ch/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.470378 ignition_api_stubs-8.1.39/stubs/ch/qos/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/ch/qos/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.470378 ignition_api_stubs-8.1.39/stubs/ch/qos/logback/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/ch/qos/logback/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/ch/qos/logback/classic/
--rw-rw-r--   0 root         (0) root         (0)      646 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/ch/qos/logback/classic/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/codahale/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/codahale/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/codahale/metrics/
--rw-rw-r--   0 root         (0) root         (0)     1271 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/codahale/metrics/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/google/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/google/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/google/common/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/google/common/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/google/common/collect/
--rw-rw-r--   0 root         (0) root         (0)     2204 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/google/common/collect/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/google/common/eventbus/
--rw-rw-r--   0 root         (0) root         (0)      355 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/google/common/eventbus/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/
--rw-rw-r--   0 root         (0) root         (0)     1776 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/binding/
--rw-rw-r--   0 root         (0) root         (0)      875 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/binding/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/components/
--rw-rw-r--   0 root         (0) root         (0)      281 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/components/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/model/
--rw-rw-r--   0 root         (0) root         (0)      193 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/model/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/script/
--rw-rw-r--   0 root         (0) root         (0)      256 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/script/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/script/builtin/
--rw-rw-r--   0 root         (0) root         (0)     7672 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/script/builtin/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/sqltags/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/sqltags/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.474377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/sqltags/project/
--rw-rw-r--   0 root         (0) root         (0)      136 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/sqltags/project/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/alarming/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/alarming/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/alarming/common/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/alarming/common/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/alarming/common/rosters/
--rw-rw-r--   0 root         (0) root         (0)      610 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/alarming/common/rosters/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/launch/
--rw-rw-r--   0 root         (0) root         (0)     6078 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/launch/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/model/
--rw-rw-r--   0 root         (0) root         (0)     4071 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/model/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/util/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/util/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/util/gui/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/util/gui/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/util/gui/progress/
--rw-rw-r--   0 root         (0) root         (0)     1598 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/util/gui/progress/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/util/gui/scheduling/
--rw-rw-r--   0 root         (0) root         (0)     1398 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/util/gui/scheduling/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/
--rw-rw-r--   0 root         (0) root         (0)    10147 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/alarming/
--rw-rw-r--   0 root         (0) root         (0)     3224 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/alarming/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/alarming/evaluation/
--rw-rw-r--   0 root         (0) root         (0)     1224 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/alarming/evaluation/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/alarming/query/
--rw-rw-r--   0 root         (0) root         (0)      814 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/alarming/query/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/binding/
--rw-rw-r--   0 root         (0) root         (0)       78 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/binding/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/browsing/
--rw-rw-r--   0 root         (0) root         (0)     3586 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/browsing/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/config/
--rw-rw-r--   0 root         (0) root         (0)     3184 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/config/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/db/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/db/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.478377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/db/namedquery/
--rw-rw-r--   0 root         (0) root         (0)      773 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/db/namedquery/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/document/
--rw-rw-r--   0 root         (0) root         (0)      215 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/document/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/execution/
--rw-rw-r--   0 root         (0) root         (0)     1165 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/execution/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/expressions/
--rw-rw-r--   0 root         (0) root         (0)     1020 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/expressions/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/expressions/functions/
--rw-rw-r--   0 root         (0) root         (0)      672 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/expressions/functions/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/functional/
--rw-rw-r--   0 root         (0) root         (0)       54 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/functional/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/gson/
--rw-rw-r--   0 root         (0) root         (0)     8729 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/gson/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/gson/reflect/
--rw-rw-r--   0 root         (0) root         (0)      284 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/gson/reflect/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/gson/stream/
--rw-rw-r--   0 root         (0) root         (0)     2052 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/gson/stream/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/gui/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/gui/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/gui/progress/
--rw-rw-r--   0 root         (0) root         (0)     1370 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/gui/progress/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/i18n/
--rw-rw-r--   0 root         (0) root         (0)      921 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/i18n/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/i18n/keyboard/
--rw-rw-r--   0 root         (0) root         (0)      862 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/i18n/keyboard/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/i18n/translation/
--rw-rw-r--   0 root         (0) root         (0)      238 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/i18n/translation/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/jsonschema/
--rw-rw-r--   0 root         (0) root         (0)     4053 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/jsonschema/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/licensing/
--rw-rw-r--   0 root         (0) root         (0)     1351 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/licensing/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/logging/
--rw-rw-r--   0 root         (0) root         (0)      883 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/logging/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/messages/
--rw-rw-r--   0 root         (0) root         (0)     1262 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/messages/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/model/
--rw-rw-r--   0 root         (0) root         (0)     3271 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/model/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/model/values/
--rw-rw-r--   0 root         (0) root         (0)     4717 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/model/values/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.482378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/modules/
--rw-rw-r--   0 root         (0) root         (0)     4705 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/modules/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/opc/
--rw-rw-r--   0 root         (0) root         (0)     3830 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/opc/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/project/
--rw-rw-r--   0 root         (0) root         (0)     3511 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/project/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/project/resource/
--rw-rw-r--   0 root         (0) root         (0)     5710 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/project/resource/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/
--rw-rw-r--   0 root         (0) root         (0)     2536 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/abc/
--rw-rw-r--   0 root         (0) root         (0)     4500 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/abc/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/adapters/
--rw-rw-r--   0 root         (0) root         (0)     1293 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/adapters/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/builtin/
--rw-rw-r--   0 root         (0) root         (0)     8418 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/builtin/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/builtin/http/
--rw-rw-r--   0 root         (0) root         (0)     2698 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/builtin/http/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/builtin/ialabs/
--rw-rw-r--   0 root         (0) root         (0)     1798 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/builtin/ialabs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/hints/
--rw-rw-r--   0 root         (0) root         (0)      370 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/hints/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/message/
--rw-rw-r--   0 root         (0) root         (0)      594 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/message/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/sqltags/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/sqltags/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/sqltags/history/
--rw-rw-r--   0 root         (0) root         (0)      414 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/sqltags/history/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/sqltags/history/annotations/
--rw-rw-r--   0 root         (0) root         (0)     1927 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/sqltags/history/annotations/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/sqltags/model/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/sqltags/model/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/sqltags/model/types/
--rw-rw-r--   0 root         (0) root         (0)     1946 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/sqltags/model/types/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/config/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/config/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/config/types/
--rw-rw-r--   0 root         (0) root         (0)      307 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/config/types/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.486378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/model/
--rw-rw-r--   0 root         (0) root         (0)     2029 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/model/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/paths/
--rw-rw-r--   0 root         (0) root         (0)     1501 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/paths/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/paths/parser/
--rw-rw-r--   0 root         (0) root         (0)      795 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/paths/parser/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/tagpaths/
--rw-rw-r--   0 root         (0) root         (0)      248 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/tagpaths/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/user/
--rw-rw-r--   0 root         (0) root         (0)     4586 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/user/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/user/schedule/
--rw-rw-r--   0 root         (0) root         (0)     4953 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/user/schedule/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/util/
--rw-rw-r--   0 root         (0) root         (0)     6003 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/util/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/xmlserialization/
--rw-rw-r--   0 root         (0) root         (0)      590 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/xmlserialization/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/xmlserialization/deserialization/
--rw-rw-r--   0 root         (0) root         (0)     2814 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/xmlserialization/deserialization/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/xmlserialization/encoding/
--rw-rw-r--   0 root         (0) root         (0)       63 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/xmlserialization/encoding/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/
--rw-rw-r--   0 root         (0) root         (0)     2234 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/equalitydelegates/
--rw-rw-r--   0 root         (0) root         (0)      139 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/equalitydelegates/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/gateway/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/gateway/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/gateway/project/
--rw-rw-r--   0 root         (0) root         (0)     1155 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/gateway/project/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/modules/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/modules/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/modules/serial/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/modules/serial/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/modules/serial/scripting/
--rw-rw-r--   0 root         (0) root         (0)     2334 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/modules/serial/scripting/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/opccom/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/opccom/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/opccom/hda/
--rw-rw-r--   0 root         (0) root         (0)     1163 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/opccom/hda/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/perspective/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/perspective/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.490378 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/perspective/common/
--rw-rw-r--   0 root         (0) root         (0)      911 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/perspective/common/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/sfc/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/sfc/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/sfc/api/
--rw-rw-r--   0 root         (0) root         (0)      104 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/sfc/api/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/vision/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/vision/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/vision/api/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/vision/api/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/vision/api/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/vision/api/client/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/vision/api/client/components/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/vision/api/client/components/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/vision/api/client/components/model/
--rw-rw-r--   0 root         (0) root         (0)      277 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/vision/api/client/components/model/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/com/palantir/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/palantir/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/com/palantir/ptoss/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/palantir/ptoss/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/com/palantir/ptoss/cinch/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/palantir/ptoss/cinch/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/com/palantir/ptoss/cinch/core/
--rw-rw-r--   0 root         (0) root         (0)      413 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/palantir/ptoss/cinch/core/__init__.pyi
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/com/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/dev/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/dev/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/dev/coatl/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/dev/coatl/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/dev/coatl/helper/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/dev/coatl/helper/__init__.pyi
--rw-rw-r--   0 root         (0) root         (0)       88 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/dev/coatl/helper/types.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.494377 ignition_api_stubs-8.1.39/stubs/dev/coatl/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/dev/coatl/utils/__init__.pyi
--rw-rw-r--   0 root         (0) root         (0)       70 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/dev/coatl/utils/decorators.pyi
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/dev/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.514378 ignition_api_stubs-8.1.39/stubs/ignition_api_stubs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4745 2024-04-12 21:08:48.000000 ignition_api_stubs-8.1.39/stubs/ignition_api_stubs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11006 2024-04-12 21:08:48.000000 ignition_api_stubs-8.1.39/stubs/ignition_api_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 21:08:48.000000 ignition_api_stubs-8.1.39/stubs/ignition_api_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-12 21:08:48.000000 ignition_api_stubs-8.1.39/stubs/ignition_api_stubs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-12 21:08:48.000000 ignition_api_stubs-8.1.39/stubs/ignition_api_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/awt/
--rw-rw-r--   0 root         (0) root         (0)     3143 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/awt/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/awt/event/
--rw-rw-r--   0 root         (0) root         (0)     2579 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/awt/event/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/awt/geom/
--rw-rw-r--   0 root         (0) root         (0)     1312 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/awt/geom/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/awt/image/
--rw-rw-r--   0 root         (0) root         (0)      128 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/awt/image/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/awt/print/
--rw-rw-r--   0 root         (0) root         (0)     1107 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/awt/print/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/beans/
--rw-rw-r--   0 root         (0) root         (0)      564 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/beans/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/io/
--rw-rw-r--   0 root         (0) root         (0)     4595 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/io/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/lang/
--rw-rw-r--   0 root         (0) root         (0)     9829 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/lang/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/lang/reflect/
--rw-rw-r--   0 root         (0) root         (0)       96 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/lang/reflect/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/math/
--rw-rw-r--   0 root         (0) root         (0)     1128 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/math/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/net/
--rw-rw-r--   0 root         (0) root         (0)     6190 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/net/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/net/http/
--rw-rw-r--   0 root         (0) root         (0)       84 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/net/http/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/nio/
--rw-rw-r--   0 root         (0) root         (0)     7653 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/nio/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/nio/channels/
--rw-rw-r--   0 root         (0) root         (0)     4672 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/nio/channels/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/nio/charset/
--rw-rw-r--   0 root         (0) root         (0)     2022 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/nio/charset/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/nio/file/
--rw-rw-r--   0 root         (0) root         (0)     7939 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/nio/file/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/nio/file/attribute/
--rw-rw-r--   0 root         (0) root         (0)     1809 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/nio/file/attribute/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.498378 ignition_api_stubs-8.1.39/stubs/java/org/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/org/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/org/jdesktop/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/org/jdesktop/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/org/jdesktop/core/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/org/jdesktop/core/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/org/jdesktop/core/animation/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/org/jdesktop/core/animation/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/org/jdesktop/core/animation/timing/
--rw-rw-r--   0 root         (0) root         (0)      155 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/org/jdesktop/core/animation/timing/__init__.pyi
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/security/
--rw-rw-r--   0 root         (0) root         (0)      343 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/security/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/text/
--rw-rw-r--   0 root         (0) root         (0)     8251 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/text/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/time/
--rw-rw-r--   0 root         (0) root         (0)     2428 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/time/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/time/format/
--rw-rw-r--   0 root         (0) root         (0)      221 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/time/format/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/time/temporal/
--rw-rw-r--   0 root         (0) root         (0)     3688 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/time/temporal/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/util/
--rw-rw-r--   0 root         (0) root         (0)    16255 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/util/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/util/concurrent/
--rw-rw-r--   0 root         (0) root         (0)     1919 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/util/concurrent/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/util/function/
--rw-rw-r--   0 root         (0) root         (0)     1427 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/util/function/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/util/regex/
--rw-rw-r--   0 root         (0) root         (0)     2813 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/util/regex/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/java/util/stream/
--rw-rw-r--   0 root         (0) root         (0)     1594 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/java/util/stream/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/javax/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/javax/__init__.pyi
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/javax/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/javax/security/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/javax/security/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/javax/security/auth/
--rw-rw-r--   0 root         (0) root         (0)      125 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/javax/security/auth/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/javax/swing/
--rw-rw-r--   0 root         (0) root         (0)     6503 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/javax/swing/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/javax/swing/event/
--rw-rw-r--   0 root         (0) root         (0)      639 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/javax/swing/event/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.502378 ignition_api_stubs-8.1.39/stubs/javax/swing/plaf/
--rw-rw-r--   0 root         (0) root         (0)      392 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/javax/swing/plaf/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/javax/swing/text/
--rw-rw-r--   0 root         (0) root         (0)      202 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/javax/swing/text/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/apache/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/apache/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/apache/commons/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/apache/commons/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/apache/commons/lang3/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/apache/commons/lang3/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/apache/commons/lang3/builder/
--rw-rw-r--   0 root         (0) root         (0)      780 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/apache/commons/lang3/builder/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/apache/commons/math3/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/apache/commons/math3/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/apache/commons/math3/exception/
--rw-rw-r--   0 root         (0) root         (0)      587 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/apache/commons/math3/exception/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/apache/commons/math3/exception/util/
--rw-rw-r--   0 root         (0) root         (0)      678 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/apache/commons/math3/exception/util/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/apache/log4j/
--rw-rw-r--   0 root         (0) root         (0)     2413 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/apache/log4j/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/apache/log4j/spi/
--rw-rw-r--   0 root         (0) root         (0)     2010 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/apache/log4j/spi/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/bson/
--rw-rw-r--   0 root         (0) root         (0)     1997 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/bson/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/bson/codecs/
--rw-rw-r--   0 root         (0) root         (0)       17 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/bson/codecs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/bson/codecs/configuration/
--rw-rw-r--   0 root         (0) root         (0)      130 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/bson/codecs/configuration/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/bson/types/
--rw-rw-r--   0 root         (0) root         (0)     2627 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/bson/types/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/json/
--rw-rw-r--   0 root         (0) root         (0)     4114 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/json/__init__.pyi
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/python/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/python/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/python/core/
--rw-rw-r--   0 root         (0) root         (0)    23034 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/python/core/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/python/expose/
--rw-rw-r--   0 root         (0) root         (0)      350 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/python/expose/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.506378 ignition_api_stubs-8.1.39/stubs/org/slf4j/
--rw-rw-r--   0 root         (0) root         (0)     1122 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/slf4j/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.510378 ignition_api_stubs-8.1.39/stubs/org/slf4j/event/
--rw-rw-r--   0 root         (0) root         (0)      167 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/org/slf4j/event/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.514378 ignition_api_stubs-8.1.39/stubs/system/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/__init__.pyi
--rw-rw-r--   0 root         (0) root         (0)       15 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/__version__.pyi
--rw-rw-r--   0 root         (0) root         (0)     2133 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/alarm.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.514378 ignition_api_stubs-8.1.39/stubs/system/bacnet/
--rw-rw-r--   0 root         (0) root         (0)     1305 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/bacnet/__init__.pyi
--rw-rw-r--   0 root         (0) root         (0)    12890 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/bacnet/enumerated.pyi
--rw-rw-r--   0 root         (0) root         (0)      780 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/bacnet/enums.pyi
--rw-rw-r--   0 root         (0) root         (0)     2380 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/dataset.pyi
--rw-rw-r--   0 root         (0) root         (0)     2292 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/date.pyi
--rw-rw-r--   0 root         (0) root         (0)     3586 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/db.pyi
--rw-rw-r--   0 root         (0) root         (0)      687 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/device.pyi
--rw-rw-r--   0 root         (0) root         (0)     1275 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/dnp3.pyi
--rw-rw-r--   0 root         (0) root         (0)      718 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/eam.pyi
--rw-rw-r--   0 root         (0) root         (0)      810 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/file.pyi
--rw-rw-r--   0 root         (0) root         (0)      220 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/groups.pyi
--rw-rw-r--   0 root         (0) root         (0)     3216 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/gui.pyi
--rw-rw-r--   0 root         (0) root         (0)      726 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/iec61850.pyi
--rw-rw-r--   0 root         (0) root         (0)     1090 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/math.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.514378 ignition_api_stubs-8.1.39/stubs/system/mongodb/
--rw-rw-r--   0 root         (0) root         (0)     2252 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/mongodb/__init__.pyi
--rw-rw-r--   0 root         (0) root         (0)      495 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/mongodb/types.pyi
--rw-rw-r--   0 root         (0) root         (0)     1095 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/nav.pyi
--rw-rw-r--   0 root         (0) root         (0)     2245 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/net.pyi
--rw-rw-r--   0 root         (0) root         (0)     1500 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/opc.pyi
--rw-rw-r--   0 root         (0) root         (0)     1539 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/opchda.pyi
--rw-rw-r--   0 root         (0) root         (0)      478 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/opcua.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:08:48.514378 ignition_api_stubs-8.1.39/stubs/system/perspective/
--rw-rw-r--   0 root         (0) root         (0)     3884 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/perspective/__init__.pyi
--rw-rw-r--   0 root         (0) root         (0)       81 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/perspective/workstation.pyi
--rw-rw-r--   0 root         (0) root         (0)      592 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/print.pyi
--rw-rw-r--   0 root         (0) root         (0)      196 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/project.pyi
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/py.typed
--rw-rw-r--   0 root         (0) root         (0)      737 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/report.pyi
--rw-rw-r--   0 root         (0) root         (0)      633 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/roster.pyi
--rw-rw-r--   0 root         (0) root         (0)     1276 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/secsgem.pyi
--rw-rw-r--   0 root         (0) root         (0)      704 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/security.pyi
--rw-rw-r--   0 root         (0) root         (0)     2308 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/serial.pyi
--rw-rw-r--   0 root         (0) root         (0)      866 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/sfc.pyi
--rw-rw-r--   0 root         (0) root         (0)     4729 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/tag.pyi
--rw-rw-r--   0 root         (0) root         (0)      456 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/twilio.pyi
--rw-rw-r--   0 root         (0) root         (0)     2346 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/user.pyi
--rw-rw-r--   0 root         (0) root         (0)     4751 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/util.pyi
--rw-rw-r--   0 root         (0) root         (0)      194 2024-04-12 21:06:46.000000 ignition_api_stubs-8.1.39/stubs/system/vision.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.545440 ignition_api_stubs-8.1.39.post1/
+-rw-rw-r--   0 root         (0) root         (0)     5004 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/CHANGELOG.md
+-rw-rw-r--   0 root         (0) root         (0)     1070 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       21 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4751 2024-04-30 18:35:45.545440 ignition_api_stubs-8.1.39.post1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2042 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/README.md
+-rw-rw-r--   0 root         (0) root         (0)     1590 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 18:35:45.545440 ignition_api_stubs-8.1.39.post1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.497439 ignition_api_stubs-8.1.39.post1/stubs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.497439 ignition_api_stubs-8.1.39.post1/stubs/ch/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/ch/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/ch/qos/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/ch/qos/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/ch/qos/logback/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/ch/qos/logback/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/ch/qos/logback/classic/
+-rw-rw-r--   0 root         (0) root         (0)      646 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/ch/qos/logback/classic/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/codahale/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/codahale/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/codahale/metrics/
+-rw-rw-r--   0 root         (0) root         (0)     1271 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/codahale/metrics/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/google/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/google/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/google/common/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/google/common/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/google/common/collect/
+-rw-rw-r--   0 root         (0) root         (0)     2204 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/google/common/collect/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/google/common/eventbus/
+-rw-rw-r--   0 root         (0) root         (0)      355 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/google/common/eventbus/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/
+-rw-rw-r--   0 root         (0) root         (0)     1776 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/binding/
+-rw-rw-r--   0 root         (0) root         (0)      875 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/binding/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/components/
+-rw-rw-r--   0 root         (0) root         (0)      281 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/components/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/model/
+-rw-rw-r--   0 root         (0) root         (0)      193 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/model/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/script/
+-rw-rw-r--   0 root         (0) root         (0)      256 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/script/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.501439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/script/builtin/
+-rw-rw-r--   0 root         (0) root         (0)     7672 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/script/builtin/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/sqltags/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/sqltags/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/sqltags/project/
+-rw-rw-r--   0 root         (0) root         (0)      136 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/sqltags/project/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/alarming/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/alarming/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/alarming/common/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/alarming/common/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/alarming/common/rosters/
+-rw-rw-r--   0 root         (0) root         (0)      610 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/alarming/common/rosters/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/launch/
+-rw-rw-r--   0 root         (0) root         (0)     6078 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/launch/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/model/
+-rw-rw-r--   0 root         (0) root         (0)     4071 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/model/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/util/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/util/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/util/gui/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/util/gui/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/util/gui/progress/
+-rw-rw-r--   0 root         (0) root         (0)     1598 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/util/gui/progress/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/util/gui/scheduling/
+-rw-rw-r--   0 root         (0) root         (0)     1398 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/util/gui/scheduling/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/
+-rw-rw-r--   0 root         (0) root         (0)    10147 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/alarming/
+-rw-rw-r--   0 root         (0) root         (0)     3224 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/alarming/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/alarming/evaluation/
+-rw-rw-r--   0 root         (0) root         (0)     1224 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/alarming/evaluation/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/alarming/query/
+-rw-rw-r--   0 root         (0) root         (0)      814 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/alarming/query/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/binding/
+-rw-rw-r--   0 root         (0) root         (0)       78 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/binding/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.505439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/browsing/
+-rw-rw-r--   0 root         (0) root         (0)     3586 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/browsing/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/config/
+-rw-rw-r--   0 root         (0) root         (0)     3184 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/config/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/db/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/db/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/db/namedquery/
+-rw-rw-r--   0 root         (0) root         (0)      773 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/db/namedquery/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/document/
+-rw-rw-r--   0 root         (0) root         (0)      215 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/document/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/execution/
+-rw-rw-r--   0 root         (0) root         (0)     1165 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/execution/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/expressions/
+-rw-rw-r--   0 root         (0) root         (0)     1020 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/expressions/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/expressions/functions/
+-rw-rw-r--   0 root         (0) root         (0)      672 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/expressions/functions/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/functional/
+-rw-rw-r--   0 root         (0) root         (0)       54 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/functional/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/gson/
+-rw-rw-r--   0 root         (0) root         (0)     8729 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/gson/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/gson/reflect/
+-rw-rw-r--   0 root         (0) root         (0)      284 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/gson/reflect/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/gson/stream/
+-rw-rw-r--   0 root         (0) root         (0)     2052 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/gson/stream/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/gui/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/gui/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/gui/progress/
+-rw-rw-r--   0 root         (0) root         (0)     1370 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/gui/progress/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/i18n/
+-rw-rw-r--   0 root         (0) root         (0)      921 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/i18n/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/i18n/keyboard/
+-rw-rw-r--   0 root         (0) root         (0)      862 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/i18n/keyboard/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/i18n/translation/
+-rw-rw-r--   0 root         (0) root         (0)      238 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/i18n/translation/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/jsonschema/
+-rw-rw-r--   0 root         (0) root         (0)     4053 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/jsonschema/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/licensing/
+-rw-rw-r--   0 root         (0) root         (0)     1351 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/licensing/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.509439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/logging/
+-rw-rw-r--   0 root         (0) root         (0)      883 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/logging/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/messages/
+-rw-rw-r--   0 root         (0) root         (0)     1262 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/messages/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/model/
+-rw-rw-r--   0 root         (0) root         (0)     3271 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/model/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/model/values/
+-rw-rw-r--   0 root         (0) root         (0)     4717 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/model/values/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/modules/
+-rw-rw-r--   0 root         (0) root         (0)     4705 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/modules/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/opc/
+-rw-rw-r--   0 root         (0) root         (0)     3830 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/opc/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/project/
+-rw-rw-r--   0 root         (0) root         (0)     3511 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/project/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/project/resource/
+-rw-rw-r--   0 root         (0) root         (0)     5710 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/project/resource/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/
+-rw-rw-r--   0 root         (0) root         (0)     2536 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/abc/
+-rw-rw-r--   0 root         (0) root         (0)     4500 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/abc/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/adapters/
+-rw-rw-r--   0 root         (0) root         (0)     1293 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/adapters/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/builtin/
+-rw-rw-r--   0 root         (0) root         (0)     8418 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/builtin/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/builtin/http/
+-rw-rw-r--   0 root         (0) root         (0)     2698 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/builtin/http/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/builtin/ialabs/
+-rw-rw-r--   0 root         (0) root         (0)     1798 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/builtin/ialabs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/hints/
+-rw-rw-r--   0 root         (0) root         (0)      370 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/hints/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/message/
+-rw-rw-r--   0 root         (0) root         (0)      594 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/message/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/sqltags/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/sqltags/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/sqltags/history/
+-rw-rw-r--   0 root         (0) root         (0)      414 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/sqltags/history/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.513439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/sqltags/history/annotations/
+-rw-rw-r--   0 root         (0) root         (0)     1927 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/sqltags/history/annotations/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/sqltags/model/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/sqltags/model/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/sqltags/model/types/
+-rw-rw-r--   0 root         (0) root         (0)     1946 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/sqltags/model/types/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/config/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/config/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/config/types/
+-rw-rw-r--   0 root         (0) root         (0)      307 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/config/types/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/model/
+-rw-rw-r--   0 root         (0) root         (0)     2029 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/model/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/paths/
+-rw-rw-r--   0 root         (0) root         (0)     1501 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/paths/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/paths/parser/
+-rw-rw-r--   0 root         (0) root         (0)      795 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/paths/parser/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/tagpaths/
+-rw-rw-r--   0 root         (0) root         (0)      248 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/tagpaths/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/user/
+-rw-rw-r--   0 root         (0) root         (0)     4586 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/user/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/user/schedule/
+-rw-rw-r--   0 root         (0) root         (0)     4953 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/user/schedule/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/util/
+-rw-rw-r--   0 root         (0) root         (0)     6003 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/util/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/xmlserialization/
+-rw-rw-r--   0 root         (0) root         (0)      590 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/xmlserialization/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/xmlserialization/deserialization/
+-rw-rw-r--   0 root         (0) root         (0)     2814 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/xmlserialization/deserialization/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/xmlserialization/encoding/
+-rw-rw-r--   0 root         (0) root         (0)       63 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/xmlserialization/encoding/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/
+-rw-rw-r--   0 root         (0) root         (0)     2234 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/equalitydelegates/
+-rw-rw-r--   0 root         (0) root         (0)      139 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/equalitydelegates/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/gateway/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/gateway/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.517439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/gateway/project/
+-rw-rw-r--   0 root         (0) root         (0)     1155 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/gateway/project/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/modules/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/modules/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/modules/serial/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/modules/serial/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/modules/serial/scripting/
+-rw-rw-r--   0 root         (0) root         (0)     2334 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/modules/serial/scripting/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/opccom/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/opccom/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/opccom/hda/
+-rw-rw-r--   0 root         (0) root         (0)     1163 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/opccom/hda/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/perspective/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/perspective/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/perspective/common/
+-rw-rw-r--   0 root         (0) root         (0)      911 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/perspective/common/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/sfc/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/sfc/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/sfc/api/
+-rw-rw-r--   0 root         (0) root         (0)      104 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/sfc/api/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/vision/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/vision/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/vision/api/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/vision/api/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/vision/api/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/vision/api/client/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/vision/api/client/components/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/vision/api/client/components/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/vision/api/client/components/model/
+-rw-rw-r--   0 root         (0) root         (0)      277 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/vision/api/client/components/model/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/palantir/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/palantir/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/palantir/ptoss/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/palantir/ptoss/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/palantir/ptoss/cinch/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/palantir/ptoss/cinch/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/com/palantir/ptoss/cinch/core/
+-rw-rw-r--   0 root         (0) root         (0)      413 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/palantir/ptoss/cinch/core/__init__.pyi
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/com/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.521439 ignition_api_stubs-8.1.39.post1/stubs/dev/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/dev/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.525439 ignition_api_stubs-8.1.39.post1/stubs/dev/coatl/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/dev/coatl/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.525439 ignition_api_stubs-8.1.39.post1/stubs/dev/coatl/helper/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/dev/coatl/helper/__init__.pyi
+-rw-rw-r--   0 root         (0) root         (0)       88 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/dev/coatl/helper/types.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.525439 ignition_api_stubs-8.1.39.post1/stubs/dev/coatl/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/dev/coatl/utils/__init__.pyi
+-rw-rw-r--   0 root         (0) root         (0)       70 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/dev/coatl/utils/decorators.pyi
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/dev/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.545440 ignition_api_stubs-8.1.39.post1/stubs/ignition_api_stubs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4751 2024-04-30 18:35:45.000000 ignition_api_stubs-8.1.39.post1/stubs/ignition_api_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11006 2024-04-30 18:35:45.000000 ignition_api_stubs-8.1.39.post1/stubs/ignition_api_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 18:35:45.000000 ignition_api_stubs-8.1.39.post1/stubs/ignition_api_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-30 18:35:45.000000 ignition_api_stubs-8.1.39.post1/stubs/ignition_api_stubs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-30 18:35:45.000000 ignition_api_stubs-8.1.39.post1/stubs/ignition_api_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.525439 ignition_api_stubs-8.1.39.post1/stubs/java/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.525439 ignition_api_stubs-8.1.39.post1/stubs/java/awt/
+-rw-rw-r--   0 root         (0) root         (0)     3143 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/awt/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.525439 ignition_api_stubs-8.1.39.post1/stubs/java/awt/event/
+-rw-rw-r--   0 root         (0) root         (0)     2579 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/awt/event/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.525439 ignition_api_stubs-8.1.39.post1/stubs/java/awt/geom/
+-rw-rw-r--   0 root         (0) root         (0)     1312 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/awt/geom/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.525439 ignition_api_stubs-8.1.39.post1/stubs/java/awt/image/
+-rw-rw-r--   0 root         (0) root         (0)      128 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/awt/image/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.525439 ignition_api_stubs-8.1.39.post1/stubs/java/awt/print/
+-rw-rw-r--   0 root         (0) root         (0)     1107 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/awt/print/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.525439 ignition_api_stubs-8.1.39.post1/stubs/java/beans/
+-rw-rw-r--   0 root         (0) root         (0)      564 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/beans/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.525439 ignition_api_stubs-8.1.39.post1/stubs/java/io/
+-rw-rw-r--   0 root         (0) root         (0)     4595 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/io/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.525439 ignition_api_stubs-8.1.39.post1/stubs/java/lang/
+-rw-rw-r--   0 root         (0) root         (0)     9829 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/lang/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/lang/reflect/
+-rw-rw-r--   0 root         (0) root         (0)       96 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/lang/reflect/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/math/
+-rw-rw-r--   0 root         (0) root         (0)     1128 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/math/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/net/
+-rw-rw-r--   0 root         (0) root         (0)     6190 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/net/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/net/http/
+-rw-rw-r--   0 root         (0) root         (0)       84 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/net/http/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/nio/
+-rw-rw-r--   0 root         (0) root         (0)     7653 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/nio/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/nio/channels/
+-rw-rw-r--   0 root         (0) root         (0)     4672 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/nio/channels/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/nio/charset/
+-rw-rw-r--   0 root         (0) root         (0)     2022 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/nio/charset/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/nio/file/
+-rw-rw-r--   0 root         (0) root         (0)     7939 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/nio/file/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/nio/file/attribute/
+-rw-rw-r--   0 root         (0) root         (0)     1809 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/nio/file/attribute/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/org/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/org/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/org/jdesktop/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/org/jdesktop/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/org/jdesktop/core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/org/jdesktop/core/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/org/jdesktop/core/animation/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/org/jdesktop/core/animation/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/org/jdesktop/core/animation/timing/
+-rw-rw-r--   0 root         (0) root         (0)      155 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/org/jdesktop/core/animation/timing/__init__.pyi
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/security/
+-rw-rw-r--   0 root         (0) root         (0)      343 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/security/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/text/
+-rw-rw-r--   0 root         (0) root         (0)     8251 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/text/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/time/
+-rw-rw-r--   0 root         (0) root         (0)     2428 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/time/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/time/format/
+-rw-rw-r--   0 root         (0) root         (0)      221 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/time/format/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/time/temporal/
+-rw-rw-r--   0 root         (0) root         (0)     3688 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/time/temporal/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.529439 ignition_api_stubs-8.1.39.post1/stubs/java/util/
+-rw-rw-r--   0 root         (0) root         (0)    16549 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/util/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/java/util/concurrent/
+-rw-rw-r--   0 root         (0) root         (0)     1919 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/util/concurrent/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/java/util/function/
+-rw-rw-r--   0 root         (0) root         (0)     1427 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/util/function/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/java/util/regex/
+-rw-rw-r--   0 root         (0) root         (0)     2813 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/util/regex/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/java/util/stream/
+-rw-rw-r--   0 root         (0) root         (0)     1594 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/java/util/stream/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/javax/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/javax/__init__.pyi
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/javax/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/javax/security/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/javax/security/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/javax/security/auth/
+-rw-rw-r--   0 root         (0) root         (0)      125 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/javax/security/auth/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/javax/swing/
+-rw-rw-r--   0 root         (0) root         (0)     6503 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/javax/swing/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/javax/swing/event/
+-rw-rw-r--   0 root         (0) root         (0)      639 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/javax/swing/event/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/javax/swing/plaf/
+-rw-rw-r--   0 root         (0) root         (0)      392 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/javax/swing/plaf/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/javax/swing/text/
+-rw-rw-r--   0 root         (0) root         (0)      202 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/javax/swing/text/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/org/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/org/apache/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/apache/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/lang3/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/lang3/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/lang3/builder/
+-rw-rw-r--   0 root         (0) root         (0)      780 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/lang3/builder/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/math3/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/math3/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/math3/exception/
+-rw-rw-r--   0 root         (0) root         (0)      587 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/math3/exception/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.533439 ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/math3/exception/util/
+-rw-rw-r--   0 root         (0) root         (0)      678 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/math3/exception/util/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.537439 ignition_api_stubs-8.1.39.post1/stubs/org/apache/log4j/
+-rw-rw-r--   0 root         (0) root         (0)     2413 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/apache/log4j/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.537439 ignition_api_stubs-8.1.39.post1/stubs/org/apache/log4j/spi/
+-rw-rw-r--   0 root         (0) root         (0)     2010 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/apache/log4j/spi/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.537439 ignition_api_stubs-8.1.39.post1/stubs/org/bson/
+-rw-rw-r--   0 root         (0) root         (0)     1997 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/bson/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.537439 ignition_api_stubs-8.1.39.post1/stubs/org/bson/codecs/
+-rw-rw-r--   0 root         (0) root         (0)       17 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/bson/codecs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.537439 ignition_api_stubs-8.1.39.post1/stubs/org/bson/codecs/configuration/
+-rw-rw-r--   0 root         (0) root         (0)      130 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/bson/codecs/configuration/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.537439 ignition_api_stubs-8.1.39.post1/stubs/org/bson/types/
+-rw-rw-r--   0 root         (0) root         (0)     2627 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/bson/types/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.537439 ignition_api_stubs-8.1.39.post1/stubs/org/json/
+-rw-rw-r--   0 root         (0) root         (0)     4114 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/json/__init__.pyi
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.537439 ignition_api_stubs-8.1.39.post1/stubs/org/python/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/python/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.537439 ignition_api_stubs-8.1.39.post1/stubs/org/python/core/
+-rw-rw-r--   0 root         (0) root         (0)    23034 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/python/core/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.537439 ignition_api_stubs-8.1.39.post1/stubs/org/python/expose/
+-rw-rw-r--   0 root         (0) root         (0)      350 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/python/expose/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.537439 ignition_api_stubs-8.1.39.post1/stubs/org/slf4j/
+-rw-rw-r--   0 root         (0) root         (0)     1122 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/slf4j/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.537439 ignition_api_stubs-8.1.39.post1/stubs/org/slf4j/event/
+-rw-rw-r--   0 root         (0) root         (0)      167 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/org/slf4j/event/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.545440 ignition_api_stubs-8.1.39.post1/stubs/system/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/__init__.pyi
+-rw-rw-r--   0 root         (0) root         (0)       15 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/__version__.pyi
+-rw-rw-r--   0 root         (0) root         (0)     2133 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/alarm.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.545440 ignition_api_stubs-8.1.39.post1/stubs/system/bacnet/
+-rw-rw-r--   0 root         (0) root         (0)     1305 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/bacnet/__init__.pyi
+-rw-rw-r--   0 root         (0) root         (0)    12890 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/bacnet/enumerated.pyi
+-rw-rw-r--   0 root         (0) root         (0)      780 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/bacnet/enums.pyi
+-rw-rw-r--   0 root         (0) root         (0)     2380 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/dataset.pyi
+-rw-rw-r--   0 root         (0) root         (0)     2292 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/date.pyi
+-rw-rw-r--   0 root         (0) root         (0)     3586 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/db.pyi
+-rw-rw-r--   0 root         (0) root         (0)      687 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/device.pyi
+-rw-rw-r--   0 root         (0) root         (0)     1275 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/dnp3.pyi
+-rw-rw-r--   0 root         (0) root         (0)      718 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/eam.pyi
+-rw-rw-r--   0 root         (0) root         (0)      810 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/file.pyi
+-rw-rw-r--   0 root         (0) root         (0)      220 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/groups.pyi
+-rw-rw-r--   0 root         (0) root         (0)     3216 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/gui.pyi
+-rw-rw-r--   0 root         (0) root         (0)      726 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/iec61850.pyi
+-rw-rw-r--   0 root         (0) root         (0)     1090 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/math.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.545440 ignition_api_stubs-8.1.39.post1/stubs/system/mongodb/
+-rw-rw-r--   0 root         (0) root         (0)     2252 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/mongodb/__init__.pyi
+-rw-rw-r--   0 root         (0) root         (0)      495 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/mongodb/types.pyi
+-rw-rw-r--   0 root         (0) root         (0)     1095 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/nav.pyi
+-rw-rw-r--   0 root         (0) root         (0)     2245 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/net.pyi
+-rw-rw-r--   0 root         (0) root         (0)     1500 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/opc.pyi
+-rw-rw-r--   0 root         (0) root         (0)     1539 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/opchda.pyi
+-rw-rw-r--   0 root         (0) root         (0)      478 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/opcua.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:35:45.545440 ignition_api_stubs-8.1.39.post1/stubs/system/perspective/
+-rw-rw-r--   0 root         (0) root         (0)     3884 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/perspective/__init__.pyi
+-rw-rw-r--   0 root         (0) root         (0)       81 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/perspective/workstation.pyi
+-rw-rw-r--   0 root         (0) root         (0)      592 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/print.pyi
+-rw-rw-r--   0 root         (0) root         (0)      196 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/project.pyi
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/py.typed
+-rw-rw-r--   0 root         (0) root         (0)      737 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/report.pyi
+-rw-rw-r--   0 root         (0) root         (0)      633 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/roster.pyi
+-rw-rw-r--   0 root         (0) root         (0)     1276 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/secsgem.pyi
+-rw-rw-r--   0 root         (0) root         (0)      704 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/security.pyi
+-rw-rw-r--   0 root         (0) root         (0)     2308 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/serial.pyi
+-rw-rw-r--   0 root         (0) root         (0)      866 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/sfc.pyi
+-rw-rw-r--   0 root         (0) root         (0)     4729 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/tag.pyi
+-rw-rw-r--   0 root         (0) root         (0)      456 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/twilio.pyi
+-rw-rw-r--   0 root         (0) root         (0)     2346 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/user.pyi
+-rw-rw-r--   0 root         (0) root         (0)     4751 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/util.pyi
+-rw-rw-r--   0 root         (0) root         (0)      194 2024-04-30 18:33:44.000000 ignition_api_stubs-8.1.39.post1/stubs/system/vision.pyi
```

### Comparing `ignition_api_stubs-8.1.39/CHANGELOG.md` & `ignition_api_stubs-8.1.39.post1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v8.1.39.post1 (2024-04-30)
+
+### Feat
+
+- **java**: add all Calendar methods (#171)
+
 ## v8.1.39 (2024-04-12)
 
 ## v8.1.38 (2024-03-06)
 
 ## v8.1.37.post1 (2024-02-21)
 
 ## v8.1.37.post1 (2024-02-21)
```

### Comparing `ignition_api_stubs-8.1.39/LICENSE` & `ignition_api_stubs-8.1.39.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/PKG-INFO` & `ignition_api_stubs-8.1.39.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignition-api-stubs
-Version: 8.1.39
+Version: 8.1.39.post1
 Summary: Ignition Scripting API Stubs
 Author-email: César Román <cesar@coatl.dev>
 License: MIT License
         
         Copyright (c) 2022 César Román
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ignition_api_stubs-8.1.39/README.md` & `ignition_api_stubs-8.1.39.post1/README.md`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/pyproject.toml` & `ignition_api_stubs-8.1.39.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools>=61.2",
 ]
 
 [project]
 name = "ignition-api-stubs"
-version = "8.1.39"
+version = "8.1.39.post1"
 description = "Ignition Scripting API Stubs"
 readme = "README.md"
 keywords = [
   "hmi",
   "ignition",
   "inductive automation",
   "scada",
```

### Comparing `ignition_api_stubs-8.1.39/stubs/ch/qos/logback/classic/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/ch/qos/logback/classic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/codahale/metrics/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/codahale/metrics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/google/common/collect/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/google/common/collect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/binding/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/binding/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/factorypmi/application/script/builtin/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/factorypmi/application/script/builtin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/alarming/common/rosters/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/alarming/common/rosters/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/launch/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/launch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/model/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/model/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/util/gui/progress/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/util/gui/progress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/client/util/gui/scheduling/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/client/util/gui/scheduling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/alarming/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/alarming/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/alarming/evaluation/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/alarming/evaluation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/alarming/query/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/alarming/query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/browsing/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/browsing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/config/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/db/namedquery/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/db/namedquery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/execution/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/execution/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/expressions/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/expressions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/expressions/functions/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/expressions/functions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/gson/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/gson/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/gson/stream/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/gson/stream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/gui/progress/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/gui/progress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/i18n/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/i18n/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/i18n/keyboard/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/i18n/keyboard/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/jsonschema/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/jsonschema/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/licensing/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/licensing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/logging/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/logging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/messages/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/messages/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/model/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/model/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/model/values/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/model/values/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/modules/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/modules/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/opc/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/opc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/project/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/project/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/project/resource/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/project/resource/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/abc/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/abc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/adapters/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/adapters/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/builtin/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/builtin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/builtin/http/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/builtin/http/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/builtin/ialabs/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/builtin/ialabs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/script/message/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/script/message/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/sqltags/history/annotations/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/sqltags/history/annotations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/sqltags/model/types/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/sqltags/model/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/model/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/model/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/paths/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/paths/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/tags/paths/parser/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/tags/paths/parser/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/user/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/user/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/user/schedule/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/user/schedule/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/util/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/util/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/xmlserialization/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/xmlserialization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/xmlserialization/deserialization/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/xmlserialization/deserialization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/gateway/project/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/gateway/project/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/ignition/modules/serial/scripting/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/ignition/modules/serial/scripting/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/opccom/hda/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/opccom/hda/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/com/inductiveautomation/perspective/common/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/com/inductiveautomation/perspective/common/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/ignition_api_stubs.egg-info/PKG-INFO` & `ignition_api_stubs-8.1.39.post1/stubs/ignition_api_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignition-api-stubs
-Version: 8.1.39
+Version: 8.1.39.post1
 Summary: Ignition Scripting API Stubs
 Author-email: César Román <cesar@coatl.dev>
 License: MIT License
         
         Copyright (c) 2022 César Román
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ignition_api_stubs-8.1.39/stubs/ignition_api_stubs.egg-info/SOURCES.txt` & `ignition_api_stubs-8.1.39.post1/stubs/ignition_api_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/awt/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/awt/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/awt/event/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/awt/event/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/awt/geom/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/awt/geom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/awt/print/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/awt/print/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/beans/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/beans/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/io/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/lang/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/lang/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/math/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/net/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/net/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/nio/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/nio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/nio/channels/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/nio/channels/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/nio/charset/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/nio/charset/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/nio/file/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/nio/file/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/nio/file/attribute/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/nio/file/attribute/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/text/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/text/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/time/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/time/temporal/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/time/temporal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/util/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/util/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,22 @@
     def getCalendarType(self) -> AnyStr: ...
     def getDisplayName(self, field: int, style: int, locale: Locale) -> AnyStr: ...
     def getDisplayNames(
         self, field: int, style: int, locale: Locale
     ) -> Dict[AnyStr, int]: ...
     def getFirstDayOfWeek(self) -> int: ...
     def getGreatestMinimum(self, field: int) -> int: ...
-    def getInstance(self, *args: Any) -> Calendar: ...
+    @staticmethod
+    def getInstance(*args: Any) -> Calendar: ...
+    def getLeastMaximum(self, field: int) -> int: ...
+    def getMaximum(self, field: int) -> int: ...
+    def getMinimalDaysInFirstWeek(self) -> int: ...
+    def getMinimum(self, field: int) -> int: ...
+    def getTime(self) -> Date: ...
+    def getTimeInMillis(self) -> long: ...
     def getTimeZone(self) -> TimeZone: ...
     def getWeeksInWeekYear(self) -> int: ...
     def getWeekYear(self) -> int: ...
     def isLenient(self) -> bool: ...
     def isSet(self, field: int) -> bool: ...
     def isWeekDateSUpported(self) -> bool: ...
     def roll(self, field: int, amount: int) -> None: ...
```

### Comparing `ignition_api_stubs-8.1.39/stubs/java/util/concurrent/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/util/concurrent/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/util/function/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/util/function/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/util/regex/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/util/regex/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/java/util/stream/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/java/util/stream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/javax/swing/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/javax/swing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/javax/swing/event/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/javax/swing/event/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/org/apache/commons/lang3/builder/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/lang3/builder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/org/apache/commons/math3/exception/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/math3/exception/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/org/apache/commons/math3/exception/util/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/org/apache/commons/math3/exception/util/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/org/apache/log4j/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/org/apache/log4j/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/org/apache/log4j/spi/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/org/apache/log4j/spi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/org/bson/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/org/bson/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/org/bson/types/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/org/bson/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/org/json/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/org/json/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/org/python/core/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/org/python/core/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/org/slf4j/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/org/slf4j/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/alarm.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/alarm.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/bacnet/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/bacnet/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/bacnet/enumerated.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/bacnet/enumerated.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/bacnet/enums.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/bacnet/enums.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/dataset.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/dataset.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/date.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/date.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/db.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/db.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/device.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/device.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/dnp3.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/dnp3.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/eam.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/eam.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/file.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/file.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/gui.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/gui.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/iec61850.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/iec61850.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/math.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/math.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/mongodb/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/mongodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/nav.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/nav.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/net.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/net.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/opc.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/opc.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/opchda.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/opchda.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/perspective/__init__.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/perspective/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/print.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/print.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/report.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/report.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/roster.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/roster.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/secsgem.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/secsgem.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/security.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/security.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/serial.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/serial.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/sfc.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/sfc.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/tag.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/tag.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/user.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/user.pyi`

 * *Files identical despite different names*

### Comparing `ignition_api_stubs-8.1.39/stubs/system/util.pyi` & `ignition_api_stubs-8.1.39.post1/stubs/system/util.pyi`

 * *Files identical despite different names*

