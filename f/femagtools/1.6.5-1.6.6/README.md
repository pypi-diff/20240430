# Comparing `tmp/femagtools-1.6.5.tar.gz` & `tmp/femagtools-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femagtools-1.6.5.tar", last modified: Mon Mar 25 06:45:25 2024, max compression
+gzip compressed data, was "femagtools-1.6.6.tar", last modified: Tue Apr 30 15:54:56 2024, max compression
```

## Comparing `femagtools-1.6.5.tar` & `femagtools-1.6.6.tar`

### file list

```diff
@@ -1,232 +1,238 @@
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.754620 femagtools-1.6.5/
--rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.6.5/LICENSE
--rw-r--r--   0 tar        (210) tar        (210)       39 2023-08-31 09:32:32.000000 femagtools-1.6.5/MANIFEST.in
--rw-r--r--   0 tar        (210) tar        (210)     5677 2024-03-25 06:45:25.754620 femagtools-1.6.5/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.6.5/README.md
--rw-r--r--   0 tar        (210) tar        (210)     1316 2023-11-29 08:38:16.000000 femagtools-1.6.5/pyproject.toml
--rw-r--r--   0 tar        (210) tar        (210)       38 2024-03-25 06:45:25.754620 femagtools-1.6.5/setup.cfg
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.701621 femagtools-1.6.5/src/
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.719621 femagtools-1.6.5/src/femagtools/
--rw-r--r--   0 tar        (210) tar        (210)     1615 2024-03-25 06:44:06.000000 femagtools-1.6.5/src/femagtools/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     1577 2024-01-31 08:22:56.000000 femagtools-1.6.5/src/femagtools/airgap.py
--rw-r--r--   0 tar        (210) tar        (210)    12069 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/amazon.py
--rw-r--r--   0 tar        (210) tar        (210)    13891 2023-12-15 11:25:08.000000 femagtools-1.6.5/src/femagtools/amela.py
--rw-r--r--   0 tar        (210) tar        (210)     7660 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    71680 2024-03-06 12:39:21.000000 femagtools-1.6.5/src/femagtools/bch.py
--rw-r--r--   0 tar        (210) tar        (210)     3142 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/bchxml.py
--rw-r--r--   0 tar        (210) tar        (210)    10766 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/condor.py
--rw-r--r--   0 tar        (210) tar        (210)     1076 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     3136 2023-10-30 08:37:24.000000 femagtools-1.6.5/src/femagtools/config.py
--rw-r--r--   0 tar        (210) tar        (210)    26478 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/convert.py
--rw-r--r--   0 tar        (210) tar        (210)     6901 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/dakota.py
--rwxr-xr-x   0 tar        (210) tar        (210)     4068 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/dakota_femag.py
--rw-r--r--   0 tar        (210) tar        (210)     5573 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/dakotaout.py
--rw-r--r--   0 tar        (210) tar        (210)     7460 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/docker.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.722621 femagtools-1.6.5/src/femagtools/dxfsl/
--rw-r--r--   0 tar        (210) tar        (210)       76 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/dxfsl/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)    58173 2024-03-25 06:43:31.000000 femagtools-1.6.5/src/femagtools/dxfsl/area.py
--rw-r--r--   0 tar        (210) tar        (210)    20849 2024-03-18 10:17:09.000000 femagtools-1.6.5/src/femagtools/dxfsl/areabuilder.py
--rw-r--r--   0 tar        (210) tar        (210)    13381 2024-03-18 10:17:09.000000 femagtools-1.6.5/src/femagtools/dxfsl/concat.py
--rw-r--r--   0 tar        (210) tar        (210)     9236 2024-02-16 13:30:18.000000 femagtools-1.6.5/src/femagtools/dxfsl/conv.py
--rw-r--r--   0 tar        (210) tar        (210)    20821 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/dxfsl/converter.py
--rw-r--r--   0 tar        (210) tar        (210)     1266 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/dxfsl/corner.py
--rw-r--r--   0 tar        (210) tar        (210)     1861 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/dxfsl/dumprenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    23377 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/dxfsl/fslrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    11705 2024-03-18 13:35:38.000000 femagtools-1.6.5/src/femagtools/dxfsl/functions.py
--rw-r--r--   0 tar        (210) tar        (210)   164336 2024-03-18 10:17:09.000000 femagtools-1.6.5/src/femagtools/dxfsl/geom.py
--rw-r--r--   0 tar        (210) tar        (210)     3567 2024-03-18 10:17:09.000000 femagtools-1.6.5/src/femagtools/dxfsl/journal.py
--rw-r--r--   0 tar        (210) tar        (210)    42548 2024-03-25 06:43:31.000000 femagtools-1.6.5/src/femagtools/dxfsl/machine.py
--rw-r--r--   0 tar        (210) tar        (210)    12710 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/dxfsl/plotrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    48608 2024-03-25 06:43:31.000000 femagtools-1.6.5/src/femagtools/dxfsl/shape.py
--rw-r--r--   0 tar        (210) tar        (210)     8959 2024-03-25 06:43:31.000000 femagtools-1.6.5/src/femagtools/dxfsl/symmetry.py
--rw-r--r--   0 tar        (210) tar        (210)    12832 2024-01-05 09:49:19.000000 femagtools-1.6.5/src/femagtools/ecloss.py
--rw-r--r--   0 tar        (210) tar        (210)     1224 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/erg.py
--rw-r--r--   0 tar        (210) tar        (210)    43124 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/femag.py
--rw-r--r--   0 tar        (210) tar        (210)     7415 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/forcedens.py
--rw-r--r--   0 tar        (210) tar        (210)    31994 2024-03-18 10:17:09.000000 femagtools-1.6.5/src/femagtools/fsl.py
--rw-r--r--   0 tar        (210) tar        (210)     3017 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/getset.py
--rw-r--r--   0 tar        (210) tar        (210)     3903 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/gmsh.py
--rw-r--r--   0 tar        (210) tar        (210)    17144 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/google.py
--rw-r--r--   0 tar        (210) tar        (210)     1561 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/grid.py
--rw-r--r--   0 tar        (210) tar        (210)     6275 2023-12-20 15:28:20.000000 femagtools-1.6.5/src/femagtools/hxy.py
--rw-r--r--   0 tar        (210) tar        (210)    58336 2024-03-06 12:39:21.000000 femagtools-1.6.5/src/femagtools/isa7.py
--rw-r--r--   0 tar        (210) tar        (210)     1779 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/jhb.py
--rw-r--r--   0 tar        (210) tar        (210)    11320 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/job.py
--rw-r--r--   0 tar        (210) tar        (210)     5397 2023-11-29 08:38:16.000000 femagtools-1.6.5/src/femagtools/losscoeffs.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.724621 femagtools-1.6.5/src/femagtools/machine/
--rw-r--r--   0 tar        (210) tar        (210)     7174 2024-03-06 12:39:21.000000 femagtools-1.6.5/src/femagtools/machine/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)    24766 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/machine/afpm.py
--rw-r--r--   0 tar        (210) tar        (210)    13138 2024-03-06 12:39:21.000000 femagtools-1.6.5/src/femagtools/machine/effloss.py
--rw-r--r--   0 tar        (210) tar        (210)    37882 2024-03-25 06:43:31.000000 femagtools-1.6.5/src/femagtools/machine/im.py
--rwxr-xr-x   0 tar        (210) tar        (210)    56229 2024-03-18 10:17:09.000000 femagtools-1.6.5/src/femagtools/machine/pm.py
--rw-r--r--   0 tar        (210) tar        (210)    23096 2023-12-20 15:28:20.000000 femagtools-1.6.5/src/femagtools/machine/sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    34320 2024-02-16 13:30:18.000000 femagtools-1.6.5/src/femagtools/machine/sm.py
--rw-r--r--   0 tar        (210) tar        (210)    18621 2024-03-25 06:43:31.000000 femagtools-1.6.5/src/femagtools/machine/utils.py
--rw-r--r--   0 tar        (210) tar        (210)     1093 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/magnet.py
--rw-r--r--   0 tar        (210) tar        (210)    40673 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/mcv.py
--rw-r--r--   0 tar        (210) tar        (210)     1833 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/me.py
--rw-r--r--   0 tar        (210) tar        (210)    15119 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/model.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.725621 femagtools-1.6.5/src/femagtools/moo/
--rw-r--r--   0 tar        (210) tar        (210)      175 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/moo/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     5445 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/moo/algorithm.py
--rw-r--r--   0 tar        (210) tar        (210)    10100 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/moo/population.py
--rw-r--r--   0 tar        (210) tar        (210)     2391 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/moo/problem.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.725621 femagtools-1.6.5/src/femagtools/moo/test/
--rwxr-xr-x   0 tar        (210) tar        (210)     2535 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/moo/test/AlgorithmTest.py
--rwxr-xr-x   0 tar        (210) tar        (210)     5529 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/moo/test/PopulationTest.py
--rwxr-xr-x   0 tar        (210) tar        (210)      505 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/moo/test/ProblemTest.py
--rw-r--r--   0 tar        (210) tar        (210)     2825 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/moproblem.py
--rw-r--r--   0 tar        (210) tar        (210)     8435 2023-12-15 11:25:08.000000 femagtools-1.6.5/src/femagtools/multiproc.py
--rw-r--r--   0 tar        (210) tar        (210)     2151 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/mxw2msh.py
--rw-r--r--   0 tar        (210) tar        (210)    14532 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/nc.py
--rw-r--r--   0 tar        (210) tar        (210)     2052 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/netlist.py
--rw-r--r--   0 tar        (210) tar        (210)     3099 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/ntib.py
--rw-r--r--   0 tar        (210) tar        (210)     8687 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/opt.py
--rw-r--r--   0 tar        (210) tar        (210)    18799 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/parstudy.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.728621 femagtools-1.6.5/src/femagtools/plot/
--rw-r--r--   0 tar        (210) tar        (210)      920 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/plot/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)    28525 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/plot/bch.py
--rw-r--r--   0 tar        (210) tar        (210)    11192 2023-11-29 08:38:16.000000 femagtools-1.6.5/src/femagtools/plot/char.py
--rw-r--r--   0 tar        (210) tar        (210)     1136 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/plot/fieldlines.py
--rw-r--r--   0 tar        (210) tar        (210)     1082 2023-10-30 08:37:24.000000 femagtools-1.6.5/src/femagtools/plot/fluxdens.py
--rw-r--r--   0 tar        (210) tar        (210)     2996 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/plot/forcedens.py
--rw-r--r--   0 tar        (210) tar        (210)     2960 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/plot/mcv.py
--rw-r--r--   0 tar        (210) tar        (210)     9516 2023-12-20 15:28:20.000000 femagtools-1.6.5/src/femagtools/plot/nc.py
--rw-r--r--   0 tar        (210) tar        (210)     4765 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/plot/phasor.py
--rw-r--r--   0 tar        (210) tar        (210)     8462 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/plot/wdg.py
--rw-r--r--   0 tar        (210) tar        (210)     6536 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/poc.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.745621 femagtools-1.6.5/src/femagtools/templates/
--rw-r--r--   0 tar        (210) tar        (210)      874 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/FE-losses.mako
--rw-r--r--   0 tar        (210) tar        (210)     3112 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/templates/afm_rotor.mako
--rw-r--r--   0 tar        (210) tar        (210)     5344 2023-12-15 11:25:08.000000 femagtools-1.6.5/src/femagtools/templates/afm_stator.mako
--rw-r--r--   0 tar        (210) tar        (210)      246 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/airgapinduc.mako
--rw-r--r--   0 tar        (210) tar        (210)     2879 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/asyn_motor.mako
--rw-r--r--   0 tar        (210) tar        (210)     3259 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/templates/basic_modpar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1346 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/templates/bertotti.mako
--rw-r--r--   0 tar        (210) tar        (210)     1911 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/calc_field_ts.mako
--rw-r--r--   0 tar        (210) tar        (210)     1600 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/calc_therm_field.mako
--rw-r--r--   0 tar        (210) tar        (210)     1867 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/cogg_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)      400 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/colorgrad.mako
--rw-r--r--   0 tar        (210) tar        (210)     1264 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/com_motor_sim.mako
--rw-r--r--   0 tar        (210) tar        (210)      472 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/conduct-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      663 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/connect_models.mako
--rw-r--r--   0 tar        (210) tar        (210)     1339 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/cu_losses.mako
--rw-r--r--   0 tar        (210) tar        (210)     1672 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/ec-rotorbar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1983 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/fe-contr.mako
--rw-r--r--   0 tar        (210) tar        (210)      806 2023-12-15 11:25:08.000000 femagtools-1.6.5/src/femagtools/templates/fieldcalc.mako
--rw-r--r--   0 tar        (210) tar        (210)     3834 2023-11-06 06:50:13.000000 femagtools-1.6.5/src/femagtools/templates/gen_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)      560 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/inductances.mako
--rw-r--r--   0 tar        (210) tar        (210)     1359 2023-09-06 13:17:09.000000 femagtools-1.6.5/src/femagtools/templates/ld_lq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      600 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/leak_dist_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      770 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/leak_evol_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      431 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/leak_tooth_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)     1271 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/magnet-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      788 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/magnetFC2.mako
--rw-r--r--   0 tar        (210) tar        (210)     2268 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/magnetIron.mako
--rw-r--r--   0 tar        (210) tar        (210)     1426 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/magnetIron2.mako
--rw-r--r--   0 tar        (210) tar        (210)     2315 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/magnetIron3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1413 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/magnetIron4.mako
--rw-r--r--   0 tar        (210) tar        (210)     1376 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/magnetIron5.mako
--rw-r--r--   0 tar        (210) tar        (210)     3960 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/magnetIronV.mako
--rw-r--r--   0 tar        (210) tar        (210)     3520 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/templates/magnetSector.mako
--rw-r--r--   0 tar        (210) tar        (210)      727 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/magnetSectorLinear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1295 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/magnetShell.mako
--rw-r--r--   0 tar        (210) tar        (210)     4080 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/magnetShell2.mako
--rw-r--r--   0 tar        (210) tar        (210)     3425 2023-11-06 06:50:13.000000 femagtools-1.6.5/src/femagtools/templates/mesh-airgap.mako
--rw-r--r--   0 tar        (210) tar        (210)     2298 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/modal_analysis.mako
--rw-r--r--   0 tar        (210) tar        (210)     1327 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/templates/modified_steinmetz.mako
--rw-r--r--   0 tar        (210) tar        (210)     1255 2023-09-06 13:17:09.000000 femagtools-1.6.5/src/femagtools/templates/mult_cal_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      345 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/new_model.mako
--rw-r--r--   0 tar        (210) tar        (210)     3209 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/noloadflux-rot.mako
--rw-r--r--   0 tar        (210) tar        (210)     4661 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/noloadflux.mako
--rw-r--r--   0 tar        (210) tar        (210)     3146 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/noloadfluxdc.mako
--rw-r--r--   0 tar        (210) tar        (210)      344 2023-08-31 09:32:32.000000 femagtools-1.6.5/src/femagtools/templates/open.mako
--rw-r--r--   0 tar        (210) tar        (210)      630 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/plots.mako
--rw-r--r--   0 tar        (210) tar        (210)     1464 2023-09-06 13:17:09.000000 femagtools-1.6.5/src/femagtools/templates/pm_sym_f_cur.mako
--rw-r--r--   0 tar        (210) tar        (210)     2361 2023-09-06 13:17:09.000000 femagtools-1.6.5/src/femagtools/templates/pm_sym_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)     1009 2023-09-06 13:17:09.000000 femagtools-1.6.5/src/femagtools/templates/pm_sym_loss.mako
--rw-r--r--   0 tar        (210) tar        (210)     1339 2023-09-06 13:17:09.000000 femagtools-1.6.5/src/femagtools/templates/psd_psq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      643 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/ring.mako
--rw-r--r--   0 tar        (210) tar        (210)      973 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/rot_hsm.mako
--rw-r--r--   0 tar        (210) tar        (210)     2280 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/rotorAsyn.mako
--rw-r--r--   0 tar        (210) tar        (210)     1908 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/rotorKs2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1910 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/rotor_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)      753 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/rotor_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)     1981 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/shortcircuit.mako
--rw-r--r--   0 tar        (210) tar        (210)     2077 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/srm.mako
--rw-r--r--   0 tar        (210) tar        (210)      761 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/stator1.mako
--rw-r--r--   0 tar        (210) tar        (210)      599 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/stator2.mako
--rw-r--r--   0 tar        (210) tar        (210)      760 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/stator3Linear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1179 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/stator4.mako
--rw-r--r--   0 tar        (210) tar        (210)      893 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/statorBG.mako
--rw-r--r--   0 tar        (210) tar        (210)     2071 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/statorRing.mako
--rw-r--r--   0 tar        (210) tar        (210)     4942 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/statorRotor3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1799 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/stator_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)     3142 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/templates/therm-dynamic.mako
--rw-r--r--   0 tar        (210) tar        (210)     1427 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/templates/therm-static.mako
--rw-r--r--   0 tar        (210) tar        (210)     2264 2024-01-31 08:22:56.000000 femagtools-1.6.5/src/femagtools/templates/torq_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)     6228 2023-11-29 08:38:16.000000 femagtools-1.6.5/src/femagtools/tks.py
--rw-r--r--   0 tar        (210) tar        (210)    47216 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/femagtools/ts.py
--rw-r--r--   0 tar        (210) tar        (210)     1581 2024-02-16 13:30:18.000000 femagtools-1.6.5/src/femagtools/utils.py
--rw-r--r--   0 tar        (210) tar        (210)     2444 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/femagtools/vbf.py
--rw-r--r--   0 tar        (210) tar        (210)    10723 2023-12-20 15:28:20.000000 femagtools-1.6.5/src/femagtools/vtu.py
--rw-r--r--   0 tar        (210) tar        (210)    22197 2023-10-25 05:52:21.000000 femagtools-1.6.5/src/femagtools/windings.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.753620 femagtools-1.6.5/src/femagtools.egg-info/
--rw-r--r--   0 tar        (210) tar        (210)     5677 2024-03-25 06:45:25.000000 femagtools-1.6.5/src/femagtools.egg-info/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     6893 2024-03-25 06:45:25.000000 femagtools-1.6.5/src/femagtools.egg-info/SOURCES.txt
--rw-r--r--   0 tar        (210) tar        (210)        1 2024-03-25 06:45:25.000000 femagtools-1.6.5/src/femagtools.egg-info/dependency_links.txt
--rw-r--r--   0 tar        (210) tar        (210)      195 2024-03-25 06:45:25.000000 femagtools-1.6.5/src/femagtools.egg-info/entry_points.txt
--rw-r--r--   0 tar        (210) tar        (210)      147 2024-03-25 06:45:25.000000 femagtools-1.6.5/src/femagtools.egg-info/requires.txt
--rw-r--r--   0 tar        (210) tar        (210)       17 2024-03-25 06:45:25.000000 femagtools-1.6.5/src/femagtools.egg-info/top_level.txt
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.752621 femagtools-1.6.5/src/tests/
--rwxr-xr-x   0 tar        (210) tar        (210)        0 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/__init__.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.752621 femagtools-1.6.5/src/tests/engines/
--rwxr-xr-x   0 tar        (210) tar        (210)      808 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/engines/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     2014 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/engines/test_amazon.py
--rw-r--r--   0 tar        (210) tar        (210)      663 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/engines/test_config.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.752621 femagtools-1.6.5/src/tests/geom/
--rwxr-xr-x   0 tar        (210) tar        (210)      808 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/geom/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     1219 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/geom/test_functions.py
--rw-r--r--   0 tar        (210) tar        (210)     3183 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/geom/test_point_inside.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-03-25 06:45:25.753620 femagtools-1.6.5/src/tests/moo/
--rwxr-xr-x   0 tar        (210) tar        (210)      808 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/moo/__init__.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2563 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/moo/test_algorithm.py
--rwxr-xr-x   0 tar        (210) tar        (210)     5471 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/moo/test_population.py
--rwxr-xr-x   0 tar        (210) tar        (210)      467 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/moo/test_problem.py
--rw-r--r--   0 tar        (210) tar        (210)    11031 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_afpm.py
--rw-r--r--   0 tar        (210) tar        (210)     1065 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_airgap_induction.py
--rw-r--r--   0 tar        (210) tar        (210)      637 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_amela.py
--rw-r--r--   0 tar        (210) tar        (210)     1398 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    15497 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/tests/test_bchreader.py
--rw-r--r--   0 tar        (210) tar        (210)      332 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     6497 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_convert.py
--rw-r--r--   0 tar        (210) tar        (210)     1142 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_effloss.py
--rw-r--r--   0 tar        (210) tar        (210)      523 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_erg.py
--rw-r--r--   0 tar        (210) tar        (210)     1934 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/tests/test_femag.py
--rw-r--r--   0 tar        (210) tar        (210)      536 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_forcedens.py
--rwxr-xr-x   0 tar        (210) tar        (210)    16623 2024-02-08 08:06:18.000000 femagtools-1.6.5/src/tests/test_fsl.py
--rw-r--r--   0 tar        (210) tar        (210)      640 2023-12-20 15:28:20.000000 femagtools-1.6.5/src/tests/test_hxy.py
--rw-r--r--   0 tar        (210) tar        (210)      662 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_im.py
--rw-r--r--   0 tar        (210) tar        (210)     3001 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_isa7.py
--rw-r--r--   0 tar        (210) tar        (210)      824 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_jhb.py
--rw-r--r--   0 tar        (210) tar        (210)      981 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_job.py
--rw-r--r--   0 tar        (210) tar        (210)     2012 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_losscoeffs.py
--rwxr-xr-x   0 tar        (210) tar        (210)    12881 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_machine.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2608 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_magncurv.py
--rw-r--r--   0 tar        (210) tar        (210)      276 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_magnet.py
--rw-r--r--   0 tar        (210) tar        (210)      283 2023-09-08 08:10:31.000000 femagtools-1.6.5/src/tests/test_mcv.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2118 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_mcvreader.py
--rwxr-xr-x   0 tar        (210) tar        (210)     3986 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_mcvwriter.py
--rw-r--r--   0 tar        (210) tar        (210)      196 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_me.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2372 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_model.py
--rw-r--r--   0 tar        (210) tar        (210)     4205 2024-01-31 08:22:56.000000 femagtools-1.6.5/src/tests/test_nc.py
--rw-r--r--   0 tar        (210) tar        (210)     1340 2024-01-31 08:22:56.000000 femagtools-1.6.5/src/tests/test_parident.py
--rw-r--r--   0 tar        (210) tar        (210)     3200 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_parstudy.py
--rwxr-xr-x   0 tar        (210) tar        (210)     5816 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_pocfile.py
--rw-r--r--   0 tar        (210) tar        (210)     1131 2023-12-20 15:28:20.000000 femagtools-1.6.5/src/tests/test_sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    83524 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_sm.py
--rwxr-xr-x   0 tar        (210) tar        (210)      766 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_tksreader.py
--rw-r--r--   0 tar        (210) tar        (210)     1833 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_ts.py
--rwxr-xr-x   0 tar        (210) tar        (210)      832 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_vbfreader.py
--rw-r--r--   0 tar        (210) tar        (210)     1469 2023-12-20 15:28:20.000000 femagtools-1.6.5/src/tests/test_vtu.py
--rw-r--r--   0 tar        (210) tar        (210)     4912 2023-08-30 14:12:51.000000 femagtools-1.6.5/src/tests/test_windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.695255 femagtools-1.6.6/
+-rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.6.6/LICENSE
+-rw-r--r--   0 tar        (210) tar        (210)       39 2023-08-31 09:32:32.000000 femagtools-1.6.6/MANIFEST.in
+-rw-r--r--   0 tar        (210) tar        (210)     5827 2024-04-30 15:54:56.695255 femagtools-1.6.6/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.6.6/README.md
+-rw-r--r--   0 tar        (210) tar        (210)     1414 2024-04-30 15:50:23.000000 femagtools-1.6.6/pyproject.toml
+-rw-r--r--   0 tar        (210) tar        (210)       38 2024-04-30 15:54:56.695255 femagtools-1.6.6/setup.cfg
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.649256 femagtools-1.6.6/src/
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.661256 femagtools-1.6.6/src/femagtools/
+-rw-r--r--   0 tar        (210) tar        (210)     1615 2024-04-30 15:51:21.000000 femagtools-1.6.6/src/femagtools/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     1577 2024-01-31 08:22:56.000000 femagtools-1.6.6/src/femagtools/airgap.py
+-rw-r--r--   0 tar        (210) tar        (210)    12069 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/amazon.py
+-rw-r--r--   0 tar        (210) tar        (210)    13891 2023-12-15 11:25:08.000000 femagtools-1.6.6/src/femagtools/amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     7660 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    71680 2024-03-06 12:39:21.000000 femagtools-1.6.6/src/femagtools/bch.py
+-rw-r--r--   0 tar        (210) tar        (210)     3142 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/bchxml.py
+-rw-r--r--   0 tar        (210) tar        (210)    10766 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/condor.py
+-rw-r--r--   0 tar        (210) tar        (210)     1076 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     3136 2023-10-30 08:37:24.000000 femagtools-1.6.6/src/femagtools/config.py
+-rw-r--r--   0 tar        (210) tar        (210)    26478 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     6901 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/dakota.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     4068 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/dakota_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     5573 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/dakotaout.py
+-rw-r--r--   0 tar        (210) tar        (210)     7460 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/docker.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.666256 femagtools-1.6.6/src/femagtools/dxfsl/
+-rw-r--r--   0 tar        (210) tar        (210)       76 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/dxfsl/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    58872 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/area.py
+-rw-r--r--   0 tar        (210) tar        (210)    26928 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/areabuilder.py
+-rw-r--r--   0 tar        (210) tar        (210)    13385 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/concat.py
+-rw-r--r--   0 tar        (210) tar        (210)     9236 2024-02-16 13:30:18.000000 femagtools-1.6.6/src/femagtools/dxfsl/conv.py
+-rw-r--r--   0 tar        (210) tar        (210)    21322 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/converter.py
+-rw-r--r--   0 tar        (210) tar        (210)     1266 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/dxfsl/corner.py
+-rw-r--r--   0 tar        (210) tar        (210)     1861 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/dxfsl/dumprenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    13451 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/dxfparser.py
+-rw-r--r--   0 tar        (210) tar        (210)     2120 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/femparser.py
+-rw-r--r--   0 tar        (210) tar        (210)    23377 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/dxfsl/fslrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    11705 2024-04-30 15:49:42.000000 femagtools-1.6.6/src/femagtools/dxfsl/functions.py
+-rw-r--r--   0 tar        (210) tar        (210)   149449 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/geom.py
+-rw-r--r--   0 tar        (210) tar        (210)     3239 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/journal.py
+-rw-r--r--   0 tar        (210) tar        (210)    42548 2024-04-30 15:49:42.000000 femagtools-1.6.6/src/femagtools/dxfsl/machine.py
+-rw-r--r--   0 tar        (210) tar        (210)    12710 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/dxfsl/plotrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    48608 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/shape.py
+-rw-r--r--   0 tar        (210) tar        (210)     2905 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/svgparser.py
+-rw-r--r--   0 tar        (210) tar        (210)    13835 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/dxfsl/symmetry.py
+-rw-r--r--   0 tar        (210) tar        (210)    12832 2024-01-05 09:49:19.000000 femagtools-1.6.6/src/femagtools/ecloss.py
+-rw-r--r--   0 tar        (210) tar        (210)     1224 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/erg.py
+-rw-r--r--   0 tar        (210) tar        (210)    43124 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     7415 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/forcedens.py
+-rw-r--r--   0 tar        (210) tar        (210)    31994 2024-04-30 15:49:42.000000 femagtools-1.6.6/src/femagtools/fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)     3017 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/getset.py
+-rw-r--r--   0 tar        (210) tar        (210)     3903 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/gmsh.py
+-rw-r--r--   0 tar        (210) tar        (210)    17144 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/google.py
+-rw-r--r--   0 tar        (210) tar        (210)     1561 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/grid.py
+-rw-r--r--   0 tar        (210) tar        (210)     6275 2023-12-20 15:28:20.000000 femagtools-1.6.6/src/femagtools/hxy.py
+-rw-r--r--   0 tar        (210) tar        (210)    58332 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)     1779 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)    11320 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/job.py
+-rw-r--r--   0 tar        (210) tar        (210)     5397 2023-11-29 08:38:16.000000 femagtools-1.6.6/src/femagtools/losscoeffs.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.668256 femagtools-1.6.6/src/femagtools/machine/
+-rw-r--r--   0 tar        (210) tar        (210)     7174 2024-03-06 12:39:21.000000 femagtools-1.6.6/src/femagtools/machine/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    24766 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/machine/afpm.py
+-rw-r--r--   0 tar        (210) tar        (210)    13151 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/machine/effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)    37925 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/machine/im.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    58517 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/machine/pm.py
+-rw-r--r--   0 tar        (210) tar        (210)    23096 2023-12-20 15:28:20.000000 femagtools-1.6.6/src/femagtools/machine/sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    34398 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/machine/sm.py
+-rw-r--r--   0 tar        (210) tar        (210)    18621 2024-04-30 15:49:42.000000 femagtools-1.6.6/src/femagtools/machine/utils.py
+-rw-r--r--   0 tar        (210) tar        (210)     1093 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/magnet.py
+-rw-r--r--   0 tar        (210) tar        (210)    40673 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/mcv.py
+-rw-r--r--   0 tar        (210) tar        (210)     1833 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/me.py
+-rw-r--r--   0 tar        (210) tar        (210)    15119 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/model.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.669256 femagtools-1.6.6/src/femagtools/moo/
+-rw-r--r--   0 tar        (210) tar        (210)      175 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moo/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     5445 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/moo/algorithm.py
+-rw-r--r--   0 tar        (210) tar        (210)    10100 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moo/population.py
+-rw-r--r--   0 tar        (210) tar        (210)     2391 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moo/problem.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.669256 femagtools-1.6.6/src/femagtools/moo/test/
+-rwxr-xr-x   0 tar        (210) tar        (210)     2535 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moo/test/AlgorithmTest.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     5529 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moo/test/PopulationTest.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      505 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moo/test/ProblemTest.py
+-rw-r--r--   0 tar        (210) tar        (210)     2825 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/moproblem.py
+-rw-r--r--   0 tar        (210) tar        (210)     8435 2023-12-15 11:25:08.000000 femagtools-1.6.6/src/femagtools/multiproc.py
+-rw-r--r--   0 tar        (210) tar        (210)     2151 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/mxw2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)    14532 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     2052 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/netlist.py
+-rw-r--r--   0 tar        (210) tar        (210)     3099 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/ntib.py
+-rw-r--r--   0 tar        (210) tar        (210)     8687 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/opt.py
+-rw-r--r--   0 tar        (210) tar        (210)    18799 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/parstudy.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.671255 femagtools-1.6.6/src/femagtools/plot/
+-rw-r--r--   0 tar        (210) tar        (210)      920 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/plot/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    28525 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/plot/bch.py
+-rw-r--r--   0 tar        (210) tar        (210)    11192 2023-11-29 08:38:16.000000 femagtools-1.6.6/src/femagtools/plot/char.py
+-rw-r--r--   0 tar        (210) tar        (210)     1136 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/plot/fieldlines.py
+-rw-r--r--   0 tar        (210) tar        (210)     1082 2023-10-30 08:37:24.000000 femagtools-1.6.6/src/femagtools/plot/fluxdens.py
+-rw-r--r--   0 tar        (210) tar        (210)     2996 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/plot/forcedens.py
+-rw-r--r--   0 tar        (210) tar        (210)     2960 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/plot/mcv.py
+-rw-r--r--   0 tar        (210) tar        (210)     9548 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/plot/nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     4765 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/plot/phasor.py
+-rw-r--r--   0 tar        (210) tar        (210)     8462 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/plot/wdg.py
+-rw-r--r--   0 tar        (210) tar        (210)     6536 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/poc.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.672256 femagtools-1.6.6/src/femagtools/svgfsl/
+-rw-r--r--   0 tar        (210) tar        (210)     2738 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/femagtools/svgfsl/converter.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.683255 femagtools-1.6.6/src/femagtools/templates/
+-rw-r--r--   0 tar        (210) tar        (210)      874 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/FE-losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3112 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/templates/afm_rotor.mako
+-rw-r--r--   0 tar        (210) tar        (210)     5344 2023-12-15 11:25:08.000000 femagtools-1.6.6/src/femagtools/templates/afm_stator.mako
+-rw-r--r--   0 tar        (210) tar        (210)      246 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/airgapinduc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2879 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/asyn_motor.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3259 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/templates/basic_modpar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1346 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/templates/bertotti.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1911 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/calc_field_ts.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1600 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/calc_therm_field.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1867 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/cogg_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      400 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/colorgrad.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1264 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/com_motor_sim.mako
+-rw-r--r--   0 tar        (210) tar        (210)      472 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/conduct-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      663 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/connect_models.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1339 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/cu_losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1672 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/ec-rotorbar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1983 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/fe-contr.mako
+-rw-r--r--   0 tar        (210) tar        (210)      806 2023-12-15 11:25:08.000000 femagtools-1.6.6/src/femagtools/templates/fieldcalc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3834 2023-11-06 06:50:13.000000 femagtools-1.6.6/src/femagtools/templates/gen_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)      560 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/inductances.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1359 2023-09-06 13:17:09.000000 femagtools-1.6.6/src/femagtools/templates/ld_lq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      600 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/leak_dist_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      770 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/leak_evol_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      431 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/leak_tooth_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1271 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnet-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      788 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetFC2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2268 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetIron.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1426 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetIron2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2315 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetIron3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1413 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetIron4.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1376 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetIron5.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3960 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetIronV.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3520 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/templates/magnetSector.mako
+-rw-r--r--   0 tar        (210) tar        (210)      727 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetSectorLinear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1295 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetShell.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4080 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/magnetShell2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3425 2023-11-06 06:50:13.000000 femagtools-1.6.6/src/femagtools/templates/mesh-airgap.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2298 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/modal_analysis.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1327 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/templates/modified_steinmetz.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1255 2023-09-06 13:17:09.000000 femagtools-1.6.6/src/femagtools/templates/mult_cal_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      345 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/new_model.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3209 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/noloadflux-rot.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4661 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/noloadflux.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3146 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/noloadfluxdc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      344 2023-08-31 09:32:32.000000 femagtools-1.6.6/src/femagtools/templates/open.mako
+-rw-r--r--   0 tar        (210) tar        (210)      630 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/plots.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1464 2023-09-06 13:17:09.000000 femagtools-1.6.6/src/femagtools/templates/pm_sym_f_cur.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2361 2023-09-06 13:17:09.000000 femagtools-1.6.6/src/femagtools/templates/pm_sym_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1009 2023-09-06 13:17:09.000000 femagtools-1.6.6/src/femagtools/templates/pm_sym_loss.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1339 2023-09-06 13:17:09.000000 femagtools-1.6.6/src/femagtools/templates/psd_psq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      643 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/ring.mako
+-rw-r--r--   0 tar        (210) tar        (210)      973 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/rot_hsm.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2280 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/rotorAsyn.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1908 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/rotorKs2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1910 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/rotor_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)      753 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/rotor_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1981 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/shortcircuit.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2077 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/srm.mako
+-rw-r--r--   0 tar        (210) tar        (210)      761 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/stator1.mako
+-rw-r--r--   0 tar        (210) tar        (210)      599 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/stator2.mako
+-rw-r--r--   0 tar        (210) tar        (210)      760 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/stator3Linear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1179 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/stator4.mako
+-rw-r--r--   0 tar        (210) tar        (210)      893 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/statorBG.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2071 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/statorRing.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4942 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/statorRotor3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1799 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/stator_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3142 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/templates/therm-dynamic.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1427 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/templates/therm-static.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2264 2024-01-31 08:22:56.000000 femagtools-1.6.6/src/femagtools/templates/torq_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     6228 2023-11-29 08:38:16.000000 femagtools-1.6.6/src/femagtools/tks.py
+-rw-r--r--   0 tar        (210) tar        (210)    47216 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/femagtools/ts.py
+-rw-r--r--   0 tar        (210) tar        (210)     1581 2024-02-16 13:30:18.000000 femagtools-1.6.6/src/femagtools/utils.py
+-rw-r--r--   0 tar        (210) tar        (210)     2444 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/femagtools/vbf.py
+-rw-r--r--   0 tar        (210) tar        (210)    10723 2023-12-20 15:28:20.000000 femagtools-1.6.6/src/femagtools/vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)    22197 2023-10-25 05:52:21.000000 femagtools-1.6.6/src/femagtools/windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.694255 femagtools-1.6.6/src/femagtools.egg-info/
+-rw-r--r--   0 tar        (210) tar        (210)     5827 2024-04-30 15:54:56.000000 femagtools-1.6.6/src/femagtools.egg-info/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     7054 2024-04-30 15:54:56.000000 femagtools-1.6.6/src/femagtools.egg-info/SOURCES.txt
+-rw-r--r--   0 tar        (210) tar        (210)        1 2024-04-30 15:54:56.000000 femagtools-1.6.6/src/femagtools.egg-info/dependency_links.txt
+-rw-r--r--   0 tar        (210) tar        (210)      248 2024-04-30 15:54:56.000000 femagtools-1.6.6/src/femagtools.egg-info/entry_points.txt
+-rw-r--r--   0 tar        (210) tar        (210)      182 2024-04-30 15:54:56.000000 femagtools-1.6.6/src/femagtools.egg-info/requires.txt
+-rw-r--r--   0 tar        (210) tar        (210)       17 2024-04-30 15:54:56.000000 femagtools-1.6.6/src/femagtools.egg-info/top_level.txt
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.692255 femagtools-1.6.6/src/tests/
+-rwxr-xr-x   0 tar        (210) tar        (210)        0 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/__init__.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.692255 femagtools-1.6.6/src/tests/engines/
+-rwxr-xr-x   0 tar        (210) tar        (210)      808 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/engines/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     2014 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/engines/test_amazon.py
+-rw-r--r--   0 tar        (210) tar        (210)      663 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/engines/test_config.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.693255 femagtools-1.6.6/src/tests/geom/
+-rwxr-xr-x   0 tar        (210) tar        (210)      808 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/geom/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     1219 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/geom/test_functions.py
+-rw-r--r--   0 tar        (210) tar        (210)     3183 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/geom/test_point_inside.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2024-04-30 15:54:56.693255 femagtools-1.6.6/src/tests/moo/
+-rwxr-xr-x   0 tar        (210) tar        (210)      808 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/moo/__init__.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2563 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/moo/test_algorithm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     5471 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/moo/test_population.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      467 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/moo/test_problem.py
+-rw-r--r--   0 tar        (210) tar        (210)    11031 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_afpm.py
+-rw-r--r--   0 tar        (210) tar        (210)     1065 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_airgap_induction.py
+-rw-r--r--   0 tar        (210) tar        (210)      637 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     1398 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    15497 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/tests/test_bchreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      332 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     6497 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_convert.py
+-rw-r--r--   0 tar        (210) tar        (210)      383 2024-04-30 15:50:23.000000 femagtools-1.6.6/src/tests/test_dxfsl.py
+-rw-r--r--   0 tar        (210) tar        (210)     1142 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)      523 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_erg.py
+-rw-r--r--   0 tar        (210) tar        (210)     1934 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/tests/test_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)      536 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_forcedens.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    16623 2024-02-08 08:06:18.000000 femagtools-1.6.6/src/tests/test_fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)      640 2023-12-20 15:28:20.000000 femagtools-1.6.6/src/tests/test_hxy.py
+-rw-r--r--   0 tar        (210) tar        (210)      662 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_im.py
+-rw-r--r--   0 tar        (210) tar        (210)     3001 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)      824 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)      981 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2012 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_losscoeffs.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    12881 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_machine.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2608 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_magncurv.py
+-rw-r--r--   0 tar        (210) tar        (210)      276 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_magnet.py
+-rw-r--r--   0 tar        (210) tar        (210)      283 2023-09-08 08:10:31.000000 femagtools-1.6.6/src/tests/test_mcv.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2118 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_mcvreader.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     3986 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_mcvwriter.py
+-rw-r--r--   0 tar        (210) tar        (210)      196 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_me.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2372 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_model.py
+-rw-r--r--   0 tar        (210) tar        (210)     4205 2024-01-31 08:22:56.000000 femagtools-1.6.6/src/tests/test_nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1340 2024-01-31 08:22:56.000000 femagtools-1.6.6/src/tests/test_parident.py
+-rw-r--r--   0 tar        (210) tar        (210)     3200 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_parstudy.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     5816 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_pocfile.py
+-rw-r--r--   0 tar        (210) tar        (210)     1131 2023-12-20 15:28:20.000000 femagtools-1.6.6/src/tests/test_sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    83524 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_sm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      766 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_tksreader.py
+-rw-r--r--   0 tar        (210) tar        (210)     1833 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_ts.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      832 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_vbfreader.py
+-rw-r--r--   0 tar        (210) tar        (210)     1469 2023-12-20 15:28:20.000000 femagtools-1.6.6/src/tests/test_vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)     4912 2023-08-30 14:12:51.000000 femagtools-1.6.6/src/tests/test_windings.py
```

### Comparing `femagtools-1.6.5/LICENSE` & `femagtools-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/PKG-INFO` & `femagtools-1.6.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.6.5
+Version: 1.6.6
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <dzhang@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
@@ -41,14 +41,18 @@
 Requires-Dist: mako
 Requires-Dist: six
 Requires-Dist: lmfit
 Requires-Dist: netCDF4>=1.6.5
 Provides-Extra: dxfsl
 Requires-Dist: dxfgrabber; extra == "dxfsl"
 Requires-Dist: networkx; extra == "dxfsl"
+Provides-Extra: svgfsl
+Requires-Dist: dxfgrabber; extra == "svgfsl"
+Requires-Dist: networkx; extra == "svgfsl"
+Requires-Dist: lxml; extra == "svgfsl"
 Provides-Extra: mplot
 Requires-Dist: matplotlib; extra == "mplot"
 Provides-Extra: meshio
 Requires-Dist: meshio; extra == "meshio"
 Provides-Extra: vtk
 Requires-Dist: vtk; extra == "vtk"
 Provides-Extra: zmq
```

### Comparing `femagtools-1.6.5/README.md` & `femagtools-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/pyproject.toml` & `femagtools-1.6.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -29,21 +29,23 @@
     'lmfit',
     'netCDF4>=1.6.5',     # >=1.6.5 to mitigate CVE-2023-38545
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dxfsl = ['dxfgrabber', 'networkx']
+svgfsl = ['dxfgrabber', 'networkx','lxml']
 mplot =  ['matplotlib']
 meshio = ['meshio']
 vtk = ['vtk']
 zmq = ['pyzmq']
 test = ['pytest']
 
 [project.scripts]
 femagtools-plot = "femagtools.plot.bch:main"
 femagtools-convert = "femagtools.convert:main"
 femagtools-bchxml = "femagtools.bchxml:main"
 femagtools-dxfsl = "femagtools.dxfsl.conv:main"
+femagtools-svgfsl = "femagtools.svgfsl.converter:main"
 
 [tool.setuptools.dynamic]
 version = {attr = "femagtools.__version__"}
```

### Comparing `femagtools-1.6.5/src/femagtools/__init__.py` & `femagtools-1.6.6/src/femagtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Python API for FEMAG
 
 """
 __title__ = 'femagtools'
-__version__ = '1.6.5'
+__version__ = '1.6.6'
 __author__ = 'Ronald Tanner'
 __license__ = 'BSD'
 __copyright__ = 'Copyright 2016-2022 SEMAFOR Informatik & Energie AG'
 
 from .asm import read
 from .bch import Reader
 from .model import MachineModel
```

### Comparing `femagtools-1.6.5/src/femagtools/airgap.py` & `femagtools-1.6.6/src/femagtools/airgap.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/amazon.py` & `femagtools-1.6.6/src/femagtools/amazon.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/amela.py` & `femagtools-1.6.6/src/femagtools/amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/asm.py` & `femagtools-1.6.6/src/femagtools/asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/bch.py` & `femagtools-1.6.6/src/femagtools/bch.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/bchxml.py` & `femagtools-1.6.6/src/femagtools/bchxml.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/condor.py` & `femagtools-1.6.6/src/femagtools/condor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/conductor.py` & `femagtools-1.6.6/src/femagtools/conductor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/config.py` & `femagtools-1.6.6/src/femagtools/config.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/convert.py` & `femagtools-1.6.6/src/femagtools/convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/dakota.py` & `femagtools-1.6.6/src/femagtools/dakota.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/dakota_femag.py` & `femagtools-1.6.6/src/femagtools/dakota_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/dakotaout.py` & `femagtools-1.6.6/src/femagtools/dakotaout.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/docker.py` & `femagtools-1.6.6/src/femagtools/docker.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/area.py` & `femagtools-1.6.6/src/femagtools/dxfsl/area.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         self.close_to_ag_startcorner = False
         self.close_to_ag_endcorner = False
         self.close_to_startangle = False
         self.close_to_endangle = False
         self.mag_rectangle = False
         self.min_dist = 99999.0
         self.max_dist = 0.0
+        self.minmax_xy = [0,0,0,0]
         self.height = 0.0
         self.alpha = 0.0
         self.count = 1
         self.equal_areas = []
         self.delta = 0.0
         self.start = 0.0
         self.sym_startangle = 0.0
@@ -265,14 +266,15 @@
     def set_type(self, t):
         self.type = t
 
     def calc_signature(self, center):
         if not self.area:
             return
 
+        self.minmax_xy = self.minmax()
         s = self.area[0]
         mm_angle = s.minmax_angle_from_center(center)
         self.min_angle = mm_angle[0]
         self.max_angle = mm_angle[1]
 
         for s in self.area:
             mm_dist = s.minmax_from_center(center)
@@ -282,14 +284,20 @@
 
             mm_angle = s.minmax_angle_from_center(center)
             self.min_angle = min_angle(self.min_angle, mm_angle[0])
             self.max_angle = max_angle(self.max_angle, mm_angle[1])
 
         self.alpha = round(alpha_angle(self.min_angle, self.max_angle), 3)
 
+    def center_is_inside(self, center):
+        if self.minmax_xy[0] < center[0] and self.minmax_xy[1] > center[0] and \
+           self.minmax_xy[2] < center[1] and self.minmax_xy[3] > center[1]:
+            return True
+        return False
+
     def minmax_angle_dist_from_center(self, center, dist):
         circ = Circle(Element(center=center, radius=dist))
         s = self.area[0]
         my_min_angle = self.max_angle
         my_max_angle = self.min_angle
         mm_angle = None
         for s in self.area:
@@ -425,18 +433,22 @@
         if the_area_p is None:
             return (None, None, None)
 
         return (dist,
                 (the_axis_p[0], the_axis_p[1]),
                 (the_area_p[0], the_area_p[1]))
 
-    def get_alpha(self):
+    def get_alpha(self, center):
+        if self.center_is_inside(center):
+            return np.pi*2.0
         return alpha_angle(self.min_angle, self.max_angle)
 
-    def get_mid_angle(self):
+    def get_mid_angle(self, center):
+        if self.center_is_inside(center):
+            return np.pi
         return middle_angle(self.min_angle, self.max_angle)
 
     def is_equal(self, a, sym_tolerance):
         if sym_tolerance > 0.0:
             if np.isclose(round(self.min_dist, 4),
                           round(a.min_dist, 4),
                           1e-03, sym_tolerance) and \
@@ -632,15 +644,15 @@
     def is_point_inside(self, pt):
         for e in self.area:
             if e.is_point_inside(pt, include_end=True):
                 return True
         return False
 
     def get_best_point_inside(self, geom):
-        mm = self.minmax()
+        mm = self.minmax_xy
         px1 = mm[0]-5
         px2 = mm[1]+5
 
         y_dist = mm[3] - mm[2]
         step = y_dist / 6
         y_list = np.arange(mm[2] + step*0.3, mm[3] - step*0.3, step)
 
@@ -729,15 +741,15 @@
         d1 = distance(c, points[0])
         d2 = distance(c, points[1])
         p = point(c, (d1 + d2) / 2, mid_angle)
         return p
 
     def get_point_inside(self, geom):
         """return point inside area"""
-        mm = self.minmax()
+        mm = self.minmax_xy
         y = (mm[2]+mm[3])/2
         p1 = (mm[0]-5, y)
         p2 = (mm[1]+5, y)
         line = Line(Element(start=p1, end=p2))
 
         points = []
         for e in self.area:
@@ -1462,14 +1474,22 @@
                 if points_are_close(n, start_cp):
                     self.close_to_ag_startcorner = True
             if self.close_to_endangle:
                 if points_are_close(n, end_cp):
                     self.close_to_ag_endcorner = True
 
     def area_size(self):
+        if len(self.area) == 0:
+            return 0.0
+        if self.number_of_elements() < 2:
+            e = self.area[0]
+            if not is_Circle(e):
+                return 0.0
+            return np.pi * e.radius**2
+
         nodes = [n for n in self.list_of_nodes()]
         return area_size(nodes)
 
     def set_surface(self, mirrored):
         self.surface = self.area_size()
         if self.close_to_endangle and mirrored:
             self.surface = self.area_size() * 2.0
```

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/areabuilder.py` & `femagtools-1.6.6/src/femagtools/dxfsl/areabuilder.py`

 * *Files 17% similar despite different names*

```diff
@@ -337,32 +337,40 @@
         return left
 
 
 class AreaBuilder(object):
     def __init__(self,
                  geom=None,
                  rtol=1e-04,
-                 atol=1e-04):
+                 atol=1e-04,
+                 ndec=6):
         self.rtol = rtol
         self.atol = atol
+        self.ndec = ndec
         self.geom = geom
         self.area_list = []
         self.journal = getJournal()
 
     def __str__(self):
         return "rtol: {}\n".format(self.rtol) + \
                "atol: {}\n".format(self.atol)
 
     def all_neighbors(self, n):
         for n in self.geom.g.neighbors(n):
             yield n
 
     def set_edge_attributes(self):
         self.geom.set_edge_attributes()
-    
+
+    def append_new_area(self, area_list, elements):
+        a = Area(elements, self.geom.center, 0.0)
+        a.type = 0  # air
+        area_list.append(a)
+        return a
+
     def create_list_of_areas(self, main=False):
         logger.debug("Begin of create_list_of_areas")
         assert(len(self.area_list) == 0)
         self.errors = 0
 
         def append(area_list, a):
             for area in area_list:
@@ -378,18 +386,16 @@
             finished = False
             while not finished:
                 finished = True
                 nbrs = [nbr for nbr in self.geom.g.neighbors(n)]
                 for next_n in nbrs:
                     result = self.get_new_area(n, next_n)
                     if result['ok']:
-                        area = result['area']
-                        a = Area(area, self.geom.center, 0.0)
+                        a = self.append_new_area(self.area_list, result['area'])
                         logger.debug("Area %s found", a.identifier())
-                        append(self.area_list, a)
 
         t = timer.stop("{} areas created in %0.4f seconds".format(len(self.area_list)))
         if main:
             self.journal.put('time_build_areas', t)
         if self.errors > 0:
             logger.warning("WARNING: %s errors while creating %s areas",
                            self.errors, len(self.area_list))
@@ -560,7 +566,148 @@
             if nbr2.myself_direction_lefthand(start_edge, nbr1, self):
                 nbr1 = nbr2
                 logger.debug("-- is new lefthand neighbor")
 
         nbr1.log_edge(">>>> LEFT")
         logger.debug("end of next_edge_lefthand_side")
         return nbr1
+
+    def create_inner_corner_auxiliary_areas(self):
+        logger.debug("begin of create_inner_corner_auxiliary_areas")
+        if not self.geom.is_inner:
+            logger.debug("end of create_inner_corner_auxiliary_areas: not inner")
+            return
+
+        self.set_edge_attributes()
+
+        start_cp, start_exists = self.geom.get_start_airgap_corner()
+        end_cp, end_exists = self.geom.get_end_airgap_corner()
+        if start_exists and end_exists:
+            logger.debug("end of create_inner_corner_auxiliary_areas: no aktion")
+            return
+
+        airgap_line, airgap_el = self.get_inner_airgap_line()
+        if not airgap_el:
+            logger.debug("end of create_inner_corner_auxiliary_areas: no airgapline found")
+            return
+
+        logger.debug("airgapline found !!")
+        airgap_nodes = [n for n in airgap_line[1:]]
+        del airgap_nodes[-1]
+
+        if not start_exists:
+            cp = self.geom.start_corners[-1]
+            logger.debug("Start Corner: %s -- %s", cp, start_cp)
+            start_line = Line(Element(start=cp, end=start_cp),
+                              color='red',
+                              linestyle='dotted')
+
+            start_cp = start_line.node2(self.ndec)
+            for n in airgap_nodes:
+                ag_line = Line(Element(start=start_cp, end=n))
+                points = self.geom.get_intersection_points(airgap_el, ag_line, n)
+                if not points:  # no intersection
+                    d = distance(self.geom.center, n)
+                    if np.isclose(d, self.geom.max_radius):
+                        self.geom.add_arc(start_cp,
+                                          n,
+                                          self.geom.center,
+                                          self.geom.max_radius,
+                                          color='red',
+                                          linestyle='dotted')
+                    else:
+                        self.geom.add_line(start_cp,
+                                           n,
+                                           color='red',
+                                           linestyle='dotted')
+                    self.geom.add_edge(cp, start_cp, start_line)
+                    result = self.get_new_area(start_cp, n)
+                    if result['ok']:
+                        self.append_new_area(self.geom.area_list,
+                                             result['area'])
+                    self.geom.set_start_corners(self.geom.center, 0.0)
+                    break
+
+        if not end_exists:
+            cp = self.geom.end_corners[-1]
+            logger.debug("End Corner: %s -- %s", cp, end_cp)
+            end_line = Line(Element(start=cp, end=end_cp),
+                            color='red',
+                            linestyle='dotted')
+            end_cp = end_line.node2(self.ndec)
+            airgap_nodes.reverse()
+            for n in airgap_nodes:
+                ag_line = Line(Element(start=end_cp, end=n))
+                points = self.geom.get_intersection_points(airgap_el, ag_line, n)
+                if not points:  # no intersection
+                    d = distance(self.geom.center, n)
+                    if np.isclose(d, self.geom.max_radius):
+                        self.geom.add_arc(n, end_cp,
+                                          self.geom.center,
+                                          self.geom.max_radius,
+                                          color='red',
+                                          linestyle='dotted')
+                    else:
+                        self.geom.add_line(end_cp, n,
+                                           color='red',
+                                           linestyle='dotted')
+                    self.geom.add_edge(cp, end_cp, end_line)
+                    result = self.get_new_area(n, end_cp)
+                    if result['ok']:
+                        self.append_new_area(self.geom.area_list,
+                                             result['area'])
+                    self.geom.set_end_corners(self.geom.center, self.geom.alfa)
+                    break
+
+        logger.debug("end of create_inner_corner_auxiliary_areas")
+
+    def get_inner_airgap_line(self):
+        logger.debug("begin of get_inner_airgap_line")
+        assert(self.geom.is_inner)
+        assert(self.geom.area_list)
+
+        area = [a for a in self.geom.area_list if a.close_to_ag_endcorner]
+        if len(area) != 1:
+            logger.debug("end of get_inner_airgap_line: %s areas found", len(area))
+            return [], []
+
+        end_corner = self.geom.end_corners[-1]
+        logger.debug("END CORNER %s", end_corner)
+
+        nodes = [n for n in area[0].list_of_nodes()]
+        if not nodes:
+            logger.debug("end of get_inner_airgap_line: no nodes found")
+            return [], []
+
+        n1 = nodes[0]
+        if points_are_close(end_corner, n1):
+            n2 = nodes[-1]
+        else:
+            n2 = n1
+            for n1 in nodes[1:]:
+                if points_are_close(end_corner, n1):
+                    break
+                n2 = n1
+
+        if not points_are_close(end_corner, n1):
+            logger.debug("end of get_inner_airgap_line: not close to endcorner")
+            return [], []
+
+        start_corner = self.geom.start_corners[-1]
+        logger.debug("START CORNER %s", end_corner)
+
+        logger.debug("EDGE FOUND: %s - %s", n1, n2)
+        nodes = [n1, n2]
+        info = self.get_edge_info(n1, n2)
+        elements = [info.element]
+
+        while not points_are_close(start_corner, n2):
+            info.set_start_angle()
+            info = self.next_edge_lefthand_side(info)
+            if not info:  # bad
+                return []
+            n2 = info.n2
+            nodes.append(n2)
+            elements.append(info.element)
+
+        logger.debug("end of get_inner_airgap_line #%s", len(nodes))
+        return nodes, elements
```

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/concat.py` & `femagtools-1.6.6/src/femagtools/dxfsl/concat.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,17 +200,17 @@
                   e) for e in elements if is_Line(e)]
         if not elmts:
             return 0  # no lines available
 
         elmts.sort()
 
         logger.debug("Concatenate Line Elements")
-        for m, a, p, e in elmts:
-            logger.debug("Line from %s to %s [m=%s, a=%s]",
-                         e.p1, e.p2, m, a)
+        #for m, a, p, e in elmts:
+        #    logger.debug("Line from %s to %s [m=%s, a=%s]",
+        #                 e.p1, e.p2, m, a)
         logger.debug("*************************")
 
         lines_available = len(elmts)
         count = 0
         if len(elmts) < 2:
             timer.stop()
             return 0
@@ -277,17 +277,17 @@
             timer.stop("-- no arcs found in %0.4f seconds --")
             logger.debug("End of concatenate_matching_arc_elements")
             return 0  # no arcs available
 
         elmts.sort()
 
         logger.debug("Concatenate Arc Elements")
-        for c, r, a, e in elmts:
-            logger.debug("%s from %s to %s [c=%s, r=%s, a=%s]",
-                         e.classname(), e.p1, e.p2, c, r, a)
+        #for c, r, a, e in elmts:
+        #    logger.debug("%s from %s to %s [c=%s, r=%s, a=%s]",
+        #                 e.classname(), e.p1, e.p2, c, r, a)
         logger.debug("*************************")
  
         arcs_available = len(elmts)
         count = 0
 
         c1, r1, a1, e1 = elmts[0]
         arc_elements = [e1]
@@ -350,8 +350,8 @@
         new_list = [e for e in src_elements if not e.has_attribute("del")]
 
         t = timer.stop("-- {} concatenations in %0.4f seconds --".format(count))
         if main:
             self.journal.put('time_concatenation', t)
 
         logger.debug("End of concatenate_matching_elements")
-        return count>0, new_list
+        return count, new_list
```

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/conv.py` & `femagtools-1.6.6/src/femagtools/dxfsl/conv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/converter.py` & `femagtools-1.6.6/src/femagtools/dxfsl/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """read a dxf file and create a plot or fsl file
 
 """
-import os
-from femagtools.dxfsl.geom import Geometry, dxfshapes, femshapes
+from pathlib import Path
+from femagtools.dxfsl.geom import Geometry
 from femagtools.dxfsl.shape import Shape
 from femagtools.dxfsl.fslrenderer import FslRenderer, agndst
 from femagtools.dxfsl.plotrenderer import PlotRenderer
+from femagtools.dxfsl.functions import Timer
 import logging
 import logging.config
 import numpy as np
 import sys
 
 logger = logging.getLogger(__name__)
 
@@ -120,16 +121,17 @@
             write_fsl=True,
             write_png=False,
             write_id=False,
             debug_mode=False):
     layers = ()
     conv = {}
 
-    basename = os.path.basename(dxfile).split('.')[0]
-    logger.info("start processing %s", basename)
+    basename = Path(dxfile).stem
+    logger.info("***** start processing %s *****", basename)
+    timer = Timer(start_it=True)
 
     if part:
         if part[0] not in ('rotor', 'stator'):
             logger.error('FATAL: Parameter rotor or stator expected')
             return dict(error='unknown part {}'.format(part))
         if part[1] not in ('in', 'out'):
             logger.error('"{}" has to be defined in/out'.format(part[0]))
@@ -145,26 +147,36 @@
     split_ini = split
     split_cpy = False
     if not (part or view_only):
         split_ini = False
         split_cpy = split
 
     try:
-        if dxfile.split('.')[-1] == 'fem':
+        if Path(dxfile).suffix == '.fem':
+            from .femparser import femshapes
             basegeom = Geometry(femshapes(dxfile),
                                 rtol=rtol,
                                 atol=atol,
                                 split=split_ini)
-        else:
+        elif Path(dxfile).suffix == '.dxf':
+            from .dxfparser import dxfshapes
             basegeom = Geometry(dxfshapes(dxfile,
                                           mindist=mindist,
                                           layers=layers),
                                 rtol=rtol,
                                 atol=atol,
                                 split=split_ini)
+        elif Path(dxfile).suffix == '.svg':
+            from .svgparser import svgshapes
+            basegeom = Geometry(svgshapes(dxfile),
+                                rtol=rtol,
+                                atol=atol,
+                                split=split_ini)
+
+
     except FileNotFoundError as ex:
         logger.error(ex)
         return dict()
 
     logger.info("total elements %s", len(basegeom.g.edges()))
 
     p = PlotRenderer()
@@ -183,15 +195,15 @@
         return dict()
 
     basegeom.search_all_overlapping_elements()
 
     machine_base = basegeom.get_machine()
     if show_plots:
         p.render_elements(basegeom, Shape,
-                          title=os.path.basename(dxfile),
+                          title=Path(dxfile).name,
                           with_hull=False,
                           rows=3, cols=2, num=1, show=debug_mode)
 
     basegeom.search_all_appendices()
 
     if not machine_base.is_a_machine():
         logger.warn("it's Not a Machine!!")
@@ -486,14 +498,15 @@
 
             fslrenderer = FslRenderer(basename)
             conv['fsl'] = fslrenderer.render(machine, inner, outer)
             if params:
                 conv.update(params)
 
     conv['name'] = basename
+    timer.stop("-- all done in %0.4f seconds --")
     return conv
 
 
 def create_femag_parameters(m_inner, m_outer, nodedist=1):
     if not (m_inner and m_outer):
         return {}
```

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/corner.py` & `femagtools-1.6.6/src/femagtools/dxfsl/corner.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/dumprenderer.py` & `femagtools-1.6.6/src/femagtools/dxfsl/dumprenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/fslrenderer.py` & `femagtools-1.6.6/src/femagtools/dxfsl/fslrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/functions.py` & `femagtools-1.6.6/src/femagtools/dxfsl/functions.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/geom.py` & `femagtools-1.6.6/src/femagtools/dxfsl/geom.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import logging
 import sys
 from .corner import Corner
 from .area import Area
 from .shape import Element, Shape, Circle, Arc, Line, Point
 from .shape import is_Circle, is_Arc, is_Line
 from .machine import Machine
+from femagtools.dxfsl.areabuilder import AreaBuilder
 from .functions import less_equal, less, greater, greater_equal
 from .functions import distance, alpha_line, alpha_points, alpha_angle
 from .functions import point, points_are_close, is_point_inside_region
 from .functions import line_m, line_n, lines_intersect_point
 from .functions import middle_point_of_line, middle_point_of_arc
 from .functions import middle_angle
 from .functions import normalise_angle, is_same_angle
@@ -247,440 +248,14 @@
 
 def intersect(a, b):
     """checks if 2 lines intersect"""
     return ccw(a.p1, a.p2, b.p1) != ccw(a.p1, a.p2, b.p2) and \
         ccw(b.p1, b.p2, a.p1) != ccw(b.p1, b.p2, a.p2)
 
 
-def polylines(entity, lf, rf, xoff=0.0, yoff=0.0, rotation=0.0):
-    """returns a collection of bulged vertices
-    http://www.afralisp.net/archive/lisp/Bulges1.htm
-    """
-    if isinstance(entity.points, list):
-        points = [(p[0], p[1]) for p in entity.points]
-    else:
-        points = [(p[0], p[1]) for p in entity.points()]
-    i = 0
-    if isinstance(entity.vertices, list):
-        vertices = entity.vertices
-    else:
-        vertices = entity.vertices()
-
-    for v in vertices:
-        if hasattr(v, 'bulge'):
-            b = v.bulge
-        else:
-            b = v.get_dxf_attrib('bulge', 0.0)
-        p1 = points[i]
-        try:
-            p2 = points[i+1]
-        except Exception:
-            if not entity.is_closed:
-                break
-            p2 = points[0]
-        if b != 0.0:
-            dx, dy = p2[0] - p1[0], p2[1] - p1[1]
-            c = np.sqrt(dx**2 + dy**2)
-            s = b * c/2
-            r = ((c/2)**2 + s**2)/2/s
-            g = np.arctan2(dx, dy)
-            a = 2*np.arctan(b)
-            pc = (p1[0] + r*np.sin(g - np.pi/2 + a),
-                  p1[1] + r*np.cos(g - np.pi/2 + a))
-            if b < 0:
-                sa = np.arctan2(p2[1]-pc[1], p2[0]-pc[0])
-                ea = np.arctan2(p1[1]-pc[1], p1[0]-pc[0])
-            else:
-                sa = np.arctan2(p1[1]-pc[1], p1[0]-pc[0])
-                ea = np.arctan2(p2[1]-pc[1], p2[0]-pc[0])
-            logger.debug("Poly p1 %s p2 %s r %s", p1, p2, r)
-            yield Arc(Element(center=(pc[0], pc[1]),
-                              radius=np.abs(r),
-                              start_angle=sa/rf,
-                              end_angle=ea/rf),
-                      lf, rf,
-                      xoff=xoff, yoff=yoff,
-                      rotation=rotation)
-        else:
-            yield Line(Element(start=p1, end=p2), lf,
-                       xoff=xoff, yoff=yoff,
-                       rotation=rotation)
-        i += 1
-
-
-def lw_polyline(entity, lf, xoff=0.0, yoff=0.0, rotation=0.0):
-    """returns a collection of bulged vertices
-    http://www.afralisp.net/archive/lisp/Bulges1.htm
-    """
-    if isinstance(entity.points, list):
-        points = [(lf*p[0], lf*p[1]) for p in entity.points]
-    else:
-        points = [(lf*p[0], lf*p[1]) for p in entity.points()]
-
-    if points:
-        p1 = points[0]
-        for p2 in points[1:]:
-            yield Line(Element(start=p1, end=p2), lf,
-                       xoff=xoff, yoff=yoff,
-                       rotation=rotation)
-            p1 = p2
-    if entity.is_closed:
-        yield Line(Element(start=p1, end=points[0]), lf,
-                   xoff=xoff, yoff=yoff,
-                   rotation=rotation)
-
-
-def ellipse(entity, lf, xoff=0.0, yoff=0.0, rotation=0.0):
-    w = np.linalg.norm(entity.major_axis) * 2
-    h = entity.ratio * w
-    theta = np.arctan2(entity.major_axis[1], entity.major_axis[0])
-    start_angle = entity.start_param
-    end_angle = entity.end_param
-    if end_angle < start_angle:
-        end_angle += 2*np.pi
-    alfa = np.linspace(start_angle, end_angle, 20)
-    x = 0.5 * w * np.cos(alfa)
-    y = 0.5 * h * np.sin(alfa)
-    R = np.array([
-        [np.cos(theta), -np.sin(theta)],
-        [np.sin(theta),  np.cos(theta)]
-    ])
-    x, y = np.dot(R, [x, y])
-    x += entity.center[0]
-    y += entity.center[1]
-    points = np.array((x, y)).T
-    p1 = points[0]
-    for p2 in points[1:]:
-        yield Line(Element(start=p1, end=p2), lf,
-                   xoff=xoff, yoff=yoff,
-                   rotation=rotation)
-        p1 = p2
-
-
-def spline(entity, lf, min_dist=0.001, xoff=0.0, yoff=0.0, rotation=0.0):
-    if False:
-        yield Line(Element(start=entity.control_points[0],
-                           end=entity.control_points[-1]), lf,
-                   xoff=xoff, yoff=yoff,
-                   rotation=rotation)
-        return
-
-    if False:
-        p_prev = None
-        for p in entity.control_points:
-            if p_prev:
-                yield Line(Element(start=p_prev, end=p), lf,
-                           xoff=xoff, yoff=yoff,
-                           rotation=rotation)
-            p_prev = p
-        return
-
-    points_between = entity.control_points[1:-1]
-    p1 = entity.control_points[0]
-    pe = entity.control_points[-1]
-    for p2 in points_between:
-        dist_12 = distance(p1, p2)
-        dist_2e = distance(p2, pe)
-        if dist_2e < min_dist:
-            logger.debug("SPLINE: ignor small end-distance %s", dist_2e)
-            yield Line(Element(start=p1, end=pe), lf,
-                       xoff=xoff, yoff=yoff,
-                       rotation=rotation)
-            return
-
-        if dist_12 > min_dist:
-            yield Line(Element(start=p1, end=p2), lf,
-                       xoff=xoff, yoff=yoff,
-                       rotation=rotation)
-            p1 = p2
-        else:
-            logger.debug("SPLINE: ignor small distance %s", dist_12)
-
-    yield Line(Element(start=p1, end=pe), lf,
-               xoff=xoff, yoff=yoff,
-               rotation=rotation)
-
-
-def face3d(entity, lf):
-    logger.info("FACE3D: Points=%s", entity.points)
-    for i in range(len(entity.points)-1):
-        if not entity.is_edge_invisible(i):
-            ip = i+1 if i < 4 else 0
-            yield Line(Element(start=(entity.points[i][1],
-                                      entity.points[i][2]),
-                               end=(entity.points[ip][1],
-                                    entity.points[ip][2])))
-
-
-def insert_block(dwg, insert_entity, lf, rf, block, min_dist=0.001):
-    logger.debug('Insert %s entities from block %s',
-                 len(block),
-                 insert_entity.name)
-    logger.debug('Insert = %s', insert_entity.insert)
-    logger.debug('Rotation = %s', insert_entity.rotation)
-    logger.debug('Scale = %s', insert_entity.scale)
-    logger.debug('Rows = %s', insert_entity.row_count)
-    logger.debug('Cols = %s', insert_entity.col_count)
-    logger.debug('Row spacing = %s', insert_entity.row_spacing)
-    logger.debug('Col spacing = %s', insert_entity.col_spacing)
-
-    if insert_entity.insert != (0.0, 0.0, 0.0):
-        logger.debug('Different Location in Insert')
-
-    xoff = insert_entity.insert[0]
-    yoff = insert_entity.insert[1]
-
-    scale = (round(insert_entity.scale[0], 8),
-             round(insert_entity.scale[1], 8),
-             round(insert_entity.scale[2], 8))
-    if not (scale == (1.0, 1.0, 1.0) or
-            scale == (1.0, 1.0, 0.0)):
-        logger.error('Block scaling in Insert not supported')
-        logger.error('  scale = {}'.format(scale))
-        return
-
-    if(insert_entity.row_count > 1 or
-       insert_entity.col_count > 1 or
-       insert_entity.row_spacing > 0 or
-       insert_entity.col_spacing > 0):
-        logger.error('Multi Block references in Insert not supported')
-        return
-
-    for e in block:
-        if e.dxftype == 'ARC':
-            logger.debug("Block Arc")
-            yield Arc(e, lf, rf,
-                      xoff=xoff, yoff=yoff,
-                      rotation=insert_entity.rotation)
-        elif e.dxftype == 'CIRCLE':
-            logger.debug("Block Circle %s, Radius %f", e.center[:2], e.radius)
-            yield Circle(e, lf,
-                         xoff=xoff, yoff=yoff,
-                         rotation=insert_entity.rotation)
-        elif e.dxftype == 'LINE':
-            logger.debug("Block Line")
-            yield Line(e, lf,
-                       xoff=xoff, yoff=yoff,
-                       rotation=insert_entity.rotation)
-        elif e.dxftype == 'POLYLINE':
-            logger.debug("Block Polyline")
-            for p in polylines(e, lf, rf,
-                               xoff=xoff, yoff=yoff,
-                               rotation=insert_entity.rotation):
-                yield p
-        elif e.dxftype == 'LWPOLYLINE':
-            logger.debug("Block lwPolyline")
-            for p in lw_polyline(e, lf,
-                                 xoff=xoff, yoff=yoff,
-                                 rotation=insert_entity.rotation):
-                yield p
-        elif e.dxftype == 'SPLINE':
-            logger.debug("Block spline")
-            for l in spline(e, lf,
-                            min_dist=min_dist,
-                            xoff=xoff, yoff=yoff,
-                            rotation=insert_entity.rotation):
-                yield l
-        elif e.dxftype == 'INSERT':
-            logger.debug("Nested Insert of Block %s", e.name)
-            block = dwg.blocks[e.name]
-            for l in insert_block(dwg, e, lf, rf, block, min_dist=min_dist):
-                yield l
-
-        else:
-            logger.warn("unknown type %s in block %s",
-                        e.dxftype, insert_entity.name)
-
-
-def dxfshapes0(dxffile, mindist=0.01, layers=[]):
-    """returns a collection of dxf entities (ezdxf)"""
-    import ezdxf
-    dwg = ezdxf.readfile(dxffile)
-    id = 0
-    # $ACADVER: AC1006 = R10, AC1009 = R11 and R12, AC1012 = R13,
-    #   AC1014 = R14 AC1015 = Release 2000/0i/2
-    # check units:
-    # dwg.header['$ANGDIR'] 1 = Clockwise angles, 0 = Counterclockwise
-    # dwg.header['$AUNITS'] 0 Decimal Degrees, 1 Deg/Min/Sec, 2 Grads, 3 Radians
-    # dwg.header['$INSUNIT'] 1 = Inches; 2 = Feet; 3 = Miles;
-    #   4 = Millimeters; 5 = Centimeters; 6 = Meters
-    # dwg.header['$LUNITS']
-    for e in dwg.modelspace():
-        if e.dxftype() == 'ARC':
-            yield Arc(e.dxf)
-        elif e.dxftype() == 'CIRCLE':
-            logger.debug("Circle %s, Radius %f", e.center[:2], e.radius)
-            yield Circle(e.dxf)
-        elif e.dxftype() == 'LINE':
-            yield Line(e.dxf)
-        elif e.dxftype() == 'POLYLINE':
-            for p in polylines(e):
-                yield p
-        elif e.dxftype() == 'SPLINE':
-            for l in spline(e, 1.0, in_dist=mindist):
-                yield l
-        elif e.dxftype() == 'POINT':
-            logger.debug("Id %d4: type %s ignored", id, e.dxftype)
-        else:
-            logger.warning("Id %d4: unknown type %s", id, e.dxftype)
-        id += 1
-
-
-def dxfshapes(dxffile, mindist=0.01, layers=[]):
-    """returns a collection of dxf entities (dxfgrabber)"""
-    import dxfgrabber
-    dwg = dxfgrabber.readfile(dxffile)
-    # print("Layers = {}".format(dwg.layers.names()))
-    id = 0
-    # $ACADVER: AC1006 = R10, AC1009 = R11 and R12, AC1012 = R13,
-    #   AC1014 = R14 AC1015 = Release 2000/0i/2
-    # check units:
-    # dwg.header['$ANGDIR'] 1 = Clockwise angles, 0 = Counterclockwise
-    # dwg.header['$AUNITS'] Decimal Degrees, Deg/Min/Sec, Grads, Radians
-    # dwg.header['$INSUNIT'] 1 = Inches; 2 = Feet; 3 = Miles;
-    #   4 = Millimeters; 5 = Centimeters; 6 = Meters
-    # dwg.header['$LUNITS']
-    lf = 1
-    if dwg.header.get('$LUNITS', 0) == 1:
-        # conv = [1, 2.54e-2, 10.12, 633.0, 1e-3, 1e-2, 1]
-        lf = 2.54e3
-
-    rf = np.pi/180
-    if dwg.header.get('$AUNITS', 0) == 4:
-        rf = 1
-
-    for e in dwg.modelspace():
-        if not layers or e.layer in layers:
-            if e.dxftype == 'ARC':
-                yield Arc(e, lf, rf)
-            elif e.dxftype == 'CIRCLE':
-                logger.debug("Circle %s, Radius %f", e.center[:2], e.radius)
-                yield Circle(e, lf)
-            elif e.dxftype == 'LINE':
-                yield Line(e, lf)
-            elif e.dxftype == 'POLYLINE':
-                for p in polylines(e, lf, rf):
-                    yield p
-            elif e.dxftype == 'LWPOLYLINE':
-                for p in lw_polyline(e, lf):
-                    yield p
-            elif e.dxftype == 'SPLINE':
-                for l in spline(e, lf, min_dist=mindist):
-                    yield l
-            elif e.dxftype == 'INSERT':
-                logger.debug("Insert of Block %s", e.name)
-                block = dwg.blocks[e.name]
-                for l in insert_block(dwg, e, lf, rf, block, min_dist=mindist):
-                    yield l
-            elif e.dxftype == 'ELLIPSE':
-                for l in ellipse(e, lf):
-                    yield l
-                #w = np.linalg.norm(e.major_axis) * 2
-                #h = e.ratio * w
-                #rtheta = np.arctan2(e.major_axis[1], e.major_axis[0])
-                #angle = rtheta*180/np.pi
-                #start_angle = e.start_param*180/np.pi + angle
-                #end_angle = e.end_param*180/np.pi + angle
-                #if end_angle < start_angle:
-                #    end_angle += 360
-                #arc = Arc(Element(center=e.center,
-                #                  radius=w/2,
-                #                  start_angle=start_angle,
-                #                  end_angle=end_angle,
-                #                  width=w,
-                #                  height=h,
-                #                  rtheta=rtheta,
-                #                  start_param=e.start_param,
-                #                  end_param=e.end_param))
-                #yield arc
-
-            elif e.dxftype == 'POINT':
-                logger.debug("Id %d4: type %s ignored", id, e.dxftype)
-            elif e.dxftype == '3DFACE':
-                logger.warning(
-                    "Id %d4: type %s not implemented", id, e.dxftype)
-                # for l in face3d(e, lf):
-                #     yield l
-            else:
-                logger.warning("Id %d4: unknown type %s", id, e.dxftype)
-            id += 1
-
-
-fem_points = []
-
-
-def read_fem_points(f, num):
-    for x in range(num):
-        p = f.readline().split()
-        fem_points.append([float(p[0]), float(p[1])])
-
-
-def read_fem_lines(f, num):
-    for x in range(num):
-        p = f.readline().split()
-        i1 = int(p[0])
-        i2 = int(p[1])
-        p1 = fem_points[i1]
-        p2 = fem_points[i2]
-        if points_are_close(p1, p2):
-            logger.warning("FEMM: Line with points close together")
-            logger.warning("      p1 = %s, p2 =%s", p1, p2)
-        yield Line(Element(start=p1, end=p2))
-
-
-def read_fem_arcs(f, num):
-    for x in range(num):
-        p = f.readline().split()
-        i1 = int(p[0])
-        i2 = int(p[1])
-        alpha = float(p[2])
-        p1 = fem_points[i1]
-        p2 = fem_points[i2]
-        if points_are_close(p1, p2):
-            logger.warning("FEMM: Arc with points close together")
-            logger.warning("      p1 = %s, p2 = %s", p1, p2)
-        for e in get_fem_arc(p1, p2, alpha):
-            yield e
-
-
-def get_fem_arc(pA, pB, alfa):
-    alpha = alfa/180.0*np.pi/2.0
-    y = distance(pA, pB) / 2.0
-    x = y / np.tan(alpha)
-    r = np.sqrt(x**2 + y**2)
-
-    delta = alpha_line(pA, pB)
-
-    c = [pA[0] + y, pA[1] + x]
-    phi = alpha_line(pA, c) + delta
-    pC = point_on_arc(pA, r, phi)
-
-    startangle = alpha_line(pC, pA)
-    endangle = alpha_line(pC, pB)
-    yield Arc(Element(center=pC,
-                      radius=r,
-                      start_angle=startangle*180/np.pi,
-                      end_angle=endangle*180/np.pi))
-
-
-def femshapes(femfile):
-    f = open(femfile, 'r')
-
-    for data in f:
-        text = data.split()
-        if text[0] == '[NumPoints]':
-            read_fem_points(f, int(text[2]))
-        elif text[0] == '[NumSegments]':
-            for e in read_fem_lines(f,  int(text[2])):
-                yield e
-        elif text[0] == '[NumArcSegments]':
-            for e in read_fem_arcs(f,  int(text[2])):
-                yield e
-
-
 def is_connected(a, b):
     if a == b:
         return False
     return a[0] == b[0] or a[1] == b[0] or a[0] == b[1] or a[1] == b[1]
 
 
 def single_path(edges):
@@ -1075,14 +650,22 @@
                         self.atol)
 
     def circles(self):
         """return list of circle nodes"""
         return [n[1]['object'] for n in self.g.nodes(data=True)
                 if n[1] and isinstance(n[1]['object'], Circle)]
 
+    def nodes(self):
+        for n in self.g.nodes():
+            yield n
+
+    def get_nodes(self):
+        nodes = [n for n in self.g.nodes()]
+        return nodes
+
     def virtual_nodes(self):
         nodes = []
         for e in self.elements(Shape):
             nodes += e.get_nodes()
         return nodes
 
     def angle_nodes(self, center, angle, rtol, atol):
@@ -1692,14 +1275,19 @@
         """ return list of areas for each node and their neighbors
         """
         if len(self.area_list) > 0:
             logger.debug("area list already available")
             # list already available
             return
 
+        areabuilder = AreaBuilder(geom=self)
+        areabuilder.create_list_of_areas(main=False)
+        self.area_list = areabuilder.area_list
+        return
+
         def append(area_list, a):
             for area in area_list:
                 if area.is_identical(a):
                     return
             area_list.append(a)
 
         logger.debug("create new area list")
```

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/journal.py` & `femagtools-1.6.6/src/femagtools/dxfsl/journal.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,86 +51,78 @@
                     self.journal = {}
                 f.close()
 
     def write_journal(self):
         if not self.journal:
             return
         self.set_benchmark()
-
         with open(self.filename, 'w') as f:
             f.write(json.dumps(self.journal, indent=4))
             f.close()
 
     def get_journal(self, name):
         if not self.aktiv:
             return None
 
         if self.data:
             return self.data
 
         self.open_journal()
         self.data = self.journal.get(name, None)
-        if not self.data:
-            self.data = {'filename': "",
-                         'elements': 0,
-                         'nodes': 0,
-                         'concat_lines': 0,
-                         'concat_arcs': 0,
-                         'appendices': 0,
-                         'appendices_connected': 0,
-                         'appendices_remaining': 0,
-                         'areas': 0,
-                         'area_errors': 0}
-            self.journal[name] = self.data
+        self.data = {'filename': ""}  # initialise
+        self.journal[name] = self.data
         return self.data
 
     def set_benchmark(self):
         if self.data.get('area_errors', 0) > 0:
             self.put_warning("Problem with areas")
         if self.data.get('appendices_deleted', 0) > 0:
             self.put_warning("Problem with appendices")
-          
+
     def put(self, name, val):
         if self.data:
             self.data[name] = val
 
+    def add(self, name, val):
+        if self.data:
+            self.data[name] = val + self.data.get(name, 0)
+
     def put_filename(self, val):
         self.put('filename', val)
 
     def put_areas(self, val):
-        self.put('areas', val)
+        self.add('areas', val)
 
     def put_area_errors(self, val):
-        self.put('area_errors', val)
+        self.add('area_errors', val)
 
     def put_elements(self, val):
         self.put('elements', val)
 
     def put_nodes(self, val):
         self.put('nodes', val)
 
     def put_concat_lines(self, val):
-        self.put('concat_lines', val)
+        self.add('concat_lines', val)
 
     def put_concat_arcs(self, val):
-        self.put('concat_arcs', val)
+        self.add('concat_arcs', val)
 
     def put_appendices(self, val):
-        self.put('appendices', val)
+        self.add('appendices', val)
 
     def put_appendices_connected(self, val):
-        self.put('appendices_connected', val)
+        self.add('appendices_connected', val)
 
     def put_appendices_remaining(self, val):
-        self.put('appendices_remaining', val)
+        self.add('appendices_remaining', val)
 
     def put_appendices_deleted(self, val):
-        self.put('appendices_deleted', val)
+        self.add('appendices_deleted', val)
        
     def put_exception(self, msg):
         self.put('exception', msg)
 
     def put_warning(self, msg):
-        print(msg)
         lst = self.data.get('warning', [])
         lst.append(msg)
         self.put('warning', lst)
```

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/machine.py` & `femagtools-1.6.6/src/femagtools/dxfsl/machine.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/plotrenderer.py` & `femagtools-1.6.6/src/femagtools/dxfsl/plotrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/shape.py` & `femagtools-1.6.6/src/femagtools/dxfsl/shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -1004,15 +1004,15 @@
 
         alpha_min = alpha_line(center, self.p1)
         alpha_max = alpha_min
 
         for p in points:
             alpha_p = alpha_line(center, p)
             alpha_min = min_angle(alpha_min, alpha_p)
-            alpha_max = min_angle(alpha_max, alpha_p)
+            alpha_max = max_angle(alpha_max, alpha_p)
 
         return (alpha_min, alpha_max)
 
     def get_nodes(self, parts=8, render=False):
         """ Die Funktion liefert eine Liste von virtuellen Nodes, welche man
             zum Rechnen der convex_hull() benötigt.
         """
```

### Comparing `femagtools-1.6.5/src/femagtools/dxfsl/symmetry.py` & `femagtools-1.6.6/src/femagtools/dxfsl/symmetry.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from __future__ import print_function
 
 import numpy as np
 import logging
 import sys
 from femagtools.dxfsl.shape import Element, Line
 from femagtools.dxfsl.area import Area
-from femagtools.dxfsl.functions import alpha_angle, positive_angle
+from femagtools.dxfsl.functions import alpha_angle, positive_angle, is_same_angle
 from femagtools.dxfsl.functions import min_angle, max_angle, gcd, point
-from femagtools.dxfsl.functions import less_equal, less
+from femagtools.dxfsl.functions import less_equal, less, points_are_close
+from femagtools.dxfsl.functions import line_m, line_n, mirror_point
 
 logger = logging.getLogger('femagtools.symmetry')
 
 
 #############################
 #         symmetry          #
 #############################
@@ -34,18 +35,26 @@
         assert(geom is not None)
         assert(startangle is not None)
         assert(endangle is not None)
         
         self.geom = geom
         self.startangle = startangle
         self.endangle = endangle
+        self.delta_check_count = 0
+        self.delta_angle_korr = 0.0
         self.rtol = rtol
         self.atol = atol
-
-        logger.debug("Symmetry(rtol=%s, atol=%s)", rtol, atol)
+        self.full = False
+        if np.isclose(self.startangle, self.endangle):
+            self.alpha = 2.0*np.pi
+            self.full = True
+        else:
+            self.alpha = alpha_angle(self.startangle, self.endangle)
+            self.full = False
+        logger.debug("Symmetry(alpha=%s, rtol=%s, atol=%s)", self.alpha, rtol, atol)
 
     def __str__(self):
         return "rtol: {}\n".format(self.rtol) + \
                "atol: {}\n".format(self.atol)
 
     def equal_area(self,
                    d1, h1, a1,
@@ -58,204 +67,304 @@
             logger.debug("height NOT close (%s/%s)", h1, h2)
             return False
         if not np.isclose(a1, a2, rtol=rtol, atol=atol):
             logger.debug("alpha NOT close (%s/%s)", a1, a2)
             return False
         return True
 
+    def calc_mid_angle(self, a):
+        return positive_angle(alpha_angle(self.startangle,
+                                          a.get_mid_angle(self.geom.center)))
+
     def find_symmetry(self):
         arealist = self.geom.list_of_areas()
         logger.debug("begin of Symmetry::find_symmetry: %s areas available", len(arealist))
         if len(arealist) == 0:
             logger.debug("end of find_symmetry: no areas")
             return 0
 
         areas = []
         for a in arealist:
-            areas.append((a.get_alpha(),
-                          a.get_mid_angle(),
-                          a.min_dist,
-                          a.height,
+            areas.append((round(a.get_alpha(self.geom.center), 3),
+                          round(a.min_dist, 1),
+                          round(a.height, 1),
+                          self.calc_mid_angle(a),
                           a))
-        areas.sort()
-        parts_possible = None
+        areas.sort(reverse=True)
 
-        a0_alpha, a0_mid_angle, a0_min_dist, a0_height, a0 = areas[0]
+        a0_alpha, a0_min_dist, a0_height, a0_mid_angle, a0 = areas[0]
         equal_areas = [(a0_mid_angle, a0)]
-
-        for a1_alpha, a1_mid_angle, a1_min_dist, a1_height, a1 in areas[1:]:
+        check_rslt = []
+        for a1_alpha, a1_min_dist, a1_height, a1_mid_angle, a1 in areas[1:]:
             if self.equal_area(a0_min_dist, a0_height, a0_alpha,
                                a1_min_dist, a1_height, a1_alpha,
                                rtol=0.01, atol=0.05):
                 a0_min_dist = (a0_min_dist + a1_min_dist) / 2
                 a0_height = (a0_height + a1_height) / 2
                 a0_alpha = (a0_alpha + a1_alpha) / 2
                 equal_areas.append((a1_mid_angle, a1))
             else:
                 parts = self.check_delta(equal_areas)
-                if parts_possible is None:
-                    parts_possible = parts
-                else:
-                    parts_possible = self.calc_parts(parts_possible, parts)
+                check_rslt.append((a0.area_size(), parts, len(equal_areas), a0))
+
                 equal_areas = [(a1_mid_angle, a1)]
                 a0_min_dist = a1_min_dist
                 a0_height = a1_height
                 a0_alpha = a1_alpha
                 a0 = a1
 
         parts = self.check_delta(equal_areas)
-        if parts_possible is None:
-            parts_possible = parts
-        else:
-            parts_possible = self.calc_parts(parts_possible, parts)
+        check_rslt.append((a0.area_size(), parts, len(equal_areas), a0))
 
-        if parts_possible is None:
-            parts_possible = 0
-        if parts_possible < 2:
+        parts = self.get_symmetry_parts(check_rslt)
+        if parts < 2:
             logger.debug("end of Symmetry::find_symmetry: no symmetry")
-            return parts_possible
-    
+            return parts
+
         self.geom.clear_cut_lines()
-        for alpha in self.symmetry_lines(parts_possible,
+        for alpha in self.symmetry_lines(parts,
                                          self.startangle,
                                          self.endangle):
-            min_radius = max(10, self.geom.min_radius - 10)
+            plus = self.geom.max_radius / 10
+            min_radius = max(10, self.geom.min_radius - plus)
             p1 = point(self.geom.center, min_radius, alpha)
-            p2 = point(self.geom.center, self.geom.max_radius+10, alpha)
+            p2 = point(self.geom.center, self.geom.max_radius + plus, alpha)
             line = Line(Element(start=p1, end=p2))
             line.init_attributes(color='green')
             self.geom.add_cut_line(line)
-                    
-        logger.debug("end of Symmetry::find_symmetry")
-        return parts_possible
+
+        logger.debug("end of Symmetry::find_symmetry: -> %s", parts)
+        return parts
     
     def check_delta(self, area_list):
-        logger.debug("==> %s equal areas", len(area_list))
+        logger.debug("begin of check_delta: %s equal areas", len(area_list))
         if not area_list:
+            logger.debug("end of check_delta: no areas")
             return None
 
         if len(area_list) == 1:
             mid_angle, a = area_list[0]
-            if np.isclose(a.min_angle, self.startangle) and \
-               np.isclose(a.max_angle, self.endangle):
+            alpha = a.get_alpha(self.geom.center)
+            if np.isclose(alpha, self.alpha):
+                logger.debug("end of check_delta: one area from start to end")
                 return None  # ok
 
+        self.delta_check_count += 1
         area_list.sort()
-        start = self.startangle
-        mid_angle, a = area_list[0]
 
-        delta = alpha_angle(start, mid_angle) * 2
+        mid_angle, a = area_list[0]
+        delta = positive_angle(mid_angle * 2)
+        delta_total = mid_angle
         delta_list = [delta]
-        logger.debug("geom: start=%s,  end=%s", self.startangle, self.endangle)
+
+        logger.debug("First mid = %s, delta = %s", mid_angle, delta)
         logger.debug("%s:  d=%s,  h=%s,  a=%s, mid=%s, delta=%s",
                      a.identifier(),
                      a.min_dist,
                      a.height,
-                     a.get_alpha(),
-                     a.get_mid_angle(),
+                     a.get_alpha(self.geom.center),
+                     mid_angle,
                      delta)
-        logger.debug("  min=%s,  max%s",
-                     a.min_angle,
-                     a.max_angle)
 
-        start = mid_angle
+        geom_alpha = alpha_angle(self.startangle, self.endangle)
+        geom_alpha = positive_angle(geom_alpha)
+
+        start_angle = mid_angle
         for mid_angle, a in area_list[1:]:
-            delta = alpha_angle(start, mid_angle)
+            delta_angle = alpha_angle(start_angle, mid_angle)
+            delta = positive_angle(delta_angle)
+            delta_total += delta_angle
             delta_list.append(delta)
 
             logger.debug("%s:  d=%s,  h=%s,  a=%s, mid=%s, delta=%s",
                          a.identifier(),
                          a.min_dist,
                          a.height,
-                         a.get_alpha(),
-                         a.get_mid_angle(),
+                         a.get_alpha(self.geom.center),
+                         mid_angle,
                          delta)
-            logger.debug("  min=%s,  max%s",
-                         a.min_angle,
-                         a.max_angle)
-
-            start = mid_angle
+            start_angle = mid_angle
             
-        delta = alpha_angle(start, self.endangle) * 2
+        delta_angle = alpha_angle(start_angle, geom_alpha)
+        delta = positive_angle(delta_angle * 2)
+        delta_total += delta_angle
         delta_list.append(delta)
         logger.debug("final delta=%s", delta)
 
+        if not np.isclose(geom_alpha, delta_total):
+            logger.debug("-- deltas: %s", delta_list)
+            logger.debug("end of check_delta: BAD DELTA %s, (expected %s)",
+                         delta_angle, geom_alpha)
+            return 0  # very bad
+
         sz = len(delta_list)
         mid = int(sz / 2)
         ix1 = 0
         ix2 = sz - 1
+        first_last_bad = False
         for ix1 in range(0, mid):
             if not np.isclose(delta_list[ix1], delta_list[ix2], rtol=1e-3, atol=1e-3):
-                logger.debug("NO SYM")
-                return 0
+                if self.full and \
+                   self.delta_check_count == 1 and \
+                   ix1 == 0 and \
+                   self.delta_angle_korr == 0.0:
+                    first_last_bad = True
+                else:
+                    logger.debug("end of check_delta: NO SYM")
+                    return 0
             ix2 -= 1
 
-        geom_alpha = alpha_angle(self.startangle, self.endangle)
-        delta_alpha = 0.0
-        for d in delta_list:
-            delta_alpha += d
-
-        geom_alpha = positive_angle(geom_alpha)
-
-        delta_alpha -= delta_list[0] / 2
-        delta_alpha -= delta_list[-1] / 2
-        delta_alpha = positive_angle(delta_alpha)
-        if not np.isclose(geom_alpha, delta_alpha):
-            logger.debug("BAD DELTA ?!?")
-            return 0  # very bad
+        if first_last_bad:
+            delta_korr = (delta_list[0] + delta_list[-1]) / 2.0
+            logger.debug("STARTANGLE CORRECTION")
+            self.delta_angle_korr = (delta_korr - delta_list[0]) / 2
+            logger.debug("-- delta[0] from %s to %s", delta_list[0], delta_korr)
+            logger.debug("Delta Angle Korr = %s", self.delta_angle_korr)
+            delta_list[0] = delta_korr
+            delta_list[-1] = delta_korr
+            assert(self.full)
+            self.startangle = self.startangle - self.delta_angle_korr
+            self.endangle = self.endangle - self.delta_angle_korr
+            logger.debug("New startangle = %s", self.startangle)
+            logger.debug("Delta List: %s", delta_list)
 
         d1 = delta_list[0]
         d1_count = 1
         inx_list = [0]
         for x in range(1, len(delta_list)):
             if np.isclose(d1, delta_list[x], rtol=1e-3, atol=1e-3):
                 inx_list.append(x)
                 d1_count += 1
 
         if d1_count == len(delta_list):
-            logger.debug("SYMMETRY FOUND")
+            logger.debug("end of check_delta: SYMMETRY FOUND")
             return d1_count -1  # very simple
         if len(delta_list) < 2:
+            logger.debug("end of check_delta: One delta only ?!")
             return 0
 
         logger.debug("index of delta %s = %s", d1, inx_list)
         x1 = inx_list[0]
         x2 = inx_list[1]
         step = x2 - x1
         x1 = x2
         for x2 in inx_list[2:]:
             if not (x2 - x1 == step):
                 return 0
             x1 = x2
         
-        logger.debug("SYMMETRY FOUND")
+        logger.debug("end of check_delta: SYMMETRY FOUND")
         return len(inx_list) -1
 
+    def get_symmetry_parts(self, check_rslt):
+        max_size = 0
+        max_areas = 0
+        parts_possible = None
+
+        check_rslt.sort(reverse=True)
+        for size, parts, count, area in check_rslt:
+            logger.debug("Result: %s, %s, %s", size, parts, count)
+
+        for size, parts, count, area in check_rslt:
+            if parts is not None and parts > 0:
+                max_size = max(max_size, size)
+                max_areas = max(max_areas, count)
+
+        logger.debug("max size: %s,  max areas: %s", max_size, max_areas)
+
+        for size, parts, count, area in check_rslt:
+            if parts is not None and parts <= 1:  # critical
+                if count <= max(1, max_areas / 5):
+                    if size < max_size / 25:
+                        parts = None
+
+            parts_possible = self.calc_parts(parts_possible, parts)
+
+        if parts_possible is None:
+            parts_possible = 0
+        return parts_possible
+
     def calc_parts(self, parts1, parts2):
         logger.debug("Calc symmetry Parts (%s, %s)", parts1, parts2)
         if parts2 is None:
+            logger.debug("return %s parts", parts1)
             return parts1
-
-        return gcd(parts1, parts2)
+        if parts1 is None:
+            logger.debug("return %s parts", parts2)
+            return parts2
+        if parts1 == 0 or parts2 == 0:
+            logger.debug("return %s parts", 0)
+            return 0
+        parts = gcd(parts1, parts2)
+        logger.debug("return %s parts", parts)
+        return parts
 
     def symmetry_lines(self, parts, startangle, endangle):
         logger.debug("begin symmetry_lines from %s to %s",
                      startangle,
                      endangle)
         if less_equal(endangle, startangle):
             endangle += 2*np.pi
 
         delta = alpha_angle(startangle, endangle) / parts
         start = startangle + delta
         while less(start, endangle):
             yield start
             start += delta
-            
+
+        if is_same_angle(startangle, endangle):
+            yield start
+
         # Damit man anschliessend ohne Umstände schneiden kann.
         self.geom.sym_startangle = startangle
         self.geom.sym_endangle = startangle + delta
         self.geom.sym_slices = parts
         self.geom.sym_slice_angle = delta
         self.geom.sym_area = Area([], (0,0), 0.0)
         self.geom.sym_area.sym_startangle = self.geom.sym_startangle
         self.geom.sym_area.sym_endangle = self.geom.sym_endangle
         logger.debug("end symmetry_lines")
+
+    def check_symmetry_of_mirror(self, mirror_geom, mirrorangle):
+        logger.debug("begin of Symmetry::check_symmetry_of_mirror")
+        assert(mirror_geom is not None)
+
+        axis_p = point(self.geom.center, self.geom.max_radius, mirrorangle)
+        axis_m = line_m(self.geom.center, axis_p)
+        axis_n = line_n(self.geom.center, axis_m)
+
+        def counterpart_found(node, nodes, rtol, atol):
+            hits = 0
+            for n in nodes:
+                if points_are_close(node, n, rtol, atol):
+                    logger.debug(" ---- %s is %s", node, n)
+                    return True
+            return False
+
+        def check_differences(geom, mirror_geom):
+            geom_ag_nodes = []
+            geom_nodes = [n for n in geom.g.nodes() if not (n in geom_ag_nodes)]
+
+            hit = 0
+            for n in geom_nodes:
+                mirror_n = mirror_point(n, geom.center, axis_m, axis_n)
+                if counterpart_found(mirror_n,
+                                     mirror_geom.g.nodes(),
+                                     self.rtol,
+                                     self.atol):
+                    hit += 1
+            min_nodes = min(len(geom_nodes), int(len(geom_nodes) * 0.95) + 1)
+            logger.debug("Nodes=%s,  Counterparts=%s", len(geom_nodes), hit)
+            if hit < min_nodes:
+                return hit / len(geom_nodes)
+            else:
+                return 1.0
+
+        # ----------------
+        logger.debug("check geom - mirror")
+        f1 = check_differences(self.geom, mirror_geom)
+        logger.debug("check mirror - geom")
+        f2 = check_differences(mirror_geom, self.geom)
+        logger.debug("Factor 1: %s,  2: %s", f1, f2)
+        ok = f1 > 0.97 and f2 > 0.97
+        logger.debug("end of Symmetry::check_symmetry_of_mirror => %s", ok)
+        return ok
```

### Comparing `femagtools-1.6.5/src/femagtools/ecloss.py` & `femagtools-1.6.6/src/femagtools/ecloss.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/erg.py` & `femagtools-1.6.6/src/femagtools/erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/femag.py` & `femagtools-1.6.6/src/femagtools/femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/forcedens.py` & `femagtools-1.6.6/src/femagtools/forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/fsl.py` & `femagtools-1.6.6/src/femagtools/fsl.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/getset.py` & `femagtools-1.6.6/src/femagtools/getset.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/gmsh.py` & `femagtools-1.6.6/src/femagtools/gmsh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/google.py` & `femagtools-1.6.6/src/femagtools/google.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/grid.py` & `femagtools-1.6.6/src/femagtools/grid.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/hxy.py` & `femagtools-1.6.6/src/femagtools/hxy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/isa7.py` & `femagtools-1.6.6/src/femagtools/isa7.py`

 * *Files identical despite different names*

```diff
@@ -864,22 +864,22 @@
         try:
             self.current_id = np.asarray(reader.CURRENT_ID)
             self.ide_flux = np.asarray(reader.IDE_FLUX)
             self.ide_beta = np.asarray(reader.IDE_BETA)
         except AttributeError:
             pass
 
-        try: 
+        try:
             flx_fac = 1000
-            if isinstance(reader.el_fe_induction_1, list): 
+            if isinstance(reader.el_fe_induction_1, list):
                 pass
-            else: 
-                if reader.el_fe_induction_1.dtype == 'int16': 
+            else:
+                if reader.el_fe_induction_1.dtype == 'int16':
                     flx_fac = 1000
-                else: 
+                else:
                     flx_fac = 1
             el_fe_ind = [np.array(reader.el_fe_induction_1).T/flx_fac,
                         np.array(reader.el_fe_induction_2).T/flx_fac]
             eddy_cu_vpot = np.array(reader.eddy_cu_vpot).T/1000
             if len(el_fe_ind[0].shape) == 4:
                 pdim = self.pos_el_fe_induction.shape[0]
                 if pdim < el_fe_ind[0].shape[1]:
@@ -1428,14 +1428,15 @@
                 return self.loss_density
         return 0
 
     def temp(self):
         """return temperature of this element"""
         return sum([v.vpot[1] for v in self.vertices])/len(self.vertices)
 
+
 class SuperElement(BaseEntity):
     def __init__(self, key, sr_key, elements, nodechains, color,
                  nc_keys, mcvtype, condtype, conduc, length,
                  velsys, velo_1, velo_2, curd_re, curd_im,
                  fillfactor, temp_coef, temperature):
         super(self.__class__, self).__init__(key)
         self.sr_key = sr_key
```

### Comparing `femagtools-1.6.5/src/femagtools/jhb.py` & `femagtools-1.6.6/src/femagtools/jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/job.py` & `femagtools-1.6.6/src/femagtools/job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/losscoeffs.py` & `femagtools-1.6.6/src/femagtools/losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/machine/__init__.py` & `femagtools-1.6.6/src/femagtools/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/machine/afpm.py` & `femagtools-1.6.6/src/femagtools/machine/afpm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/machine/effloss.py` & `femagtools-1.6.6/src/femagtools/machine/effloss.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
                 rb['T'] = None
         if 'n' not in rb:
             rb = m.characteristics(-T, max(r['n']), u1, nsamples=nsamples,
                                    with_mtpv=with_mtpv, with_mtpa=with_mtpa,
                                    with_pmconst=with_pmconst, with_tmech=with_tmech)  # braking mode
     
     if kwargs.get('mesh_func', 0):
-        ntmesh = kwargs['mesh_func'](r['n'], r['T'],
+        ntmesh = kwargs['mesh_func'](r['n_type'], r['n'], r['T'],
                                     rb['n'], rb['T'], npoints)
     else: 
         ntmesh = _generate_mesh(r['n'], r['T'],
                                 rb['n'], rb['T'], npoints)
 
     logger.info("total speed,torque samples %d", ntmesh.shape[1])
     if isinstance(m, (PmRelMachine, SynchronousMachine)):
```

### Comparing `femagtools-1.6.5/src/femagtools/machine/im.py` & `femagtools-1.6.6/src/femagtools/machine/im.py`

 * *Files 0% similar despite different names*

```diff
@@ -618,14 +618,15 @@
 
     optional:
     num_steps: (int) number of current steps for the no-load calculation (default 5)
     logspace: (bool) uses log distributed current samples if true linear otherwise (default true)
     i_max_fact: (float) factor for maximum current to calculate no_load flux (default=2.5)
     templatedirs: (list of str) names of directories to search for templates
     """
+    cmd = kwargs.get("cmd", None)
     CON = {'open': 0, 'wye': 1, 'star': 1, 'delta': 2}
     p = machine['poles']//2
     slip = 1e-2
     u1ph = u1
     w1 = 2*np.pi*f1
     wdgk = 'windings' if 'windings' in machine else 'winding'
     if CON[wdgcon] == 1:
@@ -672,15 +673,15 @@
     try:
         m[wdgk].pop('resistance')
     except KeyError:
         pass
 
     parstudy = femagtools.parstudy.ParameterStudy(
         workdir, condMat=condMat,
-        magnetizingCurves=magnetizingCurves)
+        magnetizingCurves=magnetizingCurves, cmd=cmd)
 
     builder = femagtools.fsl.Builder(kwargs.get('templatedirs', []))
     model = femagtools.model.MachineModel(m)
     # modelfiles = parstudy.setup_model(builder, model)
     extra_result_files = [f'noloadbag-{i+1}.dat'
                           for i in range(num_steps)] + [
         'psi-rot-mag.dat']
```

### Comparing `femagtools-1.6.5/src/femagtools/machine/pm.py` & `femagtools-1.6.6/src/femagtools/machine/pm.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         self.kh = 2
         self.kpfe = 1 # iron loss factor
         self.kpmag = 1 # magnet loss factor
         self.kfric_b = 1
         self.rotor_mass = 0
         self.kth1 = KTH
         self.bertotti = False
+        self.max_torque = 0.0
         self.losskeys = ['styoke_hyst', 'stteeth_hyst',
                         'styoke_eddy', 'stteeth_eddy',
                         'rotor_hyst', 'rotor_eddy',
                         'magnet']
         # overwritable function: skin_resistance(r0, w, tcu, kth)
         # Arguments:
         # r0: (float) dc resistance in Ohm at 20°C
@@ -165,14 +166,54 @@
         return iq, 0, self.torque_iqd(iq, 0)
 
     def iqd_tmech(self, torque, n, iqd0=0, with_mtpa=True):
         """return minimum d-q-current for shaft torque"""
         if np.abs(torque) < 1e-2:
             return (0, 0)
         if np.isscalar(iqd0):
+            tx = self.tmech_iqd(self.io[0], 0, n)
+            iq0 = min(0.9*self.i1range[1]/np.sqrt(2),
+                      np.abs(torque)/tx*self.io[0])
+            if torque < 0:
+                i0 = (-iq0, 0)
+            else:
+                i0 = (iq0, 0)
+            logger.debug("initial guess i0 %f -> %s tx %f torque %f",
+                        self.io[0], i0, tx, torque)
+        else:
+            i0 = iqd0
+
+        if with_mtpa:
+            k=0
+            while k < 6:
+                res = so.minimize(
+                    lambda iqd: la.norm(iqd), i0, method='SLSQP',
+                    constraints=({'type': 'eq',
+                                  'fun': lambda iqd:
+                                  self.tmech_iqd(*iqd, n) - torque}))
+                if res.success:
+                    return res.x
+                # make new initial guess:
+                tx = self.tmech_iqd(*i0, n)
+                logger.debug("k %d new guess i0 %s tx %f torque %f",
+                            k, i0, tx, torque)
+                i0=(min(0.9*self.i1range[1]/np.sqrt(2), torque/tx*i0[0]), 0)
+                k += 1
+            raise ValueError(
+                f'Torque {torque} speed {n} {i0} {res.message}')
+        def tqiq(iq):
+            return torque - self.tmech_iqd(float(iq), 0, n)
+        iq = so.fsolve(tqiq, (i0[0],))[0]
+        return iq, 0, self.tmech_iqd(iq, 0, n)
+
+    def iqd_tmech0(self, torque, n, iqd0=0, with_mtpa=True):
+        """return minimum d-q-current for shaft torque"""
+        if np.abs(torque) < 1e-2:
+            return (0, 0)
+        if np.isscalar(iqd0):
             i0 = self.io
         else:
             i0 = iqd0
 
         if with_mtpa:
             res = so.minimize(
                 lambda iqd: la.norm(iqd), i0, method='SLSQP',
@@ -677,25 +718,32 @@
         """
         if with_tmech:
             w1type, T = self.w1_imax_umax(i1max, u1max)
         else:
             iq, id, T = self.mtpa(i1max)
             w1type = self.w1_umax(u1max, iq, id)
         Pmax = w1type/self.p*T
-        w1max = 2*np.pi*speedmax*self.p
         # check max speed:
-        if with_pmconst:
-            iq, id, tq = self.iqd_pmech_imax_umax(
-                speedmax, Pmax, i1max, u1max,
-                with_mtpa, with_tmech)
-        else:
-            iq, id, tq = self.iqd_imax_umax(
-                i1max, w1max, u1max,
-                T, with_mtpv=False,
-                with_tmech=with_tmech)
+        sp = speedmax
+        while sp > w1type/2/np.pi/self.p:
+            w1max = 2*np.pi*sp*self.p
+            try:
+                if with_pmconst:
+                    iq, id, tq = self.iqd_pmech_imax_umax(
+                        sp, Pmax, i1max, u1max,
+                        with_mtpa, with_tmech)
+                else:
+                    iq, id, tq = self.iqd_imax_umax(
+                        i1max, w1max, u1max,
+                        T, with_mtpv=False,
+                        with_tmech=with_tmech)
+                break
+            except ValueError:
+                sp -= 5e-2*speedmax
+        speedmax = sp
         i1 = betai1(iq, id)[1]
         if (abs(i1max) >= i1
             and round(u1max, 1) >= round(np.linalg.norm(
                 self.uqd(w1max, iq, id)/np.sqrt(2)), 1)):
             return [w1type/2/np.pi/self.p, speedmax]
         wl, wu = [w1type, min(4*w1type, w1max)]
         if with_mtpv:
@@ -839,15 +887,15 @@
         r['t_mag'] = self.tmag
 
         return r
 
     def characteristics(self, T, n, u1max, nsamples=60,
                         with_mtpv=True, with_mtpa=True,
                         with_pmconst=True, with_tmech=True,
-                        with_torque_corr=False):
+                        with_torque_corr=False, **kwargs):
         """calculate torque speed characteristics.
         return dict with list values of
         id, iq, n, T, ud, uq, u1, i1,
         beta, gamma, phi, cosphi, pmech, n_type
 
         Keyword arguments:
         T -- the maximum torque or the list of torque values in Nm
@@ -859,14 +907,17 @@
         with_mtpa -- (optional) use mtpa if True (default) in const speed range, set id=0 if false
         with_tmech -- (optional) use friction and windage losses if True (default)
         with_torque_corr -- (optional) T is corrected if out of range
         """
         r = dict(id=[], iq=[], uq=[], ud=[], u1=[], i1=[], T=[],
                  beta=[], gamma=[], phi=[], cosphi=[], pmech=[], n=[])
 
+        if kwargs.get('i1max', 0):
+            w1type, T = self.w1_imax_umax(kwargs['i1max'], u1max)
+
         if np.isscalar(T):
             tmax = self.torquemax(self.i1range[1])
             tmin = 0
             if self.betarange[0] < -np.pi/2:
                 tmin = -self.torquemin(self.i1range[1])
             if tmin > T or T > tmax:
                 if with_torque_corr:
@@ -919,14 +970,17 @@
                 nmax = min(nmax, self.w1_umax(
                     u1max, *iqd(-np.pi/2, abs(i1max))))/2/np.pi/self.p
                 speedrange = [0, n1, nmax]
 
             if speedrange[-1] < speedrange[-2]:
                 speedrange = speedrange[:-1]
             logger.info("Speedrange T=%g Nm %s", Tf, speedrange)
+            if speedrange[-1] < nmax:
+                logger.warning("adjusted nmax %f -> %f", nmax, speedrange[-1])
+
             n3 = speedrange[-1]
             nstab = [int(nsamples*(x1-x2)/n3)
                      for x1, x2 in zip(speedrange[1:],
                                        speedrange)]
             logger.info("sample intervals %s", nstab)
             for nx in np.linspace(0, n1, nstab[0]):
                 if with_tmech:
@@ -1131,15 +1185,20 @@
             logger.debug("ld %s lq %s psim %s", ld, lq, psim)
             return
 
         beta = np.asarray(beta)/180.0*np.pi
         if np.any(beta[beta > np.pi]):
             beta[beta > np.pi] = beta - 2*np.pi
 
-        self.io = iqd((np.min(beta)+max(beta))/2, np.max(i1)/2)
+        self.betarange = min(beta), max(beta)
+        if min(beta) < -np.pi/2 and max(beta) > -np.pi/2:
+            self.io = iqd(-np.pi/4, np.max(i1)/2)
+        else:
+            self.io = iqd((np.min(beta)+max(beta))/2, np.max(i1)/2)
+
         kx = ky = 3
         if len(i1) < 4:
             ky = len(i1)-1
         if len(beta) < 4:
             kx = len(beta)-1
         try:
             pfe = kwargs['losses']
```

### Comparing `femagtools-1.6.5/src/femagtools/machine/sizing.py` & `femagtools-1.6.6/src/femagtools/machine/sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/machine/sm.py` & `femagtools-1.6.6/src/femagtools/machine/sm.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,28 +42,29 @@
         optional arguments:
         num_cur_steps: number of current steps (default 5)
         num_beta_steps: number of current steps (default 13)
         num_exc_steps: number of excitation current (default 7)
         speed: rotor speed in 1/s (default 160/p)
         i1_max: maximum current in A rms (default approx 3*i1nom)
         """
+        cmd = kwargs.get('cmd', None)
         da1 = machine['outer_diam']
         Q1 = machine['stator']['num_slots']
         if 'statorRotor3' in machine['stator']:
             hs = machine['stator']['statorRotor3']['slot_height']
         elif 'stator1' in machine['stator']:
             hs = machine['stator']['stator1']['slot_rf1'] - machine['stator']['stator1']['tip_rh1']
         elif 'stator4' in machine['stator']:
             hs = machine['stator']['stator4']['slot_height']
         Jmax = 15  # max current density in A/mm2
         wdgk = 'windings' if 'windings' in machine else 'winding'
         N = machine[wdgk]['num_wires']
         i1_max = round(0.28*np.pi*hs*(da1+hs)/Q1/N*Jmax*1e5)*10 * \
             machine[wdgk].get('num_par_wdgs', 1)
-
+        
         ifnom = machine['rotor']['ifnom']
         exc_logspace = True
         if exc_logspace:
             excur = np.logspace(np.log(ifnom/10), np.log(1.5*ifnom),
                                 kwargs.get("num_exc_steps", 6),
                                 base=np.exp(1)).tolist()
         else:
@@ -74,15 +75,15 @@
             "decision_vars": [
                 {"values": excur, "name": "load_ex_cur"}
             ]
         }
 
         parvar = parstudy.List(
             workdir,  condMat=condMat,
-            magnetizingCurves=magnetizingCurves)
+            magnetizingCurves=magnetizingCurves, cmd=cmd)
 
         simulation = dict(
                 calculationMode=kwargs.get('calculationMode',
                                            'ld_lq_fast'),
                 wind_temp=20.0,
                 i1_max=kwargs.get('i1_max', i1_max),
                 maxid=0,
@@ -236,14 +237,15 @@
     Arguments:
     eecpars: dict() electrical circuit parameters
     """
     def __init__(self, eecpars, **kwargs):
         self.kth1 = KTH
         self.kth2 = KTH
         self.skin_resistance = [None, None]
+        self.kpmag = 1
         # here you can set user defined functions for calculating the skin-resistance,
         # according to the current frequency w. First function in list is for stator, second for rotor.
         # If None, the femagtools intern default implementation is used.
         # User defined functions need to have the following arguments:
         # - r0: (float) dc-resistance at 20°C
         # - w: (float)  current frequency in rad (2*pi*f)
         # - tcu: (float) conductor temperature in deg Celsius
```

### Comparing `femagtools-1.6.5/src/femagtools/machine/utils.py` & `femagtools-1.6.6/src/femagtools/machine/utils.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/magnet.py` & `femagtools-1.6.6/src/femagtools/magnet.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/mcv.py` & `femagtools-1.6.6/src/femagtools/mcv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/me.py` & `femagtools-1.6.6/src/femagtools/me.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/model.py` & `femagtools-1.6.6/src/femagtools/model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/moo/algorithm.py` & `femagtools-1.6.6/src/femagtools/moo/algorithm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/moo/population.py` & `femagtools-1.6.6/src/femagtools/moo/population.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/moo/problem.py` & `femagtools-1.6.6/src/femagtools/moo/problem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/moo/test/AlgorithmTest.py` & `femagtools-1.6.6/src/femagtools/moo/test/AlgorithmTest.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/moo/test/PopulationTest.py` & `femagtools-1.6.6/src/femagtools/moo/test/PopulationTest.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/moproblem.py` & `femagtools-1.6.6/src/femagtools/moproblem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/multiproc.py` & `femagtools-1.6.6/src/femagtools/multiproc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/mxw2msh.py` & `femagtools-1.6.6/src/femagtools/mxw2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/nc.py` & `femagtools-1.6.6/src/femagtools/nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/netlist.py` & `femagtools-1.6.6/src/femagtools/netlist.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/ntib.py` & `femagtools-1.6.6/src/femagtools/ntib.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/opt.py` & `femagtools-1.6.6/src/femagtools/opt.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/parstudy.py` & `femagtools-1.6.6/src/femagtools/parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/plot/__init__.py` & `femagtools-1.6.6/src/femagtools/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/plot/bch.py` & `femagtools-1.6.6/src/femagtools/plot/bch.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/plot/char.py` & `femagtools-1.6.6/src/femagtools/plot/char.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/plot/fieldlines.py` & `femagtools-1.6.6/src/femagtools/plot/fieldlines.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/plot/fluxdens.py` & `femagtools-1.6.6/src/femagtools/plot/fluxdens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/plot/forcedens.py` & `femagtools-1.6.6/src/femagtools/plot/forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/plot/mcv.py` & `femagtools-1.6.6/src/femagtools/plot/mcv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/plot/nc.py` & `femagtools-1.6.6/src/femagtools/plot/nc.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,16 +145,15 @@
 def __elements_of_subreg(isa, subreg):
     if subreg:
         if isinstance(subreg, list):
             sr = subreg
         else:
             sr = [subreg]
         for s in sr:
-            for e in isa.get_subregion(s).elements():
-                yield e
+            yield from isa.get_subregion(s).elements()
     else:
         for e in isa.elements:
             yield e
 
 
 def flux_density(isa, subreg=[], cmap=DEFAULT_CMAP, ax=0):
     """plot flux density of NC/I7/ISA7 model
@@ -228,15 +227,16 @@
     Args:
         isa: Isa7/NC object
         ipos: position index
         icur: cur index or last index if -1
         ibeta: beta angle index or last index if -1
 
     """
-    elements = [e for e in __elements_of_subreg(isa, subreg)]
+    elements = [e for e in __elements_of_subreg(isa, subreg)
+                if e not in isa.airgap_center_elements]
     b = []
     for e in elements:
         fd = isa.flux_density(e, icur, ibeta)
         b.append(np.linalg.norm(
             (fd['bx'][ipos], fd['by'][ipos])))
     fluxd = np.array(b)
     pos = isa.pos_el_fe_induction[ipos]*180/np.pi
```

### Comparing `femagtools-1.6.5/src/femagtools/plot/phasor.py` & `femagtools-1.6.6/src/femagtools/plot/phasor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/plot/wdg.py` & `femagtools-1.6.6/src/femagtools/plot/wdg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/poc.py` & `femagtools-1.6.6/src/femagtools/poc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/FE-losses.mako` & `femagtools-1.6.6/src/femagtools/templates/FE-losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/afm_rotor.mako` & `femagtools-1.6.6/src/femagtools/templates/afm_rotor.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/afm_stator.mako` & `femagtools-1.6.6/src/femagtools/templates/afm_stator.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/asyn_motor.mako` & `femagtools-1.6.6/src/femagtools/templates/asyn_motor.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/basic_modpar.mako` & `femagtools-1.6.6/src/femagtools/templates/basic_modpar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/bertotti.mako` & `femagtools-1.6.6/src/femagtools/templates/bertotti.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/calc_field_ts.mako` & `femagtools-1.6.6/src/femagtools/templates/calc_field_ts.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/calc_therm_field.mako` & `femagtools-1.6.6/src/femagtools/templates/calc_therm_field.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/cogg_calc.mako` & `femagtools-1.6.6/src/femagtools/templates/cogg_calc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/com_motor_sim.mako` & `femagtools-1.6.6/src/femagtools/templates/com_motor_sim.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/connect_models.mako` & `femagtools-1.6.6/src/femagtools/templates/connect_models.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/cu_losses.mako` & `femagtools-1.6.6/src/femagtools/templates/cu_losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/ec-rotorbar.mako` & `femagtools-1.6.6/src/femagtools/templates/ec-rotorbar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/fe-contr.mako` & `femagtools-1.6.6/src/femagtools/templates/fe-contr.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/fieldcalc.mako` & `femagtools-1.6.6/src/femagtools/templates/fieldcalc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/gen_winding.mako` & `femagtools-1.6.6/src/femagtools/templates/gen_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/inductances.mako` & `femagtools-1.6.6/src/femagtools/templates/inductances.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/ld_lq_fast.mako` & `femagtools-1.6.6/src/femagtools/templates/ld_lq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/leak_dist_wind.mako` & `femagtools-1.6.6/src/femagtools/templates/leak_dist_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/leak_evol_wind.mako` & `femagtools-1.6.6/src/femagtools/templates/leak_evol_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/magnet-data.mako` & `femagtools-1.6.6/src/femagtools/templates/magnet-data.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/magnetFC2.mako` & `femagtools-1.6.6/src/femagtools/templates/magnetFC2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/magnetIron.mako` & `femagtools-1.6.6/src/femagtools/templates/magnetIron.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/magnetIron2.mako` & `femagtools-1.6.6/src/femagtools/templates/magnetIron2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/magnetIron3.mako` & `femagtools-1.6.6/src/femagtools/templates/magnetIron3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/magnetIron4.mako` & `femagtools-1.6.6/src/femagtools/templates/magnetIron4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/magnetIron5.mako` & `femagtools-1.6.6/src/femagtools/templates/magnetIron5.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/magnetIronV.mako` & `femagtools-1.6.6/src/femagtools/templates/magnetIronV.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/magnetSector.mako` & `femagtools-1.6.6/src/femagtools/templates/magnetSector.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/magnetSectorLinear.mako` & `femagtools-1.6.6/src/femagtools/templates/magnetSectorLinear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/magnetShell.mako` & `femagtools-1.6.6/src/femagtools/templates/magnetShell.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/magnetShell2.mako` & `femagtools-1.6.6/src/femagtools/templates/magnetShell2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/mesh-airgap.mako` & `femagtools-1.6.6/src/femagtools/templates/mesh-airgap.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/modal_analysis.mako` & `femagtools-1.6.6/src/femagtools/templates/modal_analysis.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/modified_steinmetz.mako` & `femagtools-1.6.6/src/femagtools/templates/modified_steinmetz.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/mult_cal_fast.mako` & `femagtools-1.6.6/src/femagtools/templates/mult_cal_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/noloadflux-rot.mako` & `femagtools-1.6.6/src/femagtools/templates/noloadflux-rot.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/noloadflux.mako` & `femagtools-1.6.6/src/femagtools/templates/noloadflux.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/noloadfluxdc.mako` & `femagtools-1.6.6/src/femagtools/templates/noloadfluxdc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/plots.mako` & `femagtools-1.6.6/src/femagtools/templates/plots.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/pm_sym_f_cur.mako` & `femagtools-1.6.6/src/femagtools/templates/pm_sym_f_cur.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/pm_sym_fast.mako` & `femagtools-1.6.6/src/femagtools/templates/pm_sym_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/pm_sym_loss.mako` & `femagtools-1.6.6/src/femagtools/templates/pm_sym_loss.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/psd_psq_fast.mako` & `femagtools-1.6.6/src/femagtools/templates/psd_psq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/ring.mako` & `femagtools-1.6.6/src/femagtools/templates/ring.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/rot_hsm.mako` & `femagtools-1.6.6/src/femagtools/templates/rot_hsm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/rotorAsyn.mako` & `femagtools-1.6.6/src/femagtools/templates/rotorAsyn.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/rotorKs2.mako` & `femagtools-1.6.6/src/femagtools/templates/rotorKs2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/rotor_msh.mako` & `femagtools-1.6.6/src/femagtools/templates/rotor_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/rotor_winding.mako` & `femagtools-1.6.6/src/femagtools/templates/rotor_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/shortcircuit.mako` & `femagtools-1.6.6/src/femagtools/templates/shortcircuit.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/srm.mako` & `femagtools-1.6.6/src/femagtools/templates/srm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/stator1.mako` & `femagtools-1.6.6/src/femagtools/templates/stator1.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/stator2.mako` & `femagtools-1.6.6/src/femagtools/templates/stator2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/stator3Linear.mako` & `femagtools-1.6.6/src/femagtools/templates/stator3Linear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/stator4.mako` & `femagtools-1.6.6/src/femagtools/templates/stator4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/statorBG.mako` & `femagtools-1.6.6/src/femagtools/templates/statorBG.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/statorRing.mako` & `femagtools-1.6.6/src/femagtools/templates/statorRing.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/statorRotor3.mako` & `femagtools-1.6.6/src/femagtools/templates/statorRotor3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/stator_msh.mako` & `femagtools-1.6.6/src/femagtools/templates/stator_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/therm-dynamic.mako` & `femagtools-1.6.6/src/femagtools/templates/therm-dynamic.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/therm-static.mako` & `femagtools-1.6.6/src/femagtools/templates/therm-static.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/templates/torq_calc.mako` & `femagtools-1.6.6/src/femagtools/templates/torq_calc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/tks.py` & `femagtools-1.6.6/src/femagtools/tks.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/ts.py` & `femagtools-1.6.6/src/femagtools/ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/utils.py` & `femagtools-1.6.6/src/femagtools/utils.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/vbf.py` & `femagtools-1.6.6/src/femagtools/vbf.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/vtu.py` & `femagtools-1.6.6/src/femagtools/vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools/windings.py` & `femagtools-1.6.6/src/femagtools/windings.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/femagtools.egg-info/PKG-INFO` & `femagtools-1.6.6/src/femagtools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.6.5
+Version: 1.6.6
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <dzhang@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
@@ -41,14 +41,18 @@
 Requires-Dist: mako
 Requires-Dist: six
 Requires-Dist: lmfit
 Requires-Dist: netCDF4>=1.6.5
 Provides-Extra: dxfsl
 Requires-Dist: dxfgrabber; extra == "dxfsl"
 Requires-Dist: networkx; extra == "dxfsl"
+Provides-Extra: svgfsl
+Requires-Dist: dxfgrabber; extra == "svgfsl"
+Requires-Dist: networkx; extra == "svgfsl"
+Requires-Dist: lxml; extra == "svgfsl"
 Provides-Extra: mplot
 Requires-Dist: matplotlib; extra == "mplot"
 Provides-Extra: meshio
 Requires-Dist: meshio; extra == "meshio"
 Provides-Extra: vtk
 Requires-Dist: vtk; extra == "vtk"
 Provides-Extra: zmq
```

### Comparing `femagtools-1.6.5/src/femagtools.egg-info/SOURCES.txt` & `femagtools-1.6.6/src/femagtools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -60,21 +60,24 @@
 src/femagtools/dxfsl/area.py
 src/femagtools/dxfsl/areabuilder.py
 src/femagtools/dxfsl/concat.py
 src/femagtools/dxfsl/conv.py
 src/femagtools/dxfsl/converter.py
 src/femagtools/dxfsl/corner.py
 src/femagtools/dxfsl/dumprenderer.py
+src/femagtools/dxfsl/dxfparser.py
+src/femagtools/dxfsl/femparser.py
 src/femagtools/dxfsl/fslrenderer.py
 src/femagtools/dxfsl/functions.py
 src/femagtools/dxfsl/geom.py
 src/femagtools/dxfsl/journal.py
 src/femagtools/dxfsl/machine.py
 src/femagtools/dxfsl/plotrenderer.py
 src/femagtools/dxfsl/shape.py
+src/femagtools/dxfsl/svgparser.py
 src/femagtools/dxfsl/symmetry.py
 src/femagtools/machine/__init__.py
 src/femagtools/machine/afpm.py
 src/femagtools/machine/effloss.py
 src/femagtools/machine/im.py
 src/femagtools/machine/pm.py
 src/femagtools/machine/sizing.py
@@ -93,14 +96,15 @@
 src/femagtools/plot/fieldlines.py
 src/femagtools/plot/fluxdens.py
 src/femagtools/plot/forcedens.py
 src/femagtools/plot/mcv.py
 src/femagtools/plot/nc.py
 src/femagtools/plot/phasor.py
 src/femagtools/plot/wdg.py
+src/femagtools/svgfsl/converter.py
 src/femagtools/templates/FE-losses.mako
 src/femagtools/templates/afm_rotor.mako
 src/femagtools/templates/afm_stator.mako
 src/femagtools/templates/airgapinduc.mako
 src/femagtools/templates/asyn_motor.mako
 src/femagtools/templates/basic_modpar.mako
 src/femagtools/templates/bertotti.mako
@@ -170,14 +174,15 @@
 src/tests/test_afpm.py
 src/tests/test_airgap_induction.py
 src/tests/test_amela.py
 src/tests/test_asm.py
 src/tests/test_bchreader.py
 src/tests/test_conductor.py
 src/tests/test_convert.py
+src/tests/test_dxfsl.py
 src/tests/test_effloss.py
 src/tests/test_erg.py
 src/tests/test_femag.py
 src/tests/test_forcedens.py
 src/tests/test_fsl.py
 src/tests/test_hxy.py
 src/tests/test_im.py
```

### Comparing `femagtools-1.6.5/src/tests/engines/__init__.py` & `femagtools-1.6.6/src/tests/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/engines/test_amazon.py` & `femagtools-1.6.6/src/tests/engines/test_amazon.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/engines/test_config.py` & `femagtools-1.6.6/src/tests/engines/test_config.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/geom/__init__.py` & `femagtools-1.6.6/src/tests/geom/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/geom/test_functions.py` & `femagtools-1.6.6/src/tests/geom/test_functions.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/geom/test_point_inside.py` & `femagtools-1.6.6/src/tests/geom/test_point_inside.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/moo/__init__.py` & `femagtools-1.6.6/src/tests/moo/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/moo/test_algorithm.py` & `femagtools-1.6.6/src/tests/moo/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/moo/test_population.py` & `femagtools-1.6.6/src/tests/moo/test_population.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_afpm.py` & `femagtools-1.6.6/src/tests/test_afpm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_airgap_induction.py` & `femagtools-1.6.6/src/tests/test_airgap_induction.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_amela.py` & `femagtools-1.6.6/src/tests/test_amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_asm.py` & `femagtools-1.6.6/src/tests/test_asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_bchreader.py` & `femagtools-1.6.6/src/tests/test_bchreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_convert.py` & `femagtools-1.6.6/src/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_effloss.py` & `femagtools-1.6.6/src/tests/test_effloss.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_erg.py` & `femagtools-1.6.6/src/tests/test_erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_femag.py` & `femagtools-1.6.6/src/tests/test_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_forcedens.py` & `femagtools-1.6.6/src/tests/test_forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_fsl.py` & `femagtools-1.6.6/src/tests/test_fsl.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_hxy.py` & `femagtools-1.6.6/src/tests/test_hxy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_im.py` & `femagtools-1.6.6/src/tests/test_im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_isa7.py` & `femagtools-1.6.6/src/tests/test_isa7.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_jhb.py` & `femagtools-1.6.6/src/tests/test_jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_job.py` & `femagtools-1.6.6/src/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_losscoeffs.py` & `femagtools-1.6.6/src/tests/test_losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_machine.py` & `femagtools-1.6.6/src/tests/test_machine.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_magncurv.py` & `femagtools-1.6.6/src/tests/test_magncurv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_mcvreader.py` & `femagtools-1.6.6/src/tests/test_mcvreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_mcvwriter.py` & `femagtools-1.6.6/src/tests/test_mcvwriter.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_model.py` & `femagtools-1.6.6/src/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_nc.py` & `femagtools-1.6.6/src/tests/test_nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_parident.py` & `femagtools-1.6.6/src/tests/test_parident.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_parstudy.py` & `femagtools-1.6.6/src/tests/test_parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_pocfile.py` & `femagtools-1.6.6/src/tests/test_pocfile.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_sizing.py` & `femagtools-1.6.6/src/tests/test_sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_sm.py` & `femagtools-1.6.6/src/tests/test_sm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_tksreader.py` & `femagtools-1.6.6/src/tests/test_tksreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_ts.py` & `femagtools-1.6.6/src/tests/test_ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_vbfreader.py` & `femagtools-1.6.6/src/tests/test_vbfreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_vtu.py` & `femagtools-1.6.6/src/tests/test_vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.6.5/src/tests/test_windings.py` & `femagtools-1.6.6/src/tests/test_windings.py`

 * *Files identical despite different names*

