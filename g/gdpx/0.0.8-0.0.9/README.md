# Comparing `tmp/gdpx-0.0.8.tar.gz` & `tmp/gdpx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdpx-0.0.8.tar", last modified: Sun Apr 21 01:05:46 2024, max compression
+gzip compressed data, was "gdpx-0.0.9.tar", last modified: Tue Apr 30 02:48:50 2024, max compression
```

## Comparing `gdpx-0.0.8.tar` & `gdpx-0.0.9.tar`

### file list

```diff
@@ -1,321 +1,330 @@
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.370157 gdpx-0.0.8/
--rw-r--r--   0 jx1279   (353055) chem     (30004)    35149 2023-04-10 18:29:40.000000 gdpx-0.0.8/LICENSE
--rw-r--r--   0 jx1279   (353055) chem     (30004)    47632 2024-04-21 01:05:46.370157 gdpx-0.0.8/PKG-INFO
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6294 2023-12-12 17:08:13.000000 gdpx-0.0.8/README.md
--rw-r--r--   0 jx1279   (353055) chem     (30004)      878 2024-04-21 01:05:10.000000 gdpx-0.0.8/pyproject.toml
--rw-r--r--   0 jx1279   (353055) chem     (30004)       38 2024-04-21 01:05:46.370157 gdpx-0.0.8/setup.cfg
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:45.220143 gdpx-0.0.8/src/
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:45.918151 gdpx-0.0.8/src/gdpx/
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.007152 gdpx-0.0.8/src/gdpx/bias/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1216 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/__init__.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.008152 gdpx-0.0.8/src/gdpx/bias/afir/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      119 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/afir/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4571 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/afir/afir.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1679 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/bias/bias.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7641 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/bondboost.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.010152 gdpx-0.0.8/src/gdpx/bias/gaussian/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      309 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/gaussian/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9777 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/gaussian/bond.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5649 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/gaussian/com.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3047 2024-04-21 01:03:18.000000 gdpx-0.0.8/src/gdpx/bias/gaussian/gaussian.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5429 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/gaussian/rmsd.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.012153 gdpx-0.0.8/src/gdpx/bias/harmonic/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      248 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/harmonic/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3923 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/bias/harmonic/distance.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2740 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/harmonic/harmonic.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2192 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/harmonic/plane.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1209 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/bias/nuclei.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1404 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/timeio.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.013152 gdpx-0.0.8/src/gdpx/bias/utils/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      224 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/utils/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2696 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/bias/utils/bondpair.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.113154 gdpx-0.0.8/src/gdpx/builder/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2881 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/builder/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3100 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/builder/builder.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      800 2023-12-03 04:28:22.000000 gdpx-0.0.8/src/gdpx/builder/cleave_group.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2659 2023-12-03 04:22:10.000000 gdpx-0.0.8/src/gdpx/builder/cleave_surface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5743 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/builder/constraints.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      384 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/builder/crossover.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1469 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/builder/dimer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7451 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/builder/direct.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.115154 gdpx-0.0.8/src/gdpx/builder/graph/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      287 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/builder/graph/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5942 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/builder/graph/exchange.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5089 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/builder/graph/insert.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5355 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/builder/graph/modifier.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5664 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/builder/graph/remove.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5373 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/builder/group.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6914 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/builder/hypercube.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8530 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/builder/insert.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8537 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/builder/interface.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.116154 gdpx-0.0.8/src/gdpx/builder/mutation/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      892 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/builder/mutation/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5565 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/builder/packer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3406 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/builder/perturbator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    15179 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/builder/randomBuilder.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    19280 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/builder/region.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      745 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/builder/repeat.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3614 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/builder/species.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7762 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/builder/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1391 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/builder/zoom.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.116154 gdpx-0.0.8/src/gdpx/cli/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3613 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/cli/compute.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.156154 gdpx-0.0.8/src/gdpx/colvar/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      463 2024-04-21 01:03:18.000000 gdpx-0.0.8/src/gdpx/colvar/__init__.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2622 2023-09-06 03:11:48.000000 gdpx-0.0.8/src/gdpx/colvar/compute_reweight.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1554 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/colvar/coordination.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      636 2024-04-21 01:03:18.000000 gdpx-0.0.8/src/gdpx/colvar/distance.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3567 2024-02-19 02:43:10.000000 gdpx-0.0.8/src/gdpx/colvar/fingerprint.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     5096 2023-08-21 19:26:15.000000 gdpx-0.0.8/src/gdpx/colvar/plot_meta.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5603 2023-11-09 19:54:15.000000 gdpx-0.0.8/src/gdpx/colvar/plot_string.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4637 2023-08-31 04:35:40.000000 gdpx-0.0.8/src/gdpx/colvar/plotstring.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      178 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/colvar/position.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2749 2023-09-05 04:11:13.000000 gdpx-0.0.8/src/gdpx/colvar/reweight.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1461 2024-02-21 03:43:26.000000 gdpx-0.0.8/src/gdpx/colvar/rmsd.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.186154 gdpx-0.0.8/src/gdpx/comparator/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      954 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/comparator/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2739 2023-12-06 01:21:35.000000 gdpx-0.0.8/src/gdpx/comparator/cartesian.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      827 2024-01-23 21:20:47.000000 gdpx-0.0.8/src/gdpx/comparator/comparator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5645 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/comparator/coordination.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4595 2023-12-06 01:21:35.000000 gdpx-0.0.8/src/gdpx/comparator/graph.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1193 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/comparator/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3067 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/comparator/reaction.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5123 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/comparator/singlepoint.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.190155 gdpx-0.0.8/src/gdpx/computation/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      657 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/computation/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    28108 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/computation/asedriver.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    21677 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/computation/cp2k.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    17920 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/computation/driver.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8651 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/computation/espresso.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    19844 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/computation/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    31347 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/computation/lammps.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    22229 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/computation/lasp.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.207155 gdpx-0.0.8/src/gdpx/computation/mc/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4259 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/computation/mc/tfmc.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.208155 gdpx-0.0.8/src/gdpx/computation/md/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1082 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/computation/md/md_utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5296 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/computation/md/nosehoover.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/computation/reann.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2372 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/computation/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    20268 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/computation/vasp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1463 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/config.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.211155 gdpx-0.0.8/src/gdpx/core/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      108 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/core/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2415 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/core/node.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2492 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/core/operation.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      861 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/core/placeholder.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7122 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/core/register.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.213155 gdpx-0.0.8/src/gdpx/core/session/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      148 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/core/session/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12927 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/core/session/active.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2007 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/core/session/basic.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7922 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/core/session/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2686 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/core/session/session.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1998 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/core/session/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1461 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/core/variable.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.235155 gdpx-0.0.8/src/gdpx/data/
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6210 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/data/ClusterAndCUR.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      249 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/data/__init__.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    57236 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/data/analyser.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    14976 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/data/array.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7981 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/data/cleave_deviation.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1901 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/data/convert.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3103 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/data/correction.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9171 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/data/database.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11961 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/data/dataset.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1552 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/data/extatoms.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3389 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/data/extract_evolution.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    14345 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/data/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    10543 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/data/operators.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1950 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/data/system.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1210 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/data/utils.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.238155 gdpx-0.0.8/src/gdpx/describer/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      441 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/describer/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2325 2024-02-09 18:38:45.000000 gdpx-0.0.8/src/gdpx/describer/describer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2066 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/describer/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2365 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/describer/soap.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2438 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/describer/spc.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.240155 gdpx-0.0.8/src/gdpx/expedition/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1360 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/expedition/__init__.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.241155 gdpx-0.0.8/src/gdpx/expedition/accelerated_dynamics/
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    16224 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/expedition/accelerated_dynamics/prev_example.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.242155 gdpx-0.0.8/src/gdpx/expedition/af/
--rw-r--r--   0 jx1279   (353055) chem     (30004)    10315 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/expedition/af/afir.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1793 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/expedition/expedition.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.243155 gdpx-0.0.8/src/gdpx/expedition/ga/
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    25876 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/expedition/ga/engine.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    18347 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/expedition/ga/population.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5346 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/expedition/interface.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.245155 gdpx-0.0.8/src/gdpx/expedition/monte_carlo/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      149 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/expedition/monte_carlo/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      802 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/expedition/monte_carlo/basin_hopping.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    20408 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/expedition/monte_carlo/monte_carlo.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.248155 gdpx-0.0.8/src/gdpx/expedition/monte_carlo/operators/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2356 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/expedition/monte_carlo/operators/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9188 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/expedition/monte_carlo/operators/exchange.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5008 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/expedition/monte_carlo/operators/move.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8411 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/expedition/monte_carlo/operators/operator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11096 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/expedition/monte_carlo/operators/react.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4394 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/expedition/monte_carlo/operators/swap.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.248155 gdpx-0.0.8/src/gdpx/expedition/simulated_annealing/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5956 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/expedition/simulated_annealing/simulated_annealing.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.253155 gdpx-0.0.8/src/gdpx/graph/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      147 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/graph/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    13870 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/graph/comparison.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12839 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/graph/creator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12200 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/graph/graph_main.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5142 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/graph/molecule.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    31066 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/graph/sites.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2905 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/graph/surface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1849 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/graph/utils.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     8811 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/main.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2242 2023-07-23 06:17:20.000000 gdpx-0.0.8/src/gdpx/nanoparticle.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.255155 gdpx-0.0.8/src/gdpx/potential/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      274 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/potential/__init__.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.256155 gdpx-0.0.8/src/gdpx/potential/calculators/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      654 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/potential/calculators/dummy.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4675 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/potential/calculators/mixer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1256 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/potential/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6073 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/potential/manager.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.266156 gdpx-0.0.8/src/gdpx/potential/managers/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3069 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/potential/managers/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1430 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/potential/managers/asepot.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2787 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/potential/managers/bias.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2947 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/cp2k.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.268156 gdpx-0.0.8/src/gdpx/potential/managers/deepmd/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      225 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/potential/managers/deepmd/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7170 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/potential/managers/deepmd/calculator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4058 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/potential/managers/deepmd/convert.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    23429 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/potential/managers/deepmd/deepmd.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1141 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/potential/managers/dftd3.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2231 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/eam.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1117 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/emt.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2363 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/espresso.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.271156 gdpx-0.0.8/src/gdpx/potential/managers/gp/
--rw-r--r--   0 jx1279   (353055) chem     (30004)       83 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/gp/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2348 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/gp/bench.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1376 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/gp/fgp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3746 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/gp/gptools.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3474 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/gp/representation.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    46869 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/gp/sgp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2715 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/potential/managers/grid.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1986 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/lasp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    17115 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/potential/managers/mace.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5167 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/potential/managers/mixer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7976 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/potential/managers/nequip.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.271156 gdpx-0.0.8/src/gdpx/potential/managers/plumed/
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.272156 gdpx-0.0.8/src/gdpx/potential/managers/plumed/calculators/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2728 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/potential/managers/plumed/calculators/plumed.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9361 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/potential/managers/plumed/calculators/plumed2.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2394 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/potential/managers/plumed/plumed.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.273156 gdpx-0.0.8/src/gdpx/potential/managers/reann/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7421 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/potential/managers/reann/beann.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.274156 gdpx-0.0.8/src/gdpx/potential/managers/reann/calculators/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3484 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/potential/managers/reann/calculators/reann.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    17636 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/potential/managers/reann/reann.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1396 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/reax.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8903 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/schnet.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3654 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/vasp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1207 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/potential/managers/xtb.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5499 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/potential/trainer.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.276156 gdpx-0.0.8/src/gdpx/reactor/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      860 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/reactor/__init__.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.282156 gdpx-0.0.8/src/gdpx/reactor/future/
--rw-r--r--   0 jx1279   (353055) chem     (30004)    23672 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/reactor/future/AccCons.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2601 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/reactor/future/AccNEB.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2921 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/reactor/future/cmp_mep.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3833 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/reactor/future/constrain.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7051 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/reactor/future/crs.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2226 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/reactor/future/diffusion3.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    11410 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/reactor/future/find_adsorption.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3188 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/reactor/future/find_inter.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3002 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/reactor/future/muller-brown.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     1154 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/reactor/future/test_mh.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4115 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/reactor/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1482 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/reactor/reactor.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.284156 gdpx-0.0.8/src/gdpx/reactor/string/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      232 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/reactor/string/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    17830 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/reactor/string/cp2k.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5117 2024-03-17 21:29:29.000000 gdpx-0.0.8/src/gdpx/reactor/string/grid.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    10477 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/reactor/string/pathway.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11906 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/reactor/string/string.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9158 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/reactor/string/vasp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2320 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/reactor/utils.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.287156 gdpx-0.0.8/src/gdpx/scheduler/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      699 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/scheduler/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      624 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/scheduler/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      631 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/scheduler/local.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3553 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/scheduler/lsf.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1147 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/scheduler/pbs.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4439 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/scheduler/scheduler.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3226 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/scheduler/slurm.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.306156 gdpx-0.0.8/src/gdpx/selector/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1078 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/selector/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3664 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/selector/basin.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6276 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/selector/compare.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1376 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/selector/composition.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8362 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/selector/cur.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7241 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/selector/descriptor.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5631 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/selector/graph.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6398 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/selector/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2905 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/selector/interval.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      622 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/selector/invariant.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3284 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/selector/locate.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    14855 2024-04-20 02:06:51.000000 gdpx-0.0.8/src/gdpx/selector/property.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1987 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/selector/random.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      955 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/selector/scf.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    10041 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/selector/selector.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.307156 gdpx-0.0.8/src/gdpx/trainer/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1050 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/trainer/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6277 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/trainer/interface.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.314156 gdpx-0.0.8/src/gdpx/utils/
--rw-r--r--   0 jx1279   (353055) chem     (30004)       83 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/utils/__init__.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7894 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/utils/atomUtils.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2908 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/utils/cleave_cluster.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1247 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/utils/cmdrun.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6500 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/utils/cmp_refdat.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6476 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/utils/command.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    12328 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/utils/comparision.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.354157 gdpx-0.0.8/src/gdpx/utils/dputils/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9418 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/utils/dputils/DeepPot.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    14661 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/utils/dputils/acquire_dmat.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1095 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/utils/geometry.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2147 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/utils/plot_dimer.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7761 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/utils/reduce_dataset.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6200 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/utils/second_reduce.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     5412 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/utils/split-dataset.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2444 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/utils/strucopy.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.364157 gdpx-0.0.8/src/gdpx/validator/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1945 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/validator/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5610 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/validator/diffusion_coefficient.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4095 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/validator/dimer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2640 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/validator/eos.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4779 2024-03-02 03:59:21.000000 gdpx-0.0.8/src/gdpx/validator/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5879 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/validator/mdf.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7477 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/validator/melting_point.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5744 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/validator/minima.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      583 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/validator/rank.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9391 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/validator/rdf.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3436 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/validator/rxn.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8794 2024-04-07 20:49:18.000000 gdpx-0.0.8/src/gdpx/validator/spc.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3690 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/validator/surface_energy.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2029 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/validator/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      980 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/validator/validator.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.369157 gdpx-0.0.8/src/gdpx/worker/
--rw-r--r--   0 jx1279   (353055) chem     (30004)       84 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/worker/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    32598 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/worker/drive.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6935 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/worker/explore.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7188 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/worker/grid.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11187 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/worker/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    18256 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/worker/react.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12736 2024-04-21 01:03:27.000000 gdpx-0.0.8/src/gdpx/worker/single.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11940 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/worker/train.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1958 2023-12-01 19:22:44.000000 gdpx-0.0.8/src/gdpx/worker/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6077 2024-03-17 21:29:30.000000 gdpx-0.0.8/src/gdpx/worker/worker.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-21 01:05:46.369157 gdpx-0.0.8/src/gdpx.egg-info/
--rw-r--r--   0 jx1279   (353055) chem     (30004)    47632 2024-04-21 01:05:45.000000 gdpx-0.0.8/src/gdpx.egg-info/PKG-INFO
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8681 2024-04-21 01:05:45.000000 gdpx-0.0.8/src/gdpx.egg-info/SOURCES.txt
--rw-r--r--   0 jx1279   (353055) chem     (30004)        1 2024-04-21 01:05:45.000000 gdpx-0.0.8/src/gdpx.egg-info/dependency_links.txt
--rw-r--r--   0 jx1279   (353055) chem     (30004)       39 2024-04-21 01:05:45.000000 gdpx-0.0.8/src/gdpx.egg-info/entry_points.txt
--rw-r--r--   0 jx1279   (353055) chem     (30004)       95 2024-04-21 01:05:45.000000 gdpx-0.0.8/src/gdpx.egg-info/requires.txt
--rw-r--r--   0 jx1279   (353055) chem     (30004)        5 2024-04-21 01:05:45.000000 gdpx-0.0.8/src/gdpx.egg-info/top_level.txt
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.117353 gdpx-0.0.9/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    35149 2023-04-10 18:29:40.000000 gdpx-0.0.9/LICENSE
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    47632 2024-04-30 02:48:50.117353 gdpx-0.0.9/PKG-INFO
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6294 2023-12-12 17:08:13.000000 gdpx-0.0.9/README.md
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      878 2024-04-30 02:48:26.000000 gdpx-0.0.9/pyproject.toml
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       38 2024-04-30 02:48:50.117353 gdpx-0.0.9/setup.cfg
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.647347 gdpx-0.0.9/src/
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.658347 gdpx-0.0.9/src/gdpx/
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.663348 gdpx-0.0.9/src/gdpx/bias/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1373 2024-04-30 02:46:58.000000 gdpx-0.0.9/src/gdpx/bias/__init__.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.664348 gdpx-0.0.9/src/gdpx/bias/afir/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      119 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/bias/afir/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4620 2024-04-30 02:46:58.000000 gdpx-0.0.9/src/gdpx/bias/afir/afir.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1679 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/bias/bias.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7641 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/bias/bondboost.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.667348 gdpx-0.0.9/src/gdpx/bias/gaussian/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      309 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/bias/gaussian/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9777 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/bias/gaussian/bond.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5649 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/bias/gaussian/com.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3047 2024-04-30 02:47:37.000000 gdpx-0.0.9/src/gdpx/bias/gaussian/gaussian.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5429 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/bias/gaussian/rmsd.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.669348 gdpx-0.0.9/src/gdpx/bias/harmonic/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      248 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/bias/harmonic/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4478 2024-04-30 02:46:58.000000 gdpx-0.0.9/src/gdpx/bias/harmonic/distance.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2740 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/bias/harmonic/harmonic.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2192 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/bias/harmonic/plane.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3270 2024-04-30 02:46:58.000000 gdpx-0.0.9/src/gdpx/bias/nuclei.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1473 2024-04-30 02:46:58.000000 gdpx-0.0.9/src/gdpx/bias/timeio.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.670348 gdpx-0.0.9/src/gdpx/bias/utils/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      262 2024-04-30 02:46:58.000000 gdpx-0.0.9/src/gdpx/bias/utils/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4070 2024-04-30 02:46:58.000000 gdpx-0.0.9/src/gdpx/bias/utils/bondpair.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.679348 gdpx-0.0.9/src/gdpx/builder/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3154 2024-04-30 02:46:58.000000 gdpx-0.0.9/src/gdpx/builder/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3100 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/builder/builder.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      800 2024-04-26 06:39:22.000000 gdpx-0.0.9/src/gdpx/builder/cleave_group.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2659 2023-12-03 04:22:10.000000 gdpx-0.0.9/src/gdpx/builder/cleave_surface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5743 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/builder/constraints.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      384 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/builder/crossover.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1581 2024-04-30 02:46:58.000000 gdpx-0.0.9/src/gdpx/builder/dimer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7769 2024-04-30 02:46:58.000000 gdpx-0.0.9/src/gdpx/builder/direct.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.693348 gdpx-0.0.9/src/gdpx/builder/graph/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      287 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/builder/graph/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5942 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/builder/graph/exchange.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5089 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/builder/graph/insert.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5355 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/builder/graph/modifier.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5664 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/builder/graph/remove.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5373 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/builder/group.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8530 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/builder/insert.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8546 2024-04-30 02:46:58.000000 gdpx-0.0.9/src/gdpx/builder/interface.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.694348 gdpx-0.0.9/src/gdpx/builder/mutation/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      892 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/builder/mutation/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5565 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/builder/packer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3406 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/builder/perturbator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    15179 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/builder/randomBuilder.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    19280 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/builder/region.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      745 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/builder/repeat.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.696348 gdpx-0.0.9/src/gdpx/builder/scan/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2863 2024-04-30 02:46:58.000000 gdpx-0.0.9/src/gdpx/builder/scan/angle.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7274 2024-04-30 02:46:58.000000 gdpx-0.0.9/src/gdpx/builder/scan/hypercube.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1189 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/builder/scan/intercoord.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3614 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/builder/species.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7762 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/builder/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1672 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/builder/wulff.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1391 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/builder/zoom.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.697348 gdpx-0.0.9/src/gdpx/cli/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      669 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/cli/build.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6550 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/cli/compute.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1739 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/cli/explore.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.740349 gdpx-0.0.9/src/gdpx/colvar/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      463 2024-04-30 02:47:37.000000 gdpx-0.0.9/src/gdpx/colvar/__init__.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2622 2024-04-26 06:39:22.000000 gdpx-0.0.9/src/gdpx/colvar/compute_reweight.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1554 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/colvar/coordination.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      636 2024-04-30 02:47:37.000000 gdpx-0.0.9/src/gdpx/colvar/distance.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3567 2024-04-26 06:39:22.000000 gdpx-0.0.9/src/gdpx/colvar/fingerprint.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     5096 2024-04-26 06:39:22.000000 gdpx-0.0.9/src/gdpx/colvar/plot_meta.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5603 2024-04-26 06:39:22.000000 gdpx-0.0.9/src/gdpx/colvar/plot_string.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4637 2024-04-26 06:39:22.000000 gdpx-0.0.9/src/gdpx/colvar/plotstring.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      178 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/colvar/position.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2749 2024-04-26 06:39:22.000000 gdpx-0.0.9/src/gdpx/colvar/reweight.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1461 2024-04-26 06:39:22.000000 gdpx-0.0.9/src/gdpx/colvar/rmsd.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.744349 gdpx-0.0.9/src/gdpx/comparator/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      954 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/comparator/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2739 2023-12-06 01:21:35.000000 gdpx-0.0.9/src/gdpx/comparator/cartesian.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      827 2024-01-23 21:20:47.000000 gdpx-0.0.9/src/gdpx/comparator/comparator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5645 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/comparator/coordination.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4595 2023-12-06 01:21:35.000000 gdpx-0.0.9/src/gdpx/comparator/graph.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1193 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/comparator/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3067 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/comparator/reaction.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5123 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/comparator/singlepoint.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.849350 gdpx-0.0.9/src/gdpx/computation/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      657 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/computation/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    30744 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/computation/asedriver.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    21677 2024-04-21 01:03:27.000000 gdpx-0.0.9/src/gdpx/computation/cp2k.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    21683 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/computation/driver.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8651 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/computation/espresso.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    20073 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/computation/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    37804 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/computation/lammps.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    22229 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/computation/lasp.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.849350 gdpx-0.0.9/src/gdpx/computation/mc/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4259 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/computation/mc/tfmc.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.850350 gdpx-0.0.9/src/gdpx/computation/md/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1082 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/computation/md/md_utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5296 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/computation/md/nosehoover.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6166 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/computation/observer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2372 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/computation/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    20268 2024-04-25 21:47:58.000000 gdpx-0.0.9/src/gdpx/computation/vasp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1463 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/config.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.853350 gdpx-0.0.9/src/gdpx/core/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      108 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/core/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2415 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/core/node.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2492 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/core/operation.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      861 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/core/placeholder.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7122 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/core/register.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.856350 gdpx-0.0.9/src/gdpx/core/session/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      148 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/core/session/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    12927 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/core/session/active.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2007 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/core/session/basic.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7922 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/core/session/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2686 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/core/session/session.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1998 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/core/session/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1461 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/core/variable.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.864350 gdpx-0.0.9/src/gdpx/data/
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6210 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/data/ClusterAndCUR.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      249 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/data/__init__.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    57236 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/data/analyser.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    14976 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/data/array.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7981 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/data/cleave_deviation.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1901 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/data/convert.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3103 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/data/correction.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9171 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/data/database.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11961 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/data/dataset.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1552 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/data/extatoms.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3389 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/data/extract_evolution.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    14345 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/data/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    10543 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/data/operators.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1950 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/data/system.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1210 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/data/utils.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.867350 gdpx-0.0.9/src/gdpx/describer/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      441 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/describer/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2325 2024-02-09 18:38:45.000000 gdpx-0.0.9/src/gdpx/describer/describer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2066 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/describer/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2365 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/describer/soap.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2438 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/describer/spc.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.886350 gdpx-0.0.9/src/gdpx/expedition/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1344 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/expedition/__init__.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.886350 gdpx-0.0.9/src/gdpx/expedition/accelerated_dynamics/
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    16224 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/expedition/accelerated_dynamics/prev_example.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.887350 gdpx-0.0.9/src/gdpx/expedition/artificial_force/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11656 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/expedition/artificial_force/afir.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2349 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/expedition/expedition.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.888350 gdpx-0.0.9/src/gdpx/expedition/ga/
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    25876 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/expedition/ga/engine.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    18347 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/expedition/ga/population.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3742 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/expedition/interface.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.890350 gdpx-0.0.9/src/gdpx/expedition/monte_carlo/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      149 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/expedition/monte_carlo/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      802 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/expedition/monte_carlo/basin_hopping.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    20408 2024-04-21 01:03:27.000000 gdpx-0.0.9/src/gdpx/expedition/monte_carlo/monte_carlo.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.893350 gdpx-0.0.9/src/gdpx/expedition/monte_carlo/operators/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2356 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/expedition/monte_carlo/operators/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9188 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/expedition/monte_carlo/operators/exchange.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5008 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/expedition/monte_carlo/operators/move.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8411 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/expedition/monte_carlo/operators/operator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11096 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/expedition/monte_carlo/operators/react.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4394 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/expedition/monte_carlo/operators/swap.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.894350 gdpx-0.0.9/src/gdpx/expedition/simulated_annealing/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5956 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/expedition/simulated_annealing/simulated_annealing.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.899351 gdpx-0.0.9/src/gdpx/graph/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      147 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/graph/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    13870 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/graph/comparison.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    12839 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/graph/creator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    12200 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/graph/graph_main.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5431 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/graph/molecule.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    31066 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/graph/sites.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2905 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/graph/surface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1849 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/graph/utils.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     9536 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/main.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2242 2024-04-26 06:39:22.000000 gdpx-0.0.9/src/gdpx/nanoparticle.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.902351 gdpx-0.0.9/src/gdpx/potential/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      274 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/potential/__init__.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.903350 gdpx-0.0.9/src/gdpx/potential/calculators/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      654 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/potential/calculators/dummy.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4675 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/potential/calculators/mixer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1256 2024-04-23 06:22:16.000000 gdpx-0.0.9/src/gdpx/potential/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6073 2024-04-21 01:03:27.000000 gdpx-0.0.9/src/gdpx/potential/manager.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.912351 gdpx-0.0.9/src/gdpx/potential/managers/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3069 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/potential/managers/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1430 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/potential/managers/asepot.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2787 2024-04-21 01:03:27.000000 gdpx-0.0.9/src/gdpx/potential/managers/bias.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2947 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/cp2k.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.914351 gdpx-0.0.9/src/gdpx/potential/managers/deepmd/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      225 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/potential/managers/deepmd/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7170 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/potential/managers/deepmd/calculator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4058 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/potential/managers/deepmd/convert.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    23429 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/potential/managers/deepmd/deepmd.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1141 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/potential/managers/dftd3.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2231 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/eam.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1117 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/emt.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2363 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/espresso.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.917351 gdpx-0.0.9/src/gdpx/potential/managers/gp/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       83 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/gp/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2348 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/gp/bench.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1376 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/gp/fgp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3746 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/gp/gptools.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3474 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/gp/representation.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    46869 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/gp/sgp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2715 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/potential/managers/grid.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1986 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/lasp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    17115 2024-04-21 01:03:27.000000 gdpx-0.0.9/src/gdpx/potential/managers/mace.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4925 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/potential/managers/mixer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7976 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/potential/managers/nequip.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:49.990352 gdpx-0.0.9/src/gdpx/potential/managers/plumed/
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.013352 gdpx-0.0.9/src/gdpx/potential/managers/plumed/calculators/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2728 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/potential/managers/plumed/calculators/plumed.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9361 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/potential/managers/plumed/calculators/plumed2.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2394 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/potential/managers/plumed/plumed.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.014352 gdpx-0.0.9/src/gdpx/potential/managers/reann/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7421 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/potential/managers/reann/beann.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.015352 gdpx-0.0.9/src/gdpx/potential/managers/reann/calculators/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3496 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/potential/managers/reann/calculators/reann.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    17636 2024-04-21 01:03:27.000000 gdpx-0.0.9/src/gdpx/potential/managers/reann/reann.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1396 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/reax.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8903 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/schnet.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3654 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/vasp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1207 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/potential/managers/xtb.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5499 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/potential/trainer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1739 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/potential/utils.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.017352 gdpx-0.0.9/src/gdpx/reactor/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      860 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/reactor/__init__.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.022352 gdpx-0.0.9/src/gdpx/reactor/future/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    23672 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/reactor/future/AccCons.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2601 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/reactor/future/AccNEB.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2921 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/reactor/future/cmp_mep.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3833 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/reactor/future/constrain.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7051 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/reactor/future/crs.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2226 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/reactor/future/diffusion3.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    11410 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/reactor/future/find_adsorption.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3188 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/reactor/future/find_inter.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3002 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/reactor/future/muller-brown.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     1154 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/reactor/future/test_mh.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4115 2024-04-21 01:03:27.000000 gdpx-0.0.9/src/gdpx/reactor/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1482 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/reactor/reactor.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.025352 gdpx-0.0.9/src/gdpx/reactor/string/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      232 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/reactor/string/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    17830 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/reactor/string/cp2k.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5117 2024-03-17 21:29:29.000000 gdpx-0.0.9/src/gdpx/reactor/string/grid.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    10477 2024-04-21 01:03:27.000000 gdpx-0.0.9/src/gdpx/reactor/string/pathway.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11906 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/reactor/string/string.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9158 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/reactor/string/vasp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2320 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/reactor/utils.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.028352 gdpx-0.0.9/src/gdpx/scheduler/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      699 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/scheduler/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      624 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/scheduler/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      631 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/scheduler/local.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3553 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/scheduler/lsf.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1147 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/scheduler/pbs.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4439 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/scheduler/scheduler.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3226 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/scheduler/slurm.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.069352 gdpx-0.0.9/src/gdpx/selector/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1078 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/selector/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3664 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/selector/basin.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6276 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/selector/compare.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1376 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/selector/composition.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8362 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/selector/cur.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7241 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/selector/descriptor.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5631 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/selector/graph.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6398 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/selector/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2905 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/selector/interval.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      622 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/selector/invariant.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3284 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/selector/locate.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    14855 2024-04-20 02:06:51.000000 gdpx-0.0.9/src/gdpx/selector/property.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1987 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/selector/random.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      955 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/selector/scf.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    10041 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/selector/selector.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.071353 gdpx-0.0.9/src/gdpx/trainer/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1050 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/trainer/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6277 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/trainer/interface.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.092353 gdpx-0.0.9/src/gdpx/utils/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       83 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/utils/__init__.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7894 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/utils/atomUtils.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2908 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/utils/cleave_cluster.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1247 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/utils/cmdrun.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6500 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/utils/cmp_refdat.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6476 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/utils/command.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    12328 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/utils/comparision.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.093353 gdpx-0.0.9/src/gdpx/utils/dputils/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9418 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/utils/dputils/DeepPot.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    14661 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/utils/dputils/acquire_dmat.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1095 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/utils/geometry.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2147 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/utils/plot_dimer.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7761 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/utils/reduce_dataset.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6200 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/utils/second_reduce.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     5412 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/utils/split-dataset.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1891 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/utils/strconv.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2444 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/utils/strucopy.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.102353 gdpx-0.0.9/src/gdpx/validator/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2039 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/validator/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5610 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/validator/diffusion_coefficient.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4200 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/validator/dimer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2640 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/validator/eos.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4779 2024-03-02 03:59:21.000000 gdpx-0.0.9/src/gdpx/validator/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5879 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/validator/mdf.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7477 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/validator/melting_point.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5744 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/validator/minima.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      583 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/validator/rank.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9391 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/validator/rdf.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3436 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/validator/rxn.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8794 2024-04-07 20:49:18.000000 gdpx-0.0.9/src/gdpx/validator/spc.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3690 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/validator/surface_energy.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4396 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/validator/trimer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2029 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/validator/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      980 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/validator/validator.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.108353 gdpx-0.0.9/src/gdpx/worker/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       84 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/worker/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    32598 2024-04-22 03:53:10.000000 gdpx-0.0.9/src/gdpx/worker/drive.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7047 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/worker/explore.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    14319 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/worker/grid.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9743 2024-04-30 02:46:59.000000 gdpx-0.0.9/src/gdpx/worker/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    18256 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/worker/react.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    12736 2024-04-21 01:03:27.000000 gdpx-0.0.9/src/gdpx/worker/single.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11940 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/worker/train.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1958 2023-12-01 19:22:44.000000 gdpx-0.0.9/src/gdpx/worker/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6077 2024-03-17 21:29:30.000000 gdpx-0.0.9/src/gdpx/worker/worker.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-30 02:48:50.116353 gdpx-0.0.9/src/gdpx.egg-info/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    47632 2024-04-30 02:48:49.000000 gdpx-0.0.9/src/gdpx.egg-info/PKG-INFO
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8925 2024-04-30 02:48:49.000000 gdpx-0.0.9/src/gdpx.egg-info/SOURCES.txt
+-rw-r--r--   0 jx1279   (353055) chem     (30004)        1 2024-04-30 02:48:49.000000 gdpx-0.0.9/src/gdpx.egg-info/dependency_links.txt
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       39 2024-04-30 02:48:49.000000 gdpx-0.0.9/src/gdpx.egg-info/entry_points.txt
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       95 2024-04-30 02:48:49.000000 gdpx-0.0.9/src/gdpx.egg-info/requires.txt
+-rw-r--r--   0 jx1279   (353055) chem     (30004)        5 2024-04-30 02:48:49.000000 gdpx-0.0.9/src/gdpx.egg-info/top_level.txt
```

### Comparing `gdpx-0.0.8/LICENSE` & `gdpx-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/PKG-INFO` & `gdpx-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdpx
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automate computational chemistry/materials sciance and machine learning interatomic potential training workflow.
 Author-email: Jiayan Xu <ahcigar@foxmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdpx-0.0.8/README.md` & `gdpx-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/pyproject.toml` & `gdpx-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdpx"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
   "ase>=3.22",
   "h5py>=3.7.0",
   "joblib>=1.1.0",
   "networkx>=2.6.3",
   "omegaconf>=2.3.0",
   "pyyaml>=6.0",
```

### Comparing `gdpx-0.0.8/src/gdpx/bias/__init__.py` & `gdpx-0.0.9/src/gdpx/bias/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 
 from ..core.register import registers
 
+from ..utils.strconv import str2array
+
 """Add bias on potential energy surface. 
 
 Some of bias forces are based on JAX. In the future, we need replace those oft-used
 ones to pure python codes as jax need accelerate them a lot.
 
 """
 
 from .afir import AFIRCalculator
 registers.bias.register("afir")(AFIRCalculator)
 
 from .bondboost import BondBoostCalculator
 registers.bias.register("bondboost")(BondBoostCalculator)
 
+from .nuclei import NucleiRepulsionCalculator
+registers.bias.register("nuclei_repulsion")(NucleiRepulsionCalculator)
+
 # from .harmonic import HarmonicBias
 # bias_register.register("harmonic")(HarmonicBias)
 
 from .harmonic import DistanceHarmonicCalculator, PlaneHarmonicCalculator
 registers.bias.register("distance_harmonic")(DistanceHarmonicCalculator)
 registers.bias.register("plane_harmonic")(PlaneHarmonicCalculator)
```

### Comparing `gdpx-0.0.8/src/gdpx/bias/afir/afir.py` & `gdpx-0.0.9/src/gdpx/bias/afir/afir.py`

 * *Files 11% similar despite different names*

```diff
@@ -85,28 +85,30 @@
 
 class AFIRCalculator(Calculator):
 
     implemented_properties = ["energy", "free_energy", "forces"]
 
     default_parameters = dict(gamma=2.5, power=6, cutoff=6.0)
 
-    def __init__(self, groups, restart=None, label=None, atoms=None, directory=".", **kwargs):
+    def __init__(self, groups, use_pbc: bool=False, restart=None, label=None, atoms=None, directory=".", **kwargs):
         """"""
         super().__init__(
             restart=restart, label=label, atoms=atoms, directory=directory, **kwargs
         )
 
         self.gamma = self.parameters["gamma"]  # eV
         assert self.gamma > 0.
 
         self.radius = self.parameters.get("radius", R0_AFIR)
         self.epsilon = self.parameters.get("epsilon", EPS_AFIR)
         self.power = int(self.parameters.get("power", POW_AFIR))
 
         self.groups = groups
+
+        self.use_pbc = use_pbc
         self.cutoff = self.parameters["cutoff"]
 
         assert len(self.groups) == 2
 
         # ---
         self.neighlist = None
 
@@ -118,34 +120,33 @@
         properties=["energy"],
         system_changes=["positions", "numbers", "cell"],
     ):
         """"""
         super().calculate(atoms, properties, system_changes)
 
         # NOTE: check cutoff before assigning groups
-        if self.neighlist is None:
-            self.neighlist = NeighborList(
-                [self.cutoff/2.]*len(atoms),
-                skin=0.0, self_interaction=False, bothways=True
-            )
-        self.neighlist.update(atoms)
+        if self.use_pbc:
+            if self.neighlist is None:
+                self.neighlist = NeighborList(
+                    [self.cutoff/2.]*len(atoms),
+                    skin=0.0, self_interaction=False, bothways=True
+                )
+            self.neighlist.update(atoms)
+        else:
+            self.neighlist = None
 
         # - get constants
         atomic_numbers = atoms.get_atomic_numbers()
         atomic_radii = np.array([covalent_radii[i] for i in atomic_numbers])
 
         # - find bond pairs
         bond_pairs, bond_distances, bond_shifts = compute_distance_and_shift(
-            atoms, self.neighlist, self.groups[0], self.groups[1]
+            atoms, self.groups[0], self.groups[1], neighlist=self.neighlist
         )
 
-        # print(f"{bond_pairs =}")
-        # print(f"{bond_distances =}")
-        # print(f"{bond_shifts =}")
-
         # - compute properties
         energy, forces = compute_afir_energy_and_forces(
             atoms.positions,
             bond_distances,
             atomic_radii,
             bond_pairs,
             bond_shifts,
```

### Comparing `gdpx-0.0.8/src/gdpx/bias/bias.py` & `gdpx-0.0.9/src/gdpx/bias/bias.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/bias/bondboost.py` & `gdpx-0.0.9/src/gdpx/bias/bondboost.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/bias/gaussian/bond.py` & `gdpx-0.0.9/src/gdpx/bias/gaussian/bond.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/bias/gaussian/com.py` & `gdpx-0.0.9/src/gdpx/bias/gaussian/com.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/bias/gaussian/gaussian.py` & `gdpx-0.0.9/src/gdpx/bias/gaussian/gaussian.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/bias/gaussian/rmsd.py` & `gdpx-0.0.9/src/gdpx/bias/gaussian/rmsd.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/bias/harmonic/distance.py` & `gdpx-0.0.9/src/gdpx/bias/harmonic/distance.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 
 import copy
-from typing import Optional, Tuple, List
+from typing import List, Optional, Tuple
 
 import numpy as np
-
 from ase import Atoms
 from ase.calculators.calculator import Calculator
 from ase.geometry import find_mic
 
+from .. import str2array
 from ..timeio import TimeIOCalculator
 
 
 def compute_distance(cell, positions, pbc: bool = True):
     """"""
     # compute colvar
     assert positions.shape[0] == 2
@@ -24,19 +24,20 @@
 
 
 def compute_distance_harmonic_energy_and_forces(
     vec, dis: float, center: float, kspring: float
 ):
     """"""
     # compute energy
-    energy = np.sum(0.5 * kspring * (dis - center) ** 2)
+    dx = dis - center
+    energy = 0.5 * kspring * dx**2
 
     # compute forces
     forces = np.zeros((2, 3))
-    frc_i = -kspring * vec / dis
+    frc_i = -kspring * dx * vec / dis
     forces[0] += frc_i
     forces[1] += -frc_i
 
     return energy, forces
 
 
 class DistanceHarmonicCalculator(TimeIOCalculator):
@@ -50,28 +51,35 @@
         super().__init__(*args, **kwargs)
 
         num_group_atoms = len(group)
         assert num_group_atoms == 2
         self.group = group
 
         self.center = center
+        assert isinstance(self.center, float)
 
         self.kspring = kspring
+        assert isinstance(self.kspring, float)
 
         return
 
     def _icalculate(self, atoms, properties, system_changes) -> Tuple[dict, list]:
         """"""
         vec, dis = compute_distance(atoms.cell, atoms.positions[self.group], pbc=True)
 
-        energy, ext_forces = compute_distance_harmonic_energy_and_forces(
-            vec, dis, self.center, self.kspring
-        )
+        energy = 0.0
         forces = np.zeros(atoms.positions.shape)
-        forces[self.group] = ext_forces
+        if self.num_steps >= self.delay:
+            energy, ext_forces = compute_distance_harmonic_energy_and_forces(
+                vec, dis, self.center, self.kspring
+            )
+            forces = np.zeros(atoms.positions.shape)
+            forces[self.group] = ext_forces
+        else:
+            ...
 
         results = {}
         results["energy"] = energy
         results["free_energy"] = energy
         results["forces"] = forces
 
         step_info = (self.num_steps, dis, energy)
@@ -82,15 +90,15 @@
         """"""
         content = f"# {self.pace =} {self.group =} {self.center =} {self.kspring =}\n"
         content += "# {:>10s}  {:>12s}  {:>12s}\n".format("step", "distance", "energy")
         with open(self.log_fpath, "w") as fopen:
             fopen.write(content)
 
         return
-    
+
     def _write_step(self):
         """"""
         content = "{:>12d}  {:>12.4f}  {:>12.4f}\n".format(*self.step_info)
         with open(self.log_fpath, "a") as fopen:
             fopen.write(content)
 
         return
@@ -98,19 +106,27 @@
     @staticmethod
     def broadcast_params(inp_dict: dict) -> List[dict]:
         """"""
         # broadcast center or kspring
         centers = inp_dict.get("center", [])
         if isinstance(centers, float):
             centers = [centers]
+        elif isinstance(centers, str):
+            centers = str2array(centers)
+        else:
+            raise TypeError(f"{centers =}")
         num_centers = len(centers)
 
         ksprings = inp_dict.get("kspring", [])
         if isinstance(ksprings, float):
             ksprings = [ksprings]
+        elif isinstance(ksprings, str):
+            ksprings = str2array(ksprings)
+        else:
+            raise TypeError(f"{ksprings =}")
         num_ksprings = len(ksprings)
 
         new_inputs = []
         if num_centers == 1 and num_ksprings == 1:
             new_inputs = [inp_dict]
         elif num_centers == 1 and num_ksprings > 1:
             new_inputs = [copy.deepcopy(inp_dict) for _ in range(num_ksprings)]
@@ -120,15 +136,15 @@
             new_inputs = [copy.deepcopy(inp_dict) for _ in range(num_centers)]
             for i, x in enumerate(new_inputs):
                 x["center"] = centers[i]
         else:
             raise RuntimeError("Broadcast cannot.")
 
         return new_inputs
-    
+
     @staticmethod
     def broadcast(inp_dict: dict) -> List["DistanceHarmonicCalculator"]:
         """Create a list of calculators based on input parameters."""
 
         new_inputs = DistanceHarmonicCalculator.broadcast_params(inp_dict)
         calcs = [DistanceHarmonicCalculator(**x) for x in new_inputs]
```

### Comparing `gdpx-0.0.8/src/gdpx/bias/harmonic/harmonic.py` & `gdpx-0.0.9/src/gdpx/bias/harmonic/harmonic.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/bias/harmonic/plane.py` & `gdpx-0.0.9/src/gdpx/bias/harmonic/plane.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/bias/timeio.py` & `gdpx-0.0.9/src/gdpx/bias/timeio.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 import pathlib
 
 from ase.calculators.calculator import Calculator
 
 
 class TimeIOCalculator(Calculator):
 
-    def __init__(self, pace: int=1, *args, **kwargs):
+    def __init__(self, pace: int = 1, delay: int = 0, *args, **kwargs):
         """"""
         super().__init__(*args, **kwargs)
 
         self.pace = pace
 
+        self.delay = delay
+
         self._num_steps = 0
 
         return
 
     @property
     def num_steps(self) -> int:
         """Finished steps that match the host driver e.g. MD."""
@@ -38,15 +40,17 @@
         system_changes=["positions", "numbers", "cell"],
     ):
         super().calculate(atoms, properties, system_changes)
 
         if self.num_steps == 0:
             self._write_first_step()
 
-        self.results, self.step_info = self._icalculate(atoms, properties, system_changes)
+        self.results, self.step_info = self._icalculate(
+            atoms, properties, system_changes
+        )
 
         if self.num_steps % self.pace == 0:
             self._write_step()
 
         self._num_steps += 1
 
         return
@@ -62,9 +66,10 @@
         raise NotImplementedError()
 
     def _write_step(self):
         """"""
 
         raise NotImplementedError()
 
+
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.8/src/gdpx/builder/__init__.py` & `gdpx-0.0.9/src/gdpx/builder/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 
 import warnings
 
 from .. import config
 from ..utils.command import CustomTimer
+from ..utils.strconv import str2array
 
 from .interface import create_builder
 
 from ..core.register import registers
 from .direct import DirectBuilder, ReadBuilder
 from .species import MoleculeBuilder
 from .dimer import DimerBuilder
@@ -33,14 +34,17 @@
 
 # - basic builders and modifiers
 registers.builder.register("direct")(DirectBuilder)
 registers.builder.register("reader")(ReadBuilder)
 registers.builder.register("dimer")(DimerBuilder)
 registers.builder.register("molecule")(MoleculeBuilder)
 
+from .wulff import WulffConstructionBuilder
+registers.builder.register("wulff_construction")(WulffConstructionBuilder)
+
 from .perturbator import PerturbatorBuilder
 registers.builder.register("perturb")(PerturbatorBuilder)
 
 from .packer import PackerBuilder
 registers.builder.register("pack")(PackerBuilder)
 
 from .insert import InsertModifier
@@ -72,15 +76,17 @@
 # - extra modifiers
 from .zoom import ZoomModifier
 registers.builder.register("zoom")(ZoomModifier)
 
 
 # - optional
 try:
-    from .hypercube import HypercubeBuilder
+    from .scan.angle import ScanAngleModifier
+    registers.builder.register("scan_angle")(ScanAngleModifier)
+    from .scan.hypercube import HypercubeBuilder
     registers.builder.register("hypercube")(HypercubeBuilder)
 except ImportError as e:
     warnings.warn("Module {} import failed: {}".format("hypercube", e), UserWarning)
 
 # - extra utilities
 from .utils import remove_vacuum, reset_cell
 registers.operation.register(remove_vacuum)
```

### Comparing `gdpx-0.0.8/src/gdpx/builder/builder.py` & `gdpx-0.0.9/src/gdpx/builder/builder.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/cleave_group.py` & `gdpx-0.0.9/src/gdpx/builder/cleave_group.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/cleave_surface.py` & `gdpx-0.0.9/src/gdpx/builder/cleave_surface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/constraints.py` & `gdpx-0.0.9/src/gdpx/builder/constraints.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/dimer.py` & `gdpx-0.0.9/src/gdpx/builder/dimer.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,44 +10,53 @@
 from ase.constraints import FixAtoms
 
 from .builder import StructureBuilder
 
 
 class DimerBuilder(StructureBuilder):
 
-    def __init__(self, elements: List[str], distances: List[float]=[0.8,2.5,0.05], directory=Path.cwd(), *args, **kwargs):
+    def __init__(
+        self,
+        elements: List[str],
+        distances: List[float] = [0.8, 2.5, 0.05],
+        directory=Path.cwd(),
+        *args,
+        **kwargs,
+    ):
         """"""
         super().__init__(directory, *args, **kwargs)
 
         self.elements = elements
-        assert len(self.elements) == 2, "DimerBuilder needs two chemical symbols as elements."
+        assert (
+            len(self.elements) == 2
+        ), "DimerBuilder needs two chemical symbols as elements."
 
         self.distances = distances
-        assert len(self.distances) == 3, "DimerBuilder needs min, max and intv for the distance."
+        assert (
+            len(self.distances) == 3
+        ), "DimerBuilder needs min, max and intv for the distance."
 
         return
 
     def run(self, *args, **kwargs) -> List[Atoms]:
         """"""
         super().run(*args, **kwargs)
 
         dmin, dmax, intv = self.distances
-        distances = np.arange(dmin, dmax+intv, intv)
+        distances = np.arange(dmin, dmax + intv, intv)
+        self._print(f"{distances}")
 
         frames = []
         for dis in distances:
             atoms = Atoms(
-                symbols=self.elements, 
-                positions=[
-                    [0., 0., 0.],
-                    [0., 0., dis]
-                ],
-                #cell = 20.*np.eye(3),
-                cell = [[19., 0., 0.], [0., 20., 0.], [0., 0., 21.]],
-                pbc=[True,True,True]
+                symbols=self.elements,
+                positions=[[10.0, 10.0, 10.0], [10.0, 10.0, 10.0+dis]],
+                # cell = 20.*np.eye(3),
+                cell=[[19.0, 0.0, 0.0], [0.0, 20.0, 0.0], [0.0, 0.0, 21.0]],
+                pbc=[True, True, True],
             )
             atoms.set_constraint(FixAtoms(indices=[0]))
             frames.append(atoms)
 
         return frames
```

### Comparing `gdpx-0.0.8/src/gdpx/builder/direct.py` & `gdpx-0.0.9/src/gdpx/builder/direct.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 
 from ase import Atoms
 from ase.io import read, write
 from ase.constraints import FixAtoms
 
 from .builder import StructureBuilder
 
+
 def read_xsd2(fd) -> Atoms:
     """read xsd file by Material Studio
 
     NOTE:
         support reading constraints...
 
     """
     import xml.etree.ElementTree as ET
-    from xml.dom import minidom 
+    from xml.dom import minidom
 
     tree = ET.parse(fd)
     root = tree.getroot()
 
     atomtreeroot = root.find("AtomisticTreeRoot")
     # if periodic system
     if atomtreeroot.find("SymmetrySystem") is not None:
@@ -32,63 +33,65 @@
         system = mappingfamily.find("IdentityMapping")
 
         coords = list()
         cell = list()
         formula = str()
 
         names = list()
-        restrictions = list() 
+        restrictions = list()
 
         for atom in system:
             if atom.tag == "Atom3d":
                 symbol = atom.get("Components")
                 formula += symbol
 
                 xyz = atom.get("XYZ")
                 if xyz:
                     coord = [float(coord) for coord in xyz.split(",")]
                 else:
                     coord = [0.0, 0.0, 0.0]
                 coords.append(coord)
 
-                name = atom.get("Name") 
+                name = atom.get("Name")
                 if name:
-                    pass # find name 
-                else: 
-                    name = symbol + str(len(names)+1) # None due to copy atom 
+                    pass  # find name
+                else:
+                    name = symbol + str(len(names) + 1)  # None due to copy atom
                 names.append(name)
 
                 restriction = atom.get("RestrictedProperties", None)
                 if restriction:
-                    if restriction.startswith("FractionalXYZ"):  # TODO: may have 1-3 flags
+                    if restriction.startswith(
+                        "FractionalXYZ"
+                    ):  # TODO: may have 1-3 flags
                         restrictions.append(True)
-                    else: 
+                    else:
                         raise ValueError("unknown RestrictedProperties")
-                else: 
+                else:
                     restrictions.append(False)
             elif atom.tag == "SpaceGroup":
-                avec = [float(vec) for vec in atom.get('AVector').split(',')]
-                bvec = [float(vec) for vec in atom.get('BVector').split(',')]
-                cvec = [float(vec) for vec in atom.get('CVector').split(',')]
+                avec = [float(vec) for vec in atom.get("AVector").split(",")]
+                bvec = [float(vec) for vec in atom.get("BVector").split(",")]
+                cvec = [float(vec) for vec in atom.get("CVector").split(",")]
 
                 cell.append(avec)
                 cell.append(bvec)
                 cell.append(cvec)
 
         atoms = Atoms(formula, cell=cell, pbc=True)
         atoms.set_scaled_positions(coords)
 
-        # add constraints 
+        # add constraints
         fixed_indices = [idx for idx, val in enumerate(restrictions) if val]
         if fixed_indices:
             atoms.set_constraint(FixAtoms(indices=fixed_indices))
 
-        # add two atoms constrained optimisation 
+        # add two atoms constrained optimisation
         constrained_indices = [
-            idx for idx, name in enumerate(names) if name.endswith('_c') 
+            idx for idx, name in enumerate(names) if name.endswith("_c")
         ]
         if constrained_indices:
             assert len(constrained_indices) == 2
             atoms.info["copt"] = constrained_indices
 
         return atoms
         # if non-periodic system
@@ -107,115 +110,135 @@
                 coord = [float(coord) for coord in xyz.split(",")]
                 coords.append(coord)
 
         atoms = Atoms(formula, pbc=False)
         atoms.set_scaled_positions(coords)
         return atoms
 
+
 class ReadBuilder(StructureBuilder):
 
     def __init__(
-        self, fname, index=":", format=None, use_tags=False, 
-        directory="./", random_seed=None, *args, **kwargs
+        self,
+        fname,
+        index=":",
+        format=None,
+        use_tags=False,
+        directory="./",
+        random_seed=None,
+        *args,
+        **kwargs,
     ):
         """"""
-        super().__init__(use_tags=use_tags, directory=directory, random_seed=random_seed, *args, **kwargs)
+        super().__init__(
+            use_tags=use_tags,
+            directory=directory,
+            random_seed=random_seed,
+            *args,
+            **kwargs,
+        )
 
         self.fname = pathlib.Path(fname)
         self.index = index
         self.format = format
-        #self.kwargs = kwargs
+        # self.kwargs = kwargs
 
         return
-    
+
     def run(self, *args, **kwargs):
         """"""
         frames = read(self.fname, self.index, self.format)
+        if isinstance(frames, Atoms):
+            frames = [frames]
 
         return frames
-    
+
     def as_dict(self) -> dict:
         """"""
         params = {}
         params["method"] = "reader"
         params["fname"] = str(self.fname.resolve())
         params["index"] = self.index
         params["format"] = self.format
 
         return params
 
 
 class DirectBuilder(StructureBuilder):
-    """This generator directly returns structures that it stores.
-    """
+    """This generator directly returns structures that it stores."""
 
     #: Builder's name.
     name: str = "direct"
 
-    default_parameters: dict= {
-
-    }
+    default_parameters: dict = {}
 
     #: Stored structures.
     _frames: Optional[List[Atoms]] = None
 
     #: The file path of stored structures.
-    _fpath: Optional[Union[str,pathlib.Path]] = None
+    _fpath: Optional[Union[str, pathlib.Path]] = None
 
     #: Selected structure indices.
-    _indices: Union[str,List[int]] = None
+    _indices: Union[str, List[int]] = None
 
     def __init__(
-        self, frames: Union[str,pathlib.Path,List[Atoms]], 
-        indices: Union[str,List[int]] = None, directory: Union[str,pathlib.Path]="./", 
-        *args, **kwargs
+        self,
+        frames: Union[str, pathlib.Path, List[Atoms]],
+        indices: Union[str, List[int]] = None,
+        directory: Union[str, pathlib.Path] = "./",
+        *args,
+        **kwargs,
     ):
         """Create a direct generator.
 
         Args:
             frames: The structure file path or a list of ase atoms.
             directory: Working directory.
 
         """
         super().__init__(directory, *args, **kwargs)
 
-        if isinstance(frames, (str,pathlib.Path)):
+        if isinstance(frames, (str, pathlib.Path)):
             self._fpath = pathlib.Path(frames).resolve()
         else:
-            assert all(isinstance(x,Atoms) for x in frames), "Input should be a list of atoms."
+            assert all(
+                isinstance(x, Atoms) for x in frames
+            ), "Input should be a list of atoms."
             self._frames = frames
 
         self._indices = indices
 
         return
-    
+
     @property
-    def fpath(self) -> Union[str,pathlib.Path]:
+    def fpath(self) -> Union[str, pathlib.Path]:
         """Return the file path of stored structures."""
         return self._fpath
-    
+
     @property
-    def indices(self) -> Union[str,List[int]]:
+    def indices(self) -> Union[str, List[int]]:
         """Return selected indices."""
         return self._indices
-    
-    def run(self, indices: Union[str,List[int]]=[], *args, **kwargs) -> List[Atoms]:
+
+    def run(self, indices: Union[str, List[int]] = [], *args, **kwargs) -> List[Atoms]:
         """Return stored structures.
 
         Args:
             indices: Selected frames.
 
         """
         # - check indices
         if indices:
             indices_ = indices
         else:
             indices_ = self.indices
 
-        assert (bool(self._frames) ^ bool(self.fpath)), "Cant have frames and fpath at the same time."
+        assert bool(self._frames) ^ bool(
+            self.fpath
+        ), "Cant have frames and fpath at the same time."
 
         # - read frames if it is a path
         if self.fpath:
             # NOTE: custom read_xsd can retrieve stored constraints
             fpath_ = str(self.fpath)
             if fpath_.endswith(".xsd"):
                 frames_ = read_xsd2(fpath_)
@@ -234,21 +257,23 @@
 
         # - get structures
         if indices_:
             ret_frames = [frames_[i] for i in indices_]
         else:
             ret_frames = frames_
         return ret_frames
-    
+
     def as_dict(self) -> dict:
         """Return generator parameters"""
         params = dict(
-            method = "direct",
-            frames = str(self._fpath.resolve()), # TODO: if not exists, and only have _frames
-            indices = self.indices
+            method="direct",
+            frames=str(
+                self._fpath.resolve()
+            ),  # TODO: if not exists, and only have _frames
+            indices=self.indices,
         )
 
         return params
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.8/src/gdpx/builder/graph/exchange.py` & `gdpx-0.0.9/src/gdpx/builder/graph/exchange.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/graph/insert.py` & `gdpx-0.0.9/src/gdpx/builder/graph/insert.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/graph/modifier.py` & `gdpx-0.0.9/src/gdpx/builder/graph/modifier.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/graph/remove.py` & `gdpx-0.0.9/src/gdpx/builder/graph/remove.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/group.py` & `gdpx-0.0.9/src/gdpx/builder/group.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/hypercube.py` & `gdpx-0.0.9/src/gdpx/builder/scan/hypercube.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,102 +8,112 @@
 import numpy as np
 from scipy.stats import qmc
 
 import jax
 import jax.numpy as jnp
 from jax import grad, value_and_grad, jit, jacfwd, jacrev
 
+jax.config.update("jax_enable_x64", True)
+
 from ase import Atoms
 from ase.io import read, write
 
-from .builder import StructureModifier
+from ..builder import StructureModifier
 
 """Sample small molecule.
 """
 
+
 @jit
 def bond_distance(positions, indices: List[int]):
     """"""
     a1, a2 = indices
-    dis = jnp.linalg.norm(positions[a2]-positions[a1])
+    dis = jnp.linalg.norm(positions[a2] - positions[a1])
 
     return dis
+
+
 grad_bond_distance = grad(bond_distance, argnums=0)
 
+
 @jit
 def compute_bond_distances(positions: np.array, pair_indices: np.array):
     """Compute distances.
 
     Args:
         positions: Positions with shape of (natoms,3).
         pair_distances: Indices of atoms for distances [[0,1],[0,2]].
-    
+
     Examples:
 
         >>> pairs = np.array([[0,1]])
         >>> distances = compute_bond_distances(positions, pairs)
-    
+
     Returns:
         An array of distances.
 
     """
     pair_positions = jnp.take(positions, pair_indices.T, axis=0)
-    dvecs = pair_positions[0] - pair_positions[1] # TODO: + pair_shifts
+    dvecs = pair_positions[0] - pair_positions[1]  # TODO: + pair_shifts
     distances = jnp.linalg.norm(dvecs, axis=1)
 
     return distances
 
+
 @jit
 def bond_angle(positions, indices):
     """"""
     a1, a2, a3 = indices
     dvec1 = positions[a2] - positions[a1]
     dvec2 = positions[a3] - positions[a1]
 
-    #angle = jnp.arccos(jnp.dot(dvec1,dvec2)/jnp.linalg.norm(dvec1)/jnp.linalg.norm(dvec2))
-    angle = jnp.arctan2(jnp.linalg.norm(jnp.cross(dvec1,dvec2)), jnp.dot(dvec1,dvec2))
+    # angle = jnp.arccos(jnp.dot(dvec1,dvec2)/jnp.linalg.norm(dvec1)/jnp.linalg.norm(dvec2))
+    angle = jnp.arctan2(jnp.linalg.norm(jnp.cross(dvec1, dvec2)), jnp.dot(dvec1, dvec2))
 
     return angle
 
+
 @jit
 def compute_bond_angles(positions, trimer_indices):
     """Compute angles.
 
-    For very small/acute angles, results by arccos are inaccurate. arctan may be 
+    For very small/acute angles, results by arccos are inaccurate. arctan may be
     more effective.
 
     """
     trimer_positions = jnp.take(positions, trimer_indices.T, axis=0)
     # TODO: shifts
     dvecs1 = trimer_positions[1] - trimer_positions[0]
     dnorms1 = jnp.linalg.norm(dvecs1, axis=1)
     dvecs2 = trimer_positions[2] - trimer_positions[0]
     dnorms2 = jnp.linalg.norm(dvecs2, axis=1)
 
-    angles = jnp.arccos(jnp.sum(dvecs1*dvecs2, axis=1) / dnorms1 / dnorms2)
+    angles = jnp.arccos(jnp.sum(dvecs1 * dvecs2, axis=1) / dnorms1 / dnorms2)
 
     return angles
 
+
 @jit
 def pseudo_inverse_of_jacobian(jac, eps=0.0001):
     """"""
     dim = jac.shape[0]
-    jac_inv = jnp.transpose(jac)@jnp.linalg.inv(jac@jnp.transpose(jac)+eps*jnp.eye(dim))
+    jac_inv = jnp.transpose(jac) @ jnp.linalg.inv(
+        jac @ jnp.transpose(jac) + eps * jnp.eye(dim)
+    )
 
     return jac_inv
 
 
 class HypercubeBuilder(StructureModifier):
-
     """Use hypercube sampling to generate internal coordinates.
 
-    The implementation is not exact the same as the references. Here, we only 
+    The implementation is not exact the same as the references. Here, we only
     use hypercube to generate structures. No symmetry constraints is applied.
 
-    TODO: 
+    TODO:
         * Support dihedrals.
 
     References:
         [1] J. Chem. Phys. 2017, 147, 161706.
         [2] J. Chem. Phys. 2018, 149, 174114.
 
     """
@@ -111,17 +121,22 @@
     #: Maximum number of updates of positions.
     MAX_ATTEMPTS_UPDATE: int = 100
 
     #: Tolerance of target internal coordinates.
     TOL_INTCOORD: float = 1e-4
 
     def __init__(
-        self, distances, disrange: List[float], 
-        angles=None, angrange: List[float]=None, 
-        substrates=None, *args, **kwargs
+        self,
+        distances,
+        disrange: List[float],
+        angles=None,
+        angrange: List[float] = None,
+        substrates=None,
+        *args,
+        **kwargs,
     ):
         """"""
         super().__init__(substrates=substrates, *args, **kwargs)
 
         self.dimers = np.array(distances)
 
         if angles:
@@ -133,94 +148,106 @@
 
         self.ndof = len(self.dimers) + len(self.trimers)
 
         bounds_ = []
         if disrange:
             if isinstance(disrange[0], list):
                 bounds_.extend(disrange)
-            else: # two floats
-                bounds_.extend([disrange]*len(self.dimers))
+            else:  # two floats
+                bounds_.extend([disrange] * len(self.dimers))
         if self._use_ang:
             if angrange:
                 if isinstance(angrange[0], list):
                     bounds_.extend(angrange)
                 else:
-                    bounds_.extend([angrange]*len(self.trimers))
+                    bounds_.extend([angrange] * len(self.trimers))
             else:
-                ... # TODO: set default 15,165?
+                ...  # TODO: set default 15,165?
         self.bounds = np.array(bounds_).T
 
-        assert self.bounds.shape[1] == self.ndof, "Inconsistent number of freedoms and ranges."
+        assert (
+            self.bounds.shape[1] == self.ndof
+        ), "Inconsistent number of freedoms and ranges."
 
         return
-    
-    def run(self, substrates: List[Atoms]=None, size: int=1, *args, **kwargs) -> List[Atoms]:
-        """Modify input structures to generate random hypercube structures.
-        """
+
+    def run(
+        self, substrates: List[Atoms] = None, size: int = 1, *args, **kwargs
+    ) -> List[Atoms]:
+        """Modify input structures to generate random hypercube structures."""
         super().run(substrates=substrates, *args, **kwargs)
 
         frames = []
         for substrate in self.substrates:
             curr_frames = self._irun(substrate=substrate, size=size, *args, **kwargs)
             frames.extend(curr_frames)
 
         return frames
-    
+
     def _irun(self, substrate: Atoms, size=1, *args, **kwargs) -> List[Atoms]:
         """"""
         # NOTE: strength new in 1.8.0
-        #sampler = qmc.LatinHypercube(d=ninternals, strength=2, seed=self.rng) 
+        # sampler = qmc.LatinHypercube(d=ninternals, strength=2, seed=self.rng)
         sampler = qmc.LatinHypercube(d=self.ndof, seed=self.rng)
         samples = sampler.random(n=size)
 
         l_bounds, u_bounds = self.bounds
         scaled_samples = qmc.scale(samples, l_bounds, u_bounds)
 
         # - generate structures
         frames = []
         for sample in scaled_samples:
             curr_atoms = copy.deepcopy(substrate)
-            curr_atoms = self._approx_structure(curr_atoms, sample, self.dimers, self.trimers)
+            curr_atoms = self._approx_structure(
+                curr_atoms, sample, self.dimers, self.trimers
+            )
+            # wrap structures as sometimes the atoms are out of box
+            curr_atoms.wrap()
             frames.append(curr_atoms)
 
         return frames
-    
+
     def _approx_structure(self, atoms: Atoms, targets, pairs, trimers=None):
         """"""
         natoms = len(atoms)
 
+        maxstep = 1.00
+
         # - compute pseudo inverse of the jacobian matrix
+        self._debug(f"{targets =}")
         positions = copy.deepcopy(atoms.positions)
         for i in range(self.MAX_ATTEMPTS_UPDATE):
             distances = compute_bond_distances(positions, pairs)
             if self._use_ang:
                 angles = compute_bond_angles(positions, trimers)
             else:
                 angles = []
-            internals = np.hstack((distances,angles))
+            internals = np.hstack((distances, angles))
             self._debug(f"internals: {internals}")
-            disp = targets - internals 
+            disp = targets - internals
             if np.max(np.fabs(disp)) < self.TOL_INTCOORD:
                 break
             dis_jac_ = jacrev(compute_bond_distances, argnums=0)(positions, pairs)
-            dis_jac = dis_jac_.reshape(-1,natoms*3)
+            dis_jac = dis_jac_.reshape(-1, natoms * 3)
             if self._use_ang:
                 ang_jac_ = jacrev(compute_bond_angles, argnums=0)(positions, trimers)
-                ang_jac = ang_jac_.reshape(-1,natoms*3)
-                jac = np.vstack((dis_jac,ang_jac))
+                ang_jac = ang_jac_.reshape(-1, natoms * 3)
+                jac = np.vstack((dis_jac, ang_jac))
             else:
                 ang_jac = []
                 jac = dis_jac
             jac_inv = pseudo_inverse_of_jacobian(jac)
-            positions = copy.deepcopy(positions) + jnp.reshape(jac_inv@disp, (-1,3))
+            positions = copy.deepcopy(positions) + maxstep * jnp.reshape(
+                jac_inv @ disp, (-1, 3)
+            )
         else:
-            #warnings.warn("Iterative approximation is not converged.", UserWarning)
+            # warnings.warn("Iterative approximation is not converged.", UserWarning)
             self._print("Iterative approximation is not converged.")
-        
+
         # - update positions
         atoms.positions = positions
-        
+
         return atoms
 
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.8/src/gdpx/builder/insert.py` & `gdpx-0.0.9/src/gdpx/builder/insert.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/interface.py` & `gdpx-0.0.9/src/gdpx/builder/interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -181,31 +181,49 @@
     def __init__(self, builder, size: int = 1, directory="./") -> NoReturn:
         super().__init__(input_nodes=[builder], directory=directory)
 
         self.size = size
 
         return
 
+    @Operation.directory.setter
+    def directory(self, directory_) -> None:
+        """"""
+        self._directory = pathlib.Path(directory_)
+
+        self.input_nodes[0].directory = self._directory / "builder"
+
+        return
+
     def forward(self, builder) -> List[Atoms]:
         """"""
         super().forward()
 
-        builder.directory = self.directory
-        curr_builder_output = self.directory / f"{builder.name}_output.xyz"
-        if curr_builder_output.exists():
-            frames = read(curr_builder_output, ":")
-        else:
+        cache_path = self.directory / f"{builder.name}-out.xyz"
+        if not cache_path.exists():
             frames = builder.run(size=self.size)
-            write(curr_builder_output, frames)
-        self._print(f"{builder.name} nframes: {len(frames)}")
+            write(cache_path, frames)
+        else:
+            frames = read(cache_path, ":")
+        # self._print(f"{builder.name} nframes: {len(frames)}")
 
         self.status = "finished"
 
         return frames
 
+    def _preprocess_input_nodes(self, input_nodes):
+        """"""
+        builder = input_nodes[0]
+        if isinstance(builder, dict) or isinstance(
+            builder, omegaconf.dictconfig.DictConfig
+        ):
+            builder = BuilderVariable(directory=self.directory / "builder", **builder)
+
+        return [builder]
+
 
 @registers.operation.register
 class modify(Operation):
 
     def __init__(
         self, substrates, modifier, size: int = 1, repeat: int = 1, directory="./"
     ) -> None:
@@ -282,27 +300,9 @@
             params = dict(method="direct", frames=params)
 
     builder = BuilderVariable(**params).value
 
     return builder
 
 
-def build_structures(config: dict, substrates=None, size: int = 1, directory="./"):
-    """"""
-    directory = pathlib.Path(directory)
-
-    builder = BuilderVariable(directory=directory, **config).value
-    builder.directory = directory
-
-    # assume substrates is a file path
-    if substrates is not None:
-        substrates = read(substrates, ":")
-
-    frames = builder.run(substrates=substrates, size=size)
-
-    write(directory / "structures.xyz", frames)
-
-    return
-
-
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.8/src/gdpx/builder/mutation/__init__.py` & `gdpx-0.0.9/src/gdpx/builder/mutation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/packer.py` & `gdpx-0.0.9/src/gdpx/builder/packer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/perturbator.py` & `gdpx-0.0.9/src/gdpx/builder/perturbator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/randomBuilder.py` & `gdpx-0.0.9/src/gdpx/builder/randomBuilder.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/region.py` & `gdpx-0.0.9/src/gdpx/builder/region.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/repeat.py` & `gdpx-0.0.9/src/gdpx/builder/repeat.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/species.py` & `gdpx-0.0.9/src/gdpx/builder/species.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/utils.py` & `gdpx-0.0.9/src/gdpx/builder/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/builder/zoom.py` & `gdpx-0.0.9/src/gdpx/builder/zoom.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/colvar/compute_reweight.py` & `gdpx-0.0.9/src/gdpx/colvar/compute_reweight.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/colvar/coordination.py` & `gdpx-0.0.9/src/gdpx/colvar/coordination.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/colvar/distance.py` & `gdpx-0.0.9/src/gdpx/colvar/distance.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/colvar/fingerprint.py` & `gdpx-0.0.9/src/gdpx/colvar/fingerprint.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/colvar/plot_meta.py` & `gdpx-0.0.9/src/gdpx/colvar/plot_meta.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/colvar/plot_string.py` & `gdpx-0.0.9/src/gdpx/colvar/plot_string.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/colvar/plotstring.py` & `gdpx-0.0.9/src/gdpx/colvar/plotstring.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/colvar/reweight.py` & `gdpx-0.0.9/src/gdpx/colvar/reweight.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/colvar/rmsd.py` & `gdpx-0.0.9/src/gdpx/colvar/rmsd.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/comparator/__init__.py` & `gdpx-0.0.9/src/gdpx/comparator/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/comparator/cartesian.py` & `gdpx-0.0.9/src/gdpx/comparator/cartesian.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/comparator/comparator.py` & `gdpx-0.0.9/src/gdpx/comparator/comparator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/comparator/coordination.py` & `gdpx-0.0.9/src/gdpx/comparator/coordination.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/comparator/graph.py` & `gdpx-0.0.9/src/gdpx/comparator/graph.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/comparator/interface.py` & `gdpx-0.0.9/src/gdpx/comparator/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/comparator/reaction.py` & `gdpx-0.0.9/src/gdpx/comparator/reaction.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/comparator/singlepoint.py` & `gdpx-0.0.9/src/gdpx/comparator/singlepoint.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/computation/__init__.py` & `gdpx-0.0.9/src/gdpx/computation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/computation/asedriver.py` & `gdpx-0.0.9/src/gdpx/computation/asedriver.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,41 +5,35 @@
 import copy
 import dataclasses
 import io
 import pathlib
 import shutil
 import tarfile
 import traceback
-from typing import Optional, List, Tuple
 import warnings
+from typing import List, Optional, Tuple
 
+import ase.constraints
 import numpy as np
-
 import yaml
-
-from ase import Atoms
-from ase import units
-
-from ase.io import read, write
-import ase.constraints
-from ase.constraints import Filter
-from ase.optimize.optimize import Dynamics
-from ase.md.velocitydistribution import (
-    MaxwellBoltzmannDistribution,
-    Stationary,
-    ZeroRotation,
-)
-
+from ase import Atoms, units
 from ase.calculators.calculator import Calculator
 from ase.calculators.singlepoint import SinglePointCalculator
+from ase.constraints import Filter
+from ase.io import read, write
+from ase.md.md import MolecularDynamics
+from ase.md.velocitydistribution import (MaxwellBoltzmannDistribution,
+                                         Stationary, ZeroRotation)
+from ase.optimize.optimize import Dynamics
 
 from .. import config as GDPCONFIG
 from ..potential.calculators.mixer import EnhancedCalculator
-from .driver import AbstractDriver, DriverSetting, Controller
+from .driver import EARLYSTOP_KEY, AbstractDriver, Controller, DriverSetting
 from .md.md_utils import force_temperature
+from .observer import create_an_observer
 
 
 def set_calc_state(calc: Calculator, timestep: float, stride: int):
     """Some calculators need driver information e.g. PLUMED."""
     if calc.name == "plumed":
         calc.timestep = timestep
         calc.stride = stride
@@ -48,17 +42,17 @@
             set_calc_state(subcalc, timestep, stride)
     else:
         ...
 
     return
 
 
-def update_atoms_info(atoms: Atoms, dyn: Dynamics, start_step: int = 0) -> None:
+def update_atoms_info(atoms: Atoms, dyn: Dynamics) -> None:
     """Update step in atoms.info."""
-    atoms.info["step"] = dyn.nsteps + start_step
+    atoms.info["step"] = dyn.nsteps
 
     return
 
 
 def retrieve_and_save_deviation(atoms, devi_fpath) -> None:
     """Read model deviation and add results to atoms.info if the file exists."""
     results = copy.deepcopy(atoms.calc.results)
@@ -108,14 +102,16 @@
         energy=atoms.get_potential_energy(), forces=copy.deepcopy(atoms.get_forces())
     )
     spc = SinglePointCalculator(atoms, **results)
     atoms_to_save.calc = spc
 
     # - save atoms info...
     atoms_to_save.info["step"] = atoms.info["step"]
+    if EARLYSTOP_KEY in atoms.info:
+        atoms_to_save.info[EARLYSTOP_KEY] = atoms.info[EARLYSTOP_KEY]
 
     # - save special keys and arrays from calc
     natoms = len(atoms)
 
     # -- add deviation
     for k, v in atoms.calc.results.items():
         if k in GDPCONFIG.VALID_DEVI_FRAME_KEYS:
@@ -137,19 +133,18 @@
     # - append to traj
     write(log_fpath, atoms_to_save, append=True)
 
     return
 
 
 def save_checkpoint(
-    dyn: Dynamics, atoms: Atoms, wdir: pathlib.Path, ckpt_number: int=3,
-    start_step: int = 0
+    dyn: Dynamics, atoms: Atoms, wdir: pathlib.Path, ckpt_number: int = 3
 ):
     """"""
-    ckpt_wdir = wdir / f"checkpoint.{dyn.nsteps+start_step}"
+    ckpt_wdir = wdir / f"checkpoint.{dyn.nsteps}"
     ckpt_wdir.mkdir(parents=True, exist_ok=True)
 
     # write(ckpt_wdir/"structure.xyz", atoms)
     save_trajectory(atoms=atoms, log_fpath=ckpt_wdir / "structures.xyz")
 
     # For some optimisers and dynamics, they use random generator.
     if hasattr(dyn, "rng"):
@@ -168,14 +163,27 @@
     if num_ckpts > ckpt_number:
         for w in ckpt_wdirs[:-ckpt_number]:
             shutil.rmtree(w)
 
     return
 
 
+def monit_and_intervene(
+    atoms: Atoms, dynamics: Dynamics, observer, print_func=print
+) -> None:
+    """"""
+    if dynamics.nsteps >= observer.patience:
+        if observer.run(atoms):
+            dynamics.max_steps = 0
+            atoms.info[EARLYSTOP_KEY] = True
+            print_func(f"EARLY STOPPED at step {dynamics.nsteps}!!")
+
+    return
+
+
 @dataclasses.dataclass
 class BerendsenThermostat(Controller):
 
     name: str = "berendsen"
 
     def __post_init__(
         self,
@@ -370,15 +378,15 @@
             if self.min_style in filter_names:
                 driver_cls = BFGS
                 self.filter_cls = getattr(ase.constraints, self.min_style)
 
         if self.task == "rxn":
             # TODO: move to reactor
             try:
-                from sella import Sella, Constraints
+                from sella import Constraints, Sella
 
                 driver_cls = Sella
             except:
                 raise NotImplementedError(f"Sella is not installed.")
             ...
 
         try:
@@ -429,15 +437,15 @@
     #: List of output files would be removed when restart.
     removed_fnames: List[str] = [log_fname, xyz_fname, devi_fname]
 
     def __init__(self, calc=None, params: dict = {}, directory="./", *args, **kwargs):
         """"""
         super().__init__(calc, params, directory, *args, **kwargs)
 
-        self.setting = AseDriverSetting(**params)
+        self.setting: AseDriverSetting = AseDriverSetting(**params)
 
         self._log_fpath = self.directory / self.log_fname
 
         return
 
     @property
     def log_fpath(self):
@@ -495,24 +503,27 @@
                 vrng = np.random.Generator(np.random.PCG64(velocity_seed))
 
             ignore_atoms_velocities = init_params_.pop("ignore_atoms_velocities")
             if not ignore_atoms_velocities and atoms.get_kinetic_energy() > 0.0:
                 # atoms have momenta
                 ...
             else:
+                # nve does not have temp in dyn_params so we use setting.temp
+                # for all ensembles just for consistency
+                target_temperature = self.setting.temp
                 MaxwellBoltzmannDistribution(
-                    atoms, temperature_K=init_params_["temperature_K"], rng=vrng
+                    atoms, temperature_K=target_temperature, rng=vrng
                 )
                 if self.setting.remove_rotation:
                     ZeroRotation(atoms, preserve_temperature=False)
                 if self.setting.remove_translation:
                     Stationary(atoms, preserve_temperature=False)
                 # NOTE: respect constraints
                 #       ase code does not consider constraints
-                force_temperature(atoms, init_params_["temperature_K"], unit="K")
+                force_temperature(atoms, target_temperature, unit="K")
 
             # - some dynamics need rng
             if "rng" in init_params_:
                 self._print(f"MD Driver's rng: {self.rng.bit_generator.state}")
                 init_params_["rng"] = self.rng
 
             # - other callbacks
@@ -594,107 +605,145 @@
                 curr_params["run"] = self.setting.get_run_params()
 
                 with open(self.directory / "params.yaml", "w") as fopen:
                     yaml.safe_dump(curr_params, fopen, indent=2)
             else:  # restart ...
                 ckpt_wdir = self._find_latest_checkpoint(prev_wdir)
                 atoms, rng_state = self._load_checkpoint(ckpt_wdir)
+                write(self.directory / self.xyz_fname, atoms)
                 start_step = atoms.info["step"]
                 if hasattr(self.calc, "calcs"):
                     for calc in self.calc.calcs:
                         if hasattr(calc, "_load_checkpoint"):
                             calc._load_checkpoint(ckpt_wdir, start_step=start_step)
                 # --- update run_params in settings
                 target_steps = self.setting.get_run_params(*args, **kwargs)["steps"]
                 if target_steps > 0:
-                    steps = target_steps - start_step
+                    if self.setting.task == "md":
+                        steps = target_steps - start_step
+                    else:
+                        # ase v3.22.1 opt will reset max_steps to steps in run
+                        steps = target_steps
                 assert steps > 0, "Steps should be greater than 0."
                 kwargs.update(steps=steps)
 
                 # To restart, velocities are always retained
                 self.setting.ignore_atoms_velocities = False
 
             # - set calculator
             atoms.calc = self.calc
 
             # - set dynamics
             dynamics, run_params = self._create_dynamics(atoms, *args, **kwargs)
-            # dynamics.nsteps = start_step
+            dynamics.nsteps = start_step
+            dynamics.max_steps = self.setting.steps
             if hasattr(dynamics, "rng") and rng_state is not None:
                 dynamics.rng.bit_generator.state = rng_state
 
-            # --- callback functions
-            dynamics.insert_observer(
+            # callback functions
+            init_params = self.setting.get_init_params()
+
+            # update atoms.info at the beginning of each step
+            dynamics.attach(
                 update_atoms_info,
                 dyn=dynamics,
                 atoms=atoms,
-                start_step=start_step,
             )
-            # NOTE: traj file not stores properties (energy, forces) properly
-            init_params = self.setting.get_init_params()
+
+            # HACK: add some observers to early stop the simulation
+            #       make sure this must be added before save_trajectory
+            #       as it adds `earlystop` in atoms.info and
+            #       BE CAREFUL it changes some attributes affect convergence
+            if self.setting.observers is not None:
+                observers = []
+                for ob_params in self.setting.observers:
+                    observers.append(create_an_observer(ob_params))
+                for ob in observers:
+                    dynamics.attach(
+                        monit_and_intervene,
+                        interval=self.setting.dump_period,
+                        atoms=atoms,
+                        dynamics=dynamics,
+                        observer=ob,
+                        print_func=self._print,
+                    )
+
+            # traj file not stores properties (energy, forces) properly
             dynamics.attach(
                 save_checkpoint,
                 interval=self.setting.ckpt_period,
                 dyn=dynamics,
                 atoms=atoms,
                 wdir=self.directory,
                 ckpt_number=self.setting.ckpt_number,
-                start_step=start_step,
             )
             dynamics.attach(
                 save_trajectory,
                 interval=init_params["loginterval"],
                 atoms=atoms,
                 log_fpath=self.directory / self.xyz_fname,
             )
-            # NOTE: retrieve deviation info
             dynamics.attach(
                 retrieve_and_save_deviation,
                 interval=init_params["loginterval"],
                 atoms=atoms,
                 devi_fpath=self.directory / self.devi_fname,
             )
+
+            # run simulation
             dynamics.run(**run_params)
 
+            # make sure the max_steps are the same as input even if
+            # it is set by earlystop observer
+            dynamics.max_steps = self.setting.steps
+
             # NOTE: check if the last frame is properly stored
             dump_period = self.setting.dump_period
             assert init_params["loginterval"] == dump_period
+            ckpt_period = self.setting.ckpt_period
 
-            if dump_period > 1:
-                should_dump_last = False
-                if self.setting.task == "min":
-                    # optimiser dumps every step to log...
-                    data = np.loadtxt(self.directory / "dyn.log", dtype=str, skiprows=1)
-                    if len(data.shape) == 1:
-                        data = data[np.newaxis, :]
-                    nsteps = data.shape[0]
-                    if nsteps > 0 and (nsteps - 1) % dump_period != 0:
+            should_dump_last, should_ckpt_last = False, False
+            if self.setting.task == "min":
+                # optimiser dumps every step to log but we control saved structures
+                # by dump_period
+                nsteps = atoms.info["step"] + 1
+                if nsteps > 0 and (nsteps - 1) % dump_period != 0:
+                    should_dump_last = True
+                if nsteps > 0 and (nsteps - 1) % ckpt_period != 0:
+                    should_ckpt_last = True
+            elif self.setting.task == "md":
+                nsteps = atoms.info["step"] + 1
+                if nsteps > 0 and (nsteps - 1) % dump_period != 0:
+                    should_dump_last = True
+                    if atoms.info.get(EARLYSTOP_KEY, False):
                         should_dump_last = True
-                elif self.setting.task == "md":
-                    if dump_period > self.setting.steps:
-                        should_dump_last = True
-                if should_dump_last:
-                    update_atoms_info(atoms, dynamics, start_step=start_step)
-                    save_checkpoint(
-                        dynamics, atoms, self.directory, ckpt_number=self.setting.ckpt_number,
-                        start_step=start_step
-                    )
-                    save_trajectory(atoms, self.directory / self.xyz_fname)
-                    retrieve_and_save_deviation(atoms, self.directory / self.devi_fname)
-            else:
-                ...
+                if nsteps > 0 and (nsteps - 1) % ckpt_period != 0:
+                    should_ckpt_last = True
+            if should_dump_last:
+                self._print("dump the last frame...")
+                update_atoms_info(atoms, dynamics)
+                save_trajectory(atoms, self.directory / self.xyz_fname)
+                retrieve_and_save_deviation(atoms, self.directory / self.devi_fname)
+
+            if should_ckpt_last:
+                self._print("ckpt the last frame...")
+                save_checkpoint(
+                    dynamics,
+                    atoms,
+                    self.directory,
+                    ckpt_number=self.setting.ckpt_number,
+                )
 
             # - Some interactive calculator needs kill processes after finishing,
             #   e.g. VaspInteractive...
             if hasattr(self.calc, "finalize"):
                 self.calc.finalize()
             # To restart, velocities are always retained
             self.setting.ignore_atoms_velocities = prev_ignore_atoms_velocities
         except Exception as e:
-            self._debug(f"Exception of {self.__class__.__name__} is {e}.")
             self._debug(
                 f"Exception of {self.__class__.__name__} is {traceback.format_exc()}."
             )
 
         return
 
     def read_force_convergence(self, *args, **kwargs) -> bool:
@@ -743,14 +792,20 @@
                         )
                         frames = read(fobj, ":", format="extxyz")
                         fobj.close()
                         break
                 else:
                     frames = []
 
+        # HACK: No need cut frames to the checkpoint like other driver backends
+        #       as we always dump the last frame as a checkpoint
+        # NOTE: Actually, if the simulation stopped in the middle, we do not have
+        #       the checkpoint of the last frame thus the trajectories are not
+        #       consecutive. So we concatenate trajectoies by atoms.info["step"]!!!
+
         return frames
 
     def read_trajectory(self, archive_path=None, *args, **kwargs) -> List[Atoms]:
         """Read trajectory in the current working directory."""
         # - read trajectory
         traj_frames = self._aggregate_trajectories(archive_path=archive_path)
```

### Comparing `gdpx-0.0.8/src/gdpx/computation/cp2k.py` & `gdpx-0.0.9/src/gdpx/computation/cp2k.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/computation/driver.py` & `gdpx-0.0.9/src/gdpx/computation/driver.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,130 +5,150 @@
 import copy
 import dataclasses
 import pathlib
 import re
 import shutil
 import tarfile
 import warnings
-
-from typing import Optional, NoReturn, List, Callable, Union
 from collections.abc import Iterable
+from typing import Callable, List, NoReturn, Optional, Union
 
 import numpy as np
-
 from ase import Atoms
-from ase.constraints import FixAtoms
 from ase.calculators.calculator import compare_atoms
+from ase.constraints import FixAtoms
+from ase.md.velocitydistribution import (MaxwellBoltzmannDistribution,
+                                         Stationary, ZeroRotation)
 
-from ..builder.constraints import parse_constraint_info, convert_indices
+from ..builder.constraints import convert_indices, parse_constraint_info
 from ..core.node import AbstractNode
+from .md.md_utils import force_temperature
 
 #: Prefix of backup files
 BACKUP_PREFIX_FORMAT: str = "gbak.{:d}."
 
 #: Parameter keys used to init a minimisation task.
 MIN_INIT_KEYS: List[str] = ["min_style", "min_modify", "dump_period"]
 
 #: Parameter keys used to run a minimisation task.
 MIN_RUN_KEYS: List[str] = ["steps", "fmax"]
 
 #: Parameter keys used to init a molecular-dynamics task.
 MD_INIT_KEYS: List[str] = [
-    "md_style", "velocity_seed", "timestep", "temp", "Tdamp", 
-    "press", "Pdamp", "dump_period"
+    "md_style",
+    "velocity_seed",
+    "timestep",
+    "temp",
+    "Tdamp",
+    "press",
+    "Pdamp",
+    "dump_period",
 ]
 
+# Key name for earlystopping in atoms.info.
+EARLYSTOP_KEY: str = "earlystop"
+
 
 @dataclasses.dataclass
 class Controller:
 
     #: Thermostat name.
-    name: str = "controller" # thermostat or barostat
+    name: str = "controller"  # thermostat or barostat
+
+    #: Parameter unit type (see ase.lammps).
+    units: str = "metal"
 
     #: Parameters.
     params: dict = dataclasses.field(default_factory=dict)
 
 
 @dataclasses.dataclass
 class DriverSetting:
-
-    """These are geometric parameters. Electronic?
-    """
+    """These are geometric parameters. Electronic?"""
 
     #: Simulation task.
     task: str = "min"
 
     #: Driver setting.
     backend: str = "external"
 
-    #: 
+    #: Whether check convergence based on the trajectory.
+    check_trajectory_convergence: bool = False
+
+    #: Some observers
+    observers: Optional[List[dict]] = None
+
+    #:
     min_style: str = "bfgs"
     min_modify: str = "integrator verlet tmax 4"
     maxstep: float = 0.1
 
     #:
     md_style: str = "nvt"
 
-    velocity_seed: int = None
+    velocity_seed: Optional[int] = None
 
     #: Whether ignore atoms' velocities and initialise it from the scratch.
     ignore_atoms_velocities: bool = False
 
     #: Whether remove rotation when init velocity.
     remove_rotation: bool = True
 
     #: Whether remove translation when init velocity.
     remove_translation: bool = True
 
     timestep: float = 1.0
 
-    temp: float = 300.
+    temp: float = 300.0
     tend: float = None
-    Tdamp: float = 100. # fs
+    Tdamp: float = 100.0  # fs
 
-    press: float = 1.0 # bar
-    pend: float = None # bar
-    Pdamp: float = 100.
+    press: float = 1.0  # bar
+    pend: float = None  # bar
+    Pdamp: float = 100.0
 
     #: The interval steps to dump output files (e.g. trajectory).
     dump_period: int = 1
 
     #: The interval steps to save a check point that is used for restart.
     ckpt_period: int = 100
 
     #: The number of checkpoints to save.
     ckpt_number: int = 3
 
     #: run params
-    etol: float = None # 5e-2
-    fmax: float = None # 1e-5
+    etol: float = None  # 5e-2
+    fmax: float = None  # 1e-5
     steps: int = 0
 
     constraint: str = None
 
-    #: Parameters that are used to update 
+    #: Parameters that are used to update
     _internals: dict = dataclasses.field(default_factory=dict)
 
     def update(self, **kwargs):
         """"""
         for k, v in kwargs.items():
             if hasattr(self, k):
                 setattr(self, k, v)
         self.__post_init__()
 
         return
-    
+
     def get_init_params(self):
         """"""
 
         return copy.deepcopy(self._internals)
-    
+
     def get_run_params(self, *args, **kwargs):
         """"""
-        raise NotImplementedError(f"{self.__class__.__name__} has no function for run params.")
+        raise NotImplementedError(
+            f"{self.__class__.__name__} has no function for run params."
+        )
+
 
 class AbstractDriver(AbstractNode):
 
     #: Driver's name.
     name: str = "abstract"
 
     #: Atoms that is for state check.
@@ -149,98 +169,104 @@
     #: List of output files would be removed when restart.
     removed_fnames: List[str] = []
 
     #: Systemwise parameter keys.
     syswise_keys: list = []
 
     #: Parameters for PotentialManager.
-    pot_params: dict = None
+    pot_params: Optional[dict] = None
 
     def __init__(
-        self, calc, params: dict, directory="./", ignore_convergence: bool=False, 
-        random_seed=None, *args, **kwargs
+        self,
+        calc,
+        params: dict,
+        directory="./",
+        ignore_convergence: bool = False,
+        random_seed=None,
+        *args,
+        **kwargs,
     ):
         """Init a driver.
 
         Args:
             calc: The ase calculator.
             params: Driver parameters.
             directory: Working directory.
 
         """
-        super().__init__(
-            directory=directory, random_seed=random_seed, *args, **kwargs
-        )
+        super().__init__(directory=directory, random_seed=random_seed, *args, **kwargs)
 
         self.calc = calc
         self.calc.reset()
 
         self.ignore_convergence = ignore_convergence
 
         self._org_params = copy.deepcopy(params)
 
         return
-    
+
     @property
     @abc.abstractmethod
     def default_task(self) -> str:
         """Default simulation task."""
 
         return
 
     @property
     @abc.abstractmethod
     def supported_tasks(self) -> List[str]:
         """Supported simulation tasks"""
 
         return
-    
+
     @AbstractNode.directory.setter
     def directory(self, directory_):
         """"""
         self._directory = pathlib.Path(directory_)
         # NOTE: directory is set before self.calc is defined...
         #       ASE uses str path, so to avoid inconsistency here
         if hasattr(self, "calc"):
-            self.calc.directory = str(self.directory) 
+            self.calc.directory = str(self.directory)
 
         return
-    
+
     def get(self, key):
         """Get param value from init/run params by a mapped key name."""
         parameters = copy.deepcopy(self.init_params)
         parameters.update(copy.deepcopy(self.run_params))
 
         value = parameters.get(key, None)
         if not value:
             mapped_key = self.param_mapping.get(key, None)
             if mapped_key:
                 value = parameters.get(mapped_key, None)
 
         return value
-    
+
     def reset(self) -> None:
         """Remove results stored in dynamics calculator."""
         self.calc.reset()
 
         return
 
-    def run(self, atoms, read_ckpt: bool=True, extra_info: dict=None, *args, **kwargs) -> Atoms:
+    def run(
+        self, atoms, read_ckpt: bool = True, extra_info: dict = None, *args, **kwargs
+    ) -> None:
         """Return the last frame of the simulation.
 
         Copy input atoms, and return a new atoms. Check whether the simulation is
-        finished and retrieve stored results. If necessary, extra information could 
+        finished and retrieve stored results. If necessary, extra information could
         be added to the atoms.info.
 
-        The simulation should either run from the scratch or restart from a given 
+        The simulation should either run from the scratch or restart from a given
         checkpoint...
 
         """
-        # - NOTE: input atoms from WORKER may have minimal properties as
-        #         cell, pbc, positions, symbols, tags, momenta...
+        # NOTE: input atoms from WORKER may have minimal properties as
+        #       cell, pbc, positions, symbols, tags, momenta...
         atoms = atoms.copy()
 
         # - set driver's atoms to the current one
         if isinstance(self.atoms, Atoms):
             warnings.warn("Driver has attached atoms object.", RuntimeWarning)
             system_changes = compare_atoms(atoms1=self.atoms, atoms2=atoms, tol=1e-15)
             self._debug(f"system_changes: {system_changes}")
@@ -248,275 +274,355 @@
             if len(system_changes) > 0:
                 system_changed = True
             else:
                 system_changed = False
         else:
             system_changed = False
 
-        # - backup old params
-        params_old = copy.deepcopy(self.calc.parameters)
+        # backup old params
+        prev_params = copy.deepcopy(self.calc.parameters)
 
-        # - run dynamics
-        cache_traj = None
+        # run dynamics
+        self.cache_traj: Optional[List[Atoms]] = None
         if not self._verify_checkpoint():
             # If there is no valid checkpoint, just run the simulation from the scratch
             self._debug(f"... start from the scratch @ {self.directory.name} ...")
             self.directory.mkdir(parents=True, exist_ok=True)
             self._irun(atoms, *args, **kwargs)
         else:
-            # If there is valid checkpoints...
+            # If there is any valid checkpoint...
             if not system_changed:
                 self._debug(f"... system not changed @ {self.directory.name} ...")
-                cache_traj = self.read_trajectory()
-                converged = self.read_convergence(cache_traj=cache_traj)
+                converged = self.read_convergence()
                 self._debug(f"... convergence {converged} ...")
                 if not converged:
-                    self._debug(f"... unconverged @ {self.directory.name} ...")
+                    self._debug(
+                        f"... continue from unconverged @ {self.directory.name} ..."
+                    )
                     ckpt_wdir = self._save_checkpoint() if read_ckpt else None
                     self._debug(f"... checkpoint @ {str(ckpt_wdir)} ...")
                     self._cleanup()
-                    self._irun(atoms, ckpt_wdir=ckpt_wdir, cache_traj=cache_traj, *args, **kwargs)
-                    cache_traj = None
+                    self._irun(
+                        atoms,
+                        ckpt_wdir=ckpt_wdir,
+                        cache_traj=self.cache_traj,
+                        *args,
+                        **kwargs,
+                    )
+                    self.cache_traj = None
                 else:
                     self._debug(f"... converged @ {self.directory.name} ...")
             else:
-                self._debug(f"... clean up @ {self.directory.name} ...")
+                self._debug(f"... start after clean up @ {self.directory.name} ...")
                 self._cleanup()
                 self._irun(atoms, *args, **kwargs)
 
-        self.calc.parameters = params_old
+        self.calc.parameters = prev_params
         self.calc.reset()
-        
-        # - check again
-        cache_traj = self.read_trajectory()
-        curr_atoms, converged = None, self.read_convergence(cache_traj=cache_traj) # NOTE: This will read_trajectory
-        if converged:
-            self._debug(f"... 2. converged @ {self.directory.name} ...")
-            traj = cache_traj
-            nframes = len(traj)
-            if nframes > 0:
-                curr_atoms = traj[-1]
-                if extra_info is not None:
-                    curr_atoms.info.update(**extra_info)
-            else:
-                warnings.warn(f"The calculation at {self.directory.name} performed but failed.", RuntimeWarning)
-                curr_atoms = None
-        else:
-            self._debug(f"... 2. unconverged @ {self.directory.name} ...")
 
-        return curr_atoms # TODO: change None to ...
-    
+        return
+
     def _verify_checkpoint(self, *args, **kwargs) -> bool:
         """Check whether there is a previous calculation in the `self.directory`."""
 
         return self.directory.exists()
-    
+
     def _save_checkpoint(self, *args, **kwargs):
         """Save the previous simulation to a checkpoint directory."""
         # - find previous runs...
         prev_wdirs = sorted(self.directory.glob(r"[0-9][0-9][0-9][0-9][.]run"))
         self._debug(f"prev_wdirs: {prev_wdirs}")
         curr_index = len(prev_wdirs)
 
-        curr_wdir = self.directory/f"{str(curr_index).zfill(4)}.run"
+        curr_wdir = self.directory / f"{str(curr_index).zfill(4)}.run"
         self._debug(f"curr_wdir: {curr_wdir}")
 
         # - backup files
         curr_wdir.mkdir()
         for x in self.directory.iterdir():
             if not re.match(r"[0-9]{4}\.run", x.name):
-                #if x.name in self.saved_fnames:
+                # if x.name in self.saved_fnames:
                 #    shutil.move(x, curr_wdir)
-                #else:
+                # else:
                 #    x.unlink()
-                shutil.move(x, curr_wdir) # save everything...
+                shutil.move(x, curr_wdir)  # save everything...
             else:
                 ...
 
         return curr_wdir
-    
+
     @abc.abstractmethod
     def _irun(self, atoms: Atoms, *args, **kwargs):
         """Prepare input structure (atoms) and parameters and run the simulation."""
 
         return
-    
+
     def _cleanup(self):
         """Remove unnecessary files.
 
         Some dynamics will not overwrite old files so cleanup is needed.
 
         """
         # retain calculator-related files
         for fname in self.removed_fnames:
-            curr_fpath = self.directory/fname
+            curr_fpath = self.directory / fname
             if curr_fpath.exists():
                 curr_fpath.unlink()
 
         return
 
     def _preprocess_constraints(self, atoms: Atoms, run_params: dict) -> None:
         """Remove existing constraints on atoms and add FixAtoms.
 
         If have cons in kwargs overwrite current cons stored in atoms.
 
         """
         # - check constraint
         cons_text = run_params.pop("constraint", None)
-        if cons_text is not None: # FIXME: check cons_text in parse_?
+        if cons_text is not None:  # FIXME: check cons_text in parse_?
             atoms._del_constraints()
             mobile_indices, frozen_indices = parse_constraint_info(
                 atoms, cons_text, ignore_ase_constraints=True, ret_text=False
             )
             if frozen_indices:
                 atoms.set_constraint(FixAtoms(indices=frozen_indices))
             else:
                 ...
         else:
             ...
 
         return
-    
-    def read_convergence(self, cache_traj: List[Atoms]=None, *args, **kwargs) -> bool:
+
+    def _prepare_velocities(
+        self, atoms: Atoms, velocity_seed: Optional[int], ignore_atoms_velocities: bool
+    ):
+        """"""
+        # - velocity
+        # NOTE: every dynamics will have a new rng...
+        if velocity_seed is None:
+            self._print(f"MD Driver's velocity_seed: {self.random_seed}")
+            vrng = np.random.Generator(np.random.PCG64(self.random_seed))
+        else:
+            self._print(f"MD Driver's velocity_seed: {velocity_seed}")
+            # vrng = np.random.default_rng(velocity_seed)
+            vrng = np.random.Generator(np.random.PCG64(velocity_seed))
+
+        if not ignore_atoms_velocities and atoms.get_kinetic_energy() > 0.0:
+            # use atoms attached momenta
+            ...
+        else:
+            # nve does not have temp in dyn_params so we use setting.temp
+            # for all ensembles just for consistency
+            target_temperature = self.setting.temp
+            MaxwellBoltzmannDistribution(
+                atoms, temperature_K=target_temperature, rng=vrng
+            )
+            if self.setting.remove_rotation:
+                ZeroRotation(atoms, preserve_temperature=False)
+            if self.setting.remove_translation:
+                Stationary(atoms, preserve_temperature=False)
+            # NOTE: respect constraints
+            #       ase code does not consider constraints
+            force_temperature(atoms, target_temperature, unit="K")
+
+        return
+
+    def read_convergence_from_trajectory(self, frames: List[Atoms], *args, **kwargs):
+        """"""
+        converged = False
+
+        num_frames = len(frames)
+        if num_frames == 0:
+            return converged
+
+        if self.setting.steps > 0:
+            step = frames[-1].info["step"]
+            self._debug(f"nframes: {num_frames}")
+            if self.setting.task == "min":
+                # NOTE: check geometric convergence (forces)...
+                #       some drivers does not store constraints in trajectories
+                # NOTE: Sometimes constraint changes if `lowest` is used.
+                frozen_indices = None
+                run_params = self.setting.get_run_params()
+                cons_text = run_params.pop("constraint", None)
+                mobile_indices, beg_frozen_indices = parse_constraint_info(
+                    frames[0], cons_text, ret_text=False
+                )
+                if beg_frozen_indices:
+                    frozen_indices = beg_frozen_indices
+                end_atoms = frames[-1]
+                if frozen_indices:
+                    mobile_indices, end_frozen_indices = parse_constraint_info(
+                        end_atoms, cons_text, ret_text=False
+                    )
+                    if convert_indices(end_frozen_indices) != convert_indices(
+                        beg_frozen_indices
+                    ):
+                        self._print(
+                            "Constraint changes after calculation, which may be from `lowest`. Most times it is fine."
+                        )
+                    end_atoms._del_constraints()
+                    end_atoms.set_constraint(FixAtoms(indices=frozen_indices))
+                # TODO: Different codes have different definition for the max force
+                maxfrc = np.max(np.fabs(end_atoms.get_forces(apply_constraint=True)))
+                if maxfrc <= self.setting.fmax or step + 1 >= self.setting.steps:
+                    converged = True
+                self._debug(
+                    f"MIN convergence: {converged} STEP: {step+1} >=? {self.setting.steps} MAXFRC: {maxfrc} <=? {self.setting.fmax}"
+                )
+            elif self.setting.task == "md":
+                if step + 1 >= self.setting.steps:  # step startswith 0
+                    converged = True
+                self._debug(
+                    f"MD convergence: {converged} STEP: {step+1} >=? {self.setting.steps}"
+                )
+            else:
+                raise NotImplementedError("Unknown task in read_convergence.")
+            # check if simulation stops early
+            earlystop = frames[-1].info.get(EARLYSTOP_KEY, False)
+            if earlystop:
+                converged = True
+                self._debug("  the simulation early stopped.")
+        else:
+            # just spc, only need to check force convergence
+            if num_frames == 1:
+                converged = True
+
+        return converged
+
+    def read_convergence(self, *args, **kwargs) -> bool:
         """Read output to check whether the simulation is converged.
 
         TODO:
             If not converged, specific params in input files should be updated.
 
         """
         if self.ignore_convergence:
             return True
 
-        # - check whether the driver is coverged
-        if cache_traj is None:
-            traj_frames = self.read_trajectory() # NOTE: DEAL WITH EMPTY FILE ERROR
+        # For some large simulations, the convergence check by reading the trajectory
+        # can be very time-consuming. Thus, we implement another way to check convergence
+        # by reading some lines in the logfile for some driver backends.
+        if not self.setting.check_trajectory_convergence and hasattr(
+            self, "read_convergence_from_logfile"
+        ):
+            converged = self.read_convergence_from_logfile()
         else:
-            traj_frames = cache_traj
-
-        # - check if this structure is bad
-        is_badstru = False
-        for a in traj_frames:
-            curr_is_badstru = a.info.get("is_badstru", False)
-            if curr_is_badstru:
-                is_badstru = True
-                break
-        else:
-            ...
+            # - check whether the driver is coverged
+            if self.cache_traj is None:
+                traj_frames = self.read_trajectory()  # NOTE: DEAL WITH EMPTY FILE ERROR
+            else:
+                traj_frames = self.cache_traj
 
-        if self.accept_bad_structure:
-            return True
-        else:
-            if is_badstru:
-                return False
+            # - check if this structure is bad
+            is_badstru = False
+            for a in traj_frames:
+                curr_is_badstru = a.info.get("is_badstru", False)
+                if curr_is_badstru:
+                    is_badstru = True
+                    break
             else:
                 ...
 
-        # - check actual convergence
-        nframes = len(traj_frames)
-
-        converged = False
-        if nframes > 0:
-            if self.setting.steps > 0:
-                step = traj_frames[-1].info["step"]
-                self._debug(f"nframes: {nframes}")
-                if self.setting.task == "min":
-                    # NOTE: check geometric convergence (forces)...
-                    #       some drivers does not store constraints in trajectories
-                    # NOTE: Sometimes constraint changes if `lowest` is used.
-                    frozen_indices = None
-                    run_params = self.setting.get_run_params()
-                    cons_text = run_params.pop("constraint", None)
-                    mobile_indices, beg_frozen_indices = parse_constraint_info(traj_frames[0], cons_text, ret_text=False)
-                    if beg_frozen_indices:
-                        frozen_indices = beg_frozen_indices
-                    end_atoms = traj_frames[-1]
-                    if frozen_indices:
-                        mobile_indices, end_frozen_indices = parse_constraint_info(end_atoms, cons_text, ret_text=False)
-                        if convert_indices(end_frozen_indices) != convert_indices(beg_frozen_indices):
-                            self._print("Constraint changes after calculation, which may be from `lowest`. Most times it is fine.")
-                        end_atoms._del_constraints()
-                        end_atoms.set_constraint(FixAtoms(indices=frozen_indices))
-                    # TODO: Different codes have different definition for the max force
-                    maxfrc = np.max(np.fabs(end_atoms.get_forces(apply_constraint=True)))
-                    if maxfrc <= self.setting.fmax or step+1 >= self.setting.steps:
-                        converged = True
-                    self._debug(
-                        f"MIN convergence: {converged} STEP: {step+1} >=? {self.setting.steps} MAXFRC: {maxfrc} <=? {self.setting.fmax}"
-                    )
-                elif self.setting.task == "md":
-                    if step+1 >= self.setting.steps: # step startswith 0
-                        converged = True
-                    self._debug(f"MD convergence: {converged} STEP: {step+1} >=? {self.setting.steps}")
-                else:
-                    raise NotImplementedError("Unknown task in read_convergence.")
+            if self.accept_bad_structure:
+                return True
             else:
-                # just spc, only need to check force convergence
-                if nframes == 1:
-                    converged = True
-            # self._print(f"energy: {traj_frames[-1].get_potential_energy():12.4f}")
-        else:
-            ...
+                if is_badstru:
+                    return False
+                else:
+                    ...
+
+            # check actual convergence
+            converged = self.read_convergence_from_trajectory(traj_frames)
 
         return converged
 
     @abc.abstractmethod
     def read_trajectory(self, *args, **kwargs) -> List[Atoms]:
-        """Read trajectory in the current working directory.
-        """
+        """Read trajectory in the current working directory."""
 
         return
-    
-    def _aggregate_trajectories(self, archive_path=None) -> List[Atoms]:
+
+    def _aggregate_trajectories(
+        self, check_energy: bool = False, archive_path=None, *args, **kwargs
+    ) -> List[Atoms]:
         """"""
         prev_wdirs = []
         if archive_path is None:
             prev_wdirs = sorted(self.directory.glob(r"[0-9][0-9][0-9][0-9][.]run"))
         else:
             pattern = self.directory.name + "/" + r"[0-9][0-9][0-9][0-9][.]run"
             with tarfile.open(archive_path, "r:gz") as tar:
                 for tarinfo in tar:
                     if tarinfo.isdir() and re.match(pattern, tarinfo.name):
                         prev_wdirs.append(tarinfo.name)
-            prev_wdirs = [self.directory/pathlib.Path(p).name for p in sorted(prev_wdirs)]
-        self._debug(f"prev_wdirs: {prev_wdirs}")
+            prev_wdirs = [
+                self.directory / pathlib.Path(p).name for p in sorted(prev_wdirs)
+            ]
+        self._debug(f"prev_wdirs@{self.directory.name}: {prev_wdirs}")
 
         all_wdirs = prev_wdirs + [self.directory]
 
         traj_list = []
         for w in all_wdirs:
-            curr_frames = self._read_a_single_trajectory(w, archive_path=archive_path)
+            curr_frames = self._read_a_single_trajectory(
+                w, archive_path=archive_path, **kwargs
+            )
             if curr_frames:
                 traj_list.append(curr_frames)
 
         # -- concatenate
         # NOTE: For DFT calculations,
         #       some spin systems may give different scf convergence on the same
         #       structure. Sometimes, the preivous failed but the next run converged,
-        #       The concat below uses the previous one...
-        traj_frames, ntrajs = [], len(traj_list)
-        if ntrajs > 0:
+        #       The concat below uses the latest one...
+        # FIXME: Check if energies are consistent? DFT spin energy inconsistent see above?
+        traj_frames, num_trajs = [], len(traj_list)
+        if num_trajs == 1:
             traj_frames.extend(traj_list[0])
-            for i in range(1, ntrajs):
+        elif num_trajs > 1:
+            for i in range(1, num_trajs):
+                curr_beg_frame = traj_list[i][0]
+                curr_beg_step = curr_beg_frame.info["step"]
+                prev_steps = [a.info["step"] for a in traj_list[i - 1]]
+                prev_traj = traj_list[i - 1][: prev_steps.index(curr_beg_step) + 1]
+                prev_end_frame = prev_traj[-1]
                 assert np.allclose(
-                    traj_list[i - 1][-1].positions, traj_list[i][0].positions
-                ), f"Traj {i-1} and traj {i} are not consecutive."
-                traj_frames.extend(traj_list[i][1:])
+                    prev_end_frame.positions, curr_beg_frame.positions
+                ), f"{self.directory.name} Traj {i-1} and traj {i} are not consecutive in positions."
+                if check_energy:
+                    assert np.allclose(
+                        prev_end_frame.get_potential_energy(),
+                        curr_beg_frame.get_potential_energy(),
+                    ), f"{self.directory.name} Traj {i-1} and traj {i} are not consecutive in energy."
+                traj_frames.extend(prev_traj[:-1])
+            traj_frames.extend(traj_list[-1])
         else:
             ...
 
-        return traj_frames
-    
+        # We only keep structures at dump_period and the last one.
+        # If ckpt_period != dump_period, sometimes the structure at ckpt_period is
+        # only save but we do not need it so remove it here!
+        frames = []
+        for a in traj_frames:
+            if a.info["step"] % self.setting.dump_period == 0:
+                frames.append(a)
+        if traj_frames[-1].info["step"] % self.setting.dump_period != 0:
+            frames.append(traj_frames[-1])
+
+        return frames
+
     def as_dict(self) -> dict:
         """Return parameters of this driver."""
         params = dict(
-            backend = self.name,
-            ignore_convergence = self.ignore_convergence,
-            random_seed=self.random_seed
+            backend=self.name,
+            ignore_convergence=self.ignore_convergence,
+            random_seed=self.random_seed,
         )
-        # NOTE: we use original params otherwise internal param names would be 
+        # NOTE: we use original params otherwise internal param names would be
         #       written out and make things confusing
         #       org_params are merged params thatv have init and run sections
         org_params = copy.deepcopy(self._org_params)
 
         # - update some special parameters
         constraint = self.setting.constraint
         org_params["constraint"] = constraint
```

### Comparing `gdpx-0.0.8/src/gdpx/computation/espresso.py` & `gdpx-0.0.9/src/gdpx/computation/espresso.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/computation/interface.py` & `gdpx-0.0.9/src/gdpx/computation/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,24 +32,31 @@
 
 
 @registers.variable.register
 class DriverVariable(Variable):
 
     def __init__(self, **kwargs):
         """"""
-        # - compat
         copied_params = copy.deepcopy(kwargs)
         merged_params = dict(
-            # task=copied_params.get("task", "min"),
             backend=copied_params.get("backend", "external"),
             ignore_convergence=copied_params.get("ignore_convergence", False),
         )
         merged_params.update(**copied_params.get("init", {}))
         merged_params.update(**copied_params.get("run", {}))
 
+        # HACK: Computer and Reactor both use this variable
+        #       but Reactor does not have task keyword for now
+        #       we need update it later.
+        task = copied_params.get("task", "")
+        if task:
+            merged_params.update(task=task)
+        else:
+            ...
+
         initial_value = self._broadcast_drivers(merged_params)
 
         super().__init__(initial_value)
 
         return
 
     def _broadcast_drivers(self, params: dict) -> List[dict]:
```

### Comparing `gdpx-0.0.8/src/gdpx/computation/lammps.py` & `gdpx-0.0.9/src/gdpx/computation/lammps.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,66 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import os
 import copy
+import dataclasses
 import io
 import itertools
-import shutil
-import warnings
-import subprocess
+import os
 import pathlib
 import pickle
+import shutil
 import tarfile
-import dataclasses
-
+import traceback
 from collections.abc import Iterable
-from typing import List, Mapping, Dict, Optional, NoReturn, Tuple
+from typing import Dict, List, Mapping, NoReturn, Optional, Tuple
 
 import numpy as np
-
-from ase import Atoms
-from ase import units
-from ase.data import atomic_numbers, atomic_masses
-from ase.io import read, write
-from ase.io.lammpsrun import read_lammps_dump_text
-from ase.io.lammpsdata import read_lammps_data, write_lammps_data
-from ase.calculators.lammps import unitconvert, Prism
-from ase.calculators.calculator import (
-    CalculationFailed,
-    Calculator, all_changes, PropertyNotImplementedError, FileIOCalculator
-)
-from ase.calculators.singlepoint import SinglePointCalculator
+from ase import Atoms, units
+from ase.calculators.calculator import FileIOCalculator, all_changes
+from ase.calculators.lammps import Prism, unitconvert
 from ase.calculators.mixing import LinearCombinationCalculator
+from ase.calculators.singlepoint import SinglePointCalculator
+from ase.data import atomic_masses, atomic_numbers
+from ase.io import read, write
+from ase.io.lammpsdata import write_lammps_data
 
 from .. import config
 from ..builder.constraints import parse_constraint_info
-from .driver import AbstractDriver, DriverSetting
-
-from ..potential.managers.plumed.calculators.plumed2 import Plumed, update_stride_and_file
+from ..potential.managers.plumed.calculators.plumed2 import (
+    Plumed, update_stride_and_file)
+from .driver import AbstractDriver, Controller, DriverSetting
 
 
-dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True)
 class AseLammpsSettings:
-
     """File names."""
 
     inputstructure_filename: str = "stru.data"
     trajectory_filename: str = "traj.dump"
     input_fname: str = "in.lammps"
-    log_filename: str = "log.lammps"
+    # log_filename: str = "log.lammps"
+    log_filename: str = "lmp.out"
     deviation_filename: str = "model_devi.out"
     prism_filename: str = "ase-prism.bindat"
 
+
 #: Instance.
 ASELMPCONFIG = AseLammpsSettings()
 
+
 def parse_type_list(atoms):
     """Parse the type list based on input atoms."""
     # elements
     type_list = list(set(atoms.get_chemical_symbols()))
-    type_list.sort() # by alphabet
+    type_list.sort()  # by alphabet
 
     return type_list
 
+
 def parse_thermo_data(lines) -> dict:
     """Read energy ... results from log.lammps file."""
     # - parse input lines
     found_error = False
     start_idx, end_idx = None, None
     for idx, line in enumerate(lines):
         # - get the line index at the start of the thermo infomation
@@ -78,596 +73,839 @@
             end_idx = idx
         if line.strip().startswith("Loop time"):
             end_idx = idx
         if start_idx is not None and end_idx is not None:
             break
     else:
         end_idx = idx
-    config._debug(f"Initial lammps LOG index: {start_idx} {end_idx}")
-    
+    config._debug(f"INITIAL LAMMPS LOG INDEX: {start_idx} {end_idx}")
+
     # - check valid lines
     #   sometimes the line may not be complete
     ncols = len(lines[start_idx].strip().split())
     for i in range(end_idx, start_idx, -1):
         curr_data = lines[i].strip().split()
         curr_ncols = len(curr_data)
-        config._debug(f"Error: {lines[i]}")
-        if curr_ncols == ncols: # still log step info and no LOOP
+        config._debug(f"  LAMMPS LINE: {lines[i].strip()}")
+        if curr_ncols == ncols:  # The Line has the full thermo info...
             try:
                 step = int(curr_data[0])
-                end_idx = i+1
+                end_idx = i + 1
             except ValueError:
-                config._debug(f"Error: {lines[i]}")
+                ...
             finally:
+                end_info = lines[i].strip()
+                config._debug(f"  LAMMPS STEP: {end_info}")
                 break
         else:
             ...
     else:
-        end_idx = None # even not one single complete line
-    config._debug(f"Sanitised lammps LOG index: {start_idx} {end_idx}")
+        end_idx = None  # even not one single complete line
+    config._debug(f"FINAL   LAMMPS LOG INDEX: {start_idx} {end_idx}")
 
     if start_idx is None or end_idx is None:
-        raise RuntimeError(f"Error in lammps output with start {start_idx} end {end_idx}.")
-    end_info = lines[end_idx] # either loop time or error
-    config._debug(f"lammps END info: {end_info}")
-
-    config._debug(f"lammps LOG index: {start_idx} {end_idx}")
+        raise RuntimeError(f"ERROR   LAMMPS LOG INDEX {start_idx} {end_idx}.")
 
     # -- parse index of PotEng
     # TODO: save timestep info?
     thermo_keywords = lines[start_idx].strip().split()
     if "PotEng" not in thermo_keywords:
         raise RuntimeError(f"Cant find PotEng in lammps output.")
     thermo_data = []
-    for x in lines[start_idx+1:end_idx]:
+    for x in lines[start_idx + 1 : end_idx]:
         x_data = x.strip().split()
-        if x_data[0].isdigit(): # There may have some extra warnings... such as restart
+        if x_data[0].isdigit():  # There may have some extra warnings... such as restart
             thermo_data.append(x_data)
-    #thermo_data = np.array([line.strip().split() for line in thermo_data], dtype=float).transpose()
-    thermo_data = np.array(thermo_data, dtype=float).transpose() 
-    #config._debug(thermo_data)
+    # thermo_data = np.array([line.strip().split() for line in thermo_data], dtype=float).transpose()
+    thermo_data = np.array(thermo_data, dtype=float).transpose()
+    # config._debug(thermo_data)
     thermo_dict = {}
     for i, k in enumerate(thermo_keywords):
         thermo_dict[k] = thermo_data[i]
 
     return thermo_dict, end_info
 
-def read_single_simulation(
-        mdir, wdir: pathlib.Path, prefix: str, units: str, add_step_info=True,
-        archive_path: pathlib.Path=None
-    ):
-    """"""
-    # - get FileIO
-    if archive_path is None:
-        traj_io = open(wdir/ASELMPCONFIG.trajectory_filename, "r")
-        log_io = open(wdir/ASELMPCONFIG.log_filename, "r")
-        prism_file = wdir/ASELMPCONFIG.prism_filename
-        if prism_file.exists():
-            prism_io = open(prism_file, "rb")
-        else:
-            prism_io = None
-        devi_path = wdir / (prefix+ASELMPCONFIG.deviation_filename)
-        if devi_path.exists():
-            devi_io = open(devi_path, "r")
-        else:
-            devi_io = None
-        colvar_path = wdir/"COLVAR"
-        if colvar_path.exists():
-            colvar_io = open(colvar_path, "r")
-        else:
-            colvar_io = None
-    else:
-        rpath = wdir.relative_to(mdir.parent)
-        traj_tarname = str(rpath/ASELMPCONFIG.trajectory_filename)
-        prism_tarname = str(rpath/ASELMPCONFIG.prism_filename)
-        log_tarname = str(rpath/ASELMPCONFIG.log_filename)
-        devi_tarname = str(rpath/ASELMPCONFIG.deviation_filename)
-        colvar_tarname = str(rpath/"COLVAR")
-        prism_io, devi_io, colvar_io = None, None, None
-        with tarfile.open(archive_path, "r:gz") as tar:
-            for tarinfo in tar:
-                if tarinfo.name.startswith(wdir.name):
-                    if tarinfo.name == traj_tarname:
-                        traj_io = io.StringIO(tar.extractfile(tarinfo.name).read().decode())
-                    elif tarinfo.name == prism_tarname:
-                        prism_io = io.BytesIO(tar.extractfile(tarinfo.name).read())
-                    elif tarinfo.name == log_tarname:
-                        log_io = io.StringIO(tar.extractfile(tarinfo.name).read().decode())
-                    elif tarinfo.name == devi_tarname:
-                        devi_io = io.StringIO(tar.extractfile(tarinfo.name).read().decode())
-                    elif tarinfo.name == colvar_tarname:
-                        colvar_io = io.StringIO(tar.extractfile(tarinfo.name).read().decode())
-                    else:
-                        ...
-                else:
-                    continue
-            else: # TODO: if not find target traj?
-                ...
 
-    # - read timesteps
-    timesteps = []
-    while True:
-        line = traj_io.readline()
-        if "TIMESTEP" in line:
-            timesteps.append(int(traj_io.readline().strip()))
-        if not line:
-            break
-    traj_io.seek(0)
+@dataclasses.dataclass
+class FireMinimizer(Controller):
 
-    # - read structure trajectory
-    if prism_io is not None:
-        prismobj = pickle.load(prism_io)
-    else:
-        prismobj = None
+    name: str = "fire"
 
-    curr_traj_frames_ = read(
-        traj_io, 
-        index=":", format="lammps-dump-text", prismobj=prismobj, units=units
-    )
-    nframes_traj = len(curr_traj_frames_)
-    timesteps = timesteps[:nframes_traj] # avoid incomplete structure
+    def __post_init__(self):
+        """"""
+        self.conv_params = dict(
+            min_style="fire",
+            min_modify=self.params.get("min_modify", "integrator verlet tmax 4"),
+        )
 
-    # - read thermo data
-    thermo_dict, end_info = parse_thermo_data(log_io.readlines())
+        return
 
-    # NOTE: last frame would not be dumpped if timestep not equals multiple*dump_period
-    #       if there were any error, 
-    pot_energies = [unitconvert.convert(p, "energy", units, "ASE") for p in thermo_dict["PotEng"]]
-    nframes_thermo = len(pot_energies)
-    nframes = min([nframes_traj, nframes_thermo])
-    config._debug(f"nframes in lammps: {nframes} traj {nframes_traj} thermo {nframes_thermo}")
-
-    # NOTE: check whether steps in thermo and traj are consistent
-    #pot_energies = pot_energies[:nframes]
-    #curr_traj_frames = curr_traj_frames[:nframes]
-    #assert len(pot_energies) == len(curr_traj_frames), f"Number of pot energies and frames are inconsistent at {str(wdir)}."
-
-    curr_traj_frames, curr_energies = [], []
-    for i, t in enumerate(timesteps):
-        if t in thermo_dict["Step"]:
-            curr_atoms = curr_traj_frames_[i]
-            curr_atoms.info["step"] = t
-            curr_traj_frames.append(curr_atoms)
-            curr_energies.append(pot_energies[thermo_dict["Step"].tolist().index(t)])
-
-    for pot_eng, atoms in zip(curr_energies, curr_traj_frames):
-        forces = atoms.get_forces()
-        # NOTE: forces have already been converted in ase read, so velocities are
-        sp_calc = SinglePointCalculator(atoms, energy=pot_eng, forces=forces)
-        atoms.calc = sp_calc
-
-    # - check model_devi.out
-    # TODO: convert units?
-    if devi_io is not None:
-        lines = devi_io.readlines()
-        if "#" in lines[0]: # the first file
-            dkeys = ("".join([x for x in lines[0] if x != "#"])).strip().split()
-            dkeys = [x.strip() for x in dkeys][1:]
-        else:
-            ...
-        devi_io.seek(0)
-        data = np.loadtxt(devi_io, dtype=float)
-        ncols = data.shape[-1]
-        data = data.reshape(-1, ncols)
-        # NOTE: For some minimisers, dp gives several deviations as 
-        #       multiple force evluations are performed in one step.
-        #       Thus, we only take the last occurance of the deviation in each step.
-        step_indices = []
-        steps = data[:, 0].astype(np.int32).tolist()
-        for k, v in itertools.groupby(enumerate(steps), key=lambda x: x[1]):
-            v = sorted(v, key=lambda x: x[0])
-            step_indices.append(v[-1][0])
-        data = data.transpose()[1:, step_indices[:nframes]]
-        #config._print(data)
-
-        for i, atoms in enumerate(curr_traj_frames):
-            for j, k in enumerate(dkeys):
-                try:
-                    atoms.info[k] = data[j,i]
-                except IndexError:
-                    # NOTE: Some potentials donot print last frames of min
-                    #       for example, lammps
-                    atoms.info[k] = 0.
-    else:
-        ...
-    
-    # - check COLVAR
-    if colvar_io is not None:
-        # - read latest COLVAR Files
-        names = colvar_io.readline().split()[2:]
-        colvar_io.seek(0)
-        colvars = np.loadtxt(colvar_io)
-        #print("colvars: ", colvars.shape)
-        curr_colvars = colvars[-nframes_traj:, :]
-        for i, atoms in enumerate(curr_traj_frames):
-            for k, v in zip(names, curr_colvars[i, :]):
-                atoms.info[k] = v
-    
-    # - Close IO
-    traj_io.close()
-    log_io.close()
-    if prism_io is not None:
-        prism_io.close()
-    if devi_io is not None:
-        devi_io.close()
-    if colvar_io is not None:
-        colvar_io.close()
 
-    return curr_traj_frames
+@dataclasses.dataclass
+class LangevinThermostat(Controller):
+
+    name: str = "langevin"
+
+    def __post_init__(self):
+        """"""
+        friction = self.params.get("friction", 0.01)  # fs^-1
+        assert friction is not None
+
+        friction_seed = self.params.get("friction_seed", None)
+
+        self.conv_params = dict(
+            damp=unitconvert.convert(1.0 / friction, "time", "real", self.units)
+        )
+        if friction_seed is not None:
+            self.conv_params.update(seed=friction_seed)
+
+        return
+
+
+@dataclasses.dataclass
+class NoseHooverChainThermostat(Controller):
+
+    name: str = "nose_hoover_chain"
+
+    def __post_init__(self):
+        """"""
+        Tdamp = self.params.get("Tdamp", 100.0)
+        assert Tdamp is not None
+
+        self.conv_params = dict(
+            Tdamp=unitconvert.convert(Tdamp, "time", "real", self.units)
+        )
+
+        return
+
+
+@dataclasses.dataclass
+class ParrinelloRahmanBarostat(Controller):
+
+    name: str = "parrinello_rahman"
+
+    def __post_init__(self):
+        """"""
+        Tdamp = self.params.get("Tdamp", 100.0)
+        assert Tdamp is not None
+
+        Pdamp = self.params.get("Pdamp", 100.0)
+        assert Pdamp is not None
+
+        self.conv_params = dict(
+            Tdamp=unitconvert.convert(Tdamp, "time", "real", self.units),
+            Pdamp=unitconvert.convert(Pdamp, "time", "real", self.units),
+        )
+
+        return
+
+
+controllers = dict(
+    # nvt
+    langevin_nvt=LangevinThermostat,
+    nose_hoover_chain_nvt=NoseHooverChainThermostat,
+    parrinello_rahman_npt=ParrinelloRahmanBarostat,
+)
+
 
 @dataclasses.dataclass
 class LmpDriverSetting(DriverSetting):
 
-    min_style: str = "fire"
-    min_modify: str = "integrator verlet tmax 4"
+    units: str = "metal"
+
+    ensemble: str = "nve"
+
+    controller: dict = dataclasses.field(default_factory=dict)
+
+    use_lmpvel: bool = True
 
     etol: float = 0
     fmax: float = 0.05
 
     neighbor: str = "0.0 bin"
-    neigh_modify: str = None
+    neigh_modify: Optional[str] = None
 
     extra_fix: List[str] = dataclasses.field(default_factory=list)
 
-    plumed: str = None
+    plumed: Optional[str] = None
 
     def __post_init__(self):
         """"""
         if self.task == "min":
             self._internals.update(
-                min_style = self.min_style,
-                min_modify = self.min_modify,
-                etol = self.etol,
-                ftol = self.fmax,
-                #maxstep = self.maxstep
+                etol=self.etol,
+                ftol=self.fmax,
             )
-        
+
         if self.task == "md":
             self._internals.update(
-                md_style = self.md_style,
-                timestep = self.timestep,
-                velocity_seed = self.velocity_seed,
-                ignore_atoms_velocities = self.ignore_atoms_velocities,
-                remove_rotation = self.remove_rotation,
-                remove_translation = self.remove_translation,
-                temp = self.temp,
-                # TODO: end temperature
-                Tdamp = self.Tdamp,
-                press = self.press,
-                Pdamp = self.Pdamp,
-                # - ext
-                plumed = self.plumed,
+                plumed=self.plumed,
             )
-        
-        # - shared params
-        self._internals.update(
-            task = self.task,
-            dump_period = self.dump_period,
-            ckpt_period = self.ckpt_period
-        )
 
         # - special params
         self._internals.update(
-            neighbor = self.neighbor,
-            neigh_modify = self.neigh_modify,
-            extra_fix = self.extra_fix
+            neighbor=self.neighbor,
+            neigh_modify=self.neigh_modify,
+            extra_fix=self.extra_fix,
+        )
+
+        return
+
+    def get_minimisation_inputs(self, random_seed, group: str = "mobile") -> List[str]:
+        """"""
+        """Convert parameters into lammps input lines."""
+        MIN_FIX_ID: str = "controller"
+        _init_min_params = dict(
+            fix_id=MIN_FIX_ID,
+            group=group,
+        )
+        if self.controller:
+            min_cls_name = self.controller["name"] + "_min"
+            min_cls = controllers[min_cls_name]
+        else:
+            min_cls = FireMinimizer
+
+        minimiser = min_cls(units=self.units, **self.controller)
+        _init_min_params.update(**minimiser.conv_params)
+
+        if minimiser.name == "fire":
+            min_line = "min_style  {min_style}\nmin_modify {min_modify}".format(
+                **_init_min_params
+            )
+        else:
+            raise RuntimeError(f"Unknown minimiser {minimiser}.")
+
+        lines = [min_line]
+
+        return lines
+
+    def get_molecular_dynamics_inputs(
+        self, random_seed, group: str = "mobile"
+    ) -> List[str]:
+        """Convert parameters into lammps input lines."""
+        MD_FIX_ID: str = "controller"
+        _init_md_params = dict(
+            fix_id=MD_FIX_ID,
+            group=group,
+            timestep=unitconvert.convert(self.timestep, "time", "real", self.units),
         )
 
-        return 
-    
+        if self.ensemble == "nve":
+            lines = [
+                "fix {fix_id:>24s} {group} nve".format(**_init_md_params),
+                f"timestep {_init_md_params['timestep']}",
+            ]
+        elif self.ensemble == "nvt":
+            _init_md_params.update(
+                Tstart=self.temp,
+                Tstop=self.temp,  # FIXME: end temperature??
+            )
+            if self.controller:
+                thermo_cls_name = self.controller["name"] + "_" + self.ensemble
+                thermo_cls = controllers[thermo_cls_name]
+            else:
+                thermo_cls = LangevinThermostat
+            thermostat = thermo_cls(units=self.units, **self.controller)
+            if thermostat.name == "langevin":
+                _init_md_params.update(
+                    seed=random_seed,
+                )
+                _init_md_params.update(**thermostat.conv_params)
+                thermo_line = "fix {fix_id:>24s}0 {group} nve\n".format(
+                    **_init_md_params
+                )
+                thermo_line += "fix {fix_id:>24s}1 {group} langevin {Tstart} {Tstop} {damp} {seed}".format(
+                    **_init_md_params
+                )
+            elif thermostat.name == "nose_hoover_chain":
+                _init_md_params.update(**thermostat.conv_params)
+                thermo_line = "fix {fix_id:>24s} {group} nvt temp {Tstart} {Tstop} {Tdamp}".format(
+                    **_init_md_params
+                )
+            else:
+                raise RuntimeError(f"Unknown thermostat {thermostat}.")
+            lines = [thermo_line, f"timestep {_init_md_params['timestep']}"]
+        elif self.ensemble == "npt":
+            _init_md_params.update(
+                Tstart=self.temp,
+                Tstop=self.temp,  # FIXME: end temperature??
+                Pstart=self.press,
+                Pstop=self.press,  # FIXME: end pressure??
+            )
+            if self.controller:
+                baro_cls_name = self.controller["name"] + "_" + self.ensemble
+                baro_cls = controllers[baro_cls_name]
+            else:
+                ...
+            barostat = baro_cls(units=self.units, **self.controller)
+            if barostat.name == "parrinello_rahman":
+                _init_md_params.update(**barostat.conv_params)
+                baro_line = "fix {fix_id:>24s} {group} npt temp {Tstart} {Tstop} {Tdamp} aniso {Pstart} {Pstop} {Pdamp}".format(
+                    **_init_md_params
+                )
+            else:
+                raise RuntimeError(f"Unknown barostat {barostat}.")
+            lines = [baro_line, f"timestep {_init_md_params['timestep']}"]
+        else:
+            raise RuntimeError(f"Unknown ensemble {self.ensemble}.")
+
+        return lines
+
     def get_run_params(self, *args, **kwargs):
         """"""
         # - pop out special keywords
         # convergence criteria
         ftol_ = kwargs.pop("fmax", self.fmax)
         etol_ = kwargs.pop("etol", self.etol)
         if etol_ is None:
-            etol_ = 0.
+            etol_ = 0.0
         if ftol_ is None:
-            ftol_ = 0.
+            ftol_ = 0.0
 
         steps_ = kwargs.pop("steps", self.steps)
 
         run_params = dict(
-            constraint = kwargs.get("constraint", self.constraint),
-            etol=etol_, ftol=ftol_, maxiter=steps_, maxeval=2*steps_
+            steps=steps_,
+            constraint=kwargs.get("constraint", self.constraint),
+            etol=etol_,
+            ftol=ftol_,
         )
 
         # - add extra parameters
-        run_params.update(
-            **kwargs
-        )
+        run_params.update(**kwargs)
 
         return run_params
 
-class LmpDriver(AbstractDriver):
 
+class LmpDriver(AbstractDriver):
     """Use lammps to perform dynamics.
-    
+
     Minimisation and/or molecular dynamics.
 
     """
 
     name = "lammps"
 
     special_keywords = {}
 
     default_task = "min"
     supported_tasks = ["min", "md"]
 
     #: List of output files would be saved when restart.
-    saved_fnames: List[str] = [ASELMPCONFIG.log_filename, ASELMPCONFIG.trajectory_filename, ASELMPCONFIG.deviation_filename]
+    saved_fnames: List[str] = [
+        ASELMPCONFIG.log_filename,
+        ASELMPCONFIG.trajectory_filename,
+        ASELMPCONFIG.deviation_filename,
+    ]
 
     def __init__(self, calc, params: dict, directory="./", *args, **kwargs):
         """"""
         calc, params = self._check_plumed(calc=calc, params=params)
 
         super().__init__(calc, params, directory=directory, *args, **kwargs)
+
+        params.update(units=calc.units)
         self.setting = LmpDriverSetting(**params)
 
         return
-    
+
     def _check_plumed(self, calc, params: dict):
         """"""
         new_calc, new_params = calc, params
         if isinstance(calc, LinearCombinationCalculator):
             ncalcs = len(calc.calcs)
             assert ncalcs == 2, "Number of calculators should be 2."
             if isinstance(calc.calcs[0], Lammps) and isinstance(calc.calcs[1], Plumed):
                 new_calc = calc.calcs[0]
                 new_params = copy.deepcopy(params)
                 new_params["plumed"] = "".join(calc.calcs[1].input)
 
         return new_calc, new_params
-    
+
     def _verify_checkpoint(self, *args, **kwargs) -> bool:
         """"""
         verified = super()._verify_checkpoint(*args, **kwargs)
         if verified:
             checkpoints = list(self.directory.glob("restart.*"))
             self._debug(f"checkpoints: {checkpoints}")
             if not checkpoints:
                 verified = False
         else:
             ...
 
         return verified
 
+    def _create_dynamics(self, atoms: Atoms, *args, **kwargs):
+        """Convert parameters into lammps input lines."""
+        lines = []
+        if self.setting.task == "min":
+            dynamics = self.setting.get_minimisation_inputs(
+                random_seed=self.random_seed
+            )
+            lines.extend(dynamics)
+        else:  # assume md
+            # NOTE: Velocities by ASE may lose precision as
+            #       they are first written to data file and read by lammps then
+            if self.setting.use_lmpvel:
+                velocity_seed = self.setting.velocity_seed
+                if velocity_seed is None:
+                    velocity_seed = self.random_seed
+                self._print(f"MD Driver's velocity_seed: {velocity_seed}")
+                line = f"velocity        mobile create {self.setting.temp} {velocity_seed} dist gaussian "
+                if self.setting.remove_translation:
+                    line += "mom yes "
+                if self.setting.remove_rotation:
+                    line += "rot yes "
+                if atoms.get_kinetic_energy() > 0.0:
+                    if self.setting.ignore_atoms_velocities:
+                        atoms.set_momenta(np.zeros(atoms.positions.shape))
+                        lines.append(line)
+                    else:
+                        lines.append("# Use atoms' velocities.")
+                else:
+                    atoms.set_momenta(np.zeros(atoms.positions.shape))
+                    lines.append(line)
+            else:
+                self._prepare_velocities(
+                    atoms,
+                    self.setting.velocity_seed,
+                    self.setting.ignore_atoms_velocities,
+                )
+            dynamics = self.setting.get_molecular_dynamics_inputs(
+                random_seed=self.random_seed
+            )
+            lines.extend(dynamics)
+
+        return lines
+
     def _irun(self, atoms: Atoms, ckpt_wdir=None, *args, **kwargs):
         """"""
         try:
-            # - params
             run_params = self.setting.get_init_params()
             run_params.update(**self.setting.get_run_params(**kwargs))
 
-            if ckpt_wdir is None: # start from the scratch
+            if ckpt_wdir is None:  # start from the scratch
                 ...
             else:
-                checkpoints = sorted(list(ckpt_wdir.glob("restart.*")), key=lambda x: int(x.name.split(".")[1]))
+                checkpoints = sorted(
+                    list(ckpt_wdir.glob("restart.*")),
+                    key=lambda x: int(x.name.split(".")[1]),
+                )
                 self._debug(f"checkpoints to restart: {checkpoints}")
-                target_steps = run_params["maxiter"]
+                target_steps = run_params["steps"]
                 run_params.update(
-                    read_restart = str(checkpoints[-1].resolve()),
-                    maxiter = target_steps - int(checkpoints[-1].name.split(".")[1])
+                    read_restart=str(checkpoints[-1].resolve()),
+                    steps=target_steps - int(checkpoints[-1].name.split(".")[1]),
                 )
+                # shutil.move(
+                #     checkpoints[-1].parent / "traj.dump", self.directory / "traj.dump"
+                # )
+
+            dynamics = self._create_dynamics(atoms, *args, **kwargs)
 
             # - check constraint
-            self.calc.set(**run_params)
+            self.calc.set(
+                task=self.setting.task,
+                dump_period=self.setting.dump_period,
+                ckpt_period=self.setting.ckpt_period,
+                dynamics=dynamics,
+                steps=run_params["steps"],
+                constraint=run_params["constraint"],
+                etol=run_params["etol"],
+                ftol=run_params["ftol"],
+                # misc
+                read_restart=run_params.get("read_restart", None),
+                extra_fix=run_params["extra_fix"],  # e.g. fixcm
+                neighbor=run_params["neighbor"],
+                neighb_modify=run_params["neigh_modify"],
+            )
             atoms.calc = self.calc
 
             # - run
             _ = atoms.get_forces()
         except Exception as e:
-            config._debug(e)
+            config._debug(traceback.format_exc())
 
         return
-    
+
+    @staticmethod
+    def _read_a_single_trajectory(
+        wdir: pathlib.Path,
+        mdir,
+        units: str,
+        archive_path: pathlib.Path = None,
+        *args,
+        **kwargs,
+    ):
+        """"""
+        # - get FileIO
+        if archive_path is None:
+            traj_io = open(wdir / ASELMPCONFIG.trajectory_filename, "r")
+            log_io = open(wdir / ASELMPCONFIG.log_filename, "r")
+            prism_file = wdir / ASELMPCONFIG.prism_filename
+            if prism_file.exists():
+                prism_io = open(prism_file, "rb")
+            else:
+                prism_io = None
+            devi_path = wdir / (ASELMPCONFIG.deviation_filename)
+            if devi_path.exists():
+                devi_io = open(devi_path, "r")
+            else:
+                devi_io = None
+            colvar_path = wdir / "COLVAR"
+            if colvar_path.exists():
+                colvar_io = open(colvar_path, "r")
+            else:
+                colvar_io = None
+        else:
+            rpath = wdir.relative_to(mdir.parent)
+            traj_tarname = str(rpath / ASELMPCONFIG.trajectory_filename)
+            prism_tarname = str(rpath / ASELMPCONFIG.prism_filename)
+            log_tarname = str(rpath / ASELMPCONFIG.log_filename)
+            devi_tarname = str(rpath / ASELMPCONFIG.deviation_filename)
+            colvar_tarname = str(rpath / "COLVAR")
+            prism_io, devi_io, colvar_io = None, None, None
+            with tarfile.open(archive_path, "r:gz") as tar:
+                for tarinfo in tar:
+                    if tarinfo.name.startswith(wdir.name):
+                        if tarinfo.name == traj_tarname:
+                            traj_io = io.StringIO(
+                                tar.extractfile(tarinfo.name).read().decode()
+                            )
+                        elif tarinfo.name == prism_tarname:
+                            prism_io = io.BytesIO(tar.extractfile(tarinfo.name).read())
+                        elif tarinfo.name == log_tarname:
+                            log_io = io.StringIO(
+                                tar.extractfile(tarinfo.name).read().decode()
+                            )
+                        elif tarinfo.name == devi_tarname:
+                            devi_io = io.StringIO(
+                                tar.extractfile(tarinfo.name).read().decode()
+                            )
+                        elif tarinfo.name == colvar_tarname:
+                            colvar_io = io.StringIO(
+                                tar.extractfile(tarinfo.name).read().decode()
+                            )
+                        else:
+                            ...
+                    else:
+                        continue
+                else:  # TODO: if not find target traj?
+                    ...
+
+        # - read timesteps
+        timesteps = []
+        while True:
+            line = traj_io.readline()
+            if "TIMESTEP" in line:
+                timesteps.append(int(traj_io.readline().strip()))
+            if not line:
+                break
+        traj_io.seek(0)
+
+        # - read structure trajectory
+        if prism_io is not None:
+            prismobj = pickle.load(prism_io)
+        else:
+            prismobj = None
+
+        curr_traj_frames_ = read(
+            traj_io,
+            index=":",
+            format="lammps-dump-text",
+            prismobj=prismobj,
+            units=units,
+        )
+        nframes_traj = len(curr_traj_frames_)
+        timesteps = timesteps[:nframes_traj]  # avoid incomplete structure
+
+        # - read thermo data
+        thermo_dict, end_info = parse_thermo_data(log_io.readlines())
+
+        # NOTE: last frame would not be dumpped if timestep not equals multiple*dump_period
+        #       if there were any error,
+        pot_energies = [
+            unitconvert.convert(p, "energy", units, "ASE")
+            for p in thermo_dict["PotEng"]
+        ]
+        nframes_thermo = len(pot_energies)
+        nframes = min([nframes_traj, nframes_thermo])
+        config._debug(
+            f"nframes in lammps: {nframes} traj {nframes_traj} thermo {nframes_thermo}"
+        )
+
+        # NOTE: check whether steps in thermo and traj are consistent
+        # pot_energies = pot_energies[:nframes]
+        # curr_traj_frames = curr_traj_frames[:nframes]
+        # assert len(pot_energies) == len(curr_traj_frames), f"Number of pot energies and frames are inconsistent at {str(wdir)}."
+
+        curr_traj_frames, curr_energies = [], []
+        for i, t in enumerate(timesteps):
+            if t in thermo_dict["Step"]:
+                curr_atoms = curr_traj_frames_[i]
+                curr_atoms.info["step"] = t
+                curr_traj_frames.append(curr_atoms)
+                curr_energies.append(
+                    pot_energies[thermo_dict["Step"].tolist().index(t)]
+                )
+
+        for pot_eng, atoms in zip(curr_energies, curr_traj_frames):
+            forces = atoms.get_forces()
+            # NOTE: forces have already been converted in ase read, so velocities are
+            sp_calc = SinglePointCalculator(atoms, energy=pot_eng, forces=forces)
+            atoms.calc = sp_calc
+
+        # - check model_devi.out
+        # TODO: convert units?
+        if devi_io is not None:
+            lines = devi_io.readlines()
+            if "#" in lines[0]:  # the first file
+                dkeys = ("".join([x for x in lines[0] if x != "#"])).strip().split()
+                dkeys = [x.strip() for x in dkeys][1:]
+            else:
+                ...
+            devi_io.seek(0)
+            data = np.loadtxt(devi_io, dtype=float)
+            ncols = data.shape[-1]
+            data = data.reshape(-1, ncols)
+            # NOTE: For some minimisers, dp gives several deviations as
+            #       multiple force evluations are performed in one step.
+            #       Thus, we only take the last occurance of the deviation in each step.
+            step_indices = []
+            steps = data[:, 0].astype(np.int32).tolist()
+            for k, v in itertools.groupby(enumerate(steps), key=lambda x: x[1]):
+                v = sorted(v, key=lambda x: x[0])
+                step_indices.append(v[-1][0])
+            data = data.transpose()[1:, step_indices[:nframes]]
+            # config._print(data)
+
+            for i, atoms in enumerate(curr_traj_frames):
+                for j, k in enumerate(dkeys):
+                    try:
+                        atoms.info[k] = data[j, i]
+                    except IndexError:
+                        # NOTE: Some potentials donot print last frames of min
+                        #       for example, lammps
+                        atoms.info[k] = 0.0
+        else:
+            ...
+
+        # - check COLVAR
+        if colvar_io is not None:
+            # - read latest COLVAR Files
+            names = colvar_io.readline().split()[2:]
+            colvar_io.seek(0)
+            colvars = np.loadtxt(colvar_io)
+            # print("colvars: ", colvars.shape)
+            curr_colvars = colvars[-nframes_traj:, :]
+            for i, atoms in enumerate(curr_traj_frames):
+                for k, v in zip(names, curr_colvars[i, :]):
+                    atoms.info[k] = v
+
+        # - Close IO
+        traj_io.close()
+        log_io.close()
+        if prism_io is not None:
+            prism_io.close()
+        if devi_io is not None:
+            devi_io.close()
+        if colvar_io is not None:
+            colvar_io.close()
+
+        return curr_traj_frames
+
     def read_trajectory(
-            self, type_list=None, add_step_info=True, 
-            archive_path: pathlib.Path=None, *args, **kwargs
-        ) -> List[Atoms]:
+        self,
+        type_list=None,
+        archive_path: pathlib.Path = None,
+        *args,
+        **kwargs,
+    ) -> List[Atoms]:
         """Read trajectory in the current working directory."""
         if type_list is not None:
             self.calc.type_list = type_list
         curr_units = self.calc.units
 
-        # - find runs...
-        prev_wdirs = sorted(self.directory.glob(r"[0-9][0-9][0-9][0-9][.]run"))
-        self._debug(f"prev_wdirs: {prev_wdirs}")
-
-        traj_list = []
-        for w in prev_wdirs:
-            curr_frames = read_single_simulation(
-                mdir=self.directory, wdir=w, prefix="", units=curr_units, 
-                add_step_info=add_step_info, archive_path=archive_path
-            )
-            traj_list.append(curr_frames)
-        
-        # Even though traj file may be empty, the read can give a empty list...
-        traj_list.append(
-            read_single_simulation(
-                mdir=self.directory, wdir=self.directory, prefix="", units=curr_units, 
-                add_step_info=add_step_info, archive_path=archive_path
-            )
+        traj_frames = self._aggregate_trajectories(
+            units=curr_units,
+            mdir=self.directory,
+            check_energy=True,
+            archive_path=archive_path,
         )
 
-        # -- concatenate
-        traj_frames, ntrajs = [], len(traj_list)
-        if ntrajs > 0:
-            traj_frames.extend(traj_list[0])
-            for i in range(1, ntrajs):
-                assert np.allclose(traj_list[i-1][-1].positions, traj_list[i][0].positions), f"Traj {i-1} and traj {i} are not consecutive in positions."
-                assert np.allclose(traj_list[i-1][-1].get_potential_energy(), traj_list[i][0].get_potential_energy()), f"Traj {i-1} and traj {i} are not consecutive in energy."
-                traj_frames.extend(traj_list[i][1:])
+        return traj_frames
+
+    def read_convergence_from_logfile(self, *args, **kwargs):
+        """"""
+        converged = False
+        log_fpath = self.directory / ASELMPCONFIG.log_filename
+        if log_fpath:
+            with open(log_fpath, "r") as fopen:
+                lines = fopen.readlines()
+            if lines[-1].strip().startswith("Total wall time:"):
+                converged = True
         else:
             ...
 
-        return traj_frames
-    
+        return converged
+
 
 class Lammps(FileIOCalculator):
 
     #: Calculator name.
     name: str = "Lammps"
 
     #: Implemented properties.
     implemented_properties: List[str] = ["energy", "forces", "stress"]
 
     #: LAMMPS command.
     command: str = "lmp 2>&1 > lmp.out"
+    # command: str = "lmp"
 
     #: Default calculator parameters, NOTE which have ase units.
     default_parameters: dict = dict(
-        # ase params
-        task = "min",
-        constraint = None, # index of atoms, start from 0
-        ignore_atoms_velocities = False,
+        # ase prepared parameters
+        task="min",
+        dump_period=1,
+        ckpt_period=100,
+        dynamics="",
+        steps=0,
+        constraint=None,  # index of atoms, start from 0
+        etol=0.0,
+        ftol=0.05,
         # --- lmp params ---
-        read_restart = None,
-        units = "metal",
-        atom_style = "atomic",
-        processors = "* * 1",
-        #boundary = "p p p",
-        newton = None,
-        pair_style = None,
-        pair_coeff = None,
-        neighbor = "0.0 bin",
-        neigh_modify = None,
-        mass = "* 1.0",
-        dump_period = 1,
-        ckpt_period = 100,
-        # - md
-        md_style = "nvt",
-        md_steps = 0,
-        velocity_seed = None,
-        timestep = 1.0, # fs
-        temp = 300,
-        pres = 1.0,
-        Tdamp = 100, # fs
-        Pdamp = 100,
-        # - minimisation
-        etol = 0.0,
-        ftol = 0.05,
-        maxiter = 0, # NOTE: this is steps for MD
-        maxeval = 0,
-        min_style = "fire",
-        min_modify = "integrator verlet tmax 4",
+        read_restart=None,
+        units="metal",
+        atom_style="atomic",
+        processors="* * 1",
+        # boundary = "p p p",
+        newton=None,
+        pair_style=None,
+        pair_coeff=None,
+        neighbor="0.0 bin",
+        neigh_modify=None,
+        mass="* 1.0",
         # - extra fix
-        extra_fix = [],
+        extra_fix=[],
         # - externals
-        plumed = None
+        plumed=None,
     )
 
     #: Symbol to integer.
     type_list: List[str] = None
 
     #: Cached trajectory of the previous simulation.
     cached_traj_frames: List[Atoms] = None
 
-    def __init__(
-        self, 
-        command = None, 
-        label = name, 
-        **kwargs
-    ):
+    def __init__(self, command=None, label=name, **kwargs):
         """"""
         FileIOCalculator.__init__(self, command=command, label=label, **kwargs)
 
+        # check command
+        # if "-in" in self.command or ">" in self.command:
+        #     raise RuntimeError(f"LAMMPS command must not contain input or output files.")
+        # self.command = self.command + "  -in in.lammps 2>&1 > lmp.out"
+
         # - check potential
         assert self.pair_style is not None, "pair_style is not set."
 
         return
-    
+
     def __getattr__(self, key):
         """Corresponding getattribute-function."""
         if key != "parameters" and key in self.parameters:
             return self.parameters[key]
         return object.__getattribute__(self, key)
-    
-    def calculate(self, atoms=None, properties=["energy"],
-            system_changes=all_changes): 
+
+    def calculate(self, atoms=None, properties=["energy"], system_changes=all_changes):
         """Run calculation."""
         # TODO: should use user-custom type_list from potential manager
         #       move this part to driver?
         self.type_list = parse_type_list(atoms)
 
         # init for creating the directory
         FileIOCalculator.calculate(self, atoms, properties, system_changes)
 
         return
-    
+
     def write_input(self, atoms, properties=None, system_changes=None) -> None:
         """Write input file and input structure."""
         FileIOCalculator.write_input(self, atoms, properties, system_changes)
 
         # - check velocities
-        self.write_velocities = False
-        if atoms.get_kinetic_energy() > 0.:
-            self.write_velocities = (True and not self.ignore_atoms_velocities)
+        write_velocities = False
+        if atoms.get_kinetic_energy() > 0.0:
+            write_velocities = True
 
         # write structure
-        prismobj = Prism(atoms.get_cell()) # TODO: nonpbc?
+        prismobj = Prism(atoms.get_cell())  # TODO: nonpbc?
         prism_file = os.path.join(self.directory, ASELMPCONFIG.prism_filename)
         with open(prism_file, "wb") as fopen:
             pickle.dump(prismobj, fopen)
         stru_data = os.path.join(self.directory, ASELMPCONFIG.inputstructure_filename)
         write_lammps_data(
-            stru_data, atoms, specorder=self.type_list, 
-            force_skew=True, prismobj=prismobj, velocities=self.write_velocities,
-            units=self.units, atom_style=self.atom_style
+            stru_data,
+            atoms,
+            specorder=self.type_list,
+            force_skew=True,
+            prismobj=prismobj,
+            velocities=write_velocities,
+            units=self.units,
+            atom_style=self.atom_style,
         )
 
         # write input
         self._write_input(atoms)
 
         return
-    
+
     def _is_finished(self):
-        """Check whether the simulation finished or failed. 
+        """Check whether the simulation finished or failed.
 
         Return wall time if the simulation finished.
 
         """
 
         is_finished, end_info = False, "not finished"
-        log_filepath = pathlib.Path(os.path.join(self.directory, ASELMPCONFIG.log_filename))
+        log_filepath = pathlib.Path(
+            os.path.join(self.directory, ASELMPCONFIG.log_filename)
+        )
 
         if log_filepath.exists():
             ERR_FLAG = "ERROR: "
             END_FLAG = "Total wall time:"
             with open(log_filepath, "r") as fopen:
                 lines = fopen.readlines()
-        
+
             for line in lines:
                 if line.strip().startswith(ERR_FLAG):
                     is_finished = True
                     end_info = " ".join(line.strip().split()[1:])
                     break
                 if line.strip().startswith(END_FLAG):
                     is_finished = True
                     end_info = " ".join(line.strip().split()[1:])
                     break
             else:
                 is_finished = False
         else:
             is_finished = False
 
-        return is_finished, end_info 
-    
+        return is_finished, end_info
+
     def read_results(self):
         """ASE read results."""
         # obtain results
         self.results = {}
 
         # - Be careful with UNITS
         # read forces from dump file
         curr_wdir = pathlib.Path(self.directory)
-        self.cached_traj_frames = read_single_simulation(
-            mdir=curr_wdir, wdir=curr_wdir, prefix="", 
-            units=self.units, add_step_info=True
+        self.cached_traj_frames = LmpDriver._read_a_single_trajectory(
+            mdir=curr_wdir, wdir=curr_wdir, units=self.units
         )
         converged_frame = self.cached_traj_frames[-1]
 
         self.results["forces"] = converged_frame.get_forces().copy()
         self.results["energy"] = converged_frame.get_potential_energy()
 
         # - add deviation info
@@ -676,179 +914,172 @@
                 self.results[k] = v
 
         return
 
     def _write_input(self, atoms) -> None:
         """Write input file in.lammps"""
         # - write in.lammps
-        content =  f"restart         {self.ckpt_period}  restart.*.data\n\n"
-        content += "units           %s\n" %self.units
-        content += "atom_style      %s\n" %self.atom_style
+        content = f"restart         {self.ckpt_period}  restart.*.data\n\n"
+        content += "units           %s\n" % self.units
+        content += "atom_style      %s\n" % self.atom_style
 
         # - mpi settings
         if self.processors is not None:
-            content += "processors {}\n".format(self.processors) # if 2D simulation
-        
+            content += "processors {}\n".format(self.processors)  # if 2D simulation
+
         # - simulation box
         pbc = atoms.get_pbc()
         if "boundary" in self.parameters:
             content += "boundary {0} \n".format(self.parameters["boundary"])
         else:
             content += "boundary {0} {1} {2} \n".format(
-                *tuple("fp"[int(x)] for x in pbc) # sometimes s failed to wrap all atoms
+                *tuple(
+                    "fp"[int(x)] for x in pbc
+                )  # sometimes s failed to wrap all atoms
             )
         content += "\n"
         if self.newton:
             content += "newton {}\n".format(self.newton)
         content += "box             tilt large\n"
         if self.read_restart is None:
-            content += "read_data	    %s\n" %ASELMPCONFIG.inputstructure_filename
+            content += "read_data	    %s\n" % ASELMPCONFIG.inputstructure_filename
         else:
             content += f"read_restart    {self.read_restart}\n"
-            #os.remove(ASELMPCONFIG.inputstructure_filename)
+            # os.remove(ASELMPCONFIG.inputstructure_filename)
         content += "change_box      all triclinic\n"
 
         # - particle masses
         mass_line = "".join(
-            "mass %d %f\n" %(idx+1,atomic_masses[atomic_numbers[elem]]) for idx, elem in enumerate(self.type_list)
+            "mass %d %f\n" % (idx + 1, atomic_masses[atomic_numbers[elem]])
+            for idx, elem in enumerate(self.type_list)
         )
         content += mass_line
         content += "\n"
 
         # - pair, MLIP specific settings
-        # TODO: neigh settings?
         potential = self.pair_style.strip().split()[0]
         if potential == "reax/c":
             assert self.atom_style == "charge", "reax/c should have charge atom_style"
             content += "pair_style  {}\n".format(self.pair_style)
-            content += "pair_coeff {} {}\n".format(self.pair_coeff, " ".join(self.type_list))
+            content += "pair_coeff {} {}\n".format(
+                self.pair_coeff, " ".join(self.type_list)
+            )
             content += "fix             reaxqeq all qeq/reax 1 0.0 10.0 1e-6 reax/c\n"
         elif potential == "eann":
             pot_data = self.pair_style.strip().split()[1:]
             endp = len(pot_data)
             for ip, p in enumerate(pot_data):
                 if p == "out_freq":
                     endp = ip
                     break
             pot_data = pot_data[:endp]
             if len(pot_data) > 1:
-                pair_style = "eann {} out_freq {}".format(" ".join(pot_data), self.dump_period)
+                pair_style = "eann {} out_freq {}".format(
+                    " ".join(pot_data), self.dump_period
+                )
             else:
                 pair_style = "eann {}".format(" ".join(pot_data))
             content += "pair_style  {}\n".format(pair_style)
             # NOTE: make out_freq consistent with dump_period
             if self.pair_coeff is None:
                 pair_coeff = "double * *"
             else:
                 pair_coeff = self.pair_coeff
             content += "pair_coeff	{} {}\n".format(pair_coeff, " ".join(self.type_list))
         elif potential == "deepmd":
-            content += "pair_style  {} out_freq {}\n".format(self.pair_style, self.dump_period)
-            content += "pair_coeff	{} {}\n".format(self.pair_coeff, " ".join(self.type_list))
+            content += "pair_style  {} out_freq {}\n".format(
+                self.pair_style, self.dump_period
+            )
+            content += "pair_coeff	{} {}\n".format(
+                self.pair_coeff, " ".join(self.type_list)
+            )
         else:
             content += "pair_style {}\n".format(self.pair_style)
-            #content += "pair_coeff {} {}\n".format(self.pair_coeff, " ".join(self.type_list))
+            # content += "pair_coeff {} {}\n".format(self.pair_coeff, " ".join(self.type_list))
             content += "pair_coeff {}\n".format(self.pair_coeff)
         content += "\n"
 
         # - neighbor
         content += "neighbor        {}\n".format(self.neighbor)
         if self.neigh_modify:
             content += "neigh_modify        {}\n".format(self.neigh_modify)
         content += "\n"
 
         # - constraint
         mobile_text, frozen_text = parse_constraint_info(atoms, self.constraint)
-        if mobile_text: # NOTE: sometimes all atoms are fixed
-            content += "group mobile id %s\n" %mobile_text
+        if mobile_text:  # NOTE: sometimes all atoms are fixed
+            content += "group mobile id %s\n" % mobile_text
             content += "\n"
-        if frozen_text: # not empty string
+        if frozen_text:  # not empty string
             # content += "region bottom block INF INF INF INF 0.0 %f\n" %zmin # unit A
-            content += "group frozen id %s\n" %frozen_text
+            content += "group frozen id %s\n" % frozen_text
             content += "fix cons frozen setforce 0.0 0.0 0.0\n"
         content += "\n"
 
         # - outputs
         # TODO: use more flexible notations
         if self.task == "min":
-            content += "thermo_style    custom step pe ke etotal temp press vol fmax fnorm\n"
+            content += (
+                "thermo_style    custom step pe ke etotal temp press vol fmax fnorm\n"
+            )
         elif self.task == "md":
             content += "compute mobileTemp mobile temp\n"
             content += "thermo_style    custom step c_mobileTemp pe ke etotal press vol lx ly lz xy xz yz\n"
         else:
             pass
-        content += "thermo          {}\n".format(self.dump_period) 
+        content += "thermo          {}\n".format(self.dump_period)
+        content += "thermo_modify   flush yes\n"
 
-        # TODO: How to dump total energy?
-        content += "dump		1 all custom {} {} id type element x y z fx fy fz vx vy vz\n".format(
-            self.dump_period, ASELMPCONFIG.trajectory_filename
+        # total energy is not stored in dump so we need read from log.lammps
+        content += (
+            "dump		1 all custom {} {} id type element x y z fx fy fz vx vy vz\n".format(
+                self.dump_period, ASELMPCONFIG.trajectory_filename
+            )
+        )
+        content += "dump_modify 1 element {} flush yes\n".format(
+            " ".join(self.type_list)
         )
-        content += "dump_modify 1 element {}\n".format(" ".join(self.type_list))
         content += "\n"
 
         # - add extra fix
         for i, fix_info in enumerate(self.extra_fix):
             content += "{:<24s}  {:<24s}  {:<s}\n".format("fix", f"extra{i}", fix_info)
-        
+
         # --- run type
         if self.task == "min":
-            # - minimisation
-            content += "min_style       {}\n".format(self.min_style)
-            content += "min_modify      {}\n".format(self.min_modify)
+            content += "\n".join(self.dynamics) + "\n"
+
             content += "minimize        {:f} {:f} {:d} {:d}\n".format(
                 unitconvert.convert(self.etol, "energy", "ASE", self.units),
                 unitconvert.convert(self.ftol, "force", "ASE", self.units),
-                self.maxiter, self.maxeval
+                self.steps,
+                2 * self.steps,
             )
         elif self.task == "md":
-            if not self.write_velocities and self.read_restart is None:
-                velocity_seed = self.velocity_seed
-                if velocity_seed is None:
-                    velocity_seed = np.random.randint(0,10000)
-                velocity_command = "velocity        mobile create {} {} dist gaussian ".format(self.temp, velocity_seed)
-                if hasattr(self, "remove_translation"):
-                    if self.remove_translation:
-                        velocity_command += "mom yes "
-                if hasattr(self, "remove_rotation"):
-                    if self.remove_rotation:
-                        velocity_command += "rot yes "
-                velocity_command += "\n"
-                content += velocity_command
-        
-            if self.md_style == "nvt":
-                Tdamp_ = unitconvert.convert(self.Tdamp, "time", "real", self.units)
-                content += "fix             thermostat mobile nvt temp {} {} {}\n".format(
-                    self.temp, self.temp, Tdamp_
-                )
-            elif self.md_style == "npt":
-                pres_ = unitconvert.convert(self.pres, "pressure", "metal", self.units)
-                Tdamp_ = unitconvert.convert(self.Tdamp, "time", "real", self.units)
-                Pdamp_ = unitconvert.convert(self.Pdamp, "time", "real", self.units)
-                content += "fix             thermostat mobile npt temp {} {} {} aniso {} {} {}\n".format(
-                    self.temp, self.temp, Tdamp_, pres_, pres_, Pdamp_
-                )
-            elif self.md_style == "nve":
-                content += "fix             thermostat mobile nve \n"
+            if self.read_restart is not None:
+                # pop up velocity line
+                self.dynamics[0] = "#  use velocities in restart"
+
+            content += "\n".join(self.dynamics) + "\n"
 
-            timestep_ = unitconvert.convert(self.timestep, "time", "real", self.units)
-            content += "\n"
-            content += f"timestep        {timestep_}\n"
             if self.plumed is not None:
-                plumed_inp = update_stride_and_file(self.plumed, wdir=str(self.directory), stride=self.dump_period)
+                plumed_inp = update_stride_and_file(
+                    self.plumed, wdir=str(self.directory), stride=self.dump_period
+                )
                 with open(os.path.join(self.directory, "plumed.inp"), "w") as fopen:
                     fopen.write("".join(plumed_inp))
                 content += "fix             metad all plumed plumedfile plumed.inp outfile plumed.out\n"
-            content += f"run             {self.maxiter}\n"
+            content += f"run             {self.steps}\n"
         else:
             # TODO: NEB?
             ...
-    
+
         # - output file
         in_file = os.path.join(self.directory, ASELMPCONFIG.input_fname)
         with open(in_file, "w") as fopen:
             fopen.write(content)
 
         return
- 
+
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.8/src/gdpx/computation/lasp.py` & `gdpx-0.0.9/src/gdpx/computation/lasp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/computation/mc/tfmc.py` & `gdpx-0.0.9/src/gdpx/computation/mc/tfmc.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/computation/md/md_utils.py` & `gdpx-0.0.9/src/gdpx/computation/md/md_utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/computation/md/nosehoover.py` & `gdpx-0.0.9/src/gdpx/computation/md/nosehoover.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/computation/utils.py` & `gdpx-0.0.9/src/gdpx/computation/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/computation/vasp.py` & `gdpx-0.0.9/src/gdpx/computation/vasp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/config.py` & `gdpx-0.0.9/src/gdpx/config.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/core/node.py` & `gdpx-0.0.9/src/gdpx/core/node.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/core/operation.py` & `gdpx-0.0.9/src/gdpx/core/operation.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/core/placeholder.py` & `gdpx-0.0.9/src/gdpx/core/placeholder.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/core/register.py` & `gdpx-0.0.9/src/gdpx/core/register.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/core/session/active.py` & `gdpx-0.0.9/src/gdpx/core/session/active.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/core/session/basic.py` & `gdpx-0.0.9/src/gdpx/core/session/basic.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/core/session/interface.py` & `gdpx-0.0.9/src/gdpx/core/session/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/core/session/session.py` & `gdpx-0.0.9/src/gdpx/core/session/session.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/core/session/utils.py` & `gdpx-0.0.9/src/gdpx/core/session/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/core/variable.py` & `gdpx-0.0.9/src/gdpx/core/variable.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/ClusterAndCUR.py` & `gdpx-0.0.9/src/gdpx/data/ClusterAndCUR.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/analyser.py` & `gdpx-0.0.9/src/gdpx/data/analyser.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/array.py` & `gdpx-0.0.9/src/gdpx/data/array.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/cleave_deviation.py` & `gdpx-0.0.9/src/gdpx/data/cleave_deviation.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/convert.py` & `gdpx-0.0.9/src/gdpx/data/convert.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/correction.py` & `gdpx-0.0.9/src/gdpx/data/correction.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/database.py` & `gdpx-0.0.9/src/gdpx/data/database.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/dataset.py` & `gdpx-0.0.9/src/gdpx/data/dataset.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/extatoms.py` & `gdpx-0.0.9/src/gdpx/data/extatoms.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/extract_evolution.py` & `gdpx-0.0.9/src/gdpx/data/extract_evolution.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/interface.py` & `gdpx-0.0.9/src/gdpx/data/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/operators.py` & `gdpx-0.0.9/src/gdpx/data/operators.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/system.py` & `gdpx-0.0.9/src/gdpx/data/system.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/data/utils.py` & `gdpx-0.0.9/src/gdpx/data/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/describer/describer.py` & `gdpx-0.0.9/src/gdpx/describer/describer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/describer/interface.py` & `gdpx-0.0.9/src/gdpx/describer/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/describer/soap.py` & `gdpx-0.0.9/src/gdpx/describer/soap.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/describer/spc.py` & `gdpx-0.0.9/src/gdpx/describer/spc.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/expedition/__init__.py` & `gdpx-0.0.9/src/gdpx/expedition/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 # -*- coding: utf-8 -*-
 
 
 import traceback
 
 from .. import config
 from ..core.register import registers
+from ..data.array import AtomsNDArray
 from ..builder.builder import StructureBuilder
 from ..builder.utils import convert_string_to_atoms
 from ..worker.single import SingleWorker
 from ..worker.drive import DriverBasedWorker
 from ..worker.interface import ComputerVariable
 from ..utils.command import convert_indices, dict2str
+from ..potential.interface import create_mixer
 
 from .interface import ExpeditionVariable
 registers.variable.register(ExpeditionVariable)
 
 from .interface import explore 
 registers.operation.register(explore)
 
@@ -29,18 +31,13 @@
 
 from .monte_carlo.monte_carlo import MonteCarlo
 registers.expedition.register("monte_carlo")(MonteCarlo)
 
 from .simulated_annealing.simulated_annealing import SimulatedAnnealing
 registers.expedition.register("simulated_annealing")(SimulatedAnnealing)
 
-# - optional
-try:
-    from .af.afir import AFIRSearch
-    registers.expedition.register("artificial_reaction")(AFIRSearch)
-except:
-    config._print("AFIR is not loaded.")
-    config._print(traceback.print_exc())
+from .artificial_force.afir import AFIRSearch
+registers.expedition.register("artificial_reaction")(AFIRSearch)
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.8/src/gdpx/expedition/accelerated_dynamics/prev_example.py` & `gdpx-0.0.9/src/gdpx/expedition/accelerated_dynamics/prev_example.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/expedition/af/afir.py` & `gdpx-0.0.9/src/gdpx/selector/selector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,297 +1,323 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+import abc 
 import copy
-import logging
+import itertools
 import pathlib
-import time
-import pickle
-
-from typing import NoReturn, List, Mapping
-
-from itertools import combinations, product, chain, groupby
+from typing import Union, List, Callable, NoReturn, Optional
 
 import numpy as np
 
 from ase import Atoms
-from ase.io import read, write
-from ase.formula import Formula
 
-from .. import registers
-from .. import StructureBuilder
-from .. import ComputerVariable, DriverBasedWorker
-from ..expedition import AbstractExpedition
+from ..core.node import AbstractNode
+from ..worker.drive import DriverBasedWorker
+from ..data.array import AtomsNDArray
+
+
+"""Define an AbstractSelector that is the base class of any selector.
+"""
+
+def save_cache(fpath, data, random_seed: int=None):
+    """"""
+    header = ("#{:>11s}  {:>8s}  {:>8s}  {:>8s}  "+"{:>12s}"*4+"\n").format(
+        *"index confid step natoms ene aene maxfrc score".split()
+    )
+    footer = f"random_seed {random_seed}"
+
+    content = header
+    for x in data:
+        content += ("{:>12s}  {:>8d}  {:>8d}  {:>8d}  "+"{:>12.4f}"*4+"\n").format(*x)
+    content += footer
+
+    with open(fpath, "w") as fopen:
+        fopen.write(content)
+
+    return
 
-from gdpx.worker.grid import GridDriverBasedWorker
-from gdpx.potential.interface import create_mixer
-from gdpx.builder.group import create_a_group, create_a_molecule_group
-from gdpx.graph.molecule import find_product, find_molecules
+def load_cache(fpath, random_seed: int=None):
+    """"""
+    with open(fpath, "r") as fopen:
+        lines = fopen.readlines()
+
+    # - header
+    header = lines[0]
+
+    # - data
+    data = lines[1:-1] # TODO: test empty data
+
+    raw_markers = []
+    if data:
+        # NOTE: new_markers looks like [(0,1),(0,2),(1,0)]
+        #       If no structures are selected, the info file should only contain
+        #       the header and the footer
+        new_markers =[
+            [int(x) for x in (d.strip().split()[0]).split(",")] for d in data
+        ]
+        #new_markers = []
+        #for d in data:
+        #    curr_marker = []
+        #    for x in d.strip().split()[0].split(","):
+        #        if x.isdigit(): # MUST BE AN INTEGER
+        #            curr_marker.append(int(x))
+        #        else:
+        #            curr_marker.append(np.nan)
+        #    new_markers.append(curr_marker)
+        raw_markers = new_markers
+
+    # - footer
+    footer = lines[-1]
+    cache_random_seed = int(footer.strip().split()[-1]) # TODO: random state
+    #assert cache_random_seed == random_seed
 
+    return raw_markers
 
-def convert_index_to_formula(atoms, group_indices: List[List[int]]):
+def group_markers(new_markers_unsorted):
     """"""
-    formulae = []
-    for g in group_indices:
-        symbols = [atoms[i].symbol for i in g]
-        formulae.append(
-            Formula.from_list(symbols).format("hill")
-        )
-    #formulae = sorted(formulae)
+    new_markers = sorted(new_markers_unsorted, key=lambda x: x[0])
+    raw_markers_unsorted = []
+    for k, v in itertools.groupby(new_markers, key=lambda x: x[0]):
+        raw_markers_unsorted.append([k,[x[1] for x in v]])
 
-    return formulae
+    # traj markers are sorted when set
+    raw_markers = [[x[0],sorted(x[1])] for x in sorted(raw_markers_unsorted, key=lambda x:x[0])]
 
+    return raw_markers
 
-def find_target_fragments(atoms, target_commands: List[str]) -> Mapping[str,List[List[int]]]:
-    """Find target fragments in the structure to react.
 
-    This is a wrapper for group commands as there are several ways to defind
-    a (atomic) group but we need a group of molecules here. Optional ways are 
-    using `molecule` all, using `tag`...
+class AbstractSelector(AbstractNode):
 
-    """
-    fragments = {} # Mapping[str,List[List[int]]]
-    target_molecules = None
+    """The base class of any selector."""
 
-    ngroups = len(target_commands)
-    if ngroups == 1:
-        atomic_indices = create_a_group(atoms, target_commands[0])
-        fragments = find_molecules(atoms, atomic_indices)
-    else:
-        assert ngroups >= 2, "Need at least 2 groups..."
-        for group_command in target_commands:
-            fragments[group_command] = create_a_molecule_group(atoms, group_command)
+    #: Selector name.
+    name: str = "abstract"
 
-    return fragments
+    #: Target axis to select.
+    axis: Optional[int] = None
 
+    #: Default parameters.
+    default_parameters: dict = dict(
+        number = [4, 0.2], # number & ratio
+        verbose = False
+    )
 
-class AFIRSearch(AbstractExpedition):
+    #: A worker for potential computations.
+    worker: DriverBasedWorker = None
 
+    #: Distinguish structures when using ComposedSelector.
+    prefix: str = "selection"
 
-    def __init__(
-            self, builder, target, gamma: List[float]=[0.5, 2.5, 1.0], 
-            seed=None, directory="./", *args, **kwargs
-        ) -> None:
-        """Define some basic parameters for the afir search.
+    #: Output file name.
+    _fname: str = "info.txt"
+
+    #: Output data format (frames or trajectories).
+    _out_fmt: str = "stru"
+
+    def __init__(self, directory="./", axis=None, *args, **kwargs) -> None:
+        """Create a selector.
 
         Args:
-            builder: StructureBuilder.
-        
+            directory: Working directory.
+            *args: Variable length argument list.
+            **kwargs: Arbitrary keyword arguments.
+
         """
-        self.directory = directory
+        super().__init__(directory=directory, *args, **kwargs)
 
-        self.builder = builder
-        self.target = target
-        #assert len(self.target) == 2, "Target only supports two elements."
-        self.gamma = gamma
-
-        self.bias_params = dict(
-            name = "bias", 
-            params = dict(
-                backend="ase", type = "afir",
-                gamma = None, groups = None
-            )
-        )
+        self.axis = axis
+
+        self.fname = self.name+"-info.txt"
+        
+        # - update parameters from kwargs
+        self.parameters = copy.deepcopy(self.default_parameters)
+        for k in self.parameters:
+            if k in kwargs.keys():
+                self.parameters[k] = kwargs[k]
+
+        return
+
+    def set(self, *args, **kwargs):
+        """Set parameters."""
+        for k, v in kwargs.items():
+            if k in self.parameters:
+                self.parameters[k] = v
 
         return
 
-    def register_worker(self, worker: dict, *args, **kwargs):
+    def __getattr__(self, key):
+        """Corresponding getattribute-function."""
+        if key != "parameters" and key in self.parameters:
+            return self.parameters[key]
+
+        return object.__getattribute__(self, key)
+
+    @AbstractNode.directory.setter
+    def directory(self, directory_) -> NoReturn:
+        self._directory = pathlib.Path(directory_)
+        self.info_fpath = self._directory/self._fname
+
+        return 
+    
+    @property
+    def fname(self):
         """"""
-        if isinstance(worker, dict):
-            worker_params = copy.deepcopy(worker)
-            worker = registers.create(
-                "variable", "computer", convert_name=True, **worker_params
-            ).value[0]
-        elif isinstance(worker, list): # assume it is from a computervariable
-            worker = worker[0]
-        elif isinstance(worker, ComputerVariable):
-            worker = worker.value[0]
-        elif isinstance(worker, DriverBasedWorker):
-            worker = worker
-        else:
-            raise RuntimeError(f"Unknown worker type {worker}")
-        
+        return self._fname
+    
+    @fname.setter
+    def fname(self, fname_):
+        """"""
+        self._fname = fname_
+        self.info_fpath = self._directory/self._fname
+        return
+    
+    def attach_worker(self, worker=None) -> NoReturn:
+        """Attach a worker to this node."""
         self.worker = worker
 
         return
 
-    def _prepare_fragments(self, atoms, *args, **kwargs):
-        """"""
-        data_path = self.directory / "_data"
-        if not data_path.exists():
-            data_path.mkdir(parents=True, exist_ok=True)
-
-        # - find possible reaction pairs
-        frag_fpath = data_path/"fragments.pkl"
-        # TODO: assure the pair order is the same when restart
-        if not frag_fpath.exists():
-            fragments = find_target_fragments(atoms, self.target)
-            with open(frag_fpath, "wb") as fopen:
-                pickle.dump(fragments, fopen)
+    def select(self, inp_dat: AtomsNDArray, *args, **kargs) -> List[Atoms]:
+        """Select trajectories.
+
+        Based on used selction protocol
+
+        Args:
+            frames: A list of ase.Atoms or a list of List[ase.Atoms].
+            index_map: Global indices of frames.
+            ret_indices: Whether return selected indices or frames.
+            *args: Variable length argument list.
+            **kwargs: Arbitrary keyword arguments.
+        
+        Returns:
+            List[Atoms] or List[int]: selected results
+
+        """
+        self._print(f"@@@{self.__class__.__name__}")
+
+        if not self.directory.exists():
+            self.directory.mkdir(parents=True)
+
+        # NOTE: input structures should always be the AtomsNDArray type
+        # TODO: if inp_dat is already a AtomsNDArray, a new object is created,
+        #       which makes markers immutable... Need fix this!!
+        if isinstance(inp_dat, AtomsNDArray):
+            ...
         else:
-            with open(frag_fpath, "rb") as fopen:
-                fragments = pickle.load(fopen)
+            inp_dat = AtomsNDArray(inp_dat)
 
-        # TODO: assert molecules in one group are the same type?
-        self._print("Found Target Fragments: ")
-        for k, v in fragments.items():
-            self._print("  {:<24s}:  {}".format(k, v))
-
-        frag_list = []
-        for k, v in fragments.items():
-            frag_list.append(v)
+        frames = inp_dat
+        inp_nframes = len(frames.markers)
+
+        # - check if it is finished
+        if not (self.info_fpath).exists():
+            # -- mark structures
+            self._print("run selection...")
+            self._mark_structures(frames)
+            # -- save cached results for restart
+            self._write_cached_results(frames)
+        else:
+            # -- restart
+            self._print("use cached...")
+            raw_markers = load_cache(self.info_fpath)
+            #print(f"raw_markers: {raw_markers}")
+            frames.markers = raw_markers
         
-        ntypes = len(frag_list)
-        comb = combinations(range(ntypes), 2)
+        out_nframes = len(frames.markers)
+        self._print(f"{self.name} nstructures {inp_nframes} -> nselected {out_nframes}")
 
-        possible_pairs = []
-        for i, j in comb:
-            f1, f2 = frag_list[i], frag_list[j]
-            possible_pairs.extend(list(product(f1, f2)))
+        # - add history
+        #   get_marked_structures return reference to Atoms objects
+        #for a in inp_dat.get_marked_structures():
+        #    print(a.info.get("selection"))
+
+        marked_structures = inp_dat.get_marked_structures()
+        for atoms in marked_structures:
+            selection = atoms.info.get("selection", "")
+            atoms.info["selection"] = selection+f"->{self.name}"
         
-        with open(self.directory/"_data"/"pairs.pkl", "wb") as fopen:
-            pickle.dump(possible_pairs, fopen)
+        #for a in inp_dat.get_marked_structures():
+        #    print(a.info["selection"])
 
-        return possible_pairs
+        return marked_structures
     
-    def _create_afir_potters(self, pair: List[List[int]], gamma_list: List[float], *args, **kwargs):
-        """"""
-        if hasattr(self.worker.potter, "remove_loaded_models"):
-            self.worker.potter.remove_loaded_models()
+    @abc.abstractmethod
+    def _mark_structures(self, data, *args, **kwargs) -> None:
+        """Mark structures subject to selector's conditions."""
 
-        bias_list = []
-        for g in gamma_list:
-            curr_bias = copy.deepcopy(self.bias_params)
-            curr_bias["params"]["groups"] = pair 
-            curr_bias["params"]["gamma"] = g
-            bias_list.append(curr_bias)
-        potters = [create_mixer(self.worker.potter, b) for b in bias_list]
+        return
 
-        return potters
-    
-    def run(self, *args, **kwargs) -> None:
-        """"""
-        # - some imported packages change `logging.basicConfig` 
-        #   and accidently add a StreamHandler to logging.root
-        #   so remove it...
-        for h in logging.root.handlers:
-            if isinstance(h, logging.StreamHandler) and not isinstance(h, logging.FileHandler):
-                logging.root.removeHandler(h)
-
-        self._print("---------------------------")
-        self._print("| AFIRSearch starts...... |")
-        self._print("---------------------------")
-        # TODO: check restart
-
-        # - assume input structures are minimised
-        frames = self.builder.run()
-        nframes = len(frames)
-        assert nframes == 1, "Only one structure for now."
-        atoms = frames[0]
+    def _parse_selection_number(self, nframes: int) -> int:
+        """Compute number of selection based on the input number.
 
-        # - find fragments
-        possible_pairs = self._prepare_fragments(atoms)
-        
-        # - prepare afir bias
-        gamma_list = np.linspace(*self.gamma, endpoint=True)
+        Args:
+            nframes: Number of input frames, sometimes maybe zero.
 
-        # - run each pair
-        grid_workers = []
-        for i, pair in enumerate(possible_pairs):
-            # -- start info
-            self._print(f"===== Pair {i} =====")
-            reactants = convert_index_to_formula(atoms, pair)
-            self._print("Reactants:")
-            self._print(reactants)
-            self._print(pair)
-
-            # -- create GridWorker
-            potters = self._create_afir_potters(pair, gamma_list)
-            curr_worker = GridDriverBasedWorker(
-                potters, driver=self.worker.driver
-            )
-            curr_worker.directory = self.directory / f"pair{i}"
-            grid_workers.append(curr_worker)
-            curr_worker.run([atoms])
-        
-        # - extract each pair
-        worker_status = []
-        for i, curr_worker in enumerate(grid_workers):
-            curr_worker.inspect(resubmit=True)
-            if curr_worker.get_number_of_running_jobs() == 0:
-                worker_status.append(True)
-            else:
-                worker_status.append(False)
+        """
+        default_number, default_ratio = self.default_parameters["number"]
+        number_info = self.parameters["number"]
+        if isinstance(number_info, int):
+            num_fixed, num_percent = number_info, default_ratio
+        elif isinstance(number_info, float):
+            num_fixed, num_percent = default_number, number_info
+        else:
+            assert len(number_info) == 2, "Cant parse number for selection..."
+            num_fixed, num_percent = number_info
         
-        if all(worker_status):
-            self._print("---------------------------")
-            self._print("| AFIRSearch is finished. |")
-            self._print("---------------------------")
-            nimages = len(gamma_list)
-            for i, (pair, curr_worker) in enumerate(zip(possible_pairs, grid_workers)):
-                self._print(f"===== Pair {i} =====")
-                reactants = convert_index_to_formula(atoms, pair)
-                self._print("Reactants:")
-                self._print(reactants)
-                self._print(pair)
-                curr_trajs = curr_worker.retrieve(include_retrieved=True)
-                pseudo_pathway = [t[-1] for t in curr_trajs]
-                end_atoms = pseudo_pathway[-1]
-                prod_indices = find_product(end_atoms, pair)
-                products = convert_index_to_formula(end_atoms, prod_indices)
-                self._print("Products:")
-                self._print(products)
-                if sorted(reactants) == sorted(products):
-                    # TODO: index may change? molecule reconstruct?
-                    self._print("nothing happens...")
-                else:
-                    self._print("reaction happens...")
-                    # TODO: postprocess, minimise FS to create a pathway
-            # - 
-            with open(self.directory/"FINISHED", "w") as fopen:
-                fopen.write(
-                    f"FINISHED AT {time.asctime( time.localtime(time.time()) )}."
-                )
+        if num_fixed is not None:
+            if num_fixed > nframes:
+                num_fixed = int(nframes*num_percent)
         else:
-            self._print("Some calculations are unfinished.")
+            num_fixed = int(nframes*num_percent)
 
-        return
-    
-    def read_convergence(self, *args, **kwargs):
-        """"""
-        converged = False
-        if (self.directory/"FINISHED").exists():
-            converged = True
+        return num_fixed
 
-        return converged
-    
-    def get_workers(self, *args, **kwargs):
-        """"""
-        workers = []
-        if hasattr(self.worker.potter, "remove_loaded_models"):
-            self.worker.potter.remove_loaded_models()
-
-        pair_data_path = self.directory/"_data"/"pairs.pkl"
-        if pair_data_path.exists():
-            with open(pair_data_path, "rb") as fopen:
-                pairs = pickle.load(fopen)
-            wdirs = sorted(
-                list(self.directory.glob("pair*")), key=lambda x: int(x.name[4:])
+    def _write_cached_results(self, aa: AtomsNDArray, *args, **kwargs) -> None:
+        """Write selection results into file that can be used for restart."""
+        # - 
+        markers = aa.markers
+
+        # - output
+        data = []
+        for ind in markers:
+            atoms = aa[tuple(ind)]
+            # - gather info
+            confid = atoms.info.get("confid", -1)
+            step = atoms.info.get("step", -1) # step number in the trajectory
+            natoms = len(atoms)
+            try:
+                ene = atoms.get_potential_energy()
+                ae = ene / natoms
+            except:
+                ene, ae = np.NaN, np.NaN
+            try:
+                maxforce = np.max(np.fabs(atoms.get_forces(apply_constraint=True)))
+            except:
+                maxforce = np.NaN
+            score = atoms.info.get("score", np.nan)
+            # - add info
+            ind_str = ",".join([str(x) for x in ind])
+            data.append([f"{ind_str}", confid, step, natoms, ene, ae, maxforce, score])
+        
+        if data:
+            save_cache(self.info_fpath, data, self.random_seed)
+        else:
+            #np.savetxt(
+            #    self.info_fpath, [[np.NaN]*8],
+            #    header="{:>11s}  {:>8s}  {:>8s}  {:>8s}  {:>12s}  {:>12s}  {:>12s}  {:>12s}".format(
+            #        *"index confid step natoms ene aene maxfrc score".split()
+            #    ),
+            #    footer=f"random_seed {self.random_seed}"
+            #)
+            content ="{:>11s}  {:>8s}  {:>8s}  {:>8s}  {:>12s}  {:>12s}  {:>12s}  {:>12s}".format(
+                *"index confid step natoms ene aene maxfrc score".split()
             )
-            assert len(pairs) == len(wdirs), f"Inconsistent number of pairs {len(pairs)} and wdirs {len(wdirs)}."
+            content += f"random_seed {self.random_seed}"
+            with open(self.info_fpath, "w") as fopen:
+                fopen.write(content)
 
-            gamma_list = np.linspace(*self.gamma, endpoint=True)
-            for i, pair in enumerate(pairs):
-                potters = self._create_afir_potters(pair, gamma_list)
-                curr_worker = GridDriverBasedWorker(
-                    potters, driver=self.worker.driver
-                )
-                curr_worker.directory = self.directory / f"pair{i}"
-                workers.append(curr_worker)
-        else:
-            raise FileNotFoundError("There is no cache for pairs.")
-        
-        return workers
+        return
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.8/src/gdpx/expedition/expedition.py` & `gdpx-0.0.9/src/gdpx/expedition/expedition.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,20 +36,35 @@
         #   so remove it...
         for h in logging.root.handlers:
             if isinstance(h, logging.StreamHandler) and not isinstance(
                 h, logging.FileHandler
             ):
                 logging.root.removeHandler(h)
 
-        assert self.worker is not None, "MC has not set its worker properly."
+        assert self.worker is not None, f"{self.name} has not set its worker properly."
 
         return
 
-    def register_worker(self, worker: dict, *args, **kwargs):
-        """"""
+    def register_builder(self, builder: dict) -> None:
+        """Register StructureBuilder for this expedition."""
+        if isinstance(builder, dict):
+            builder_params = copy.deepcopy(builder)
+            builder_method = builder_params.pop("method")
+            builder = registers.create(
+                "builder", builder_method, convert_name=False, **builder_params
+            )
+        else:
+            builder = builder
+
+        self.builder = builder
+
+        return
+
+    def register_worker(self, worker: dict, *args, **kwargs) -> None:
+        """Register DriverBasedWorker for this expedition."""
         if isinstance(worker, dict):
             worker_params = copy.deepcopy(worker)
             worker = registers.create(
                 "variable", "computer", convert_name=True, **worker_params
             ).value[0]
         elif isinstance(worker, list):  # assume it is from a computervariable
             worker = worker[0]
```

### Comparing `gdpx-0.0.8/src/gdpx/expedition/ga/engine.py` & `gdpx-0.0.9/src/gdpx/expedition/ga/engine.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/expedition/ga/population.py` & `gdpx-0.0.9/src/gdpx/expedition/ga/population.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/expedition/monte_carlo/basin_hopping.py` & `gdpx-0.0.9/src/gdpx/expedition/monte_carlo/basin_hopping.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/expedition/monte_carlo/monte_carlo.py` & `gdpx-0.0.9/src/gdpx/expedition/monte_carlo/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/expedition/monte_carlo/operators/__init__.py` & `gdpx-0.0.9/src/gdpx/expedition/monte_carlo/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/expedition/monte_carlo/operators/exchange.py` & `gdpx-0.0.9/src/gdpx/expedition/monte_carlo/operators/exchange.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/expedition/monte_carlo/operators/move.py` & `gdpx-0.0.9/src/gdpx/expedition/monte_carlo/operators/move.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/expedition/monte_carlo/operators/operator.py` & `gdpx-0.0.9/src/gdpx/expedition/monte_carlo/operators/operator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/expedition/monte_carlo/operators/react.py` & `gdpx-0.0.9/src/gdpx/expedition/monte_carlo/operators/react.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/expedition/monte_carlo/operators/swap.py` & `gdpx-0.0.9/src/gdpx/expedition/monte_carlo/operators/swap.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/expedition/simulated_annealing/simulated_annealing.py` & `gdpx-0.0.9/src/gdpx/expedition/simulated_annealing/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/graph/comparison.py` & `gdpx-0.0.9/src/gdpx/graph/comparison.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/graph/creator.py` & `gdpx-0.0.9/src/gdpx/graph/creator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/graph/graph_main.py` & `gdpx-0.0.9/src/gdpx/graph/graph_main.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/graph/molecule.py` & `gdpx-0.0.9/src/gdpx/graph/molecule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+
+import dataclasses
 import itertools
 
 from typing import List, Mapping
 
+import networkx as nx
+
 from ase import Atoms
+from ase.formula import Formula
+from ase.neighborlist import NeighborList, natural_cutoffs
 
+from .utils import grid_iterator, node_symbol, unpack_node_name
 
-def find_product(atoms: Atoms, reactants: List[List[int]], grid=[1,1,0], radii_multi=1.0, skin=0.0) -> List[List[int]]:
+
+def find_product(
+    atoms: Atoms, reactants: List[List[int]], grid=[1, 1, 0], radii_multi=1.0, skin=0.0
+) -> List[List[int]]:
     """Find if there were a product from input reactants."""
     valid_indices = list(itertools.chain.from_iterable(reactants))
 
     # - create local graph
     covalent_radii = natural_cutoffs(atoms, radii_multi)
     nl = NeighborList(
-        covalent_radii, 
-        skin = skin, sorted=False,
-        self_interaction=False, 
-        bothways=True
+        covalent_radii, skin=skin, sorted=False, self_interaction=False, bothways=True
     )
     nl.update(atoms)
 
-    #print([covalent_radii[i] for i in valid_indices])
+    # print([covalent_radii[i] for i in valid_indices])
 
     graph = nx.Graph()
-    
-    #grid = [1,1,0] # for surface
+
+    # grid = [1,1,0] # for surface
     # -- add nodes
     for centre_idx in valid_indices:
         for x, y, z in grid_iterator(grid):
             graph.add_node(
-                node_symbol(atoms[centre_idx].symbol, centre_idx, (x,y,z)),
-                index=centre_idx
+                node_symbol(atoms[centre_idx].symbol, centre_idx, (x, y, z)),
+                index=centre_idx,
             )
 
     # -- add edges
     for centre_idx in valid_indices:
         for x, y, z in grid_iterator(grid):
             nei_indices, nei_offsets = nl.get_neighbors(centre_idx)
             for nei_idx, offset in zip(nei_indices, nei_offsets):
@@ -48,101 +55,115 @@
                         continue
                     if not (-grid[1] <= oy + y <= grid[1]):
                         continue
                     if not (-grid[2] <= oz + z <= grid[2]):
                         continue
                     # ---
                     graph.add_edge(
-                        node_symbol(atoms[centre_idx].symbol, centre_idx, (x,y,z)),
-                        node_symbol(atoms[nei_idx].symbol, nei_idx, (x+ox,y+oy,z+oz))
+                        node_symbol(atoms[centre_idx].symbol, centre_idx, (x, y, z)),
+                        node_symbol(
+                            atoms[nei_idx].symbol, nei_idx, (x + ox, y + oy, z + oz)
+                        ),
                     )
                 else:
                     ...
-    
-    #plot_graph(graph, "xxx.png")
+
+    # plot_graph(graph, "xxx.png")
 
     # - find products
-    reax_nodes = [node_symbol(atoms[i].symbol, i, (0,0,0)) for i in valid_indices]
+    reax_nodes = [node_symbol(atoms[i].symbol, i, (0, 0, 0)) for i in valid_indices]
     reax_graphs = nx.subgraph(graph, reax_nodes)
 
-    prod_graphs = [reax_graphs.subgraph(c) for c in nx.connected_components(reax_graphs)]
+    prod_graphs = [
+        reax_graphs.subgraph(c) for c in nx.connected_components(reax_graphs)
+    ]
 
     products = [[unpack_node_name(u)[1] for u in g.nodes()] for g in prod_graphs]
 
     return products
 
-from ase.formula import Formula
-def find_molecules(atoms: Atoms, valid_indices: List[int], grid=[1,1,0], radii_multi=1.0, skin=0.0) -> Mapping[str,List[List[int]]]:
-    """Find if there were a product from input reactants."""
-    #valid_indices = list(chain.from_iterable(reactants))
 
-    # - create local graph
+@dataclasses.dataclass
+class GraphNodeName:
+
+    #: Atom symbol.
+    symbol: str
+
+    #: Atom index.
+    index: int
+
+
+def find_molecules(
+    atoms: Atoms, reactive_indices: List[int], grid=[1, 1, 0], radii_multi: float=1.0, skin=0.0
+) -> Mapping[str, List[List[int]]]:
+    """Find molecules by graph."""
+    # valid_indices = list(chain.from_iterable(reactants))
+
+    # add a neighlist
     covalent_radii = natural_cutoffs(atoms, radii_multi)
     nl = NeighborList(
-        covalent_radii, 
-        skin = skin, sorted=False,
-        self_interaction=False, 
-        bothways=True
+        covalent_radii, skin=skin, sorted=False, self_interaction=False, bothways=True
     )
     nl.update(atoms)
 
-    #print([covalent_radii[i] for i in valid_indices])
 
+    # create a graph
     graph = nx.Graph()
-    
-    #grid = [1,1,0] # for surface
-    # -- add nodes
-    for centre_idx in valid_indices:
+
+    for centre_idx in reactive_indices:
         for x, y, z in grid_iterator(grid):
             graph.add_node(
-                node_symbol(atoms[centre_idx].symbol, centre_idx, (x,y,z)),
-                index=centre_idx
+                node_symbol(atoms[centre_idx].symbol, centre_idx, (x, y, z)),
+                index=centre_idx,
             )
 
-    # -- add edges
-    for centre_idx in valid_indices:
+    for centre_idx in reactive_indices:
         for x, y, z in grid_iterator(grid):
             nei_indices, nei_offsets = nl.get_neighbors(centre_idx)
             for nei_idx, offset in zip(nei_indices, nei_offsets):
-                if nei_idx in valid_indices:
+                if nei_idx in reactive_indices:
                     # NOTE: check if neighbour is in the grid space
                     #       this is not the case when cutoff is too large
                     ox, oy, oz = offset
                     if not (-grid[0] <= ox + x <= grid[0]):
                         continue
                     if not (-grid[1] <= oy + y <= grid[1]):
                         continue
                     if not (-grid[2] <= oz + z <= grid[2]):
                         continue
                     # ---
                     graph.add_edge(
-                        node_symbol(atoms[centre_idx].symbol, centre_idx, (x,y,z)),
-                        node_symbol(atoms[nei_idx].symbol, nei_idx, (x+ox,y+oy,z+oz))
+                        node_symbol(atoms[centre_idx].symbol, centre_idx, (x, y, z)),
+                        node_symbol(
+                            atoms[nei_idx].symbol, nei_idx, (x + ox, y + oy, z + oz)
+                        ),
                     )
                 else:
                     ...
-    
-    #plot_graph(graph, "xxx.png")
 
-    # - find products
-    reax_nodes = [node_symbol(atoms[i].symbol, i, (0,0,0)) for i in valid_indices]
+    # plot_graph(graph, "xxx.png")
+
+    # find molecules 
+    reax_nodes = [node_symbol(atoms[i].symbol, i, (0, 0, 0)) for i in reactive_indices]
     reax_graphs = nx.subgraph(graph, reax_nodes)
 
-    prod_graphs = [reax_graphs.subgraph(c) for c in nx.connected_components(reax_graphs)]
+    prod_graphs = [
+        reax_graphs.subgraph(c) for c in nx.connected_components(reax_graphs)
+    ]
 
     products = [[unpack_node_name(u)[1] for u in g.nodes()] for g in prod_graphs]
 
     # - get formula
     fragments = {}
     for atomic_indices in products:
         symbols = [atoms[i].symbol for i in atomic_indices]
         formula = Formula.from_list(symbols).format("hill")
         if formula in fragments:
             fragments[formula].append(atomic_indices)
         else:
             fragments[formula] = [atomic_indices]
 
-    return fragments 
+    return fragments
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.8/src/gdpx/graph/sites.py` & `gdpx-0.0.9/src/gdpx/graph/sites.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/graph/surface.py` & `gdpx-0.0.9/src/gdpx/graph/surface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/graph/utils.py` & `gdpx-0.0.9/src/gdpx/graph/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/main.py` & `gdpx-0.0.9/src/gdpx/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,188 +17,180 @@
 
 def main():
     # - register
     import_all_modules_for_register()
 
     description = "gdpx: Generating Deep Potential with Python\n"
 
-    # - arguments 
-    parser = argparse.ArgumentParser(
-        prog="gdp", 
-        description=description
-    )
+    # - arguments
+    parser = argparse.ArgumentParser(prog="gdp", description=description)
 
     parser.add_argument(
-        "-rs", "--random_seed", default=None, type=int,
-        help="global random seed"
+        "-rs", "--random_seed", default=None, type=int, help="global random seed"
     )
 
     parser.add_argument(
-        "-d", "--directory", default=pathlib.Path.cwd(),
-        help="working directory"
+        "-d", "--directory", default=pathlib.Path.cwd(), help="working directory"
     )
-    
+
     # the workflow tracker
     parser.add_argument(
-        "-p", "--potential", default=None,
-        help = "target potential related configuration (json/yaml)"
+        "-p",
+        "--potential",
+        default=None,
+        help="target potential related configuration (json/yaml)",
     )
 
     parser.add_argument(
-        "-nj", "--n_jobs", default = 1, type=int,
-        help = "number of processors"
+        "-nj", "--n_jobs", default=1, type=int, help="number of processors"
     )
 
     parser.add_argument(
-        "--debug", action="store_true",
-        help = "debug mode that gives more information"
-    )
-    
-    parser.add_argument(
-        "--log", default="gdp.out",
-        help = "logging output file"
+        "--debug", action="store_true", help="debug mode that gives more information"
     )
-    
-    # subcommands in the entire workflow 
+
+    parser.add_argument("--log", default="gdp.out", help="logging output file")
+
+    # subcommands in the entire workflow
     subparsers = parser.add_subparsers(
-        title="available subcommands", 
-        dest="subcommand", 
-        help="sub-command help"
+        title="available subcommands", dest="subcommand", help="sub-command help"
     )
 
     # - run session
     parser_session = subparsers.add_parser(
-        "session", help="run gdpy session", 
-        description=str(registers.variable)+"\n"+str(registers.operation), 
-        formatter_class=argparse.RawDescriptionHelpFormatter
+        "session",
+        help="run gdpy session",
+        description=str(registers.variable) + "\n" + str(registers.operation),
+        formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser_session.add_argument(
         "SESSION", help="session configuration file (json/yaml)"
     )
     parser_session.add_argument(
-        "--feed", default=None, nargs="+", 
-        help="session placeholders"
+        "--feed", default=None, nargs="+", help="session placeholders"
     )
     parser_session.add_argument(
-        "--timewait", default=-1, type=float,
-        help="waiting time between repeated running"
+        "--timewait",
+        default=-1,
+        type=float,
+        help="waiting time between repeated running",
     )
-    
+
     # - build structures
     parser_build = subparsers.add_parser(
-        "build", help="build structures",
-        description=str(registers.builder), 
-        formatter_class=argparse.RawDescriptionHelpFormatter
+        "build",
+        help="build structures",
+        description=str(registers.builder),
+        formatter_class=argparse.RawDescriptionHelpFormatter,
     )
+    parser_build.add_argument("CONFIG", help="builder configuration file (json/yaml)")
     parser_build.add_argument(
-        "CONFIG", help="builder configuration file (json/yaml)"
+        "-s",
+        "--substrates",
+        default=None,
+        help="file that stores substrates (e.g. *.xyz)",
     )
     parser_build.add_argument(
-        "-s", "--substrates", default=None,
-        help="file that stores substrates (e.g. *.xyz)"
-    )
-    parser_build.add_argument(
-        "-n", "--number", default=1, type=int,
-        help="number of structures to build"
+        "-n", "--number", default=1, type=int, help="number of structures to build"
     )
 
     # - convert dataset format
     parser_convert = subparsers.add_parser(
-        "convert", help="convert dataset formats",
-    )
-    parser_convert.add_argument(
-        "INPUT", help="path of the input dataset"
+        "convert",
+        help="convert dataset formats",
     )
-    
+    parser_convert.add_argument("INPUT", help="path of the input dataset")
+
     # - automatic training
     parser_train = subparsers.add_parser(
-        "train", help="automatic training utilities",
-        description=str(registers.trainer)+"\n"+str(registers.dataloader), 
-        formatter_class=argparse.RawDescriptionHelpFormatter
-    )
-    parser_train.add_argument(
-        "CONFIG", help="training configuration file (json/yaml)"
+        "train",
+        help="automatic training utilities",
+        description=str(registers.trainer) + "\n" + str(registers.dataloader),
+        formatter_class=argparse.RawDescriptionHelpFormatter,
     )
+    parser_train.add_argument("CONFIG", help="training configuration file (json/yaml)")
 
     # --- compute interface
     parser_compute = subparsers.add_parser(
-        "compute", help="compute structures with basic methods (MD, MIN, and ...)",
+        "compute",
+        help="compute structures with basic methods (MD, MIN, and ...)",
         description=str(registers.manager),
-        formatter_class=argparse.RawDescriptionHelpFormatter
+        formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser_compute.add_argument(
-        "STRUCTURE", nargs="*",
-        help="a structure file that stores one or more structures"
+        "STRUCTURE",
+        nargs="*",
+        help="a structure file that stores one or more structures",
     )
     parser_compute.add_argument(
-        "-b", "--batch", default=None, type=int,
-        help="run selected batch number (useful when queue run)"
+        "-b",
+        "--batch",
+        default=None,
+        type=int,
+        help="run selected batch number (useful when queue run)",
     )
     parser_compute.add_argument(
-        "--spawn", action="store_true",
-        help="If the computation is spawned, it will not save results until all jobs are finished."
+        "--spawn",
+        action="store_true",
+        help="If the computation is spawned, it will not save results until all jobs are finished.",
     )
     parser_compute.add_argument(
-        "--archive", action="store_true",
-        help="whether archive computation folders when retrieve"
+        "--archive",
+        action="store_true",
+        help="whether archive computation folders when retrieve",
     )
 
     # --- expedition interface
     parser_explore = subparsers.add_parser(
-        "explore", help="explore structures with advanced methods (GA, MC, and ...)",
+        "explore",
+        help="explore structures with advanced methods (GA, MC, and ...)",
         description=str(registers.expedition),
-        formatter_class=argparse.RawDescriptionHelpFormatter
+        formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser_explore.add_argument(
-        "CONFIG",
-        help="json/yaml file that stores parameters for a task"
+        "CONFIG", help="json/yaml file that stores parameters for a task"
     )
     parser_explore.add_argument(
-        "--wait", default=None, type=float,
-        help="wait time after each run"
+        "--wait", default=None, type=float, help="wait time after each run"
     )
 
     # selection
     parser_select = subparsers.add_parser(
         "select",
         help="apply various selection operations",
-        description=str(registers.selector), 
-        formatter_class=argparse.RawDescriptionHelpFormatter
+        description=str(registers.selector),
+        formatter_class=argparse.RawDescriptionHelpFormatter,
     )
+    parser_select.add_argument("CONFIG", help="selection configuration file")
     parser_select.add_argument(
-        "CONFIG", help="selection configuration file"
-    )
-    parser_select.add_argument(
-        "-s", "--structure", required=True, 
-        help="structure generator"
+        "-s", "--structure", required=True, help="structure generator"
     )
 
     # --- validation
     parser_validation = subparsers.add_parser(
-        "valid", help="validate properties with trained models",
-        description=str(registers.validator), 
-        formatter_class=argparse.RawDescriptionHelpFormatter
-    )
-    parser_validation.add_argument(
-        "CONFIG", help="validation configuration file"
+        "valid",
+        help="validate properties with trained models",
+        description=str(registers.validator),
+        formatter_class=argparse.RawDescriptionHelpFormatter,
     )
-    
-    # === execute 
+    parser_validation.add_argument("CONFIG", help="validation configuration file")
+
+    # === execute
     args = parser.parse_args()
-    
+
     # - update global configuration
     if args.debug:
         config.logger.setLevel(logging.DEBUG)
 
     curr_wdir = pathlib.Path(args.directory)
     if not curr_wdir.exists():
         curr_wdir.mkdir(parents=True)
 
     if args.log:
-        logfpath = curr_wdir/args.log
+        logfpath = curr_wdir / args.log
         if logfpath.exists():
             fh = logging.FileHandler(logfpath, mode="a")
         else:
             fh = logging.FileHandler(logfpath, mode="w")
         fh.setFormatter(config.formatter)
         config.logger.addHandler(fh)
 
@@ -206,15 +198,15 @@
     for line in config.LOGO_LINES:
         config._print(line)
 
     # -- set njobs
     config.NJOBS = args.n_jobs
     if config.NJOBS != 1:
         config._print(f"Use {config.NJOBS} processors.")
-    
+
     # -- set rng
     # TODO: load random state from a file???
     random_seed = args.random_seed
     if random_seed is None:
         # NOTE: np.random should only be called here once...
         random_seed = np.random.randint(0, 1e8)
     else:
@@ -224,54 +216,87 @@
 
     config._print(f"GLOBAL RANDOM SEED : {random_seed}")
     rng_state = config.GRNG.bit_generator.state
     for l in dict2str(rng_state).split("\n"):
         config._print(l)
 
     # - potential
-    potter = None
     if args.potential:
         # a worker or a List of worker
         from .cli.compute import convert_config_to_potter
-        potter = convert_config_to_potter(args.potential) 
+
+        potter = convert_config_to_potter(args.potential)
+    else:
+        potter = [None]
 
     # - use subcommands
     if args.subcommand == "session":
         from gdpx.core.session import run_session
+
         run_session(args.SESSION, args.feed, args.timewait, args.directory)
     elif args.subcommand == "convert":
         from gdpx.data import convert_dataset
+
         convert_dataset(args.INPUT)
     elif args.subcommand == "train":
         from gdpx.trainer import run_newtrainer
+
         run_newtrainer(args.CONFIG, args.directory)
     elif args.subcommand == "build":
         build_config = parse_input_file(args.CONFIG)
-        from .builder.interface import build_structures
+        from .cli.build import build_structures
+
         build_structures(build_config, args.substrates, args.number, args.directory)
     elif args.subcommand == "select":
         from gdpx.selector.interface import run_selection
+
         run_selection(args.CONFIG, args.structure, args.directory)
     elif args.subcommand == "compute":
-        from .cli.compute import run_worker
-        run_worker(
-            args.STRUCTURE, potter, batch=args.batch, 
-            spawn=args.spawn, archive=args.archive, directory=args.directory
-        )
+        if isinstance(potter, list):
+            first_worker = potter[0]
+        else:
+            # FIXME: This is for reactor but we need unify this with computer.
+            first_worker = potter
+            potter = [potter]
+        config._print(f"{first_worker =}")
+        if first_worker is not None:
+            # For compatibility, the classic mode
+            # `gdp -p ./worker.yaml compute structures.xyz`
+            from .cli.compute import run_worker
+
+            run_worker(
+                args.STRUCTURE,
+                potter,
+                batch=args.batch,
+                spawn=args.spawn,
+                archive=args.archive,
+                directory=args.directory,
+            )
+        else:  # Use GridWorker here!!
+            from .cli.compute import run_grid_worker
+
+            run_grid_worker(
+                parse_input_file(args.STRUCTURE[0]),
+                batch=args.batch,
+                spawn=args.spawn,
+                directory=args.directory,
+            )
     elif args.subcommand == "explore":
-        from .expedition.interface import run_expedition
+        from .cli.explore import run_expedition
+
         params = parse_input_file(args.CONFIG)
         run_expedition(params, args.wait, args.directory, potter[0])
     elif args.subcommand == "valid":
         from gdpx.validator import run_validation
+
         params = parse_input_file(args.CONFIG)
         run_validation(params, args.directory, potter[0])
     else:
         ...
-    
+
     # - report the end random state
     config._print(f"GLOBAL RANDOM SEED : {random_seed}")
     rng_state = config.GRNG.bit_generator.state
     for l in dict2str(rng_state).split("\n"):
         config._print(l)
 
     return
```

### Comparing `gdpx-0.0.8/src/gdpx/nanoparticle.py` & `gdpx-0.0.9/src/gdpx/nanoparticle.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/calculators/dummy.py` & `gdpx-0.0.9/src/gdpx/potential/calculators/dummy.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/calculators/mixer.py` & `gdpx-0.0.9/src/gdpx/potential/calculators/mixer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/interface.py` & `gdpx-0.0.9/src/gdpx/potential/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/manager.py` & `gdpx-0.0.9/src/gdpx/potential/manager.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/__init__.py` & `gdpx-0.0.9/src/gdpx/potential/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/asepot.py` & `gdpx-0.0.9/src/gdpx/potential/managers/asepot.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/bias.py` & `gdpx-0.0.9/src/gdpx/potential/managers/bias.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/cp2k.py` & `gdpx-0.0.9/src/gdpx/potential/managers/cp2k.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/deepmd/calculator.py` & `gdpx-0.0.9/src/gdpx/potential/managers/deepmd/calculator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/deepmd/convert.py` & `gdpx-0.0.9/src/gdpx/potential/managers/deepmd/convert.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/deepmd/deepmd.py` & `gdpx-0.0.9/src/gdpx/potential/managers/deepmd/deepmd.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/dftd3.py` & `gdpx-0.0.9/src/gdpx/potential/managers/dftd3.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/eam.py` & `gdpx-0.0.9/src/gdpx/potential/managers/eam.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/emt.py` & `gdpx-0.0.9/src/gdpx/potential/managers/emt.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/espresso.py` & `gdpx-0.0.9/src/gdpx/potential/managers/espresso.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/gp/bench.py` & `gdpx-0.0.9/src/gdpx/potential/managers/gp/bench.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/gp/fgp.py` & `gdpx-0.0.9/src/gdpx/potential/managers/gp/fgp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/gp/gptools.py` & `gdpx-0.0.9/src/gdpx/potential/managers/gp/gptools.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/gp/representation.py` & `gdpx-0.0.9/src/gdpx/potential/managers/gp/representation.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/gp/sgp.py` & `gdpx-0.0.9/src/gdpx/potential/managers/gp/sgp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/grid.py` & `gdpx-0.0.9/src/gdpx/potential/managers/grid.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/lasp.py` & `gdpx-0.0.9/src/gdpx/potential/managers/lasp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/mace.py` & `gdpx-0.0.9/src/gdpx/potential/managers/mace.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/mixer.py` & `gdpx-0.0.9/src/gdpx/potential/managers/mixer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*
 
 
 import copy
 from typing import List
 
-from . import registers
+from ase.calculators.calculator import Calculator
+
 from . import AbstractPotentialManager, DummyCalculator
 from ..calculators.mixer import EnhancedCalculator
-
-from ase.calculators.calculator import Calculator
+from ..utils import convert_input_to_potter
 
 
 class MixerManager(AbstractPotentialManager):
 
     name = "mixer"
     implemented_backends = ("ase",)
 
@@ -24,34 +24,29 @@
     )
 
     def __init__(self) -> None:
         """"""
 
         return
 
-    def register_calculator(self, calc_params) -> None:
+    def register_calculator(self, calc_params, *args, **kwargs) -> None:
         """"""
         super().register_calculator(calc_params)
 
         # some basic parameters
         save_host = calc_params.get("save_host", True)
 
         # process potters
         potters_ = calc_params.get("potters", [])
         npotters = len(potters_)
         assert npotters > 1, "Mixer needs at least two potters."
 
         potters = []
         for potter_ in potters_:
-            if isinstance(potter_, AbstractPotentialManager):
-                potter = potter_
-            else:  # assume it is a dict
-                name = potter_.get("name", None)
-                potter = registers.create("manager", name, convert_name=True)
-                potter.register_calculator(potter_.get("params", {}))
+            potter = convert_input_to_potter(potter_)
             potters.append(potter)
 
         # Used by ASE to determine timestep, dump_period ...
         self.potters = potters
 
         # try broadcasting calculators
         broadcast_index = -1
```

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/nequip.py` & `gdpx-0.0.9/src/gdpx/potential/managers/nequip.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/plumed/calculators/plumed.py` & `gdpx-0.0.9/src/gdpx/potential/managers/plumed/calculators/plumed.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/plumed/calculators/plumed2.py` & `gdpx-0.0.9/src/gdpx/potential/managers/plumed/calculators/plumed2.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/plumed/plumed.py` & `gdpx-0.0.9/src/gdpx/potential/managers/plumed/plumed.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/reann/beann.py` & `gdpx-0.0.9/src/gdpx/potential/managers/reann/beann.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/reann/calculators/reann.py` & `gdpx-0.0.9/src/gdpx/potential/managers/reann/calculators/reann.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             .to(self.device)
             .to(self.dtype)
         )
         symbols = list(self.atoms.symbols)
         species = [self.atomtype.index(i) for i in symbols]
         species = torch.tensor(species, device=self.device, dtype=torch.long)
         energy, force = self.pes(cart, neighlist, shifts, species)
-        energy = float(energy.detach().numpy())
+        energy = float(energy.detach().cpu().numpy())
         self.results["energy"] = energy
-        force = force.detach().numpy()
+        force = force.detach().cpu().numpy()
         self.results["forces"] = force.copy()
 
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/reann/reann.py` & `gdpx-0.0.9/src/gdpx/potential/managers/reann/reann.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/reax.py` & `gdpx-0.0.9/src/gdpx/potential/managers/reax.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/schnet.py` & `gdpx-0.0.9/src/gdpx/potential/managers/schnet.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/vasp.py` & `gdpx-0.0.9/src/gdpx/potential/managers/vasp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/managers/xtb.py` & `gdpx-0.0.9/src/gdpx/potential/managers/xtb.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/potential/trainer.py` & `gdpx-0.0.9/src/gdpx/potential/trainer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/__init__.py` & `gdpx-0.0.9/src/gdpx/reactor/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/future/AccCons.py` & `gdpx-0.0.9/src/gdpx/reactor/future/AccCons.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/future/AccNEB.py` & `gdpx-0.0.9/src/gdpx/reactor/future/AccNEB.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/future/cmp_mep.py` & `gdpx-0.0.9/src/gdpx/reactor/future/cmp_mep.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/future/constrain.py` & `gdpx-0.0.9/src/gdpx/reactor/future/constrain.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/future/crs.py` & `gdpx-0.0.9/src/gdpx/reactor/future/crs.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/future/diffusion3.py` & `gdpx-0.0.9/src/gdpx/reactor/future/diffusion3.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/future/find_adsorption.py` & `gdpx-0.0.9/src/gdpx/reactor/future/find_adsorption.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/future/find_inter.py` & `gdpx-0.0.9/src/gdpx/reactor/future/find_inter.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/future/muller-brown.py` & `gdpx-0.0.9/src/gdpx/reactor/future/muller-brown.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/future/test_mh.py` & `gdpx-0.0.9/src/gdpx/reactor/future/test_mh.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/interface.py` & `gdpx-0.0.9/src/gdpx/reactor/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/reactor.py` & `gdpx-0.0.9/src/gdpx/reactor/reactor.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/string/cp2k.py` & `gdpx-0.0.9/src/gdpx/reactor/string/cp2k.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/string/grid.py` & `gdpx-0.0.9/src/gdpx/reactor/string/grid.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/string/pathway.py` & `gdpx-0.0.9/src/gdpx/reactor/string/pathway.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/string/string.py` & `gdpx-0.0.9/src/gdpx/reactor/string/string.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/string/vasp.py` & `gdpx-0.0.9/src/gdpx/reactor/string/vasp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/reactor/utils.py` & `gdpx-0.0.9/src/gdpx/reactor/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/scheduler/__init__.py` & `gdpx-0.0.9/src/gdpx/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/scheduler/interface.py` & `gdpx-0.0.9/src/gdpx/scheduler/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/scheduler/local.py` & `gdpx-0.0.9/src/gdpx/scheduler/local.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/scheduler/lsf.py` & `gdpx-0.0.9/src/gdpx/scheduler/lsf.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/scheduler/pbs.py` & `gdpx-0.0.9/src/gdpx/scheduler/pbs.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/scheduler/scheduler.py` & `gdpx-0.0.9/src/gdpx/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/scheduler/slurm.py` & `gdpx-0.0.9/src/gdpx/scheduler/slurm.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/__init__.py` & `gdpx-0.0.9/src/gdpx/selector/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/basin.py` & `gdpx-0.0.9/src/gdpx/selector/basin.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/compare.py` & `gdpx-0.0.9/src/gdpx/selector/compare.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/composition.py` & `gdpx-0.0.9/src/gdpx/selector/composition.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/cur.py` & `gdpx-0.0.9/src/gdpx/selector/cur.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/descriptor.py` & `gdpx-0.0.9/src/gdpx/selector/descriptor.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/graph.py` & `gdpx-0.0.9/src/gdpx/selector/graph.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/interface.py` & `gdpx-0.0.9/src/gdpx/selector/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/interval.py` & `gdpx-0.0.9/src/gdpx/selector/interval.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/invariant.py` & `gdpx-0.0.9/src/gdpx/selector/invariant.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/locate.py` & `gdpx-0.0.9/src/gdpx/selector/locate.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/property.py` & `gdpx-0.0.9/src/gdpx/selector/property.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/random.py` & `gdpx-0.0.9/src/gdpx/selector/random.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/selector/scf.py` & `gdpx-0.0.9/src/gdpx/selector/scf.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/trainer/__init__.py` & `gdpx-0.0.9/src/gdpx/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/trainer/interface.py` & `gdpx-0.0.9/src/gdpx/trainer/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/atomUtils.py` & `gdpx-0.0.9/src/gdpx/utils/atomUtils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/cleave_cluster.py` & `gdpx-0.0.9/src/gdpx/utils/cleave_cluster.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/cmdrun.py` & `gdpx-0.0.9/src/gdpx/utils/cmdrun.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/cmp_refdat.py` & `gdpx-0.0.9/src/gdpx/utils/cmp_refdat.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/command.py` & `gdpx-0.0.9/src/gdpx/utils/command.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/comparision.py` & `gdpx-0.0.9/src/gdpx/utils/comparision.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/dputils/DeepPot.py` & `gdpx-0.0.9/src/gdpx/utils/dputils/DeepPot.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/dputils/acquire_dmat.py` & `gdpx-0.0.9/src/gdpx/utils/dputils/acquire_dmat.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/geometry.py` & `gdpx-0.0.9/src/gdpx/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/plot_dimer.py` & `gdpx-0.0.9/src/gdpx/utils/plot_dimer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/reduce_dataset.py` & `gdpx-0.0.9/src/gdpx/utils/reduce_dataset.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/second_reduce.py` & `gdpx-0.0.9/src/gdpx/utils/second_reduce.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/split-dataset.py` & `gdpx-0.0.9/src/gdpx/utils/split-dataset.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/utils/strucopy.py` & `gdpx-0.0.9/src/gdpx/utils/strucopy.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/validator/__init__.py` & `gdpx-0.0.9/src/gdpx/validator/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from typing import NoReturn, List, Union
 
 from ..core.register import registers
 
 from .dimer import DimerValidator
 registers.validator.register("dimer")(DimerValidator)
 
+from .trimer import TrimerValidator
+registers.validator.register("trimer")(TrimerValidator)
+
 from .mdf import MassDistributionValidator
 registers.validator.register("mass_distribution")(MassDistributionValidator)
 
 from .rdf import RdfValidator
 registers.validator.register("radial_distribution")(RdfValidator)
 
 from .eos import EquationOfStateValidator
@@ -67,8 +70,8 @@
     # run over validations
     directory = pathlib.Path(directory)
 
     raise NotImplementedError("Command Line Validation is NOT Suppoted.")
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.8/src/gdpx/validator/diffusion_coefficient.py` & `gdpx-0.0.9/src/gdpx/validator/diffusion_coefficient.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/validator/dimer.py` & `gdpx-0.0.9/src/gdpx/validator/dimer.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 import copy
 import itertools
 from typing import List
 import warnings
 
 import numpy as np
 
-import matplotlib as mpl
-mpl.use("Agg") #silent mode
-from matplotlib import pyplot as plt
+import matplotlib.pyplot as plt
 try:
     plt.style.use("presentation")
 except Exception as e:
-    #print("Used default matplotlib style.")
     ...
 
 from ase import Atoms
 from ase.io import read, write
 
 from ..worker.drive import DriverBasedWorker
 from .validator import AbstractValidator
@@ -32,24 +29,28 @@
         super().run()
         self._print(dataset["reference"])
         for prefix, frames in dataset["reference"].items():
             self._irun(prefix, frames, None, worker)
 
         return
 
-    def _irun(self, prefix: str, ref_frames: List[Atoms], pred_frames: List[Atoms], worker):
+    def _irun(
+        self, prefix: str, ref_frames: List[Atoms], pred_frames: List[Atoms], worker
+    ):
         """"""
         # - check if input frames are dimers...
         chemicals = []
         for atoms in ref_frames:
             natoms = len(atoms)
             assert natoms == 2, f"Input structure at {self.directory} must be a dimer."
             chemicals.append(atoms.get_chemical_formula())
-            assert len(set(chemicals)) == 1, f"Input dimers are different. Maybe {chemicals[0]}?"
-        
+            assert (
+                len(set(chemicals)) == 1
+            ), f"Input dimers are different. Maybe {chemicals[0]}?"
+
         # - read reference
         ref_symbols, ref_energies, ref_forces = get_properties(ref_frames)
         nframes = len(ref_frames)
         ref_natoms = [len(a) for a in ref_frames]
 
         if pred_frames is None:
             # NOTE: use worker to calculate
@@ -72,52 +73,66 @@
                     ...
                 write(cached_pred_fpath, pred_frames)
             else:
                 pred_frames = read(cached_pred_fpath, ":")
         else:
             ...
         pred_symbols, pred_energies, pred_forces = get_properties(pred_frames)
-    
+
         # - get reaction coordinate (dimer distance here)
         ref_distances = []
         for atoms in ref_frames:
             dis = atoms.get_distance(0, 1, mic=True)
             ref_distances.append(dis)
-        
+
         # - save data
-        abs_errors = [x-y for x,y in zip(pred_energies, ref_energies)]
-        rel_errors = [(x/y)*100. for x,y in zip(abs_errors,ref_energies)]
-        data = np.array([ref_distances,ref_energies,pred_energies,abs_errors,rel_errors]).T
+        abs_errors = [x - y for x, y in zip(pred_energies, ref_energies)]
+        rel_errors = [(x / y) * 100.0 for x, y in zip(abs_errors, ref_energies)]
+        data = np.array(
+            [ref_distances, ref_energies, pred_energies, abs_errors, rel_errors]
+        ).T
 
         np.savetxt(
-            self.directory/prefix/f"{prefix}.dat", data, 
-            fmt="%8.4f  %12.4f  %12.4f  %12.4f  %8.4f", 
+            self.directory / prefix / f"{prefix}.dat",
+            data,
+            fmt="%8.4f  %12.4f  %12.4f  %12.4f  %8.4f",
             header="{:<8s}  {:<12s}  {:<12s}  {:<12s}  {:<8s}".format(
                 "dis", "ref", "mlp", "abs", "rel [%]"
-            )
+            ),
         )
 
         # - plot data
         fig, ax = plt.subplots(
-            nrows=1, ncols=1,
-            gridspec_kw={"hspace": 0.3}, figsize=(16, 9)
+            nrows=1, ncols=1, gridspec_kw={"hspace": 0.3}, figsize=(16, 9)
         )
         plt.suptitle(f"{prefix} with nframes {nframes}")
 
-        ax.plot(ref_distances, ref_energies, marker="o",  markerfacecolor="w", label="Reference")
-        ax.plot(ref_distances, pred_energies, marker="o", markerfacecolor="w", label="Prediction")
+        ax.plot(
+            ref_distances,
+            ref_energies,
+            marker="o",
+            markerfacecolor="w",
+            label="Reference",
+        )
+        ax.plot(
+            ref_distances,
+            pred_energies,
+            marker="o",
+            markerfacecolor="w",
+            label="Prediction",
+        )
 
         ax.set_ylabel("Energy [eV]")
         ax.set_xlabel("Dimer Distance [Å]")
 
         ax.legend()
 
-        if (self.directory/f"{prefix}.png").exists():
+        if (self.directory / f"{prefix}.png").exists():
             warnings.warn(f"Figure file {prefix} exists.", UserWarning)
         else:
-            plt.savefig(self.directory/prefix/f"{prefix}.png")
+            plt.savefig(self.directory / prefix / f"{prefix}.png")
 
         return
-    
+
 
 if __name__ == "__main__":
     pass
```

### Comparing `gdpx-0.0.8/src/gdpx/validator/eos.py` & `gdpx-0.0.9/src/gdpx/validator/eos.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/validator/interface.py` & `gdpx-0.0.9/src/gdpx/validator/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/validator/mdf.py` & `gdpx-0.0.9/src/gdpx/validator/mdf.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/validator/melting_point.py` & `gdpx-0.0.9/src/gdpx/validator/melting_point.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/validator/minima.py` & `gdpx-0.0.9/src/gdpx/validator/minima.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/validator/rank.py` & `gdpx-0.0.9/src/gdpx/validator/rank.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/validator/rdf.py` & `gdpx-0.0.9/src/gdpx/validator/rdf.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/validator/rxn.py` & `gdpx-0.0.9/src/gdpx/validator/rxn.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/validator/spc.py` & `gdpx-0.0.9/src/gdpx/validator/spc.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/validator/surface_energy.py` & `gdpx-0.0.9/src/gdpx/validator/surface_energy.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/validator/utils.py` & `gdpx-0.0.9/src/gdpx/validator/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/validator/validator.py` & `gdpx-0.0.9/src/gdpx/validator/validator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/worker/drive.py` & `gdpx-0.0.9/src/gdpx/worker/drive.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/worker/explore.py` & `gdpx-0.0.9/src/gdpx/worker/explore.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,31 @@
 """Worker that manages expeditions.
 
 Since an expedition is made up of several basic workers, this worker is a monitor that 
 tracks its progress.
 
 """
 
+
 class ExpeditionBasedWorker(AbstractWorker):
 
     #: Prefix of the expedition folder name.
     EXP_INDEX: str = "expedition"
 
     batchsize: int = 1
 
     _script_name: str = "run.script"
 
-    def __init__(self, expedition, scheduler: AbstractScheduler, batchsize: int=1, directory=None) -> None:
+    def __init__(
+        self,
+        expedition,
+        scheduler: AbstractScheduler,
+        batchsize: int = 1,
+        directory=None,
+    ) -> None:
         """"""
         super().__init__(directory)
 
         self.expedition = expedition
         self.scheduler = scheduler
 
         self.batchsize = batchsize
@@ -44,18 +51,18 @@
         super().run(*args, **kwargs)
 
         expedition = self.expedition
         scheduler = self.scheduler
 
         # - read metadata from file or database
         with TinyDB(
-            self.directory/f"_{self.scheduler.name}_jobs.json", indent=2
+            self.directory / f"_{self.scheduler.name}_jobs.json", indent=2
         ) as database:
             queued_jobs = database.search(Query().queued.exists())
-        queued_names = [q["gdir"][self.UUIDLEN+1:] for q in queued_jobs]
+        queued_names = [q["gdir"][self.UUIDLEN + 1 :] for q in queued_jobs]
 
         size = 1
         for i in range(size):
             uid = str(uuid.uuid1())
             batch_name = f"{self.EXP_INDEX}-{i}"
             job_name = uid + "-" + self.EXP_INDEX + "-" + f"{i}"
             wdir = self.directory / (self.EXP_INDEX + "-" + f"{i}")
@@ -64,129 +71,131 @@
                 continue
             wdir.mkdir(parents=True, exist_ok=True)
 
             if self.scheduler.name == "local":
                 expedition.directory = wdir
                 expedition.run()
             else:
-                inp_fpath = (wdir/f"exp-{uid}.yaml").absolute()
+                inp_fpath = (wdir / f"exp-{uid}.yaml").absolute()
                 exp_params = expedition.as_dict()
                 with open(inp_fpath, "w") as fopen:
                     yaml.safe_dump(exp_params, fopen)
 
                 scheduler.job_name = job_name
-                scheduler.script = wdir/f"{self._script_name}-{uid}"
+                scheduler.script = wdir / f"{self._script_name}-{uid}"
                 scheduler.user_commands = "gdp explore {} --wait {}".format(
                     str(inp_fpath), self.wait_time
                 )
                 scheduler.write()
                 if self._submit:
                     self._print(f"{wdir.name}: {scheduler.submit()}")
                 else:
                     self._print(f"{wdir.name} waits to submit.")
 
             # - update database
             with TinyDB(
-                self.directory/f"_{self.scheduler.name}_jobs.json", indent=2
+                self.directory / f"_{self.scheduler.name}_jobs.json", indent=2
             ) as database:
                 _ = database.insert(
                     dict(
-                        uid = uid,
-                        gdir=job_name, 
-                        group_number=i, 
-                        wdir_names=[wdir.name], 
-                        queued=True
+                        uid=uid,
+                        gdir=job_name,
+                        group_number=i,
+                        wdir_names=[wdir.name],
+                        queued=True,
                     )
                 )
 
         return
-    
+
     def inspect(self, resubmit=False, *args, **kwargs):
         """"""
         self._initialise(*args, **kwargs)
         self._debug(f"~~~{self.__class__.__name__}+inspect")
 
         running_jobs = self._get_running_jobs()
 
         with TinyDB(
-            self.directory/f"_{self.scheduler.name}_jobs.json", indent=2
+            self.directory / f"_{self.scheduler.name}_jobs.json", indent=2
         ) as database:
             for job_name in running_jobs:
                 doc_data = database.get(Query().gdir == job_name)
                 uid = doc_data["uid"]
                 wdir_names = doc_data["wdir_names"]
 
                 self.scheduler.job_name = job_name
-                self.scheduler.script = self.directory/f"{self._script_name}-{uid}"
+                self.scheduler.script = self.directory / f"{self._script_name}-{uid}"
 
                 if self.scheduler.is_finished():
                     # -- check if the job finished properly
                     is_finished = False
                     for x in wdir_names:
-                        wdir_path = self.directory/x
+                        wdir_path = self.directory / x
                         if not wdir_path.exists():
                             break
                         else:
                             self.expedition.directory = wdir_path
                             if not self.expedition.read_convergence():
                                 break
                     else:
                         is_finished = True
                     if is_finished:
                         database.update({"finished": True}, doc_ids=[doc_data.doc_id])
-                        #self._print(f"{job_name} finished.")
+                        # self._print(f"{job_name} finished.")
                     else:
-                        warnings.warn("Exploration does not support re-submit.", UserWarning)
-                        #if resubmit:
+                        warnings.warn(
+                            "Exploration does not support re-submit.", UserWarning
+                        )
+                        # if resubmit:
                         #    if self.scheduler.name != "local":
                         #        jobid = self.scheduler.submit()
                         #        self._print(f"{job_name} is re-submitted with JOBID {jobid}.")
                         #    else:
                         #        self._print(f"{job_name} tries to re-run.")
                         #        warnings.warn("Local scheduelr does not support re-run.", UserWarning)
                 else:
                     self._print(f"{job_name} is running...")
 
         return
-    
-    def retrieve(self, include_retrieved: bool=False, *args, **kwargs):
+
+    def retrieve(self, include_retrieved: bool = False, *args, **kwargs):
         """"""
-        #raise NotImplementedError(f"{self.__class__.__name__}")
+        # raise NotImplementedError(f"{self.__class__.__name__}")
         self.inspect(*args, **kwargs)
         self._debug(f"~~~{self.__class__.__name__}+retrieve")
 
         unretrieved_wdirs_ = []
         if not include_retrieved:
             unretrieved_jobs = self._get_unretrieved_jobs()
         else:
             unretrieved_jobs = self._get_finished_jobs()
 
         with TinyDB(
-            self.directory/f"_{self.scheduler.name}_jobs.json", indent=2
+            self.directory / f"_{self.scheduler.name}_jobs.json", indent=2
         ) as database:
             for job_name in unretrieved_jobs:
                 doc_data = database.get(Query().gdir == job_name)
                 unretrieved_wdirs_.extend(
-                    (self.directory/w).resolve() for w in doc_data["wdir_names"]
+                    (self.directory / w).resolve() for w in doc_data["wdir_names"]
                 )
             unretrieved_wdirs = unretrieved_wdirs_
 
         workers = []
         if unretrieved_wdirs:
             unretrieved_wdirs = [pathlib.Path(x) for x in unretrieved_wdirs]
             self._debug(f"unretrieved_wdirs: {unretrieved_wdirs}")
             for p in unretrieved_wdirs:
                 self.expedition.directory = p
                 workers.extend(self.expedition.get_workers())
 
         with TinyDB(
-            self.directory/f"_{self.scheduler.name}_jobs.json", indent=2
+            self.directory / f"_{self.scheduler.name}_jobs.json", indent=2
         ) as database:
             for job_name in unretrieved_jobs:
                 doc_data = database.get(Query().gdir == job_name)
                 database.update({"retrieved": True}, doc_ids=[doc_data.doc_id])
-        
+
         return workers
 
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.8/src/gdpx/worker/interface.py` & `gdpx-0.0.9/src/gdpx/worker/interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,78 +12,35 @@
 
 from ..core.operation import Operation
 from ..core.variable import Variable
 from ..core.register import registers
 from ..utils.command import parse_input_file
 
 from ..potential.manager import AbstractPotentialManager
+from ..potential.utils import convert_input_to_potter
 from ..scheduler.scheduler import AbstractScheduler
 from .worker import AbstractWorker
 from .drive import DriverBasedWorker, CommandDriverBasedWorker, QueueDriverBasedWorker
 from .react import ReactorBasedWorker
 from .single import SingleWorker
 
 
-def convert_input_to_potter(
+def broadcast_and_adjust_potter(
     inp,
     estimate_uncertainty: Optional[bool] = False,
     switch_backend: Optional[str] = None,
     print_func: Callable = print,
 ) -> List[AbstractPotentialManager]:
     """Convert an input to a potter and adjust its behaviour."""
-    potter = None
-    if isinstance(inp, AbstractPotentialManager):
-        potter = inp
-    elif isinstance(inp, Variable):
-        potter = inp.value
-    elif isinstance(inp, dict) or isinstance(inp, omegaconf.dictconfig.DictConfig):
-        potter_params = copy.deepcopy(inp)
-        name = potter_params.get("name", None)
-        potter = registers.create(
-            "manager",
-            name,
-            convert_name=True,
-        )
-        potter.register_calculator(potter_params.get("params", {}))
-        potter.version = potter_params.get("version", "unknown")
-    elif isinstance(inp, str) or isinstance(inp, pathlib.Path):
-        if pathlib.Path(inp).exists():
-            potter_params = parse_input_file(input_fpath=inp)
-            name = potter_params.get("name", None)
-            potter = registers.create(
-                "manager",
-                name,
-                convert_name=True,
-            )
-            potter.register_calculator(potter_params.get("params", {}))
-            potter.version = potter_params.get("version", "unknown")
-        else:
-            raise RuntimeError(f"The potter configuration `{inp}` does not exist.")
-    else:
-        raise RuntimeError(f"Unknown {inp} of type {type(inp)} for the potter.")
+    # convert everything into potter
+    potter = convert_input_to_potter(inp)
 
     # HACK: broadcast potters
-
-    # if isinstance(potter.calc, list):
-    #     num_calculators = len(potter.calc)
-    #     assert num_calculators > 1
-    #     calcs = potter.calc
-    #     potter.calc = None
-    #     potters = []
-    #     for i in range(num_calculators):
-    #         p = copy.deepcopy(potter)
-    #         p.calc = calcs[i]
-    #         potters.append(p)
-    # else:
-    #     num_calculators = 1
-    #     potters = [potter]
-
     if hasattr(potter, "broadcast"):
         potters = potter.broadcast(potter)
-        # print_func(f"{potters =}")
     else:
         potters = [potter]
 
     for p in potters:
         assert isinstance(p.calc, Calculator)
 
     # adjust potter behaviour
@@ -128,15 +85,15 @@
         batchsize: int = 1,
         share_wdir: bool = False,
         use_single: bool = False,
         retain_info: bool = False,
         directory=pathlib.Path.cwd(),
     ):
         """"""
-        self.potter = convert_input_to_potter(
+        self.potter = broadcast_and_adjust_potter(
             potter,
             estimate_uncertainty=estimate_uncertainty,
             switch_backend=switch_backend,
             print_func=self._print,
         )
         self.driver = self._load_driver(driver)
         self.scheduler = self._load_scheduler(scheduler)
@@ -212,22 +169,24 @@
         num_potters = len(potters)
         self._print(f"{num_potters =}")
 
         # check if there were custom wdirs, and zip longest
         num_drivers = len(drivers)
 
         # broadcast
-        pairs = list(itertools.product(range(num_potters), range(num_drivers)))
+        # pairs = list(itertools.product(range(num_potters), range(num_drivers)))
+        pairs = list(itertools.product(range(num_drivers), range(num_potters)))
         num_pairs = len(pairs)
 
         wdirs = [self.directory / f"w{i}" for i in range(num_pairs)]
 
         # create workers
         workers = []
-        for i, (p_i, d_i) in enumerate(pairs):
+        # for i, (p_i, d_i) in enumerate(pairs):
+        for i, (d_i, p_i) in enumerate(pairs):
             # workers share calculator in potter
             driver = potters[p_i].create_driver(drivers[d_i])
             if not use_single:
                 if scheduler.name == "local":
                     worker = CommandDriverBasedWorker(potters[p_i], driver, scheduler)
                 else:
                     worker = QueueDriverBasedWorker(potters[p_i], driver, scheduler)
@@ -263,15 +222,15 @@
         estimate_uncertainty: Optional[bool] = None,
         switch_backend: Optional[str] = None,
         batchsize=1,
         directory="./",
     ):
         """"""
         # - save state by all nodes
-        self.potter = convert_input_to_potter(
+        self.potter = broadcast_and_adjust_potter(
             potter,
             estimate_uncertainty=estimate_uncertainty,
             switch_backend=switch_backend,
             print_func=self._print,
         )
         self.driver = self._load_driver(driver)
         self.scheduler = self._load_scheduler(scheduler)
```

### Comparing `gdpx-0.0.8/src/gdpx/worker/react.py` & `gdpx-0.0.9/src/gdpx/worker/react.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/worker/single.py` & `gdpx-0.0.9/src/gdpx/worker/single.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/worker/train.py` & `gdpx-0.0.9/src/gdpx/worker/train.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/worker/utils.py` & `gdpx-0.0.9/src/gdpx/worker/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx/worker/worker.py` & `gdpx-0.0.9/src/gdpx/worker/worker.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.8/src/gdpx.egg-info/PKG-INFO` & `gdpx-0.0.9/src/gdpx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdpx
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automate computational chemistry/materials sciance and machine learning interatomic potential training workflow.
 Author-email: Jiayan Xu <ahcigar@foxmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdpx-0.0.8/src/gdpx.egg-info/SOURCES.txt` & `gdpx-0.0.9/src/gdpx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,32 +33,37 @@
 src/gdpx/builder/cleave_group.py
 src/gdpx/builder/cleave_surface.py
 src/gdpx/builder/constraints.py
 src/gdpx/builder/crossover.py
 src/gdpx/builder/dimer.py
 src/gdpx/builder/direct.py
 src/gdpx/builder/group.py
-src/gdpx/builder/hypercube.py
 src/gdpx/builder/insert.py
 src/gdpx/builder/interface.py
 src/gdpx/builder/packer.py
 src/gdpx/builder/perturbator.py
 src/gdpx/builder/randomBuilder.py
 src/gdpx/builder/region.py
 src/gdpx/builder/repeat.py
 src/gdpx/builder/species.py
 src/gdpx/builder/utils.py
+src/gdpx/builder/wulff.py
 src/gdpx/builder/zoom.py
 src/gdpx/builder/graph/__init__.py
 src/gdpx/builder/graph/exchange.py
 src/gdpx/builder/graph/insert.py
 src/gdpx/builder/graph/modifier.py
 src/gdpx/builder/graph/remove.py
 src/gdpx/builder/mutation/__init__.py
+src/gdpx/builder/scan/angle.py
+src/gdpx/builder/scan/hypercube.py
+src/gdpx/builder/scan/intercoord.py
+src/gdpx/cli/build.py
 src/gdpx/cli/compute.py
+src/gdpx/cli/explore.py
 src/gdpx/colvar/__init__.py
 src/gdpx/colvar/compute_reweight.py
 src/gdpx/colvar/coordination.py
 src/gdpx/colvar/distance.py
 src/gdpx/colvar/fingerprint.py
 src/gdpx/colvar/plot_meta.py
 src/gdpx/colvar/plot_string.py
@@ -78,15 +83,15 @@
 src/gdpx/computation/asedriver.py
 src/gdpx/computation/cp2k.py
 src/gdpx/computation/driver.py
 src/gdpx/computation/espresso.py
 src/gdpx/computation/interface.py
 src/gdpx/computation/lammps.py
 src/gdpx/computation/lasp.py
-src/gdpx/computation/reann.py
+src/gdpx/computation/observer.py
 src/gdpx/computation/utils.py
 src/gdpx/computation/vasp.py
 src/gdpx/computation/mc/tfmc.py
 src/gdpx/computation/md/md_utils.py
 src/gdpx/computation/md/nosehoover.py
 src/gdpx/core/__init__.py
 src/gdpx/core/node.py
@@ -120,15 +125,15 @@
 src/gdpx/describer/interface.py
 src/gdpx/describer/soap.py
 src/gdpx/describer/spc.py
 src/gdpx/expedition/__init__.py
 src/gdpx/expedition/expedition.py
 src/gdpx/expedition/interface.py
 src/gdpx/expedition/accelerated_dynamics/prev_example.py
-src/gdpx/expedition/af/afir.py
+src/gdpx/expedition/artificial_force/afir.py
 src/gdpx/expedition/ga/engine.py
 src/gdpx/expedition/ga/population.py
 src/gdpx/expedition/monte_carlo/__init__.py
 src/gdpx/expedition/monte_carlo/basin_hopping.py
 src/gdpx/expedition/monte_carlo/monte_carlo.py
 src/gdpx/expedition/monte_carlo/operators/__init__.py
 src/gdpx/expedition/monte_carlo/operators/exchange.py
@@ -145,14 +150,15 @@
 src/gdpx/graph/sites.py
 src/gdpx/graph/surface.py
 src/gdpx/graph/utils.py
 src/gdpx/potential/__init__.py
 src/gdpx/potential/interface.py
 src/gdpx/potential/manager.py
 src/gdpx/potential/trainer.py
+src/gdpx/potential/utils.py
 src/gdpx/potential/calculators/dummy.py
 src/gdpx/potential/calculators/mixer.py
 src/gdpx/potential/managers/__init__.py
 src/gdpx/potential/managers/asepot.py
 src/gdpx/potential/managers/bias.py
 src/gdpx/potential/managers/cp2k.py
 src/gdpx/potential/managers/dftd3.py
@@ -236,14 +242,15 @@
 src/gdpx/utils/command.py
 src/gdpx/utils/comparision.py
 src/gdpx/utils/geometry.py
 src/gdpx/utils/plot_dimer.py
 src/gdpx/utils/reduce_dataset.py
 src/gdpx/utils/second_reduce.py
 src/gdpx/utils/split-dataset.py
+src/gdpx/utils/strconv.py
 src/gdpx/utils/strucopy.py
 src/gdpx/utils/dputils/DeepPot.py
 src/gdpx/utils/dputils/acquire_dmat.py
 src/gdpx/validator/__init__.py
 src/gdpx/validator/diffusion_coefficient.py
 src/gdpx/validator/dimer.py
 src/gdpx/validator/eos.py
@@ -252,14 +259,15 @@
 src/gdpx/validator/melting_point.py
 src/gdpx/validator/minima.py
 src/gdpx/validator/rank.py
 src/gdpx/validator/rdf.py
 src/gdpx/validator/rxn.py
 src/gdpx/validator/spc.py
 src/gdpx/validator/surface_energy.py
+src/gdpx/validator/trimer.py
 src/gdpx/validator/utils.py
 src/gdpx/validator/validator.py
 src/gdpx/worker/__init__.py
 src/gdpx/worker/drive.py
 src/gdpx/worker/explore.py
 src/gdpx/worker/grid.py
 src/gdpx/worker/interface.py
```

