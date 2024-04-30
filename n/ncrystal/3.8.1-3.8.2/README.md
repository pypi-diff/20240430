# Comparing `tmp/ncrystal-3.8.1.tar.gz` & `tmp/ncrystal-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncrystal-3.8.1.tar", last modified: Thu Apr 11 13:53:49 2024, max compression
+gzip compressed data, was "ncrystal-3.8.2.tar", last modified: Tue Apr 30 07:25:03 2024, max compression
```

## Comparing `ncrystal-3.8.1.tar` & `ncrystal-3.8.2.tar`

### file list

```diff
@@ -1,433 +1,433 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.136874 ncrystal-3.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.064873 ncrystal-3.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.064873 ncrystal-3.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-11 13:53:40.000000 ncrystal-3.8.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-11 13:53:40.000000 ncrystal-3.8.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-11 13:53:40.000000 ncrystal-3.8.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-11 13:53:40.000000 ncrystal-3.8.1/.github/ISSUE_TEMPLATE/request-for-new-material.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-11 13:53:40.000000 ncrystal-3.8.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.064873 ncrystal-3.8.1/.github/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-11 13:53:40.000000 ncrystal-3.8.1/.github/resources/conda_ncrystaltestenv.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.064873 ncrystal-3.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-11 13:53:40.000000 ncrystal-3.8.1/.github/workflows/basictest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-11 13:53:40.000000 ncrystal-3.8.1/.github/workflows/condatest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-11 13:53:40.000000 ncrystal-3.8.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 13:53:40.000000 ncrystal-3.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    85508 2024-04-11 13:53:40.000000 ncrystal-3.8.1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    43367 2024-04-11 13:53:40.000000 ncrystal-3.8.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-11 13:53:40.000000 ncrystal-3.8.1/FILES
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-11 13:53:40.000000 ncrystal-3.8.1/INSTALL
--rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-04-11 13:53:40.000000 ncrystal-3.8.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.068873 ncrystal-3.8.1/NCrystal/
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40733 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/_chooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/_coreimpl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/_miscimpl.py
--rw-r--r--   0 runner    (1001) docker     (127)    85698 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/_ncmatimpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    25791 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/_testimpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/atomdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/cfgstr.py
--rw-r--r--   0 runner    (1001) docker     (127)    74605 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/cifutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    75158 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/datasrc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/mcstasutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    38896 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/ncmat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/obsolete.py
--rw-r--r--   0 runner    (1001) docker     (127)    19520 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    46233 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NCrystal/vdos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-11 13:53:40.000000 ncrystal-3.8.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-11 13:53:49.136874 ncrystal-3.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14200 2024-04-11 13:53:40.000000 ncrystal-3.8.1/README
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 13:53:40.000000 ncrystal-3.8.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.072873 ncrystal-3.8.1/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-11 13:53:40.000000 ncrystal-3.8.1/cmake/NCrystalConfig.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.072873 ncrystal-3.8.1/cmake/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-11 13:53:40.000000 ncrystal-3.8.1/cmake/modules/ncrystal_legacyoptions.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-11 13:53:40.000000 ncrystal-3.8.1/cmake/modules/ncrystal_options.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-11 13:53:40.000000 ncrystal-3.8.1/cmake/modules/ncrystal_utils.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    13917 2024-04-11 13:53:40.000000 ncrystal-3.8.1/cmake/ncrystal-config.in
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-11 13:53:40.000000 ncrystal-3.8.1/cmake/template_setup.py.in
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-11 13:53:40.000000 ncrystal-3.8.1/cmake/template_setup.sh.in
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 13:53:40.000000 ncrystal-3.8.1/cmake/template_unsetup.sh.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.096874 ncrystal-3.8.1/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/AcrylicGlass_C5O2H8.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/AgBr_sg225_SilverBromide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Ag_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Al2O3_sg167_Corundum.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Al4C3_sg166_AluminiumCarbide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/AlN_sg186_AluminumNitride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Al_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Ar_Gas_STP.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Au_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/BaF2_sg225_BariumFluoride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/BaO_sg225_BariumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Ba_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Be3N2_sg206_BerylliumNitride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/BeF2_sg152_Beryllium_Fluoride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/BeO_sg186.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Be_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Bi_sg166.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/C_sg194_pyrolytic_graphite.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/C_sg227_Diamond.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/CaCO3_sg62_Aragonite.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/CaF2_sg225_CalciumFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/CaH2_sg62_CalciumHydride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/CaO2H2_sg164_CalciumHydroxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/CaO_sg225_CalciumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/CaSiO3_sg2_Wollastonite.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Ca_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Ca_sg229_Calcium-gamma.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/CeO2_sg225_CeriumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Cr_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Cu2O_sg224_Cuprite.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Cu_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Dy2O3_sg206_DysprosiumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Epoxy_Araldite506_C18H20O3.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Fe_sg225_Iron-gamma.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Fe_sg229_Iron-alpha.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/GaN_sg186_GalliumNitride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/GaSe_sg194_GalliumSelenide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Ge3Bi4O12_sg220_BismuthGermanate.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Ge_sg227.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/He_Gas_STP.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/HfO2_sg14_HafniumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Ho2O3_sg206_HolmiumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/KBr_sg225_PotassiumBromide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/KF_sg225_PotassiumFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/KOH_sg4_PotassiumHydroxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/K_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Kapton_C22H10N2O5.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Kr_Gas_STP.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/LaBr3_sg176_LanthanumBromide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Li2O_sg225_LithiumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Li3N_sg191_LithiumNitride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/LiF_sg225_LithiumFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/LiH_sg225_LithiumHydride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)  1560968 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/LiquidHeavyWaterD2O_T293.6K.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)   528493 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/LiquidWaterH2O_T293.6K.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Lu2O3_sg206_LutetiumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Lu2SiO5_sg15.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Mg2SiO4_sg62_MagnesiumSilicate.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/MgAl2O4_sg227_MAS.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/MgCO3_sg167_MagnesiumCarbonate.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/MgD2_sg136_MagnesiumDeuteride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/MgF2_sg136_MagnesiumFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/MgH2_sg136_MagnesiumHydride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/MgO2H2_sg164_MagnesiumHydroxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/MgO_sg225_Periclase.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Mg_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Mo_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Na4Si3Al3O12Cl_sg218_Sodalite.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/NaBr_sg225_SodiumBromide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/NaCl_sg225_SodiumChloride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/NaF_sg225_SodiumFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/NaI_sg225_SodiumIodide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Na_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Nb_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Ne_Gas_STP.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Ni_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Nylon11_C11H21NO.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Nylon12_C12H23NO.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Nylon610_C16H30N2O2.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Nylon66or6_C12H22N2O2.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/PEEK_C19H12O3.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/PVC_C2H3Cl.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/PbF2-beta_sg225_BetaLeadFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/PbO-alpha_sg129_Litharge.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/PbO-beta_sg57_Massicot.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/PbS_sg225_LeadSulfide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Pb_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Pd_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Polycarbonate_C16O3H14.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Polyester_C10H8O4.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Polyethylene_CH2.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Polylactide_C3H4O2.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Polypropylene_C3H6.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Polystyrene_C8H8.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Pt_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Rb_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Rubber_C5H8.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Sc_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/SiC-beta_sg216_BetaSiliconCarbide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/SiO2-alpha_sg154_AlphaQuartz.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/SiO2-beta_sg180_BetaQuartz.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Si_sg227.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Sn_sg141.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/SrF2_sg225_StrontiumFluoride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/SrH2_sg62_StrontiumHydride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Sr_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Th3N4_sg166_ThoriumNitride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/ThO2_sg225_ThoriumDioxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Th_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/TiO2_sg136_Rutile.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/TiO2_sg141_Anatase.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Ti_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/TlBr_sg221_ThaliumBromide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Tm2O3_sg206_ThuliumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/UF6_sg62_UraniumHexaflouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/UO2_sg225_UraniumDioxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/V_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/W_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Xe_Gas_STP.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Y2O3_sg206_Yttrium_Oxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Y2SiO5_sg15_YSO.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Y3Al5O12_sg230_YAG.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Y_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/ZnF2_sg136_ZincFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/ZnO_sg186_ZincOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/ZnS_sg216_Sphalerite.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Zn_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/ZrF4-beta_sg84.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/ZrO2_sg137_Zirconia.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/ZrO2_sg14_Zirconia.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/Zr_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-11 13:53:40.000000 ncrystal-3.8.1/data/void.ncmat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.096874 ncrystal-3.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    39216 2024-04-11 13:53:40.000000 ncrystal-3.8.1/docs/ncmat_doc.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.096874 ncrystal-3.8.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-11 13:53:40.000000 ncrystal-3.8.1/examples/ncrystal_example_c.c
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-11 13:53:40.000000 ncrystal-3.8.1/examples/ncrystal_example_cpp.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-04-11 13:53:40.000000 ncrystal-3.8.1/examples/ncrystal_example_customphysics.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-11 13:53:40.000000 ncrystal-3.8.1/examples/ncrystal_example_g4sim.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-11 13:53:40.000000 ncrystal-3.8.1/examples/ncrystal_example_py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.136874 ncrystal-3.8.1/ncrystal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-11 13:53:49.000000 ncrystal-3.8.1/ncrystal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14377 2024-04-11 13:53:49.000000 ncrystal-3.8.1/ncrystal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:53:49.000000 ncrystal-3.8.1/ncrystal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 13:53:49.000000 ncrystal-3.8.1/ncrystal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 13:53:49.000000 ncrystal-3.8.1/ncrystal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.060873 ncrystal-3.8.1/ncrystal_core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.060873 ncrystal-3.8.1/ncrystal_core/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.104874 ncrystal-3.8.1/ncrystal_core/include/NCrystal/
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCAtomData.hh
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCCompositionUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCDataSources.hh
--rw-r--r--   0 runner    (1001) docker     (127)    51910 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCDefs.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCDump.hh
--rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCException.hh
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCFact.hh
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCFactImpl.hh
--rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCFactRequests.hh
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCFactTypes.hh
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCFmt.hh
--rw-r--r--   0 runner    (1001) docker     (127)    16617 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCImmutBuf.hh
--rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCInfo.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCInfoBuilder.hh
--rw-r--r--   0 runner    (1001) docker     (127)    16865 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCInfoTypes.hh
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCLoadNCMAT.hh
--rw-r--r--   0 runner    (1001) docker     (127)    22393 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCMatCfg.hh
--rw-r--r--   0 runner    (1001) docker     (127)    20453 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCMem.hh
--rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCNCMATData.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCParseNCMAT.hh
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCPluginBoilerplate.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCPluginMgmt.hh
--rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCProc.hh
--rw-r--r--   0 runner    (1001) docker     (127)    20032 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCProcImpl.hh
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCRNG.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCSABData.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCSCOrientation.hh
--rw-r--r--   0 runner    (1001) docker     (127)    39167 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCSmallVector.hh
--rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCTextData.hh
--rw-r--r--   0 runner    (1001) docker     (127)    37506 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCTypes.hh
--rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCVariant.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCVersion.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCrystal.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.116874 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCAbsOOV.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCAtomDB.hh
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCAtomDBExtender.hh
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCAtomUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCBkgdExtCurve.hh
--rw-r--r--   0 runner    (1001) docker     (127)    23040 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCCfgManip.hh
--rw-r--r--   0 runner    (1001) docker     (127)    32382 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCCfgTypes.hh
--rw-r--r--   0 runner    (1001) docker     (127)    35739 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCCfgVars.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCDebyeMSD.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCDynInfoUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCDynLoader.hh
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCElIncScatter.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCElIncXS.hh
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCEqRefl.hh
--rw-r--r--   0 runner    (1001) docker     (127)    20006 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCFactoryUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCFastConvolve.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCFileUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCFillHKL.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCFreeGas.hh
--rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCFreeGasUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCGasMixUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCGaussMos.hh
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCGaussOnSphere.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCIofQHelper.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCIter.hh
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCKinUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCLCBragg.hh
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCLCRefModels.hh
--rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCLCUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCLatticeUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)    27329 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCMath.hh
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCMatrix.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCOrientUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCPCBragg.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCPlaneProvider.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCPointwiseDist.hh
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCRandUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCRomberg.hh
--rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCRotMatrix.hh
--rw-r--r--   0 runner    (1001) docker     (127)    18031 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABEval.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABExtender.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABFactory.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABIntegrator.hh
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABSampler.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABSamplerModels.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABScatter.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABScatterHelper.hh
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABUCN.hh
--rw-r--r--   0 runner    (1001) docker     (127)    14775 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABXSProvider.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSANSSphScat.hh
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSANSUtils.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSCBragg.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCScatKnlData.hh
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSpan.hh
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSpline.hh
--rw-r--r--   0 runner    (1001) docker     (127)    20133 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCStrView.hh
--rw-r--r--   0 runner    (1001) docker     (127)    15446 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCString.hh
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCVDOSEval.hh
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCVDOSGn.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCVDOSToScatKnl.hh
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCVector.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/ncapi.h
--rw-r--r--   0 runner    (1001) docker     (127)    68354 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/include/NCrystal/ncrystal.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.132874 ncrystal-3.8.1/ncrystal_core/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCAbsOOV.cc
--rw-r--r--   0 runner    (1001) docker     (127)    36781 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCAtomDB.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9819 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCAtomDBExtender.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCAtomData.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCAtomUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCBkgdExtCurve.cc
--rw-r--r--   0 runner    (1001) docker     (127)    18374 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCCfgManip.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCCfgTypes.cc
--rw-r--r--   0 runner    (1001) docker     (127)    17931 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCCfgVars.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCCompositionUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)    26285 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCDataSources.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCDebyeMSD.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCDefs.cc
--rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCDump.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCDynInfoUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCDynLoader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCElIncScatter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCElIncXS.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCEqRefl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCException.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCFact.cc
--rw-r--r--   0 runner    (1001) docker     (127)    42918 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCFactImpl.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCFactRequests.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCFactTypes.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCFactoryUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCFactory_NCMAT.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCFastConvolve.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCFileUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)    30238 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCFillHKL.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCFmt.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCFreeGas.cc
--rw-r--r--   0 runner    (1001) docker     (127)    39981 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCFreeGasUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCGasMixFact.cc
--rw-r--r--   0 runner    (1001) docker     (127)    26609 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCGasMixUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCGaussMos.cc
--rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCGaussOnSphere.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCInfo.cc
--rw-r--r--   0 runner    (1001) docker     (127)    57548 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCInfoBuilder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCIofQHelper.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCKinUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCLCBragg.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCLCRefModels.cc
--rw-r--r--   0 runner    (1001) docker     (127)    32342 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCLCUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)    19529 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCLatticeUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCLauLazyFact.cc
--rw-r--r--   0 runner    (1001) docker     (127)    30611 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCLazy.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCLazy.hh
--rw-r--r--   0 runner    (1001) docker     (127)    33292 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCLoadNCMAT.cc
--rw-r--r--   0 runner    (1001) docker     (127)    49031 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCMatCfg.cc
--rw-r--r--   0 runner    (1001) docker     (127)    23845 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCMath.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCMem.cc
--rw-r--r--   0 runner    (1001) docker     (127)    31787 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCNCMATData.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCOrientUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCPCBragg.cc
--rw-r--r--   0 runner    (1001) docker     (127)    42624 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCParseNCMAT.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCPlaneProvider.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCPluginMgmt.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCPointwiseDist.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCProc.cc
--rw-r--r--   0 runner    (1001) docker     (127)    20209 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCProcImpl.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14897 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCQuickFact.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCRNG.cc
--rw-r--r--   0 runner    (1001) docker     (127)    20337 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCRandUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCRomberg.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCRotMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSABData.cc
--rw-r--r--   0 runner    (1001) docker     (127)    31895 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSABEval.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSABExtender.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSABFactory.cc
--rw-r--r--   0 runner    (1001) docker     (127)    23459 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSABIntegrator.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSABSampler.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSABSamplerModels.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSABScatter.cc
--rw-r--r--   0 runner    (1001) docker     (127)    26316 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSABUCN.cc
--rw-r--r--   0 runner    (1001) docker     (127)    26756 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSABUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSABXSProvider.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSANSFact.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSANSSphScat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSANSUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13245 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSCBragg.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSCOrientation.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCScatKnlData.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCSpline.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCStdAbsFact.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCStdMPScatFact.cc
--rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCStdScatFact.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCStrView.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCString.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCTDProd.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCTextData.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCTypes.cc
--rw-r--r--   0 runner    (1001) docker     (127)    25956 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCVDOSEval.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCVDOSGn.cc
--rw-r--r--   0 runner    (1001) docker     (127)    38641 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCVDOSToScatKnl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCVector.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/NCVersion.cc
--rw-r--r--   0 runner    (1001) docker     (127)    72933 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_core/src/ncrystal.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.064873 ncrystal-3.8.1/ncrystal_geant4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.060873 ncrystal-3.8.1/ncrystal_geant4/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.132874 ncrystal-3.8.1/ncrystal_geant4/include/G4NCrystal/
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_geant4/include/G4NCrystal/G4NCInstall.hh
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_geant4/include/G4NCrystal/G4NCManager.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_geant4/include/G4NCrystal/G4NCMatHelper.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_geant4/include/G4NCrystal/G4NCrystal.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.136874 ncrystal-3.8.1/ncrystal_geant4/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_geant4/src/G4NCInstall.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_geant4/src/G4NCManager.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_geant4/src/G4NCMatHelper.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_geant4/src/G4NCProcWrapper.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-11 13:53:40.000000 ncrystal-3.8.1/ncrystal_geant4/src/G4NCProcWrapper.hh
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-11 13:53:40.000000 ncrystal-3.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:53:49.136874 ncrystal-3.8.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)    15960 2024-04-11 13:53:40.000000 ncrystal-3.8.1/scripts/ncrystal_cif2ncmat
--rwxr-xr-x   0 runner    (1001) docker     (127)    35171 2024-04-11 13:53:40.000000 ncrystal-3.8.1/scripts/ncrystal_endf2ncmat
--rwxr-xr-x   0 runner    (1001) docker     (127)    73858 2024-04-11 13:53:40.000000 ncrystal-3.8.1/scripts/ncrystal_hfg2ncmat
--rwxr-xr-x   0 runner    (1001) docker     (127)     1759 2024-04-11 13:53:40.000000 ncrystal-3.8.1/scripts/ncrystal_inspectfile
--rwxr-xr-x   0 runner    (1001) docker     (127)    15454 2024-04-11 13:53:40.000000 ncrystal-3.8.1/scripts/ncrystal_ncmat2cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     7565 2024-04-11 13:53:40.000000 ncrystal-3.8.1/scripts/ncrystal_ncmat2hkl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1998 2024-04-11 13:53:40.000000 ncrystal-3.8.1/scripts/ncrystal_onlinedb2ncmat
--rwxr-xr-x   0 runner    (1001) docker     (127)    20289 2024-04-11 13:53:40.000000 ncrystal-3.8.1/scripts/ncrystal_vdos2ncmat
--rwxr-xr-x   0 runner    (1001) docker     (127)    13315 2024-04-11 13:53:40.000000 ncrystal-3.8.1/scripts/ncrystal_verifyatompos
--rwxr-xr-x   0 runner    (1001) docker     (127)    35942 2024-04-11 13:53:40.000000 ncrystal-3.8.1/scripts/nctool
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:53:49.136874 ncrystal-3.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-11 13:53:40.000000 ncrystal-3.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.376909 ncrystal-3.8.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.304909 ncrystal-3.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.304909 ncrystal-3.8.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 07:24:54.000000 ncrystal-3.8.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 07:24:54.000000 ncrystal-3.8.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-30 07:24:54.000000 ncrystal-3.8.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-30 07:24:54.000000 ncrystal-3.8.2/.github/ISSUE_TEMPLATE/request-for-new-material.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-30 07:24:54.000000 ncrystal-3.8.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.304909 ncrystal-3.8.2/.github/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-30 07:24:54.000000 ncrystal-3.8.2/.github/resources/conda_ncrystaltestenv.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.308909 ncrystal-3.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-30 07:24:54.000000 ncrystal-3.8.2/.github/workflows/basictest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-30 07:24:54.000000 ncrystal-3.8.2/.github/workflows/condatest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-30 07:24:54.000000 ncrystal-3.8.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-30 07:24:54.000000 ncrystal-3.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    85714 2024-04-30 07:24:54.000000 ncrystal-3.8.2/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    43604 2024-04-30 07:24:54.000000 ncrystal-3.8.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-30 07:24:54.000000 ncrystal-3.8.2/FILES
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-30 07:24:54.000000 ncrystal-3.8.2/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-04-30 07:24:54.000000 ncrystal-3.8.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.312909 ncrystal-3.8.2/NCrystal/
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40733 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/_chooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/_coreimpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/_miscimpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85698 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/_ncmatimpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25791 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/_testimpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/atomdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/cfgstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74605 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/cifutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75158 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/datasrc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/mcstasutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38896 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/ncmat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/obsolete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19520 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46233 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NCrystal/vdos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-30 07:24:54.000000 ncrystal-3.8.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-30 07:25:03.376909 ncrystal-3.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14200 2024-04-30 07:24:54.000000 ncrystal-3.8.2/README
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 07:24:54.000000 ncrystal-3.8.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.312909 ncrystal-3.8.2/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-30 07:24:54.000000 ncrystal-3.8.2/cmake/NCrystalConfig.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.312909 ncrystal-3.8.2/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-30 07:24:54.000000 ncrystal-3.8.2/cmake/modules/ncrystal_legacyoptions.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-30 07:24:54.000000 ncrystal-3.8.2/cmake/modules/ncrystal_options.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-30 07:24:54.000000 ncrystal-3.8.2/cmake/modules/ncrystal_utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    13917 2024-04-30 07:24:54.000000 ncrystal-3.8.2/cmake/ncrystal-config.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-30 07:24:54.000000 ncrystal-3.8.2/cmake/template_setup.py.in
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-30 07:24:54.000000 ncrystal-3.8.2/cmake/template_setup.sh.in
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-30 07:24:54.000000 ncrystal-3.8.2/cmake/template_unsetup.sh.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.336909 ncrystal-3.8.2/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/AcrylicGlass_C5O2H8.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/AgBr_sg225_SilverBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Ag_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Al2O3_sg167_Corundum.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Al4C3_sg166_AluminiumCarbide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/AlN_sg186_AluminumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Al_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Ar_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Au_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/BaF2_sg225_BariumFluoride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/BaO_sg225_BariumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Ba_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Be3N2_sg206_BerylliumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/BeF2_sg152_Beryllium_Fluoride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/BeO_sg186.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Be_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Bi_sg166.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/C_sg194_pyrolytic_graphite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/C_sg227_Diamond.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/CaCO3_sg62_Aragonite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/CaF2_sg225_CalciumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/CaH2_sg62_CalciumHydride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/CaO2H2_sg164_CalciumHydroxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/CaO_sg225_CalciumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/CaSiO3_sg2_Wollastonite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Ca_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Ca_sg229_Calcium-gamma.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/CeO2_sg225_CeriumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Cr_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Cu2O_sg224_Cuprite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Cu_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Dy2O3_sg206_DysprosiumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Epoxy_Araldite506_C18H20O3.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Fe_sg225_Iron-gamma.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Fe_sg229_Iron-alpha.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/GaN_sg186_GalliumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/GaSe_sg194_GalliumSelenide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Ge3Bi4O12_sg220_BismuthGermanate.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Ge_sg227.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/He_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/HfO2_sg14_HafniumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Ho2O3_sg206_HolmiumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/KBr_sg225_PotassiumBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/KF_sg225_PotassiumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/KOH_sg4_PotassiumHydroxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/K_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Kapton_C22H10N2O5.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Kr_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/LaBr3_sg176_LanthanumBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Li2O_sg225_LithiumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Li3N_sg191_LithiumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/LiF_sg225_LithiumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/LiH_sg225_LithiumHydride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)  1560968 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/LiquidHeavyWaterD2O_T293.6K.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)   528493 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/LiquidWaterH2O_T293.6K.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Lu2O3_sg206_LutetiumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Lu2SiO5_sg15.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Mg2SiO4_sg62_MagnesiumSilicate.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/MgAl2O4_sg227_MAS.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/MgCO3_sg167_MagnesiumCarbonate.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/MgD2_sg136_MagnesiumDeuteride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/MgF2_sg136_MagnesiumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/MgH2_sg136_MagnesiumHydride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/MgO2H2_sg164_MagnesiumHydroxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/MgO_sg225_Periclase.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Mg_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Mo_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Na4Si3Al3O12Cl_sg218_Sodalite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/NaBr_sg225_SodiumBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/NaCl_sg225_SodiumChloride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/NaF_sg225_SodiumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/NaI_sg225_SodiumIodide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Na_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Nb_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Ne_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Ni_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Nylon11_C11H21NO.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Nylon12_C12H23NO.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Nylon610_C16H30N2O2.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Nylon66or6_C12H22N2O2.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/PEEK_C19H12O3.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/PVC_C2H3Cl.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/PbF2-beta_sg225_BetaLeadFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/PbO-alpha_sg129_Litharge.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/PbO-beta_sg57_Massicot.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/PbS_sg225_LeadSulfide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Pb_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Pd_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Polycarbonate_C16O3H14.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Polyester_C10H8O4.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Polyethylene_CH2.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Polylactide_C3H4O2.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Polypropylene_C3H6.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Polystyrene_C8H8.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Pt_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Rb_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Rubber_C5H8.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Sc_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/SiC-beta_sg216_BetaSiliconCarbide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/SiO2-alpha_sg154_AlphaQuartz.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/SiO2-beta_sg180_BetaQuartz.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Si_sg227.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Sn_sg141.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/SrF2_sg225_StrontiumFluoride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/SrH2_sg62_StrontiumHydride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Sr_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Th3N4_sg166_ThoriumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/ThO2_sg225_ThoriumDioxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Th_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/TiO2_sg136_Rutile.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/TiO2_sg141_Anatase.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Ti_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/TlBr_sg221_ThaliumBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Tm2O3_sg206_ThuliumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/UF6_sg62_UraniumHexaflouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/UO2_sg225_UraniumDioxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/V_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/W_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Xe_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Y2O3_sg206_Yttrium_Oxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Y2SiO5_sg15_YSO.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Y3Al5O12_sg230_YAG.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Y_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/ZnF2_sg136_ZincFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/ZnO_sg186_ZincOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/ZnS_sg216_Sphalerite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Zn_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/ZrF4-beta_sg84.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/ZrO2_sg137_Zirconia.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/ZrO2_sg14_Zirconia.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/Zr_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-30 07:24:54.000000 ncrystal-3.8.2/data/void.ncmat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.336909 ncrystal-3.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    39216 2024-04-30 07:24:54.000000 ncrystal-3.8.2/docs/ncmat_doc.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.336909 ncrystal-3.8.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-30 07:24:54.000000 ncrystal-3.8.2/examples/ncrystal_example_c.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-30 07:24:54.000000 ncrystal-3.8.2/examples/ncrystal_example_cpp.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-04-30 07:24:54.000000 ncrystal-3.8.2/examples/ncrystal_example_customphysics.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-30 07:24:54.000000 ncrystal-3.8.2/examples/ncrystal_example_g4sim.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-30 07:24:54.000000 ncrystal-3.8.2/examples/ncrystal_example_py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.376909 ncrystal-3.8.2/ncrystal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-30 07:25:03.000000 ncrystal-3.8.2/ncrystal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14377 2024-04-30 07:25:03.000000 ncrystal-3.8.2/ncrystal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:25:03.000000 ncrystal-3.8.2/ncrystal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 07:25:03.000000 ncrystal-3.8.2/ncrystal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 07:25:03.000000 ncrystal-3.8.2/ncrystal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.304909 ncrystal-3.8.2/ncrystal_core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.304909 ncrystal-3.8.2/ncrystal_core/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.340909 ncrystal-3.8.2/ncrystal_core/include/NCrystal/
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCAtomData.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCCompositionUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCDataSources.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    51910 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCDefs.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCDump.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCException.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCFact.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCFactImpl.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCFactRequests.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCFactTypes.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCFmt.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    16617 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCImmutBuf.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCInfo.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCInfoBuilder.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    16865 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCInfoTypes.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCLoadNCMAT.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    22393 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCMatCfg.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    20453 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCMem.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCNCMATData.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCParseNCMAT.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCPluginBoilerplate.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCPluginMgmt.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCProc.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    20032 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCProcImpl.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCRNG.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCSABData.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCSCOrientation.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    39167 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCSmallVector.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCTextData.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    37506 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCTypes.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCVariant.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCVersion.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCrystal.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.352909 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCAbsOOV.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCAtomDB.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCAtomDBExtender.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCAtomUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCBkgdExtCurve.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    23040 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCCfgManip.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    32382 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCCfgTypes.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    35739 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCCfgVars.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCDebyeMSD.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCDynInfoUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCDynLoader.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCElIncScatter.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCElIncXS.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCEqRefl.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    20006 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCFactoryUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCFastConvolve.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCFileUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCFillHKL.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCFreeGas.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCFreeGasUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCGasMixUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCGaussMos.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCGaussOnSphere.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCIofQHelper.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCIter.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCKinUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCLCBragg.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCLCRefModels.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCLCUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCLatticeUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    27329 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCMath.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCMatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCOrientUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCPCBragg.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCPlaneProvider.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCPointwiseDist.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCRandUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCRomberg.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCRotMatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    18031 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABEval.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABExtender.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABFactory.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABIntegrator.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABSampler.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABSamplerModels.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABScatter.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABScatterHelper.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABUCN.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    14775 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABXSProvider.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSANSSphScat.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSANSUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSCBragg.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCScatKnlData.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSpan.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSpline.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    20133 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCStrView.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    15446 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCString.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCVDOSEval.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCVDOSGn.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCVDOSToScatKnl.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCVector.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/ncapi.h
+-rw-r--r--   0 runner    (1001) docker     (127)    68354 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/include/NCrystal/ncrystal.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.372909 ncrystal-3.8.2/ncrystal_core/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCAbsOOV.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    36781 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCAtomDB.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9819 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCAtomDBExtender.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCAtomData.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCAtomUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCBkgdExtCurve.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    18374 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCCfgManip.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCCfgTypes.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    17931 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCCfgVars.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCCompositionUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    26285 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCDataSources.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCDebyeMSD.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCDefs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCDump.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCDynInfoUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCDynLoader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCElIncScatter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCElIncXS.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCEqRefl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCException.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCFact.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    42918 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCFactImpl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCFactRequests.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCFactTypes.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCFactoryUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCFactory_NCMAT.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCFastConvolve.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCFileUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    30238 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCFillHKL.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCFmt.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCFreeGas.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    39981 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCFreeGasUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCGasMixFact.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    26609 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCGasMixUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCGaussMos.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCGaussOnSphere.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCInfo.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    57548 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCInfoBuilder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCIofQHelper.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCKinUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCLCBragg.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCLCRefModels.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    32342 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCLCUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    19529 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCLatticeUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCLauLazyFact.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    30611 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCLazy.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCLazy.hh
+-rw-r--r--   0 runner    (1001) docker     (127)    33292 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCLoadNCMAT.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    49031 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCMatCfg.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    23845 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCMath.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCMem.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    31787 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCNCMATData.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCOrientUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCPCBragg.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    42624 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCParseNCMAT.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCPlaneProvider.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCPluginMgmt.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCPointwiseDist.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCProc.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    20209 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCProcImpl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14897 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCQuickFact.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13331 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCRNG.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    20337 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCRandUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCRomberg.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCRotMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSABData.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    31895 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSABEval.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSABExtender.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSABFactory.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    23459 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSABIntegrator.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSABSampler.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSABSamplerModels.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSABScatter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    26316 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSABUCN.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    26756 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSABUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSABXSProvider.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSANSFact.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSANSSphScat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSANSUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13245 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSCBragg.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSCOrientation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCScatKnlData.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCSpline.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCStdAbsFact.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCStdMPScatFact.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCStdScatFact.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCStrView.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCString.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCTDProd.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCTextData.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCTypes.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    25956 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCVDOSEval.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCVDOSGn.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    38641 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCVDOSToScatKnl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCVector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/NCVersion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    72933 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_core/src/ncrystal.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.304909 ncrystal-3.8.2/ncrystal_geant4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.304909 ncrystal-3.8.2/ncrystal_geant4/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.372909 ncrystal-3.8.2/ncrystal_geant4/include/G4NCrystal/
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_geant4/include/G4NCrystal/G4NCInstall.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_geant4/include/G4NCrystal/G4NCManager.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_geant4/include/G4NCrystal/G4NCMatHelper.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_geant4/include/G4NCrystal/G4NCrystal.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.372909 ncrystal-3.8.2/ncrystal_geant4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_geant4/src/G4NCInstall.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_geant4/src/G4NCManager.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_geant4/src/G4NCMatHelper.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_geant4/src/G4NCProcWrapper.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-30 07:24:54.000000 ncrystal-3.8.2/ncrystal_geant4/src/G4NCProcWrapper.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-30 07:24:54.000000 ncrystal-3.8.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:25:03.376909 ncrystal-3.8.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15960 2024-04-30 07:24:54.000000 ncrystal-3.8.2/scripts/ncrystal_cif2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35171 2024-04-30 07:24:54.000000 ncrystal-3.8.2/scripts/ncrystal_endf2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (127)    73858 2024-04-30 07:24:54.000000 ncrystal-3.8.2/scripts/ncrystal_hfg2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1759 2024-04-30 07:24:54.000000 ncrystal-3.8.2/scripts/ncrystal_inspectfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15454 2024-04-30 07:24:54.000000 ncrystal-3.8.2/scripts/ncrystal_ncmat2cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7565 2024-04-30 07:24:54.000000 ncrystal-3.8.2/scripts/ncrystal_ncmat2hkl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1998 2024-04-30 07:24:54.000000 ncrystal-3.8.2/scripts/ncrystal_onlinedb2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20289 2024-04-30 07:24:54.000000 ncrystal-3.8.2/scripts/ncrystal_vdos2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13315 2024-04-30 07:24:54.000000 ncrystal-3.8.2/scripts/ncrystal_verifyatompos
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35942 2024-04-30 07:24:54.000000 ncrystal-3.8.2/scripts/nctool
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:25:03.376909 ncrystal-3.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-30 07:24:54.000000 ncrystal-3.8.2/setup.py
```

### Comparing `ncrystal-3.8.1/.github/ISSUE_TEMPLATE/feature_request.md` & `ncrystal-3.8.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/.github/ISSUE_TEMPLATE/request-for-new-material.md` & `ncrystal-3.8.2/.github/ISSUE_TEMPLATE/request-for-new-material.md`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/.github/workflows/basictest.yml` & `ncrystal-3.8.2/.github/workflows/basictest.yml`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/.github/workflows/condatest.yml` & `ncrystal-3.8.2/.github/workflows/condatest.yml`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/.github/workflows/pypi.yml` & `ncrystal-3.8.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/CHANGELOG` & `ncrystal-3.8.2/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v3.8.2 2024-04-30
+     * Add importlib_metadata as python build dependency for Python < 3.8.
+     * CMake code no longer strictly disallows mixing of NCRYSTAL_NAMESPACE and
+       NCRYSTAL_GEANT4 options.
+
 v3.8.1 2024-04-11
      * Fix rare FPE in lcbragg code (github issue #171).
      * Remove a few faulty noexcept modifiers in (found by cppcheck).
      * Fix NCMatCfg::textData which technically returned a reference to a
        temporary (although this is not believed to have actually caused any
        issues, since the "temporary" came from a longer-lived shared_ptr). This
        was also found with cppcheck.
```

### Comparing `ncrystal-3.8.1/CMakeLists.txt` & `ncrystal-3.8.2/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 list( APPEND _project_metadata DESCRIPTION "Library for thermal neutron transport in crystals and other materials" )
 if( "${CMAKE_VERSION}" VERSION_GREATER_EQUAL "3.12.0" )
   list( APPEND _project_metadata HOMEPAGE_URL "https://github.com/mctools/ncrystal" )
 endif()
 
 cmake_policy( SET CMP0048 NEW )#Not sure if this is really needed
 
-project( NCrystal VERSION 3.8.1 ${_project_metadata} )
+project( NCrystal VERSION 3.8.2 ${_project_metadata} )
 
 unset( _project_metadata )
 
 if( NOT NCRYSTAL_NOTOUCH_CMAKE_BUILD_TYPE )
   if ( NOT gen_is_multicfg )
     if ( NOT CMAKE_BUILD_TYPE )
       #This can happen if parent project called the project(..) function before
@@ -766,34 +766,37 @@
   endif()
 
 endif()
 
 #G4NCrystal
 set( NCRYSTAL_GEANT4 OFF )
 if ( NOT NCRYSTAL_ENABLE_GEANT4 STREQUAL "OFF" )
-  if ( NCRYSTAL_NAMESPACE )
-    #Since we didn't implement the namespace for the G4NCrystal c++ namespace as
-    #well, it is best to error out here. Once we have migrated to new and better
-    #(and standalone) NCrystal-Geant4 hooks, they should certainly also have an
-    #option for namespace protection.
-    message( FATAL_ERROR "It is not currently supported to use NCRYSTAL_NAMESPACE without NCRYSTAL_GEANT4=OFF (please get in touch if you have a different need)" )
-  endif()
   find_package(Geant4)
   if( Geant4_FOUND )
     set( NCRYSTAL_GEANT4 ON )
   else()
     if ( NOT NCRYSTAL_ENABLE_GEANT4 STREQUAL "IFAVAILABLE" )
       message( FATAL_ERROR "NCRYSTAL_ENABLE_GEANT4 set to ON but failed to enable Geant4 support (set to IFAVAILABLE or OFF to proceed without Geant4 support)." )
     endif()
   endif()
 endif()
 
 if ( NCRYSTAL_GEANT4 )
+  set( _tmp_basiclibnameg4 "G4NCrystal" )
   add_library(G4NCrystal SHARED ${SRCS_NCG4})#NB: No SOVERSION number since we plan to migrate this library out of the NCrystal repo.
-  set(G4NCrystal_LIBNAME "${CMAKE_SHARED_LIBRARY_PREFIX}G4NCrystal${CMAKE_SHARED_LIBRARY_SUFFIX}")
+  if ( NCRYSTAL_NAMESPACE )
+    #Since we didn't implement the namespace for the G4NCrystal C++ namespace as
+    #well, it is best to error out here. Once we have migrated to new and better
+    #(and standalone) NCrystal-Geant4 hooks, they should certainly also have an
+    #option for namespace protection there.
+    message( WARNING "The NCRYSTAL_NAMESPACE feature is not actually fully implemented for the NCRYSTAL_GEANT4 extension (please get in touch if you have a different need)" )
+    set( _tmp_basiclibnameg4 "${_tmp_basiclibnameg4}-${NCRYSTAL_NAMESPACE}" )
+    set_target_properties( G4NCrystal PROPERTIES OUTPUT_NAME "${_tmp_basiclibnameg4}" )
+  endif()
+  set(G4NCrystal_LIBNAME "${CMAKE_SHARED_LIBRARY_PREFIX}${_tmp_basiclibnameg4}${CMAKE_SHARED_LIBRARY_SUFFIX}")
   #Make sure client code will use at least c++11:
   target_compile_features( G4NCrystal INTERFACE cxx_std_11 )
   set_target_common_props( G4NCrystal )
   target_include_directories(G4NCrystal
     PUBLIC
     $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/ncrystal_geant4/include>
     $<INSTALL_INTERFACE:${NCrystal_INCDIR}>
```

### Comparing `ncrystal-3.8.1/FILES` & `ncrystal-3.8.2/FILES`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/INSTALL` & `ncrystal-3.8.2/INSTALL`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/LICENSE` & `ncrystal-3.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/__init__.py` & `ncrystal-3.8.2/NCrystal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 ##  See the License for the specific language governing permissions and       ##
 ##  limitations under the License.                                            ##
 ##                                                                            ##
 ################################################################################
 
 #NB: Synchronize meta-data below with fields in setup.py+template_setup.py.in meta data:
 __license__ = "Apache 2.0, http://www.apache.org/licenses/LICENSE-2.0"
-__version__ = '3.8.1'
+__version__ = '3.8.2'
 __status__ = "Production"
 __author__ = "NCrystal developers (Thomas Kittelmann, Xiao Xiao Cai)"
 __copyright__ = "Copyright 2015-2023 %s"%__author__
 __maintainer__ = __author__
 __email__ = "ncrystal-developers@cern.ch"
 
 #Place f-string here to catch python <3.6 in a more obvious way than a syntax error below:
```

### Comparing `ncrystal-3.8.1/NCrystal/_chooks.py` & `ncrystal-3.8.2/NCrystal/_chooks.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/_common.py` & `ncrystal-3.8.2/NCrystal/_common.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/_coreimpl.py` & `ncrystal-3.8.2/NCrystal/_coreimpl.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/_miscimpl.py` & `ncrystal-3.8.2/NCrystal/_miscimpl.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/_ncmatimpl.py` & `ncrystal-3.8.2/NCrystal/_ncmatimpl.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/_numpy.py` & `ncrystal-3.8.2/NCrystal/_numpy.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/_testimpl.py` & `ncrystal-3.8.2/NCrystal/_testimpl.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/api.py` & `ncrystal-3.8.2/NCrystal/api.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/atomdata.py` & `ncrystal-3.8.2/NCrystal/atomdata.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/cfgstr.py` & `ncrystal-3.8.2/NCrystal/cfgstr.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/cifutils.py` & `ncrystal-3.8.2/NCrystal/cifutils.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/constants.py` & `ncrystal-3.8.2/NCrystal/constants.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/core.py` & `ncrystal-3.8.2/NCrystal/core.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/datasrc.py` & `ncrystal-3.8.2/NCrystal/datasrc.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/exceptions.py` & `ncrystal-3.8.2/NCrystal/exceptions.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/mcstasutils.py` & `ncrystal-3.8.2/NCrystal/mcstasutils.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/misc.py` & `ncrystal-3.8.2/NCrystal/misc.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/ncmat.py` & `ncrystal-3.8.2/NCrystal/ncmat.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/obsolete.py` & `ncrystal-3.8.2/NCrystal/obsolete.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/plot.py` & `ncrystal-3.8.2/NCrystal/plot.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/plugins.py` & `ncrystal-3.8.2/NCrystal/plugins.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/test.py` & `ncrystal-3.8.2/NCrystal/test.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NCrystal/vdos.py` & `ncrystal-3.8.2/NCrystal/vdos.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/NOTICE` & `ncrystal-3.8.2/NOTICE`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/PKG-INFO` & `ncrystal-3.8.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncrystal
-Version: 3.8.1
+Version: 3.8.2
 Summary: Library for thermal neutron transport in crystals and other materials.
 Home-page: https://github.com/mctools/ncrystal/wiki
 Author: NCrystal developers (Thomas Kittelmann, Xiao Xiao Cai)
 License: Apache-2.0
 Keywords: neutron,montecarlo,science
 Requires-Python: >=3.6, <4
 License-File: LICENSE
```

### Comparing `ncrystal-3.8.1/README` & `ncrystal-3.8.2/README`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/cmake/NCrystalConfig.cmake.in` & `ncrystal-3.8.2/cmake/NCrystalConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/cmake/modules/ncrystal_legacyoptions.cmake` & `ncrystal-3.8.2/cmake/modules/ncrystal_legacyoptions.cmake`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/cmake/modules/ncrystal_options.cmake` & `ncrystal-3.8.2/cmake/modules/ncrystal_options.cmake`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/cmake/modules/ncrystal_utils.cmake` & `ncrystal-3.8.2/cmake/modules/ncrystal_utils.cmake`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/cmake/ncrystal-config.in` & `ncrystal-3.8.2/cmake/ncrystal-config.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/cmake/template_setup.py.in` & `ncrystal-3.8.2/cmake/template_setup.py.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/cmake/template_setup.sh.in` & `ncrystal-3.8.2/cmake/template_setup.sh.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/cmake/template_unsetup.sh.in` & `ncrystal-3.8.2/cmake/template_unsetup.sh.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/AcrylicGlass_C5O2H8.ncmat` & `ncrystal-3.8.2/data/AcrylicGlass_C5O2H8.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/AgBr_sg225_SilverBromide.ncmat` & `ncrystal-3.8.2/data/AgBr_sg225_SilverBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Ag_sg225.ncmat` & `ncrystal-3.8.2/data/Ag_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Al2O3_sg167_Corundum.ncmat` & `ncrystal-3.8.2/data/Al2O3_sg167_Corundum.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Al4C3_sg166_AluminiumCarbide.ncmat` & `ncrystal-3.8.2/data/Al4C3_sg166_AluminiumCarbide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/AlN_sg186_AluminumNitride.ncmat` & `ncrystal-3.8.2/data/AlN_sg186_AluminumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Al_sg225.ncmat` & `ncrystal-3.8.2/data/Al_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Ar_Gas_STP.ncmat` & `ncrystal-3.8.2/data/Ar_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Au_sg225.ncmat` & `ncrystal-3.8.2/data/Au_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/BaF2_sg225_BariumFluoride.ncmat` & `ncrystal-3.8.2/data/BaF2_sg225_BariumFluoride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/BaO_sg225_BariumOxide.ncmat` & `ncrystal-3.8.2/data/BaO_sg225_BariumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Ba_sg229.ncmat` & `ncrystal-3.8.2/data/Ba_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Be3N2_sg206_BerylliumNitride.ncmat` & `ncrystal-3.8.2/data/Be3N2_sg206_BerylliumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/BeF2_sg152_Beryllium_Fluoride.ncmat` & `ncrystal-3.8.2/data/BeF2_sg152_Beryllium_Fluoride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/BeO_sg186.ncmat` & `ncrystal-3.8.2/data/BeO_sg186.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Be_sg194.ncmat` & `ncrystal-3.8.2/data/Be_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Bi_sg166.ncmat` & `ncrystal-3.8.2/data/Bi_sg166.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/C_sg194_pyrolytic_graphite.ncmat` & `ncrystal-3.8.2/data/C_sg194_pyrolytic_graphite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/C_sg227_Diamond.ncmat` & `ncrystal-3.8.2/data/C_sg227_Diamond.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/CaCO3_sg62_Aragonite.ncmat` & `ncrystal-3.8.2/data/CaCO3_sg62_Aragonite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/CaF2_sg225_CalciumFlouride.ncmat` & `ncrystal-3.8.2/data/CaF2_sg225_CalciumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/CaH2_sg62_CalciumHydride.ncmat` & `ncrystal-3.8.2/data/CaH2_sg62_CalciumHydride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/CaO2H2_sg164_CalciumHydroxide.ncmat` & `ncrystal-3.8.2/data/CaO2H2_sg164_CalciumHydroxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/CaO_sg225_CalciumOxide.ncmat` & `ncrystal-3.8.2/data/CaO_sg225_CalciumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/CaSiO3_sg2_Wollastonite.ncmat` & `ncrystal-3.8.2/data/CaSiO3_sg2_Wollastonite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Ca_sg225.ncmat` & `ncrystal-3.8.2/data/Ca_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Ca_sg229_Calcium-gamma.ncmat` & `ncrystal-3.8.2/data/Ca_sg229_Calcium-gamma.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/CeO2_sg225_CeriumOxide.ncmat` & `ncrystal-3.8.2/data/CeO2_sg225_CeriumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Cr_sg229.ncmat` & `ncrystal-3.8.2/data/Cr_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Cu2O_sg224_Cuprite.ncmat` & `ncrystal-3.8.2/data/Cu2O_sg224_Cuprite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Cu_sg225.ncmat` & `ncrystal-3.8.2/data/Cu_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Dy2O3_sg206_DysprosiumOxide.ncmat` & `ncrystal-3.8.2/data/Dy2O3_sg206_DysprosiumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Epoxy_Araldite506_C18H20O3.ncmat` & `ncrystal-3.8.2/data/Epoxy_Araldite506_C18H20O3.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Fe_sg225_Iron-gamma.ncmat` & `ncrystal-3.8.2/data/Fe_sg225_Iron-gamma.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Fe_sg229_Iron-alpha.ncmat` & `ncrystal-3.8.2/data/Fe_sg229_Iron-alpha.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/GaN_sg186_GalliumNitride.ncmat` & `ncrystal-3.8.2/data/GaN_sg186_GalliumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/GaSe_sg194_GalliumSelenide.ncmat` & `ncrystal-3.8.2/data/GaSe_sg194_GalliumSelenide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Ge3Bi4O12_sg220_BismuthGermanate.ncmat` & `ncrystal-3.8.2/data/Ge3Bi4O12_sg220_BismuthGermanate.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Ge_sg227.ncmat` & `ncrystal-3.8.2/data/Ge_sg227.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/He_Gas_STP.ncmat` & `ncrystal-3.8.2/data/He_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/HfO2_sg14_HafniumOxide.ncmat` & `ncrystal-3.8.2/data/HfO2_sg14_HafniumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Ho2O3_sg206_HolmiumOxide.ncmat` & `ncrystal-3.8.2/data/Ho2O3_sg206_HolmiumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/KBr_sg225_PotassiumBromide.ncmat` & `ncrystal-3.8.2/data/KBr_sg225_PotassiumBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/KF_sg225_PotassiumFlouride.ncmat` & `ncrystal-3.8.2/data/KF_sg225_PotassiumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/KOH_sg4_PotassiumHydroxide.ncmat` & `ncrystal-3.8.2/data/KOH_sg4_PotassiumHydroxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/K_sg229.ncmat` & `ncrystal-3.8.2/data/K_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Kapton_C22H10N2O5.ncmat` & `ncrystal-3.8.2/data/Kapton_C22H10N2O5.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Kr_Gas_STP.ncmat` & `ncrystal-3.8.2/data/Kr_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/LaBr3_sg176_LanthanumBromide.ncmat` & `ncrystal-3.8.2/data/LaBr3_sg176_LanthanumBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Li2O_sg225_LithiumOxide.ncmat` & `ncrystal-3.8.2/data/Li2O_sg225_LithiumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Li3N_sg191_LithiumNitride.ncmat` & `ncrystal-3.8.2/data/Li3N_sg191_LithiumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/LiF_sg225_LithiumFlouride.ncmat` & `ncrystal-3.8.2/data/LiF_sg225_LithiumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/LiH_sg225_LithiumHydride.ncmat` & `ncrystal-3.8.2/data/LiH_sg225_LithiumHydride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/LiquidHeavyWaterD2O_T293.6K.ncmat` & `ncrystal-3.8.2/data/LiquidHeavyWaterD2O_T293.6K.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/LiquidWaterH2O_T293.6K.ncmat` & `ncrystal-3.8.2/data/LiquidWaterH2O_T293.6K.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Lu2O3_sg206_LutetiumOxide.ncmat` & `ncrystal-3.8.2/data/Lu2O3_sg206_LutetiumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Lu2SiO5_sg15.ncmat` & `ncrystal-3.8.2/data/Lu2SiO5_sg15.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Mg2SiO4_sg62_MagnesiumSilicate.ncmat` & `ncrystal-3.8.2/data/Mg2SiO4_sg62_MagnesiumSilicate.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/MgAl2O4_sg227_MAS.ncmat` & `ncrystal-3.8.2/data/MgAl2O4_sg227_MAS.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/MgCO3_sg167_MagnesiumCarbonate.ncmat` & `ncrystal-3.8.2/data/MgCO3_sg167_MagnesiumCarbonate.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/MgD2_sg136_MagnesiumDeuteride.ncmat` & `ncrystal-3.8.2/data/MgD2_sg136_MagnesiumDeuteride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/MgF2_sg136_MagnesiumFlouride.ncmat` & `ncrystal-3.8.2/data/MgF2_sg136_MagnesiumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/MgH2_sg136_MagnesiumHydride.ncmat` & `ncrystal-3.8.2/data/MgH2_sg136_MagnesiumHydride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/MgO2H2_sg164_MagnesiumHydroxide.ncmat` & `ncrystal-3.8.2/data/MgO2H2_sg164_MagnesiumHydroxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/MgO_sg225_Periclase.ncmat` & `ncrystal-3.8.2/data/MgO_sg225_Periclase.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Mg_sg194.ncmat` & `ncrystal-3.8.2/data/Mg_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Mo_sg229.ncmat` & `ncrystal-3.8.2/data/Mo_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Na4Si3Al3O12Cl_sg218_Sodalite.ncmat` & `ncrystal-3.8.2/data/Na4Si3Al3O12Cl_sg218_Sodalite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/NaBr_sg225_SodiumBromide.ncmat` & `ncrystal-3.8.2/data/NaBr_sg225_SodiumBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/NaCl_sg225_SodiumChloride.ncmat` & `ncrystal-3.8.2/data/NaCl_sg225_SodiumChloride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/NaF_sg225_SodiumFlouride.ncmat` & `ncrystal-3.8.2/data/NaF_sg225_SodiumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/NaI_sg225_SodiumIodide.ncmat` & `ncrystal-3.8.2/data/NaI_sg225_SodiumIodide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Na_sg229.ncmat` & `ncrystal-3.8.2/data/Na_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Nb_sg229.ncmat` & `ncrystal-3.8.2/data/Nb_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Ne_Gas_STP.ncmat` & `ncrystal-3.8.2/data/Ne_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Ni_sg225.ncmat` & `ncrystal-3.8.2/data/Ni_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Nylon11_C11H21NO.ncmat` & `ncrystal-3.8.2/data/Nylon11_C11H21NO.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Nylon12_C12H23NO.ncmat` & `ncrystal-3.8.2/data/Nylon12_C12H23NO.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Nylon610_C16H30N2O2.ncmat` & `ncrystal-3.8.2/data/Nylon610_C16H30N2O2.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Nylon66or6_C12H22N2O2.ncmat` & `ncrystal-3.8.2/data/Nylon66or6_C12H22N2O2.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/PEEK_C19H12O3.ncmat` & `ncrystal-3.8.2/data/PEEK_C19H12O3.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/PVC_C2H3Cl.ncmat` & `ncrystal-3.8.2/data/PVC_C2H3Cl.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/PbF2-beta_sg225_BetaLeadFlouride.ncmat` & `ncrystal-3.8.2/data/PbF2-beta_sg225_BetaLeadFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/PbO-alpha_sg129_Litharge.ncmat` & `ncrystal-3.8.2/data/PbO-alpha_sg129_Litharge.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/PbO-beta_sg57_Massicot.ncmat` & `ncrystal-3.8.2/data/PbO-beta_sg57_Massicot.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/PbS_sg225_LeadSulfide.ncmat` & `ncrystal-3.8.2/data/PbS_sg225_LeadSulfide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Pb_sg225.ncmat` & `ncrystal-3.8.2/data/Pb_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Pd_sg225.ncmat` & `ncrystal-3.8.2/data/Pd_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Polycarbonate_C16O3H14.ncmat` & `ncrystal-3.8.2/data/Polycarbonate_C16O3H14.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Polyester_C10H8O4.ncmat` & `ncrystal-3.8.2/data/Polyester_C10H8O4.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Polyethylene_CH2.ncmat` & `ncrystal-3.8.2/data/Polyethylene_CH2.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Polylactide_C3H4O2.ncmat` & `ncrystal-3.8.2/data/Polylactide_C3H4O2.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Polypropylene_C3H6.ncmat` & `ncrystal-3.8.2/data/Polypropylene_C3H6.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Polystyrene_C8H8.ncmat` & `ncrystal-3.8.2/data/Polystyrene_C8H8.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Pt_sg225.ncmat` & `ncrystal-3.8.2/data/Pt_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Rb_sg229.ncmat` & `ncrystal-3.8.2/data/Rb_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Rubber_C5H8.ncmat` & `ncrystal-3.8.2/data/Rubber_C5H8.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Sc_sg194.ncmat` & `ncrystal-3.8.2/data/Sc_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/SiC-beta_sg216_BetaSiliconCarbide.ncmat` & `ncrystal-3.8.2/data/SiC-beta_sg216_BetaSiliconCarbide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/SiO2-alpha_sg154_AlphaQuartz.ncmat` & `ncrystal-3.8.2/data/SiO2-alpha_sg154_AlphaQuartz.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/SiO2-beta_sg180_BetaQuartz.ncmat` & `ncrystal-3.8.2/data/SiO2-beta_sg180_BetaQuartz.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Si_sg227.ncmat` & `ncrystal-3.8.2/data/Si_sg227.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Sn_sg141.ncmat` & `ncrystal-3.8.2/data/Sn_sg141.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/SrF2_sg225_StrontiumFluoride.ncmat` & `ncrystal-3.8.2/data/SrF2_sg225_StrontiumFluoride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/SrH2_sg62_StrontiumHydride.ncmat` & `ncrystal-3.8.2/data/SrH2_sg62_StrontiumHydride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Sr_sg225.ncmat` & `ncrystal-3.8.2/data/Sr_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Th3N4_sg166_ThoriumNitride.ncmat` & `ncrystal-3.8.2/data/Th3N4_sg166_ThoriumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/ThO2_sg225_ThoriumDioxide.ncmat` & `ncrystal-3.8.2/data/ThO2_sg225_ThoriumDioxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Th_sg225.ncmat` & `ncrystal-3.8.2/data/Th_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/TiO2_sg136_Rutile.ncmat` & `ncrystal-3.8.2/data/TiO2_sg136_Rutile.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/TiO2_sg141_Anatase.ncmat` & `ncrystal-3.8.2/data/TiO2_sg141_Anatase.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Ti_sg194.ncmat` & `ncrystal-3.8.2/data/Ti_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/TlBr_sg221_ThaliumBromide.ncmat` & `ncrystal-3.8.2/data/TlBr_sg221_ThaliumBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Tm2O3_sg206_ThuliumOxide.ncmat` & `ncrystal-3.8.2/data/Tm2O3_sg206_ThuliumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/UF6_sg62_UraniumHexaflouride.ncmat` & `ncrystal-3.8.2/data/UF6_sg62_UraniumHexaflouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/UO2_sg225_UraniumDioxide.ncmat` & `ncrystal-3.8.2/data/UO2_sg225_UraniumDioxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/V_sg229.ncmat` & `ncrystal-3.8.2/data/V_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/W_sg229.ncmat` & `ncrystal-3.8.2/data/W_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Xe_Gas_STP.ncmat` & `ncrystal-3.8.2/data/Xe_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Y2O3_sg206_Yttrium_Oxide.ncmat` & `ncrystal-3.8.2/data/Y2O3_sg206_Yttrium_Oxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Y2SiO5_sg15_YSO.ncmat` & `ncrystal-3.8.2/data/Y2SiO5_sg15_YSO.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Y3Al5O12_sg230_YAG.ncmat` & `ncrystal-3.8.2/data/Y3Al5O12_sg230_YAG.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Y_sg194.ncmat` & `ncrystal-3.8.2/data/Y_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/ZnF2_sg136_ZincFlouride.ncmat` & `ncrystal-3.8.2/data/ZnF2_sg136_ZincFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/ZnO_sg186_ZincOxide.ncmat` & `ncrystal-3.8.2/data/ZnO_sg186_ZincOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/ZnS_sg216_Sphalerite.ncmat` & `ncrystal-3.8.2/data/ZnS_sg216_Sphalerite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Zn_sg194.ncmat` & `ncrystal-3.8.2/data/Zn_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/ZrF4-beta_sg84.ncmat` & `ncrystal-3.8.2/data/ZrF4-beta_sg84.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/ZrO2_sg137_Zirconia.ncmat` & `ncrystal-3.8.2/data/ZrO2_sg137_Zirconia.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/ZrO2_sg14_Zirconia.ncmat` & `ncrystal-3.8.2/data/ZrO2_sg14_Zirconia.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/Zr_sg194.ncmat` & `ncrystal-3.8.2/data/Zr_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/data/void.ncmat` & `ncrystal-3.8.2/data/void.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/docs/ncmat_doc.md` & `ncrystal-3.8.2/docs/ncmat_doc.md`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/examples/ncrystal_example_c.c` & `ncrystal-3.8.2/examples/ncrystal_example_c.c`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/examples/ncrystal_example_cpp.cc` & `ncrystal-3.8.2/examples/ncrystal_example_cpp.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/examples/ncrystal_example_customphysics.cc` & `ncrystal-3.8.2/examples/ncrystal_example_customphysics.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/examples/ncrystal_example_g4sim.cc` & `ncrystal-3.8.2/examples/ncrystal_example_g4sim.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/examples/ncrystal_example_py` & `ncrystal-3.8.2/examples/ncrystal_example_py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal.egg-info/PKG-INFO` & `ncrystal-3.8.2/ncrystal.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncrystal
-Version: 3.8.1
+Version: 3.8.2
 Summary: Library for thermal neutron transport in crystals and other materials.
 Home-page: https://github.com/mctools/ncrystal/wiki
 Author: NCrystal developers (Thomas Kittelmann, Xiao Xiao Cai)
 License: Apache-2.0
 Keywords: neutron,montecarlo,science
 Requires-Python: >=3.6, <4
 License-File: LICENSE
```

### Comparing `ncrystal-3.8.1/ncrystal.egg-info/SOURCES.txt` & `ncrystal-3.8.2/ncrystal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCAtomData.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCAtomData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCCompositionUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCCompositionUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCDataSources.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCDataSources.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCDefs.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCDefs.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCDump.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCDump.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCException.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCException.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCFact.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCFact.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCFactImpl.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCFactImpl.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCFactRequests.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCFactRequests.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCFactTypes.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCFactTypes.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCFmt.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCFmt.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCImmutBuf.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCImmutBuf.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCInfo.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCInfo.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCInfoBuilder.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCInfoBuilder.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCInfoTypes.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCInfoTypes.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCLoadNCMAT.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCLoadNCMAT.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCMatCfg.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCMatCfg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCMem.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCMem.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCNCMATData.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCNCMATData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCParseNCMAT.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCParseNCMAT.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCPluginBoilerplate.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCPluginBoilerplate.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCPluginMgmt.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCPluginMgmt.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCProc.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCProc.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCProcImpl.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCProcImpl.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCRNG.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCRNG.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCSABData.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCSABData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCSCOrientation.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCSCOrientation.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCSmallVector.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCSmallVector.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCTextData.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCTextData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCTypes.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCTypes.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCVariant.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCVariant.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCVersion.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCVersion.hh`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,17 @@
 #endif
 #ifdef NCRYSTAL_VERSION_STR
 #  undef NCRYSTAL_VERSION_STR
 #endif
 
 #define NCRYSTAL_VERSION_MAJOR 3
 #define NCRYSTAL_VERSION_MINOR 8
-#define NCRYSTAL_VERSION_PATCH 1
-#define NCRYSTAL_VERSION   3008001 /* (1000000*MAJOR+1000*MINOR+PATCH)   */
-#define NCRYSTAL_VERSION_STR "3.8.1"
+#define NCRYSTAL_VERSION_PATCH 2
+#define NCRYSTAL_VERSION   3008002 /* (1000000*MAJOR+1000*MINOR+PATCH)   */
+#define NCRYSTAL_VERSION_STR "3.8.2"
 
 #include "NCrystal/ncapi.h"
 #include <stdexcept>
 
 namespace NCRYSTAL_NAMESPACE {
 
   //Function which returns NCRYSTAL_VERSION. If it does not, it indicates symbol
```

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/NCrystal.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/NCrystal.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCAbsOOV.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCAbsOOV.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCAtomDB.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCAtomDB.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCAtomDBExtender.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCAtomDBExtender.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCAtomUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCAtomUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCBkgdExtCurve.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCBkgdExtCurve.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCCfgManip.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCCfgManip.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCCfgTypes.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCCfgTypes.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCCfgVars.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCCfgVars.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCDebyeMSD.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCDebyeMSD.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCDynInfoUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCDynInfoUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCDynLoader.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCDynLoader.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCElIncScatter.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCElIncScatter.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCElIncXS.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCElIncXS.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCEqRefl.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCEqRefl.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCFactoryUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCFactoryUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCFastConvolve.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCFastConvolve.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCFileUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCFileUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCFillHKL.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCFillHKL.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCFreeGas.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCFreeGas.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCFreeGasUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCFreeGasUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCGasMixUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCGasMixUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCGaussMos.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCGaussMos.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCGaussOnSphere.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCGaussOnSphere.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCIofQHelper.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCIofQHelper.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCIter.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCIter.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCKinUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCKinUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCLCBragg.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCLCBragg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCLCRefModels.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCLCRefModels.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCLCUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCLCUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCLatticeUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCLatticeUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCMath.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCMath.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCMatrix.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCMatrix.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCOrientUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCOrientUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCPCBragg.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCPCBragg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCPlaneProvider.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCPlaneProvider.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCPointwiseDist.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCPointwiseDist.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCRandUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCRandUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCRomberg.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCRomberg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCRotMatrix.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCRotMatrix.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABEval.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABEval.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABExtender.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABExtender.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABFactory.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABFactory.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABIntegrator.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABIntegrator.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABSampler.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABSampler.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABSamplerModels.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABSamplerModels.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABScatter.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABScatter.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABScatterHelper.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABScatterHelper.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABUCN.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABUCN.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSABXSProvider.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSABXSProvider.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSANSSphScat.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSANSSphScat.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSANSUtils.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSANSUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSCBragg.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSCBragg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCScatKnlData.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCScatKnlData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSpan.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSpan.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCSpline.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCSpline.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCStrView.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCStrView.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCString.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCString.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCVDOSEval.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCVDOSEval.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCVDOSGn.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCVDOSGn.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCVDOSToScatKnl.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCVDOSToScatKnl.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/internal/NCVector.hh` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/internal/NCVector.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/ncapi.h` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/ncapi.h`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/include/NCrystal/ncrystal.h` & `ncrystal-3.8.2/ncrystal_core/include/NCrystal/ncrystal.h`

 * *Files 0% similar despite different names*

```diff
@@ -1160,17 +1160,17 @@
 #  undef NCRYSTAL_VERSION
 #endif
 #ifdef NCRYSTAL_VERSION_STR
 #  undef NCRYSTAL_VERSION_STR
 #endif
 #define NCRYSTAL_VERSION_MAJOR 3
 #define NCRYSTAL_VERSION_MINOR 8
-#define NCRYSTAL_VERSION_PATCH 1
-#define NCRYSTAL_VERSION   3008001 /* (1000000*MAJOR+1000*MINOR+PATCH)             */
-#define NCRYSTAL_VERSION_STR "3.8.1"
+#define NCRYSTAL_VERSION_PATCH 2
+#define NCRYSTAL_VERSION   3008002 /* (1000000*MAJOR+1000*MINOR+PATCH)             */
+#define NCRYSTAL_VERSION_STR "3.8.2"
   NCRYSTAL_API int ncrystal_version(void); /* returns NCRYSTAL_VERSION                  */
   NCRYSTAL_API const char * ncrystal_version_str(void); /* returns NCRYSTAL_VERSION_STR */
 
   /* If compiled with NCRYSTAL_NAMESPACE_PROTECTION, return the namespace here:    */
   /* (will be an empty string in default installations):                           */
   NCRYSTAL_API const char * ncrystal_namespace(void);
```

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCAbsOOV.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCAbsOOV.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCAtomDB.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCAtomDB.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCAtomDBExtender.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCAtomDBExtender.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCAtomData.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCAtomData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCAtomUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCAtomUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCBkgdExtCurve.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCBkgdExtCurve.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCCfgManip.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCCfgManip.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCCfgTypes.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCCfgTypes.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCCfgVars.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCCfgVars.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCCompositionUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCCompositionUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCDataSources.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCDataSources.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCDebyeMSD.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCDebyeMSD.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCDefs.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCDefs.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCDump.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCDump.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCDynInfoUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCDynInfoUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCDynLoader.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCDynLoader.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCElIncScatter.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCElIncScatter.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCElIncXS.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCElIncXS.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCEqRefl.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCEqRefl.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCException.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCException.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCFact.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCFactImpl.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCFactImpl.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCFactRequests.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCFactRequests.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCFactTypes.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCFactTypes.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCFactoryUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCFactoryUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCFactory_NCMAT.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCFactory_NCMAT.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCFastConvolve.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCFastConvolve.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCFileUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCFileUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCFillHKL.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCFillHKL.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCFmt.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCFmt.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCFreeGas.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCFreeGas.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCFreeGasUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCFreeGasUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCGasMixFact.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCGasMixFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCGasMixUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCGasMixUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCGaussMos.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCGaussMos.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCGaussOnSphere.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCGaussOnSphere.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCInfo.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCInfo.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCInfoBuilder.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCInfoBuilder.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCIofQHelper.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCIofQHelper.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCKinUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCKinUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCLCBragg.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCLCBragg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCLCRefModels.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCLCRefModels.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCLCUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCLCUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCLatticeUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCLatticeUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCLauLazyFact.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCLauLazyFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCLazy.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCLazy.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCLazy.hh` & `ncrystal-3.8.2/ncrystal_core/src/NCLazy.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCLoadNCMAT.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCLoadNCMAT.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCMatCfg.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCMatCfg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCMath.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCMath.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCMatrix.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCMatrix.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCMem.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCMem.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCNCMATData.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCNCMATData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCOrientUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCOrientUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCPCBragg.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCPCBragg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCParseNCMAT.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCParseNCMAT.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCPlaneProvider.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCPlaneProvider.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCPluginMgmt.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCPluginMgmt.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCPointwiseDist.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCPointwiseDist.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCProc.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCProc.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCProcImpl.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCProcImpl.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCQuickFact.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCQuickFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCRNG.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCRNG.cc`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 
 void NC::setDefaultRNGFctForAllThreads( std::function<double()> fct )
 {
   setDefaultRNG(makeSO<RNG_OneFctForAllThreads>(fct));
 }
 
 namespace NCRYSTAL_NAMESPACE {
-  struct RNGProducer::Impl {
+  struct RNGProducer::Impl final {
     Impl( shared_obj<RNGStream> rng ) : m_nextproduct( std::move(rng) ) {}
     Impl( no_init_t ) {}
     optional_shared_obj<RNGStream> m_nextproduct;
     optional_shared_obj<RNGStream> m_nextnextproduct;
     std::map<RNGStreamIndex,optional_shared_obj<RNGStream>> m_idxdb;
     std::map<ThreadID,optional_shared_obj<RNGStream>> m_thread_idxdb;
     std::mutex m_mtx;
```

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCRandUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCRandUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCRomberg.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCRomberg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCRotMatrix.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCRotMatrix.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSABData.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSABData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSABEval.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSABEval.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSABExtender.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSABExtender.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSABFactory.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSABFactory.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSABIntegrator.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSABIntegrator.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSABSampler.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSABSampler.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSABSamplerModels.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSABSamplerModels.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSABScatter.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSABScatter.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSABUCN.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSABUCN.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSABUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSABUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSABXSProvider.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSABXSProvider.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSANSFact.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSANSFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSANSSphScat.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSANSSphScat.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSANSUtils.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSANSUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSCBragg.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSCBragg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSCOrientation.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSCOrientation.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCScatKnlData.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCScatKnlData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCSpline.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCSpline.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCStdAbsFact.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCStdAbsFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCStdMPScatFact.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCStdMPScatFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCStdScatFact.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCStdScatFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCStrView.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCStrView.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCString.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCString.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCTDProd.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCTDProd.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCTextData.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCTextData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCTypes.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCTypes.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCVDOSEval.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCVDOSEval.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCVDOSGn.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCVDOSGn.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCVDOSToScatKnl.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCVDOSToScatKnl.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCVector.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCVector.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/NCVersion.cc` & `ncrystal-3.8.2/ncrystal_core/src/NCVersion.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_core/src/ncrystal.cc` & `ncrystal-3.8.2/ncrystal_core/src/ncrystal.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_geant4/include/G4NCrystal/G4NCInstall.hh` & `ncrystal-3.8.2/ncrystal_geant4/include/G4NCrystal/G4NCInstall.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_geant4/include/G4NCrystal/G4NCManager.hh` & `ncrystal-3.8.2/ncrystal_geant4/include/G4NCrystal/G4NCManager.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_geant4/include/G4NCrystal/G4NCMatHelper.hh` & `ncrystal-3.8.2/ncrystal_geant4/include/G4NCrystal/G4NCMatHelper.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_geant4/include/G4NCrystal/G4NCrystal.hh` & `ncrystal-3.8.2/ncrystal_geant4/include/G4NCrystal/G4NCrystal.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_geant4/src/G4NCInstall.cc` & `ncrystal-3.8.2/ncrystal_geant4/src/G4NCInstall.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_geant4/src/G4NCManager.cc` & `ncrystal-3.8.2/ncrystal_geant4/src/G4NCManager.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_geant4/src/G4NCMatHelper.cc` & `ncrystal-3.8.2/ncrystal_geant4/src/G4NCMatHelper.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_geant4/src/G4NCProcWrapper.cc` & `ncrystal-3.8.2/ncrystal_geant4/src/G4NCProcWrapper.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/ncrystal_geant4/src/G4NCProcWrapper.hh` & `ncrystal-3.8.2/ncrystal_geant4/src/G4NCProcWrapper.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/pyproject.toml` & `ncrystal-3.8.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 ################################################################################
 
 [build-system]
 requires = [
     "setuptools>=42",
     "scikit-build>=0.13",
     "cmake>=3.18",
-    "numpy"
+    "numpy",
+    'importlib_metadata; python_version < "3.8"',
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.cibuildwheel]
 test-command = [
   "python3 -mNCrystal.test all",
   "nctool --test",
```

### Comparing `ncrystal-3.8.1/scripts/ncrystal_cif2ncmat` & `ncrystal-3.8.2/scripts/ncrystal_cif2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/scripts/ncrystal_endf2ncmat` & `ncrystal-3.8.2/scripts/ncrystal_endf2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/scripts/ncrystal_hfg2ncmat` & `ncrystal-3.8.2/scripts/ncrystal_hfg2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/scripts/ncrystal_inspectfile` & `ncrystal-3.8.2/scripts/ncrystal_inspectfile`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/scripts/ncrystal_ncmat2cpp` & `ncrystal-3.8.2/scripts/ncrystal_ncmat2cpp`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/scripts/ncrystal_ncmat2hkl` & `ncrystal-3.8.2/scripts/ncrystal_ncmat2hkl`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/scripts/ncrystal_onlinedb2ncmat` & `ncrystal-3.8.2/scripts/ncrystal_onlinedb2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/scripts/ncrystal_vdos2ncmat` & `ncrystal-3.8.2/scripts/ncrystal_vdos2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/scripts/ncrystal_verifyatompos` & `ncrystal-3.8.2/scripts/ncrystal_verifyatompos`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/scripts/nctool` & `ncrystal-3.8.2/scripts/nctool`

 * *Files identical despite different names*

### Comparing `ncrystal-3.8.1/setup.py` & `ncrystal-3.8.2/setup.py`

 * *Files identical despite different names*

