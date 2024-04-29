# Comparing `tmp/pringles-devs-1.0.3.tar.gz` & `tmp/pringles_devs-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pringles-devs-1.0.3.tar", last modified: Mon Oct  7 21:32:40 2019, max compression
+gzip compressed data, was "pringles_devs-2.0.1.tar", last modified: Mon Apr 29 22:12:02 2024, max compression
```

## Comparing `pringles-devs-1.0.3.tar` & `pringles_devs-2.0.1.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/
--rw-r--r--   0 jlanuza   (1000) docker     (999)      128 2019-10-07 21:32:16.000000 pringles-devs-1.0.3/MANIFEST.in
--rw-r--r--   0 jlanuza   (1000) docker     (999)     2213 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/PKG-INFO
--rw-r--r--   0 jlanuza   (1000) docker     (999)     1539 2019-10-03 18:51:32.000000 pringles-devs-1.0.3/README.md
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/
--rw-r--r--   0 jlanuza   (1000) docker     (999)       18 2019-08-21 05:42:37.000000 pringles-devs-1.0.3/pringles/__init__.py
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/backends/
--rw-r--r--   0 jlanuza   (1000) docker     (999)       62 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/pringles/backends/__init__.py
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/backends/statics/
--rw-r--r--   0 jlanuza   (1000) docker     (999)     2335 2019-09-15 05:29:53.000000 pringles-devs-1.0.3/pringles/backends/statics/basic.html
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/backends/statics/css/
--rw-r--r--   0 jlanuza   (1000) docker     (999)      324 2019-09-15 05:29:53.000000 pringles-devs-1.0.3/pringles/backends/statics/css/style.css
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/backends/statics/js/
--rw-r--r--   0 jlanuza   (1000) docker     (999)     5752 2019-09-15 05:29:53.000000 pringles-devs-1.0.3/pringles/backends/statics/js/Canvas.js
--rw-r--r--   0 jlanuza   (1000) docker     (999)     2027 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/pringles/backends/statics/js/ColorCodes.js
--rw-r--r--   0 jlanuza   (1000) docker     (999)     9682 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/pringles/backends/statics/js/JSONModelGraphics.js
--rw-r--r--   0 jlanuza   (1000) docker     (999)     9704 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/pringles/backends/statics/js/Link.js
--rw-r--r--   0 jlanuza   (1000) docker     (999)    23683 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/pringles/backends/statics/js/Model.js
--rw-r--r--   0 jlanuza   (1000) docker     (999)     4914 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/pringles/backends/statics/js/Port.js
--rw-r--r--   0 jlanuza   (1000) docker     (999)     2928 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/pringles/backends/statics/js/Square.js
--rw-r--r--   0 jlanuza   (1000) docker     (999)     9768 2019-09-15 05:29:53.000000 pringles-devs-1.0.3/pringles/backends/statics/js/main.js
--rw-r--r--   0 jlanuza   (1000) docker     (999)     2053 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/pringles/backends/statics/js/manifest.js
--rw-r--r--   0 jlanuza   (1000) docker     (999)     4441 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/pringles/backends/statics/js/toposort.js
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/backends/statics/vendors/
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/backends/statics/vendors/js/
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/backends/statics/vendors/js/createjs/
--rw-r--r--   0 jlanuza   (1000) docker     (999)   152280 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/pringles/backends/statics/vendors/js/createjs/createjs-2013.12.12.min.js
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/backends/statics/vendors/js/jquery-3.2.1/
--rw-r--r--   0 jlanuza   (1000) docker     (999)    86659 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/pringles/backends/statics/vendors/js/jquery-3.2.1/jquery-3.2.1.min.js
--rw-r--r--   0 jlanuza   (1000) docker     (999)     3054 2019-09-15 05:29:53.000000 pringles-devs-1.0.3/pringles/backends/web_display.py
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/models/
--rw-r--r--   0 jlanuza   (1000) docker     (999)      129 2019-10-07 18:30:29.000000 pringles-devs-1.0.3/pringles/models/__init__.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)      219 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/pringles/models/errors.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     6640 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/pringles/models/models.py
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/serializers/
--rw-r--r--   0 jlanuza   (1000) docker     (999)      130 2019-08-21 05:42:37.000000 pringles-devs-1.0.3/pringles/serializers/__init__.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     2584 2019-08-21 05:42:37.000000 pringles-devs-1.0.3/pringles/serializers/json.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     1426 2019-08-21 05:42:37.000000 pringles-devs-1.0.3/pringles/serializers/ma.py
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/simulator/
--rw-r--r--   0 jlanuza   (1000) docker     (999)      168 2019-09-16 19:00:07.000000 pringles-devs-1.0.3/pringles/simulator/__init__.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)      327 2019-09-16 19:00:07.000000 pringles-devs-1.0.3/pringles/simulator/errors.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)      714 2019-09-16 19:00:07.000000 pringles-devs-1.0.3/pringles/simulator/events.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     4033 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/pringles/simulator/registry.py
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/simulator/registry_bootstrap/
--rw-r--r--   0 jlanuza   (1000) docker     (999)       72 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/pringles/simulator/registry_bootstrap/cpu.pringles
--rw-r--r--   0 jlanuza   (1000) docker     (999)       80 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/pringles/simulator/registry_bootstrap/generator.pringles
--rw-r--r--   0 jlanuza   (1000) docker     (999)       73 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/pringles/simulator/registry_bootstrap/qss1.pringles
--rw-r--r--   0 jlanuza   (1000) docker     (999)       73 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/pringles/simulator/registry_bootstrap/qss2.pringles
--rw-r--r--   0 jlanuza   (1000) docker     (999)       73 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/pringles/simulator/registry_bootstrap/qss3.pringles
--rw-r--r--   0 jlanuza   (1000) docker     (999)       80 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/pringles/simulator/registry_bootstrap/queue.pringles
--rw-r--r--   0 jlanuza   (1000) docker     (999)      109 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/pringles/simulator/registry_bootstrap/transducer.pringles
--rw-r--r--   0 jlanuza   (1000) docker     (999)     9588 2019-10-07 18:04:02.000000 pringles-devs-1.0.3/pringles/simulator/simulation.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     4194 2019-09-16 19:59:11.000000 pringles-devs-1.0.3/pringles/simulator/simulator.py
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles/utils/
--rw-r--r--   0 jlanuza   (1000) docker     (999)      254 2019-09-16 19:00:07.000000 pringles-devs-1.0.3/pringles/utils/__init__.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     4980 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/pringles/utils/discovery.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)      169 2019-09-16 19:00:07.000000 pringles-devs-1.0.3/pringles/utils/errors.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     1218 2019-09-16 19:00:07.000000 pringles-devs-1.0.3/pringles/utils/plotting.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     3665 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/pringles/utils/vtime.py
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles_devs.egg-info/
--rw-r--r--   0 jlanuza   (1000) docker     (999)     2213 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles_devs.egg-info/PKG-INFO
--rw-r--r--   0 jlanuza   (1000) docker     (999)     2100 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles_devs.egg-info/SOURCES.txt
--rw-r--r--   0 jlanuza   (1000) docker     (999)        1 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles_devs.egg-info/dependency_links.txt
--rw-r--r--   0 jlanuza   (1000) docker     (999)       78 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles_devs.egg-info/requires.txt
--rw-r--r--   0 jlanuza   (1000) docker     (999)       15 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/pringles_devs.egg-info/top_level.txt
--rw-r--r--   0 jlanuza   (1000) docker     (999)       77 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/requirements.txt
--rw-r--r--   0 jlanuza   (1000) docker     (999)      440 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/setup.cfg
--rw-r--r--   0 jlanuza   (1000) docker     (999)      829 2019-10-07 21:32:32.000000 pringles-devs-1.0.3/setup.py
-drwxr-xr-x   0 jlanuza   (1000) docker     (999)        0 2019-10-07 21:32:40.000000 pringles-devs-1.0.3/tests/
--rw-r--r--   0 jlanuza   (1000) docker     (999)        0 2019-08-21 05:42:37.000000 pringles-devs-1.0.3/tests/__init__.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     1403 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/tests/conftest.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     1936 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/tests/test_atomic_metadata_extractor.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)      650 2019-09-16 19:00:07.000000 pringles-devs-1.0.3/tests/test_events.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     2036 2019-09-15 05:29:53.000000 pringles-devs-1.0.3/tests/test_model_ipython_display.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     1549 2019-09-16 19:00:07.000000 pringles-devs-1.0.3/tests/test_model_metadata_and_instanciation_integration.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     2501 2019-10-07 18:30:29.000000 pringles-devs-1.0.3/tests/test_model_translation.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     3560 2019-09-16 19:00:07.000000 pringles-devs-1.0.3/tests/test_simulation.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     3836 2019-10-07 21:20:44.000000 pringles-devs-1.0.3/tests/test_simulator.py
--rw-r--r--   0 jlanuza   (1000) docker     (999)     2263 2019-09-09 18:29:41.000000 pringles-devs-1.0.3/tests/test_utils.py
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.941211 pringles_devs-2.0.1/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)    35148 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/LICENSE
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      128 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/MANIFEST.in
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     2123 2024-04-29 22:12:02.941003 pringles_devs-2.0.1/PKG-INFO
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     1539 2024-03-29 21:44:44.000000 pringles_devs-2.0.1/README.md
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.872051 pringles_devs-2.0.1/pringles/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)       18 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/__init__.py
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.874006 pringles_devs-2.0.1/pringles/backends/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)       62 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/__init__.py
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.874958 pringles_devs-2.0.1/pringles/backends/statics/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     2335 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/basic.html
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.876014 pringles_devs-2.0.1/pringles/backends/statics/css/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      324 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/css/style.css
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.889173 pringles_devs-2.0.1/pringles/backends/statics/js/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     5752 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/js/Canvas.js
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     2027 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/js/ColorCodes.js
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     9682 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/js/JSONModelGraphics.js
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     9704 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/js/Link.js
+-rw-r--r--   0 pedrotambo   (502) staff       (20)    23683 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/js/Model.js
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     4914 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/js/Port.js
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     2928 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/js/Square.js
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     9768 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/js/main.js
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     2053 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/js/manifest.js
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     4441 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/js/toposort.js
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.865698 pringles_devs-2.0.1/pringles/backends/statics/vendors/
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.866229 pringles_devs-2.0.1/pringles/backends/statics/vendors/js/
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.890282 pringles_devs-2.0.1/pringles/backends/statics/vendors/js/createjs/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)   152280 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/vendors/js/createjs/createjs-2013.12.12.min.js
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.894203 pringles_devs-2.0.1/pringles/backends/statics/vendors/js/jquery-3.2.1/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)    86659 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/backends/statics/vendors/js/jquery-3.2.1/jquery-3.2.1.min.js
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     3064 2024-03-30 00:02:41.000000 pringles_devs-2.0.1/pringles/backends/web_display.py
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.898447 pringles_devs-2.0.1/pringles/models/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      129 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/models/__init__.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      219 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/models/errors.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     6640 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/models/models.py
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.901285 pringles_devs-2.0.1/pringles/serializers/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      130 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/serializers/__init__.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     2584 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/serializers/json.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     1426 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/serializers/ma.py
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.906945 pringles_devs-2.0.1/pringles/simulator/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      168 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/simulator/__init__.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      327 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/simulator/errors.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      933 2024-03-29 23:10:25.000000 pringles_devs-2.0.1/pringles/simulator/events.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     4033 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/simulator/registry.py
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.918674 pringles_devs-2.0.1/pringles/simulator/registry_bootstrap/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)       72 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/simulator/registry_bootstrap/cpu.pringles
+-rw-r--r--   0 pedrotambo   (502) staff       (20)       80 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/simulator/registry_bootstrap/generator.pringles
+-rw-r--r--   0 pedrotambo   (502) staff       (20)       73 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/simulator/registry_bootstrap/qss1.pringles
+-rw-r--r--   0 pedrotambo   (502) staff       (20)       73 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/simulator/registry_bootstrap/qss2.pringles
+-rw-r--r--   0 pedrotambo   (502) staff       (20)       73 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/simulator/registry_bootstrap/qss3.pringles
+-rw-r--r--   0 pedrotambo   (502) staff       (20)       80 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/simulator/registry_bootstrap/queue.pringles
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      109 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/simulator/registry_bootstrap/transducer.pringles
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     9588 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/simulator/simulation.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     4194 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/simulator/simulator.py
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.923893 pringles_devs-2.0.1/pringles/utils/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      254 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/utils/__init__.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     4980 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/utils/discovery.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      169 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/utils/errors.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     1218 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/utils/plotting.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     3665 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/pringles/utils/vtime.py
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.940201 pringles_devs-2.0.1/pringles_devs.egg-info/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     2123 2024-04-29 22:12:02.000000 pringles_devs-2.0.1/pringles_devs.egg-info/PKG-INFO
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     2108 2024-04-29 22:12:02.000000 pringles_devs-2.0.1/pringles_devs.egg-info/SOURCES.txt
+-rw-r--r--   0 pedrotambo   (502) staff       (20)        1 2024-04-29 22:12:02.000000 pringles_devs-2.0.1/pringles_devs.egg-info/dependency_links.txt
+-rw-r--r--   0 pedrotambo   (502) staff       (20)       78 2024-04-29 22:12:02.000000 pringles_devs-2.0.1/pringles_devs.egg-info/requires.txt
+-rw-r--r--   0 pedrotambo   (502) staff       (20)       15 2024-04-29 22:12:02.000000 pringles_devs-2.0.1/pringles_devs.egg-info/top_level.txt
+-rw-r--r--   0 pedrotambo   (502) staff       (20)       77 2024-03-30 00:00:54.000000 pringles_devs-2.0.1/requirements.txt
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      440 2024-04-29 22:12:02.942064 pringles_devs-2.0.1/setup.cfg
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      844 2024-04-29 21:47:53.000000 pringles_devs-2.0.1/setup.py
+drwxr-xr-x   0 pedrotambo   (502) staff       (20)        0 2024-04-29 22:12:02.938989 pringles_devs-2.0.1/tests/
+-rw-r--r--   0 pedrotambo   (502) staff       (20)        0 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/tests/__init__.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     1403 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/tests/conftest.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     1936 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/tests/test_atomic_metadata_extractor.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)      648 2024-03-29 23:10:43.000000 pringles_devs-2.0.1/tests/test_events.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     2036 2024-03-29 22:53:16.000000 pringles_devs-2.0.1/tests/test_model_ipython_display.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     1549 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/tests/test_model_metadata_and_instanciation_integration.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     2501 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/tests/test_model_translation.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     3560 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/tests/test_simulation.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     3836 2024-04-05 21:28:03.000000 pringles_devs-2.0.1/tests/test_simulator.py
+-rw-r--r--   0 pedrotambo   (502) staff       (20)     2263 2024-03-26 14:33:45.000000 pringles_devs-2.0.1/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pringles-devs-1.0.3/PKG-INFO` & `pringles_devs-2.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: pringles-devs
-Version: 1.0.3
+Version: 2.0.1
 Summary: A DEVS model composition library
-Home-page: https://github.com/colonelpringles/pringles
+Home-page: https://git-modsimu.exp.dc.uba.ar/colonelpringles/pringles
 Author: Colonel Pringles
-License: UNKNOWN
-Description: ## Pringles - A DEVS model composition Python
-        [![Build Status](https://travis-ci.org/colonelpringles/pringles.svg?branch=master)](https://travis-ci.org/colonelpringles/pringles) [![Coverage](https://codecov.io/gh/colonelpringles/pringles/branch/master/graphs/badge.svg)](https://codecov.io/gh/colonelpringles/pringles/branch/master) [![pypi-version](https://img.shields.io/pypi/v/pringles-devs.svg)](https://pypi.org/project/pringles-devs/) [![Total alerts](https://img.shields.io/lgtm/alerts/g/colonelpringles/pringles.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/colonelpringles/pringles/alerts/) [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/colonelpringles/pringles.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/colonelpringles/pringles/context:python)
-        
-        Pringles is a DEVS model composition library, which makes easy to assemble and link multiple atomic/coupled models. It works as a Python library, and in its road ahead, will easily integrate with the Jupyter environment.
-        
-        
-        #### Requirements
-        - Python 3.7 (check out pyenv if you have a different python version installed)
-        
-        The library can be installed with pip:
-        ```
-        pip install pringles-devs
-        ```
-        
-        #### Extra Requirements
-        For local development, you can install everything through:
-        ```
-        make install
-        ```
-        in the repo root directory.
-        
-        After changes are made you can locally check the same things the CI does by executing:
-        ```
-        make local
-        ```
-        
-        
-        #### Pringles Examples
-        They can be found in https://github.com/colonelpringles/pringles_examples
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas==2.2.1
+Requires-Dist: ipython==8.18.1
+Requires-Dist: matplotlib==3.8.3
+Requires-Dist: asyncio==3.4.3
+Requires-Dist: tornado==6.4.0
+
+## Pringles - A DEVS model composition Python
+[![Build Status](https://travis-ci.org/colonelpringles/pringles.svg?branch=master)](https://travis-ci.org/colonelpringles/pringles) [![Coverage](https://codecov.io/gh/colonelpringles/pringles/branch/master/graphs/badge.svg)](https://codecov.io/gh/colonelpringles/pringles/branch/master) [![pypi-version](https://img.shields.io/pypi/v/pringles-devs.svg)](https://pypi.org/project/pringles-devs/) [![Total alerts](https://img.shields.io/lgtm/alerts/g/colonelpringles/pringles.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/colonelpringles/pringles/alerts/) [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/colonelpringles/pringles.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/colonelpringles/pringles/context:python)
+
+Pringles is a DEVS model composition library, which makes easy to assemble and link multiple atomic/coupled models. It works as a Python library, and in its road ahead, will easily integrate with the Jupyter environment.
+
+
+#### Requirements
+- Python 3.9 (check out pyenv if you have a different python version installed)
+
+The library can be installed with pip:
+```
+pip install pringles-devs
+```
+
+#### Extra Requirements
+For local development, you can install everything through:
+```
+make install
+```
+in the repo root directory.
+
+After changes are made you can locally check the same things the CI does by executing:
+```
+make local
+```
+
+
+#### Pringles Examples
+They can be found in https://github.com/colonelpringles/pringles_examples
```

### Comparing `pringles-devs-1.0.3/README.md` & `pringles_devs-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ## Pringles - A DEVS model composition Python
 [![Build Status](https://travis-ci.org/colonelpringles/pringles.svg?branch=master)](https://travis-ci.org/colonelpringles/pringles) [![Coverage](https://codecov.io/gh/colonelpringles/pringles/branch/master/graphs/badge.svg)](https://codecov.io/gh/colonelpringles/pringles/branch/master) [![pypi-version](https://img.shields.io/pypi/v/pringles-devs.svg)](https://pypi.org/project/pringles-devs/) [![Total alerts](https://img.shields.io/lgtm/alerts/g/colonelpringles/pringles.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/colonelpringles/pringles/alerts/) [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/colonelpringles/pringles.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/colonelpringles/pringles/context:python)
 
 Pringles is a DEVS model composition library, which makes easy to assemble and link multiple atomic/coupled models. It works as a Python library, and in its road ahead, will easily integrate with the Jupyter environment.
 
 
 #### Requirements
-- Python 3.7 (check out pyenv if you have a different python version installed)
+- Python 3.9 (check out pyenv if you have a different python version installed)
 
 The library can be installed with pip:
 ```
 pip install pringles-devs
 ```
 
 #### Extra Requirements
```

### Comparing `pringles-devs-1.0.3/pringles/backends/statics/basic.html` & `pringles_devs-2.0.1/pringles/backends/statics/basic.html`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/backends/statics/js/Canvas.js` & `pringles_devs-2.0.1/pringles/backends/statics/js/Canvas.js`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/backends/statics/js/ColorCodes.js` & `pringles_devs-2.0.1/pringles/backends/statics/js/ColorCodes.js`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/backends/statics/js/JSONModelGraphics.js` & `pringles_devs-2.0.1/pringles/backends/statics/js/JSONModelGraphics.js`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/backends/statics/js/Link.js` & `pringles_devs-2.0.1/pringles/backends/statics/js/Link.js`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/backends/statics/js/Model.js` & `pringles_devs-2.0.1/pringles/backends/statics/js/Model.js`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/backends/statics/js/Port.js` & `pringles_devs-2.0.1/pringles/backends/statics/js/Port.js`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/backends/statics/js/Square.js` & `pringles_devs-2.0.1/pringles/backends/statics/js/Square.js`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/backends/statics/js/main.js` & `pringles_devs-2.0.1/pringles/backends/statics/js/main.js`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/backends/statics/js/manifest.js` & `pringles_devs-2.0.1/pringles/backends/statics/js/manifest.js`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/backends/statics/js/toposort.js` & `pringles_devs-2.0.1/pringles/backends/statics/js/toposort.js`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/backends/statics/vendors/js/createjs/createjs-2013.12.12.min.js` & `pringles_devs-2.0.1/pringles/backends/statics/vendors/js/createjs/createjs-2013.12.12.min.js`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/backends/statics/vendors/js/jquery-3.2.1/jquery-3.2.1.min.js` & `pringles_devs-2.0.1/pringles/backends/statics/vendors/js/jquery-3.2.1/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/backends/web_display.py` & `pringles_devs-2.0.1/pringles/backends/web_display.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,16 +86,15 @@
 
 
 def _get_static_files_path() -> str:
     return os.path.join(
         os.path.dirname(__file__), 'statics')
 
 
-web_model_display_thread = ServerThread()
-
+web_model_display_thread = ServerThread(daemon=True)
 
 def ipython_inline_display(model: Model) -> bytes:
     import tornado.template
     from pringles.serializers import JsonSerializer
 
     if not web_model_display_thread.is_alive():
         web_model_display_thread.start()
```

### Comparing `pringles-devs-1.0.3/pringles/models/models.py` & `pringles_devs-2.0.1/pringles/models/models.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/serializers/json.py` & `pringles_devs-2.0.1/pringles/serializers/json.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/serializers/ma.py` & `pringles_devs-2.0.1/pringles/serializers/ma.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/simulator/events.py` & `pringles_devs-2.0.1/pringles/simulator/events.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,8 +18,14 @@
                  value: Union[float, List[float]]):
         self.time = time
         self.target_port = port
         self.value = value
 
     def serialize(self) -> str:
         """Serialize the :class:`Event` into a CD++ consumable string."""
-        return f"{str(self.time)} {self.target_port.name} {str(self.value)};"
+        return f"{str(self.time)} {self.target_port.name} {self._serialize_value()};"
+
+    def _serialize_value(self) -> str:
+        if type(self.value) == float or type(self.value) == int: 
+            return str(self.value)
+        else:
+            return f"[{','.join(map(str, self.value))}]"
```

### Comparing `pringles-devs-1.0.3/pringles/simulator/registry.py` & `pringles_devs-2.0.1/pringles/simulator/registry.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/simulator/simulation.py` & `pringles_devs-2.0.1/pringles/simulator/simulation.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/simulator/simulator.py` & `pringles_devs-2.0.1/pringles/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/utils/discovery.py` & `pringles_devs-2.0.1/pringles/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/utils/plotting.py` & `pringles_devs-2.0.1/pringles/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles/utils/vtime.py` & `pringles_devs-2.0.1/pringles/utils/vtime.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/pringles_devs.egg-info/PKG-INFO` & `pringles_devs-2.0.1/pringles_devs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: pringles-devs
-Version: 1.0.3
+Version: 2.0.1
 Summary: A DEVS model composition library
-Home-page: https://github.com/colonelpringles/pringles
+Home-page: https://git-modsimu.exp.dc.uba.ar/colonelpringles/pringles
 Author: Colonel Pringles
-License: UNKNOWN
-Description: ## Pringles - A DEVS model composition Python
-        [![Build Status](https://travis-ci.org/colonelpringles/pringles.svg?branch=master)](https://travis-ci.org/colonelpringles/pringles) [![Coverage](https://codecov.io/gh/colonelpringles/pringles/branch/master/graphs/badge.svg)](https://codecov.io/gh/colonelpringles/pringles/branch/master) [![pypi-version](https://img.shields.io/pypi/v/pringles-devs.svg)](https://pypi.org/project/pringles-devs/) [![Total alerts](https://img.shields.io/lgtm/alerts/g/colonelpringles/pringles.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/colonelpringles/pringles/alerts/) [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/colonelpringles/pringles.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/colonelpringles/pringles/context:python)
-        
-        Pringles is a DEVS model composition library, which makes easy to assemble and link multiple atomic/coupled models. It works as a Python library, and in its road ahead, will easily integrate with the Jupyter environment.
-        
-        
-        #### Requirements
-        - Python 3.7 (check out pyenv if you have a different python version installed)
-        
-        The library can be installed with pip:
-        ```
-        pip install pringles-devs
-        ```
-        
-        #### Extra Requirements
-        For local development, you can install everything through:
-        ```
-        make install
-        ```
-        in the repo root directory.
-        
-        After changes are made you can locally check the same things the CI does by executing:
-        ```
-        make local
-        ```
-        
-        
-        #### Pringles Examples
-        They can be found in https://github.com/colonelpringles/pringles_examples
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas==2.2.1
+Requires-Dist: ipython==8.18.1
+Requires-Dist: matplotlib==3.8.3
+Requires-Dist: asyncio==3.4.3
+Requires-Dist: tornado==6.4.0
+
+## Pringles - A DEVS model composition Python
+[![Build Status](https://travis-ci.org/colonelpringles/pringles.svg?branch=master)](https://travis-ci.org/colonelpringles/pringles) [![Coverage](https://codecov.io/gh/colonelpringles/pringles/branch/master/graphs/badge.svg)](https://codecov.io/gh/colonelpringles/pringles/branch/master) [![pypi-version](https://img.shields.io/pypi/v/pringles-devs.svg)](https://pypi.org/project/pringles-devs/) [![Total alerts](https://img.shields.io/lgtm/alerts/g/colonelpringles/pringles.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/colonelpringles/pringles/alerts/) [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/colonelpringles/pringles.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/colonelpringles/pringles/context:python)
+
+Pringles is a DEVS model composition library, which makes easy to assemble and link multiple atomic/coupled models. It works as a Python library, and in its road ahead, will easily integrate with the Jupyter environment.
+
+
+#### Requirements
+- Python 3.9 (check out pyenv if you have a different python version installed)
+
+The library can be installed with pip:
+```
+pip install pringles-devs
+```
+
+#### Extra Requirements
+For local development, you can install everything through:
+```
+make install
+```
+in the repo root directory.
+
+After changes are made you can locally check the same things the CI does by executing:
+```
+make local
+```
+
+
+#### Pringles Examples
+They can be found in https://github.com/colonelpringles/pringles_examples
```

### Comparing `pringles-devs-1.0.3/pringles_devs.egg-info/SOURCES.txt` & `pringles_devs-2.0.1/pringles_devs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 pringles/__init__.py
 pringles/backends/__init__.py
```

### Comparing `pringles-devs-1.0.3/setup.py` & `pringles_devs-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 
 with open('requirements.txt', 'r') as f:
     dependencies = [line.strip() for line in f.readlines()]
 
 setuptools.setup(
     name="pringles-devs",
-    version="1.0.3",
+    version="2.0.1",
     author="Colonel Pringles",
     # author_email="example@email.com",
     description="A DEVS model composition library",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/colonelpringles/pringles",
+    url="https://git-modsimu.exp.dc.uba.ar/colonelpringles/pringles",
     packages=setuptools.find_packages(),
     classifiers=[
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     install_requires=dependencies,
     include_package_data=True,
 )
```

### Comparing `pringles-devs-1.0.3/tests/conftest.py` & `pringles_devs-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/tests/test_atomic_metadata_extractor.py` & `pringles_devs-2.0.1/tests/test_atomic_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/tests/test_events.py` & `pringles_devs-2.0.1/tests/test_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 sample_port = Port("sample_port", None)
 one_hour_time = VirtualTime.of_hours(1)
 
 
 @pytest.mark.parametrize("event,expected_serialization", [
     (Event(one_hour_time, sample_port, 1.5), "01:00:00:000 sample_port 1.5;"),
     (Event(one_hour_time, sample_port, 1), "01:00:00:000 sample_port 1;"),
-    (Event(one_hour_time, sample_port, [1.5, 2.3]), "01:00:00:000 sample_port [1.5, 2.3];"),
+    (Event(one_hour_time, sample_port, [1.5,2.3]), "01:00:00:000 sample_port [1.5,2.3];"),
 ])
 def test_event_serialized_correctly(event: Event, expected_serialization: str):
     assert event.serialize() == expected_serialization
```

### Comparing `pringles-devs-1.0.3/tests/test_model_ipython_display.py` & `pringles_devs-2.0.1/tests/test_model_ipython_display.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/tests/test_model_metadata_and_instanciation_integration.py` & `pringles_devs-2.0.1/tests/test_model_metadata_and_instanciation_integration.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/tests/test_model_translation.py` & `pringles_devs-2.0.1/tests/test_model_translation.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/tests/test_simulation.py` & `pringles_devs-2.0.1/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/tests/test_simulator.py` & `pringles_devs-2.0.1/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `pringles-devs-1.0.3/tests/test_utils.py` & `pringles_devs-2.0.1/tests/test_utils.py`

 * *Files identical despite different names*

