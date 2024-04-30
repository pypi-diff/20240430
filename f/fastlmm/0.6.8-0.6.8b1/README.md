# Comparing `tmp/fastlmm-0.6.8.tar.gz` & `tmp/fastlmm-0.6.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlmm-0.6.8.tar", last modified: Tue Apr 30 20:34:06 2024, max compression
+gzip compressed data, was "fastlmm-0.6.8b1.tar", last modified: Fri Apr 26 02:01:31 2024, max compression
```

## Comparing `fastlmm-0.6.8.tar` & `fastlmm-0.6.8b1.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.314097 fastlmm-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-30 20:32:42.000000 fastlmm-0.6.8/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-30 20:32:42.000000 fastlmm-0.6.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-30 20:32:42.000000 fastlmm-0.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-30 20:34:06.314097 fastlmm-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-30 20:32:42.000000 fastlmm-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.266097 fastlmm-0.6.8/fastlmm/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.270097 fastlmm-0.6.8/fastlmm/association/
--rw-r--r--   0 runner    (1001) docker     (127)    74123 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/FastLmmSet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/FastLmmSetLOOC.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.294097 fastlmm-0.6.8/fastlmm/association/Fastlmm_autoselect/
--rw-r--r--   0 runner    (1001) docker     (127)   562014 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/Fastlmm_autoselect/FastLmmC.Manual.pdf
--rw-r--r--   0 runner    (1001) docker     (127)  8451072 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/Fastlmm_autoselect/FastLmmC.exe
--rw-r--r--   0 runner    (1001) docker     (127) 12772999 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/Fastlmm_autoselect/fastlmmc
--rw-r--r--   0 runner    (1001) docker     (127)  1170360 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/Fastlmm_autoselect/libiomp5md.dll
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/LeaveOneChromosomeOut.py
--rw-r--r--   0 runner    (1001) docker     (127)    15180 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/LocoGwas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/PairResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/PrecomputeLocoPcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/_matchscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/_pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.298097 fastlmm-0.6.8/fastlmm/association/altset_list/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/altset_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/altset_list/consecutive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/altset_list/minmaxsetsize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/altset_list/snpandsetnamecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/altset_list/subset.py
--rw-r--r--   0 runner    (1001) docker     (127)    28684 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/epistasis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/gwas.py
--rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/gwas_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    48108 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/heritability_spatial_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/lrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/meta_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    20307 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/score.py
--rw-r--r--   0 runner    (1001) docker     (127)    74820 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/single_snp.py
--rw-r--r--   0 runner    (1001) docker     (127)    26459 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/single_snp_all_plus_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/single_snp_linreg.py
--rw-r--r--   0 runner    (1001) docker     (127)    78291 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/single_snp_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/single_snp_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/snp_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     9957 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/testCV.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.302097 fastlmm-0.6.8/fastlmm/association/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/Cv.py
--rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/LRT_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/Lrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/Sc.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20390 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/test_gpu_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/test_gwas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/test_heritability_spatial_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)    52161 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/test_single_snp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/test_single_snp_all_plus_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/test_single_snp_linreg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15875 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/test_single_snp_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/test_single_snp_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     8614 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/test_snp_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    21938 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/testepistasis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/tests/tests_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/varcomp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/association/windowing_gwas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.302097 fastlmm-0.6.8/fastlmm/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30319 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/external/pca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.302097 fastlmm-0.6.8/fastlmm/external/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/external/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/external/util/math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.302097 fastlmm-0.6.8/fastlmm/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/feature_selection/PerformSelectionDistributable.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/feature_selection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.306097 fastlmm-0.6.8/fastlmm/feature_selection/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/ScanISP.Toydata.config.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/ScanLMM.Toydata.config.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/ScanOSP.Toydata.config.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/bronze.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1250003 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.5chrom.bed
--rw-r--r--   0 runner    (1001) docker     (127)   237784 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.5chrom.bim
--rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.5chrom.fam
--rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.cov
--rw-r--r--   0 runner    (1001) docker     (127)   197784 2024-04-30 20:32:42.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.map
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.phe
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.shufflePlus.phe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.sim
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/toydataTest.phe
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/feature_selection/examples/toydataTrain.phe
--rw-r--r--   0 runner    (1001) docker     (127)    43450 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/feature_selection/feature_selection_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/feature_selection/feature_selection_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/feature_selection/feature_selection_two_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/feature_selection/kernel_ridge_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)    27797 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/feature_selection/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.306097 fastlmm-0.6.8/fastlmm/inference/
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/ep.py
--rw-r--r--   0 runner    (1001) docker     (127)    38590 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/fastlmm_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    26907 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/glmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/laplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (127)    20767 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    40898 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/lmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    24225 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/lmm2k.py
--rw-r--r--   0 runner    (1001) docker     (127)    56134 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/lmm_cov.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.310097 fastlmm-0.6.8/fastlmm/inference/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    58459 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/tests/test_fastlmm_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/inference/tests/test_linear_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.310097 fastlmm-0.6.8/fastlmm/pyplink/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.310097 fastlmm-0.6.8/fastlmm/pyplink/altset_list/
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/altset_list/Consecutive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/altset_list/MinMaxSetSize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/altset_list/SnpAndSetNameCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/altset_list/Subset.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/altset_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/plink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.310097 fastlmm-0.6.8/fastlmm/pyplink/snpreader/
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/snpreader/Bed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/snpreader/Dat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/snpreader/Hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/snpreader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.310097 fastlmm-0.6.8/fastlmm/pyplink/snpset/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/snpset/AllSnps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/snpset/PositionRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/snpset/RandomSnpSet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/snpset/SnpIndexList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/snpset/SnpSetAndName.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/snpset/SnpsFromFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/snpset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/pyplink/vcfpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.314097 fastlmm-0.6.8/fastlmm/util/
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/NearBronze.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/VertexCut.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/_example_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/computePC.py
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/compute_auto_pcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/est_h2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/fastlmm.hashdown.json
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/genphen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/gensnp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.314097 fastlmm-0.6.8/fastlmm/util/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/matrix/mmultfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/mingrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/pickle_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/run_fastlmmc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.314097 fastlmm-0.6.8/fastlmm/util/standardizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/standardizer/Beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/standardizer/Unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/standardizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.314097 fastlmm-0.6.8/fastlmm/util/stats/
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13309 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/stats/chi2mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)    32930 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/stats/plotp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-04-30 20:32:43.000000 fastlmm-0.6.8/fastlmm/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.266097 fastlmm-0.6.8/fastlmm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-30 20:34:06.000000 fastlmm-0.6.8/fastlmm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-30 20:34:06.000000 fastlmm-0.6.8/fastlmm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:34:06.000000 fastlmm-0.6.8/fastlmm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 20:34:06.000000 fastlmm-0.6.8/fastlmm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 20:34:06.000000 fastlmm-0.6.8/fastlmm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-30 20:32:43.000000 fastlmm-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:34:06.314097 fastlmm-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-30 20:32:43.000000 fastlmm-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:34:06.314097 fastlmm-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-30 20:32:43.000000 fastlmm-0.6.8/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.328031 fastlmm-0.6.8b1/fastlmm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.332031 fastlmm-0.6.8b1/fastlmm/association/
+-rw-r--r--   0 runner    (1001) docker     (127)    74123 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/FastLmmSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/FastLmmSetLOOC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.360031 fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/
+-rw-r--r--   0 runner    (1001) docker     (127)   562014 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/FastLmmC.Manual.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)  8451072 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/FastLmmC.exe
+-rw-r--r--   0 runner    (1001) docker     (127) 12772999 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/fastlmmc
+-rw-r--r--   0 runner    (1001) docker     (127)  1170360 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/libiomp5md.dll
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/LeaveOneChromosomeOut.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15180 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/LocoGwas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/PairResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/PrecomputeLocoPcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/_matchscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.360031 fastlmm-0.6.8b1/fastlmm/association/altset_list/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/altset_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/altset_list/consecutive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/altset_list/minmaxsetsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/altset_list/snpandsetnamecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/altset_list/subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28684 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/epistasis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/gwas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/gwas_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48108 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/heritability_spatial_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/meta_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20307 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74820 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/single_snp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26459 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/single_snp_all_plus_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/single_snp_linreg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78291 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/single_snp_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/single_snp_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/snp_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9957 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/testCV.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.364030 fastlmm-0.6.8b1/fastlmm/association/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/Cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/LRT_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/Lrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/Sc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20390 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_gpu_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_gwas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_heritability_spatial_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52161 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_all_plus_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_linreg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15875 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8614 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/test_snp_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21938 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/testepistasis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/tests/tests_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/varcomp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/association/windowing_gwas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.364030 fastlmm-0.6.8b1/fastlmm/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30319 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/external/pca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.364030 fastlmm-0.6.8b1/fastlmm/external/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/external/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/external/util/math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.364030 fastlmm-0.6.8b1/fastlmm/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/PerformSelectionDistributable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.368030 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/ScanISP.Toydata.config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/ScanLMM.Toydata.config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/ScanOSP.Toydata.config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/bronze.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1250003 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.5chrom.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   237784 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.5chrom.bim
+-rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.5chrom.fam
+-rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-26 02:00:16.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.cov
+-rw-r--r--   0 runner    (1001) docker     (127)   197784 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.map
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.phe
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.shufflePlus.phe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.sim
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydataTest.phe
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydataTrain.phe
+-rw-r--r--   0 runner    (1001) docker     (127)    43450 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/feature_selection_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/feature_selection_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/feature_selection_two_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/kernel_ridge_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27797 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/feature_selection/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.372030 fastlmm-0.6.8b1/fastlmm/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/ep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38590 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/fastlmm_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26907 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/glmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/laplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20767 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40898 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/lmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24225 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/lmm2k.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56134 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/lmm_cov.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.372030 fastlmm-0.6.8b1/fastlmm/inference/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58459 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/tests/test_fastlmm_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/inference/tests/test_linear_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.372030 fastlmm-0.6.8b1/fastlmm/pyplink/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.376030 fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/Consecutive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/MinMaxSetSize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/SnpAndSetNameCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/Subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/plink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.376030 fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/Bed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/Dat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/Hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.376030 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/AllSnps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/PositionRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/RandomSnpSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/SnpIndexList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/SnpSetAndName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/SnpsFromFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/snpset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/pyplink/vcfpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/fastlmm/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/NearBronze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/VertexCut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/_example_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/computePC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/compute_auto_pcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/est_h2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/fastlmm.hashdown.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/genphen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/gensnp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/fastlmm/util/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/matrix/mmultfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/mingrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/pickle_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/run_fastlmmc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/fastlmm/util/standardizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/standardizer/Beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/standardizer/Unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/standardizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/fastlmm/util/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13309 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/stats/chi2mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32930 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/stats/plotp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/fastlmm/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.328031 fastlmm-0.6.8b1/fastlmm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-26 02:01:31.000000 fastlmm-0.6.8b1/fastlmm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-26 02:01:31.000000 fastlmm-0.6.8b1/fastlmm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 02:01:31.000000 fastlmm-0.6.8b1/fastlmm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-26 02:01:31.000000 fastlmm-0.6.8b1/fastlmm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-26 02:01:31.000000 fastlmm-0.6.8b1/fastlmm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 02:01:31.380030 fastlmm-0.6.8b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-26 02:00:17.000000 fastlmm-0.6.8b1/tests/test.py
```

### Comparing `fastlmm-0.6.8/LICENSE.md` & `fastlmm-0.6.8b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/PKG-INFO` & `fastlmm-0.6.8b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlmm
-Version: 0.6.8
+Version: 0.6.8b1
 Summary: Fast GWAS
 Home-page: https://fastlmm.github.io/
 Author: FaST-LMM Team
 Author-email: fastlmm-dev@python.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/fastlmm/FaST-LMM/issues
 Project-URL: Documentation, http://fastlmm.github.io/FaST-LMM
```

### Comparing `fastlmm-0.6.8/README.md` & `fastlmm-0.6.8b1/README.md`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/__init__.py` & `fastlmm-0.6.8b1/fastlmm/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/FastLmmSet.py` & `fastlmm-0.6.8b1/fastlmm/association/FastLmmSet.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/FastLmmSetLOOC.py` & `fastlmm-0.6.8b1/fastlmm/association/FastLmmSetLOOC.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/Fastlmm_autoselect/FastLmmC.Manual.pdf` & `fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/FastLmmC.Manual.pdf`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/Fastlmm_autoselect/FastLmmC.exe` & `fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/FastLmmC.exe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/Fastlmm_autoselect/fastlmmc` & `fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/fastlmmc`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/Fastlmm_autoselect/libiomp5md.dll` & `fastlmm-0.6.8b1/fastlmm/association/Fastlmm_autoselect/libiomp5md.dll`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/LeaveOneChromosomeOut.py` & `fastlmm-0.6.8b1/fastlmm/association/LeaveOneChromosomeOut.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/LocoGwas.py` & `fastlmm-0.6.8b1/fastlmm/association/LocoGwas.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/PairResult.py` & `fastlmm-0.6.8b1/fastlmm/association/PairResult.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/PrecomputeLocoPcs.py` & `fastlmm-0.6.8b1/fastlmm/association/PrecomputeLocoPcs.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/Result.py` & `fastlmm-0.6.8b1/fastlmm/association/Result.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/__init__.py` & `fastlmm-0.6.8b1/fastlmm/association/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/_matchscript.py` & `fastlmm-0.6.8b1/fastlmm/association/_matchscript.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/_pipelines.py` & `fastlmm-0.6.8b1/fastlmm/association/_pipelines.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/altset_list/__init__.py` & `fastlmm-0.6.8b1/fastlmm/association/altset_list/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/altset_list/consecutive.py` & `fastlmm-0.6.8b1/fastlmm/association/altset_list/consecutive.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/altset_list/minmaxsetsize.py` & `fastlmm-0.6.8b1/fastlmm/association/altset_list/minmaxsetsize.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/altset_list/snpandsetnamecollection.py` & `fastlmm-0.6.8b1/fastlmm/association/altset_list/snpandsetnamecollection.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/altset_list/subset.py` & `fastlmm-0.6.8b1/fastlmm/association/altset_list/subset.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/epistasis.py` & `fastlmm-0.6.8b1/fastlmm/association/epistasis.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/fixed.py` & `fastlmm-0.6.8b1/fastlmm/association/fixed.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/gwas.py` & `fastlmm-0.6.8b1/fastlmm/association/gwas.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/gwas_eval.py` & `fastlmm-0.6.8b1/fastlmm/association/gwas_eval.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/heritability_spatial_correction.py` & `fastlmm-0.6.8b1/fastlmm/association/heritability_spatial_correction.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/lrt.py` & `fastlmm-0.6.8b1/fastlmm/association/lrt.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/meta_analysis.py` & `fastlmm-0.6.8b1/fastlmm/association/meta_analysis.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/score.py` & `fastlmm-0.6.8b1/fastlmm/association/score.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/single_snp.py` & `fastlmm-0.6.8b1/fastlmm/association/single_snp.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/single_snp_all_plus_select.py` & `fastlmm-0.6.8b1/fastlmm/association/single_snp_all_plus_select.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/single_snp_linreg.py` & `fastlmm-0.6.8b1/fastlmm/association/single_snp_linreg.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/single_snp_scale.py` & `fastlmm-0.6.8b1/fastlmm/association/single_snp_scale.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/single_snp_select.py` & `fastlmm-0.6.8b1/fastlmm/association/single_snp_select.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/snp_set.py` & `fastlmm-0.6.8b1/fastlmm/association/snp_set.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/testCV.py` & `fastlmm-0.6.8b1/fastlmm/association/testCV.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/Cv.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/Cv.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/LRT_up.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/LRT_up.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/Lrt.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/Lrt.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/Sc.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/Sc.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/__init__.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/test_gpu_perf.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_gpu_perf.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/test_gwas.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_gwas.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/test_heritability_spatial_correction.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_heritability_spatial_correction.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/test_single_snp.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/test_single_snp_all_plus_select.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_all_plus_select.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/test_single_snp_linreg.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_linreg.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/test_single_snp_scale.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_scale.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/test_single_snp_select.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_single_snp_select.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/test_snp_set.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/test_snp_set.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/testepistasis.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/testepistasis.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/tests/tests_util.py` & `fastlmm-0.6.8b1/fastlmm/association/tests/tests_util.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/varcomp_test.py` & `fastlmm-0.6.8b1/fastlmm/association/varcomp_test.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/association/windowing_gwas.py` & `fastlmm-0.6.8b1/fastlmm/association/windowing_gwas.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/external/pca.py` & `fastlmm-0.6.8b1/fastlmm/external/pca.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/external/util/math.py` & `fastlmm-0.6.8b1/fastlmm/external/util/math.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/PerformSelectionDistributable.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/PerformSelectionDistributable.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/examples/ScanISP.Toydata.config.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/ScanISP.Toydata.config.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/examples/ScanLMM.Toydata.config.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/ScanLMM.Toydata.config.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/examples/ScanOSP.Toydata.config.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/ScanOSP.Toydata.config.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.5chrom.bed` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.5chrom.bed`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.5chrom.bim` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.5chrom.bim`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.5chrom.fam` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.5chrom.fam`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.cov` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.cov`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.map` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.map`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.phe` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.phe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/examples/toydata.shufflePlus.phe` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydata.shufflePlus.phe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/examples/toydataTest.phe` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydataTest.phe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/examples/toydataTrain.phe` & `fastlmm-0.6.8b1/fastlmm/feature_selection/examples/toydataTrain.phe`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/feature_selection_cv.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/feature_selection_cv.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/feature_selection_example.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/feature_selection_example.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/feature_selection_two_kernel.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/feature_selection_two_kernel.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/kernel_ridge_cv.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/kernel_ridge_cv.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/feature_selection/test.py` & `fastlmm-0.6.8b1/fastlmm/feature_selection/test.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/inference/__init__.py` & `fastlmm-0.6.8b1/fastlmm/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/inference/ep.py` & `fastlmm-0.6.8b1/fastlmm/inference/ep.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/inference/fastlmm_predictor.py` & `fastlmm-0.6.8b1/fastlmm/inference/fastlmm_predictor.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/inference/glmm.py` & `fastlmm-0.6.8b1/fastlmm/inference/glmm.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/inference/laplace.py` & `fastlmm-0.6.8b1/fastlmm/inference/laplace.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/inference/likelihood.py` & `fastlmm-0.6.8b1/fastlmm/inference/likelihood.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/inference/linear_regression.py` & `fastlmm-0.6.8b1/fastlmm/inference/linear_regression.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/inference/lmm.py` & `fastlmm-0.6.8b1/fastlmm/inference/lmm.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/inference/lmm2k.py` & `fastlmm-0.6.8b1/fastlmm/inference/lmm2k.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/inference/lmm_cov.py` & `fastlmm-0.6.8b1/fastlmm/inference/lmm_cov.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/inference/tests/test.py` & `fastlmm-0.6.8b1/fastlmm/inference/tests/test.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/inference/tests/test_fastlmm_predictor.py` & `fastlmm-0.6.8b1/fastlmm/inference/tests/test_fastlmm_predictor.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/inference/tests/test_linear_regression.py` & `fastlmm-0.6.8b1/fastlmm/inference/tests/test_linear_regression.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/altset_list/Consecutive.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/Consecutive.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/altset_list/MinMaxSetSize.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/MinMaxSetSize.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/altset_list/SnpAndSetNameCollection.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/SnpAndSetNameCollection.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/altset_list/Subset.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/Subset.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/altset_list/__init__.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/altset_list/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/plink.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/plink.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/setup.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/setup.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/snpreader/Bed.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/Bed.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/snpreader/Dat.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/Dat.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/snpreader/Hdf5.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpreader/Hdf5.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/snpset/AllSnps.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpset/AllSnps.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/snpset/PositionRange.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpset/PositionRange.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/snpset/RandomSnpSet.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpset/RandomSnpSet.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/snpset/SnpIndexList.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpset/SnpIndexList.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/snpset/SnpSetAndName.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpset/SnpSetAndName.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/snpset/SnpsFromFile.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpset/SnpsFromFile.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/snpset/__init__.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/snpset/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/test.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/test.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/pyplink/vcfpy.py` & `fastlmm-0.6.8b1/fastlmm/pyplink/vcfpy.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/NearBronze.py` & `fastlmm-0.6.8b1/fastlmm/util/NearBronze.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/VertexCut.py` & `fastlmm-0.6.8b1/fastlmm/util/VertexCut.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/_example_file.py` & `fastlmm-0.6.8b1/fastlmm/util/_example_file.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/computePC.py` & `fastlmm-0.6.8b1/fastlmm/util/computePC.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/compute_auto_pcs.py` & `fastlmm-0.6.8b1/fastlmm/util/compute_auto_pcs.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/est_h2.py` & `fastlmm-0.6.8b1/fastlmm/util/est_h2.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/fastlmm.hashdown.json` & `fastlmm-0.6.8b1/fastlmm/util/fastlmm.hashdown.json`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/genphen.py` & `fastlmm-0.6.8b1/fastlmm/util/genphen.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/gensnp.py` & `fastlmm-0.6.8b1/fastlmm/util/gensnp.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/matrix/mmultfile.py` & `fastlmm-0.6.8b1/fastlmm/util/matrix/mmultfile.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/mingrid.py` & `fastlmm-0.6.8b1/fastlmm/util/mingrid.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/pickle_io.py` & `fastlmm-0.6.8b1/fastlmm/util/pickle_io.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/preprocess.py` & `fastlmm-0.6.8b1/fastlmm/util/preprocess.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/run_fastlmmc.py` & `fastlmm-0.6.8b1/fastlmm/util/run_fastlmmc.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/standardizer/Beta.py` & `fastlmm-0.6.8b1/fastlmm/util/standardizer/Beta.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/standardizer/Unit.py` & `fastlmm-0.6.8b1/fastlmm/util/standardizer/Unit.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/standardizer/__init__.py` & `fastlmm-0.6.8b1/fastlmm/util/standardizer/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/stats/__init__.py` & `fastlmm-0.6.8b1/fastlmm/util/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/stats/chi2mixture.py` & `fastlmm-0.6.8b1/fastlmm/util/stats/chi2mixture.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/stats/plotp.py` & `fastlmm-0.6.8b1/fastlmm/util/stats/plotp.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/test.py` & `fastlmm-0.6.8b1/fastlmm/util/test.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm/util/util.py` & `fastlmm-0.6.8b1/fastlmm/util/util.py`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/fastlmm.egg-info/PKG-INFO` & `fastlmm-0.6.8b1/fastlmm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlmm
-Version: 0.6.8
+Version: 0.6.8b1
 Summary: Fast GWAS
 Home-page: https://fastlmm.github.io/
 Author: FaST-LMM Team
 Author-email: fastlmm-dev@python.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/fastlmm/FaST-LMM/issues
 Project-URL: Documentation, http://fastlmm.github.io/FaST-LMM
```

### Comparing `fastlmm-0.6.8/fastlmm.egg-info/SOURCES.txt` & `fastlmm-0.6.8b1/fastlmm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastlmm-0.6.8/setup.py` & `fastlmm-0.6.8b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Work around https://github.com/pypa/pip/issues/7953
 import site
 import sys
 
 site.ENABLE_USER_SITE = "--user" in sys.argv[1:]
 
 # Version number
-version = "0.6.8"
+version = "0.6.8b1"
 
 
 def readme():
     with open("README.md") as f:
         return f.read()
```

### Comparing `fastlmm-0.6.8/tests/test.py` & `fastlmm-0.6.8b1/tests/test.py`

 * *Files identical despite different names*

