# Comparing `tmp/jaeger-1.6.3.tar.gz` & `tmp/jaeger-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaeger-1.6.3.tar", max compression
+gzip compressed data, was "jaeger-1.6.4.tar", max compression
```

## Comparing `jaeger-1.6.3.tar` & `jaeger-1.6.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1504 2024-04-01 21:45:34.112062 jaeger-1.6.3/LICENSE.md
--rw-r--r--   0        0        0     2398 2024-04-01 21:45:34.112062 jaeger-1.6.3/README.md
--rw-r--r--   0        0        0     3477 2024-04-01 21:45:34.116062 jaeger-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     1745 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/__init__.py
--rw-r--r--   0        0        0    20331 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/__main__.py
--rw-r--r--   0        0        0       61 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/__init__.py
--rw-r--r--   0        0        0     5033 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/actor.py
--rw-r--r--   0        0        0      816 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/__init__.py
--rw-r--r--   0        0        0     1029 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/alerts.py
--rw-r--r--   0        0        0     1182 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/can.py
--rw-r--r--   0        0        0     3381 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/chiller.py
--rw-r--r--   0        0        0    35257 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/configuration.py
--rw-r--r--   0        0        0      722 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/debug.py
--rw-r--r--   0        0        0     2690 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/disable.py
--rw-r--r--   0        0        0    15031 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/fvc.py
--rw-r--r--   0        0        0    11347 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/home.py
--rw-r--r--   0        0        0     5314 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/ieb.py
--rw-r--r--   0        0        0     1410 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/pollers.py
--rw-r--r--   0        0        0    16070 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/positioner.py
--rw-r--r--   0        0        0     9994 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/power.py
--rw-r--r--   0        0        0      990 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/snapshot.py
--rw-r--r--   0        0        0     1323 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/talk.py
--rw-r--r--   0        0        0     1034 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/testing.py
--rw-r--r--   0        0        0     3579 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/unwind.py
--rw-r--r--   0        0        0      949 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/actor/commands/version.py
--rw-r--r--   0        0        0    14065 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/alerts.py
--rw-r--r--   0        0        0    21709 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/can.py
--rw-r--r--   0        0        0     5257 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/chiller.py
--rw-r--r--   0        0        0     3964 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/__init__.py
--rw-r--r--   0        0        0    22135 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/base.py
--rw-r--r--   0        0        0     9010 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/bootloader.py
--rw-r--r--   0        0        0    12181 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/calibration.py
--rw-r--r--   0        0        0    10788 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/goto.py
--rw-r--r--   0        0        0     6013 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/status.py
--rw-r--r--   0        0        0    26797 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/commands/trajectory.py
--rw-r--r--   0        0        0    10030 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/chiller_APO.yaml
--rw-r--r--   0        0        0     7487 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/chiller_APO_variables.csv
--rw-r--r--   0        0        0     1317 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/fvc.yaml
--rw-r--r--   0        0        0    10541 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/ieb_APO.yaml
--rw-r--r--   0        0        0    10539 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/ieb_LCO.yaml
--rw-r--r--   0        0        0     3329 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/jaeger_APO.yml
--rw-r--r--   0        0        0     3302 2024-04-01 21:45:34.116062 jaeger-1.6.3/python/jaeger/etc/jaeger_LCO.yml
--rw-r--r--   0        0        0     8711 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/etc/schema.json
--rw-r--r--   0        0        0     1815 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/etc/sextants/epfl.yaml
--rw-r--r--   0        0        0     2367 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/etc/sextants/osu.yaml
--rw-r--r--   0        0        0     1512 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/etc/sextants/schema.json
--rw-r--r--   0        0        0     2364 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/etc/sextants/uw.yaml
--rw-r--r--   0        0        0     3545 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/exceptions.py
--rw-r--r--   0        0        0    52222 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/fps.py
--rw-r--r--   0        0        0    40780 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/fvc.py
--rw-r--r--   0        0        0     4510 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/ieb.py
--rw-r--r--   0        0        0      162 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/interfaces/__init__.py
--rw-r--r--   0        0        0     1142 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/interfaces/bus.py
--rw-r--r--   0        0        0     6759 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/interfaces/cannet.py
--rw-r--r--   0        0        0    12892 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/interfaces/message.py
--rw-r--r--   0        0        0     1874 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/interfaces/notifier.py
--rw-r--r--   0        0        0     1199 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/interfaces/virtual.py
--rw-r--r--   0        0        0    19803 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/kaiju.py
--rw-r--r--   0        0        0     8034 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/maskbits.py
--rw-r--r--   0        0        0     7296 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/plotting.py
--rw-r--r--   0        0        0    18121 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/positioner.py
--rw-r--r--   0        0        0        0 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/scripts/__init__.py
--rw-r--r--   0        0        0     1825 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/scripts/generate_chiller_yaml.py
--rwxr-xr-x   0        0        0    19975 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/scripts/robotcalib.py
--rw-r--r--   0        0        0      293 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/target/__init__.py
--rw-r--r--   0        0        0    65093 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/target/configuration.py
--rw-r--r--   0        0        0     9413 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/target/design.py
--rw-r--r--   0        0        0    11797 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/target/tools.py
--rw-r--r--   0        0        0    12403 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/testing.py
--rw-r--r--   0        0        0       60 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/utils/__init__.py
--rw-r--r--   0        0        0     9562 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/utils/database.py
--rw-r--r--   0        0        0    14766 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/utils/helpers.py
--rw-r--r--   0        0        0     9549 2024-04-01 21:45:34.120062 jaeger-1.6.3/python/jaeger/utils/utils.py
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 jaeger-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-04-29 21:30:17.454818 jaeger-1.6.4/LICENSE.md
+-rw-r--r--   0        0        0     2398 2024-04-29 21:30:17.454818 jaeger-1.6.4/README.md
+-rw-r--r--   0        0        0     3477 2024-04-29 21:30:17.458818 jaeger-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0     1745 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/__init__.py
+-rw-r--r--   0        0        0    20331 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/__main__.py
+-rw-r--r--   0        0        0       61 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/__init__.py
+-rw-r--r--   0        0        0     5033 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/actor.py
+-rw-r--r--   0        0        0      816 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1029 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/alerts.py
+-rw-r--r--   0        0        0     1182 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/can.py
+-rw-r--r--   0        0        0     3381 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/chiller.py
+-rw-r--r--   0        0        0    35328 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/configuration.py
+-rw-r--r--   0        0        0      722 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/debug.py
+-rw-r--r--   0        0        0     2690 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/disable.py
+-rw-r--r--   0        0        0    15031 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/fvc.py
+-rw-r--r--   0        0        0    11347 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/home.py
+-rw-r--r--   0        0        0     5314 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/ieb.py
+-rw-r--r--   0        0        0     1410 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/pollers.py
+-rw-r--r--   0        0        0    16070 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/positioner.py
+-rw-r--r--   0        0        0     9994 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/power.py
+-rw-r--r--   0        0        0      990 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/snapshot.py
+-rw-r--r--   0        0        0     1323 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/talk.py
+-rw-r--r--   0        0        0     1034 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/testing.py
+-rw-r--r--   0        0        0     3579 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/unwind.py
+-rw-r--r--   0        0        0      949 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/actor/commands/version.py
+-rw-r--r--   0        0        0    14065 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/alerts.py
+-rw-r--r--   0        0        0    21709 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/can.py
+-rw-r--r--   0        0        0     5257 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/chiller.py
+-rw-r--r--   0        0        0     3964 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/commands/__init__.py
+-rw-r--r--   0        0        0    22135 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/commands/base.py
+-rw-r--r--   0        0        0     9010 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/commands/bootloader.py
+-rw-r--r--   0        0        0    12181 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/commands/calibration.py
+-rw-r--r--   0        0        0    10788 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/commands/goto.py
+-rw-r--r--   0        0        0     6013 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/commands/status.py
+-rw-r--r--   0        0        0    26797 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/commands/trajectory.py
+-rw-r--r--   0        0        0    10030 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/etc/chiller_APO.yaml
+-rw-r--r--   0        0        0     7487 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/etc/chiller_APO_variables.csv
+-rw-r--r--   0        0        0     1317 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/etc/fvc.yaml
+-rw-r--r--   0        0        0    10541 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/etc/ieb_APO.yaml
+-rw-r--r--   0        0        0    10539 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/etc/ieb_LCO.yaml
+-rw-r--r--   0        0        0     3329 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/etc/jaeger_APO.yml
+-rw-r--r--   0        0        0     3302 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/etc/jaeger_LCO.yml
+-rw-r--r--   0        0        0     8711 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/etc/schema.json
+-rw-r--r--   0        0        0     1815 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/etc/sextants/epfl.yaml
+-rw-r--r--   0        0        0     2367 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/etc/sextants/osu.yaml
+-rw-r--r--   0        0        0     1512 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/etc/sextants/schema.json
+-rw-r--r--   0        0        0     2364 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/etc/sextants/uw.yaml
+-rw-r--r--   0        0        0     3545 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/exceptions.py
+-rw-r--r--   0        0        0    52222 2024-04-29 21:30:17.458818 jaeger-1.6.4/python/jaeger/fps.py
+-rw-r--r--   0        0        0    40780 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/fvc.py
+-rw-r--r--   0        0        0     4510 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/ieb.py
+-rw-r--r--   0        0        0      162 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/interfaces/__init__.py
+-rw-r--r--   0        0        0     1142 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/interfaces/bus.py
+-rw-r--r--   0        0        0     6759 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/interfaces/cannet.py
+-rw-r--r--   0        0        0    12892 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/interfaces/message.py
+-rw-r--r--   0        0        0     1874 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/interfaces/notifier.py
+-rw-r--r--   0        0        0     1199 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/interfaces/virtual.py
+-rw-r--r--   0        0        0    19803 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/kaiju.py
+-rw-r--r--   0        0        0     8034 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/maskbits.py
+-rw-r--r--   0        0        0     7296 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/plotting.py
+-rw-r--r--   0        0        0    18121 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/positioner.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/scripts/__init__.py
+-rw-r--r--   0        0        0     1825 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/scripts/generate_chiller_yaml.py
+-rwxr-xr-x   0        0        0    19975 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/scripts/robotcalib.py
+-rw-r--r--   0        0        0      293 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/target/__init__.py
+-rw-r--r--   0        0        0    65093 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/target/configuration.py
+-rw-r--r--   0        0        0     9413 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/target/design.py
+-rw-r--r--   0        0        0    11797 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/target/tools.py
+-rw-r--r--   0        0        0    12403 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/testing.py
+-rw-r--r--   0        0        0       60 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/utils/__init__.py
+-rw-r--r--   0        0        0     9562 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/utils/database.py
+-rw-r--r--   0        0        0    14766 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/utils/helpers.py
+-rw-r--r--   0        0        0     9549 2024-04-29 21:30:17.462818 jaeger-1.6.4/python/jaeger/utils/utils.py
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 jaeger-1.6.4/PKG-INFO
```

### Comparing `jaeger-1.6.3/LICENSE.md` & `jaeger-1.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/README.md` & `jaeger-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/pyproject.toml` & `jaeger-1.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaeger"
-version = "1.6.3"
+version = "1.6.4"
 description = "Controllers for the SDSS-V FPS"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/jaeger"
 repository = "https://github.com/sdss/jaeger"
 documentation = "https://sdss-jaeger.readthedocs.io/en/latest/"
```

### Comparing `jaeger-1.6.3/python/jaeger/__init__.py` & `jaeger-1.6.4/python/jaeger/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/__main__.py` & `jaeger-1.6.4/python/jaeger/__main__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/actor.py` & `jaeger-1.6.4/python/jaeger/actor/actor.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/__init__.py` & `jaeger-1.6.4/python/jaeger/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/alerts.py` & `jaeger-1.6.4/python/jaeger/actor/commands/alerts.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/can.py` & `jaeger-1.6.4/python/jaeger/actor/commands/can.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/chiller.py` & `jaeger-1.6.4/python/jaeger/actor/commands/chiller.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/configuration.py` & `jaeger-1.6.4/python/jaeger/actor/commands/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,17 +166,18 @@
                         raise ValueError("IEB not connected")
 
                     temperature = (await command.actor.fps.ieb.read_device("T3"))[0]
                     if not isinstance(temperature, float) or temperature < -100:
                         raise ValueError("Invalid ambient temperature")
 
                     guider_scale = float(numpy.polyval(temp_coeffs, temperature))
-                    # HACK: we should redo this relation, but for now just use the
-                    # measured change in guider scale after moving the IMB.
-                    guider_scale *= 1.0018904537
+                    if command.actor.observatory == "LCO":
+                        # HACK: we should redo this relation, but for now just use the
+                        # measured change in guider scale after moving the IMB.
+                        guider_scale *= 1.0018904537
 
                     command.debug(
                         "Using focal scale factor derived from ambient "
                         f"temperature ({temperature:.2f} C): {guider_scale:.6f}"
                     )
                 except Exception as err:
                     command.warning(
```

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/debug.py` & `jaeger-1.6.4/python/jaeger/actor/commands/debug.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/disable.py` & `jaeger-1.6.4/python/jaeger/actor/commands/disable.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/fvc.py` & `jaeger-1.6.4/python/jaeger/actor/commands/fvc.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/home.py` & `jaeger-1.6.4/python/jaeger/actor/commands/home.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/ieb.py` & `jaeger-1.6.4/python/jaeger/actor/commands/ieb.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/pollers.py` & `jaeger-1.6.4/python/jaeger/actor/commands/pollers.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/positioner.py` & `jaeger-1.6.4/python/jaeger/actor/commands/positioner.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/power.py` & `jaeger-1.6.4/python/jaeger/actor/commands/power.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/snapshot.py` & `jaeger-1.6.4/python/jaeger/actor/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/talk.py` & `jaeger-1.6.4/python/jaeger/actor/commands/talk.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/testing.py` & `jaeger-1.6.4/python/jaeger/actor/commands/testing.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/unwind.py` & `jaeger-1.6.4/python/jaeger/actor/commands/unwind.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/actor/commands/version.py` & `jaeger-1.6.4/python/jaeger/actor/commands/version.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/alerts.py` & `jaeger-1.6.4/python/jaeger/alerts.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/can.py` & `jaeger-1.6.4/python/jaeger/can.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/chiller.py` & `jaeger-1.6.4/python/jaeger/chiller.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/commands/__init__.py` & `jaeger-1.6.4/python/jaeger/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/commands/base.py` & `jaeger-1.6.4/python/jaeger/commands/base.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/commands/bootloader.py` & `jaeger-1.6.4/python/jaeger/commands/bootloader.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/commands/calibration.py` & `jaeger-1.6.4/python/jaeger/commands/calibration.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/commands/goto.py` & `jaeger-1.6.4/python/jaeger/commands/goto.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/commands/status.py` & `jaeger-1.6.4/python/jaeger/commands/status.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/commands/trajectory.py` & `jaeger-1.6.4/python/jaeger/commands/trajectory.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/etc/chiller_APO.yaml` & `jaeger-1.6.4/python/jaeger/etc/chiller_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/etc/chiller_APO_variables.csv` & `jaeger-1.6.4/python/jaeger/etc/chiller_APO_variables.csv`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/etc/fvc.yaml` & `jaeger-1.6.4/python/jaeger/etc/fvc.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/etc/ieb_APO.yaml` & `jaeger-1.6.4/python/jaeger/etc/ieb_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/etc/ieb_LCO.yaml` & `jaeger-1.6.4/python/jaeger/etc/ieb_LCO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/etc/jaeger_APO.yml` & `jaeger-1.6.4/python/jaeger/etc/jaeger_APO.yml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/etc/jaeger_LCO.yml` & `jaeger-1.6.4/python/jaeger/etc/jaeger_LCO.yml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/etc/schema.json` & `jaeger-1.6.4/python/jaeger/etc/schema.json`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/etc/sextants/epfl.yaml` & `jaeger-1.6.4/python/jaeger/etc/sextants/epfl.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/etc/sextants/osu.yaml` & `jaeger-1.6.4/python/jaeger/etc/sextants/osu.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/etc/sextants/schema.json` & `jaeger-1.6.4/python/jaeger/etc/sextants/schema.json`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/etc/sextants/uw.yaml` & `jaeger-1.6.4/python/jaeger/etc/sextants/uw.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/exceptions.py` & `jaeger-1.6.4/python/jaeger/exceptions.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/fps.py` & `jaeger-1.6.4/python/jaeger/fps.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/fvc.py` & `jaeger-1.6.4/python/jaeger/fvc.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/ieb.py` & `jaeger-1.6.4/python/jaeger/ieb.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/interfaces/bus.py` & `jaeger-1.6.4/python/jaeger/interfaces/bus.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/interfaces/cannet.py` & `jaeger-1.6.4/python/jaeger/interfaces/cannet.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/interfaces/message.py` & `jaeger-1.6.4/python/jaeger/interfaces/message.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/interfaces/notifier.py` & `jaeger-1.6.4/python/jaeger/interfaces/notifier.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/interfaces/virtual.py` & `jaeger-1.6.4/python/jaeger/interfaces/virtual.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/kaiju.py` & `jaeger-1.6.4/python/jaeger/kaiju.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/maskbits.py` & `jaeger-1.6.4/python/jaeger/maskbits.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/plotting.py` & `jaeger-1.6.4/python/jaeger/plotting.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/positioner.py` & `jaeger-1.6.4/python/jaeger/positioner.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/scripts/generate_chiller_yaml.py` & `jaeger-1.6.4/python/jaeger/scripts/generate_chiller_yaml.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/scripts/robotcalib.py` & `jaeger-1.6.4/python/jaeger/scripts/robotcalib.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/target/configuration.py` & `jaeger-1.6.4/python/jaeger/target/configuration.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/target/design.py` & `jaeger-1.6.4/python/jaeger/target/design.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/target/tools.py` & `jaeger-1.6.4/python/jaeger/target/tools.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/testing.py` & `jaeger-1.6.4/python/jaeger/testing.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/utils/database.py` & `jaeger-1.6.4/python/jaeger/utils/database.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/utils/helpers.py` & `jaeger-1.6.4/python/jaeger/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/python/jaeger/utils/utils.py` & `jaeger-1.6.4/python/jaeger/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.6.3/PKG-INFO` & `jaeger-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaeger
-Version: 1.6.3
+Version: 1.6.4
 Summary: Controllers for the SDSS-V FPS
 Home-page: https://github.com/sdss/jaeger
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.9,<3.11
```

