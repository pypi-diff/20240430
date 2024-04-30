# Comparing `tmp/pyiqa-0.1.7.tar.gz` & `tmp/pyiqa-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiqa-0.1.7.tar", last modified: Fri Jun 23 11:59:10 2023, max compression
+gzip compressed data, was "dist/pyiqa-0.1.8.tar", last modified: Mon Oct  9 06:59:09 2023, max compression
```

## Comparing `pyiqa-0.1.7.tar` & `pyiqa-0.1.8.tar`

### file list

```diff
@@ -1,118 +1,122 @@
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    21165 2022-08-14 08:39:50.000000 pyiqa-0.1.7/LICENSE
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1717 2022-09-23 04:11:05.000000 pyiqa-0.1.7/LICENSE_NTU-S-Lab
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)       41 2022-08-14 08:39:50.000000 pyiqa-0.1.7/MANIFEST.in
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    12231 2023-06-23 11:59:10.000000 pyiqa-0.1.7/PKG-INFO
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11357 2023-03-30 12:36:49.000000 pyiqa-0.1.7/README.md
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)        6 2023-06-23 11:42:59.000000 pyiqa-0.1.7/VERSION
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      322 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2137 2023-03-05 10:38:17.000000 pyiqa-0.1.7/pyiqa/api_helpers.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/archs/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      881 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     8259 2023-04-21 11:24:04.000000 pyiqa-0.1.7/pyiqa/archs/ahiq_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6053 2023-04-01 05:18:18.000000 pyiqa-0.1.7/pyiqa/archs/arch_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7158 2023-05-25 19:19:58.000000 pyiqa-0.1.7/pyiqa/archs/brisque_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12397 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/ckdn_arch.py
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    25129 2023-01-11 18:50:33.000000 pyiqa-0.1.7/pyiqa/archs/clip_model.py
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     6636 2023-04-01 05:18:41.000000 pyiqa-0.1.7/pyiqa/archs/clipiqa_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1827 2023-06-09 14:01:56.000000 pyiqa-0.1.7/pyiqa/archs/clipscore_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2425 2022-11-21 12:29:26.000000 pyiqa-0.1.7/pyiqa/archs/cnniqa_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      387 2022-12-21 06:18:18.000000 pyiqa-0.1.7/pyiqa/archs/constants.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6126 2022-09-14 13:07:48.000000 pyiqa-0.1.7/pyiqa/archs/dbcnn_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5207 2023-03-05 10:40:20.000000 pyiqa-0.1.7/pyiqa/archs/dists_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1453 2023-06-16 07:14:54.000000 pyiqa-0.1.7/pyiqa/archs/entropy_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11009 2023-04-18 12:09:31.000000 pyiqa-0.1.7/pyiqa/archs/fid_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    18043 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/fsim_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6967 2023-03-29 10:09:20.000000 pyiqa-0.1.7/pyiqa/archs/func_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3471 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/gmsd_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7126 2023-04-01 05:19:52.000000 pyiqa-0.1.7/pyiqa/archs/hypernet_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12026 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/inception.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    23872 2023-04-01 05:20:23.000000 pyiqa-0.1.7/pyiqa/archs/iqt_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    14538 2022-10-13 10:06:00.000000 pyiqa-0.1.7/pyiqa/archs/lpips_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11139 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/mad_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7328 2023-04-03 07:58:57.000000 pyiqa-0.1.7/pyiqa/archs/maniqa_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16352 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/maniqa_swin.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13510 2023-05-25 16:57:19.000000 pyiqa-0.1.7/pyiqa/archs/musiq_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4013 2023-03-30 10:34:02.000000 pyiqa-0.1.7/pyiqa/archs/nima_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    19945 2023-06-01 04:20:40.000000 pyiqa-0.1.7/pyiqa/archs/niqe_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7050 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/nlpd_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16444 2023-03-29 13:57:08.000000 pyiqa-0.1.7/pyiqa/archs/nrqm_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2870 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/paq2piq_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5467 2022-12-21 06:09:37.000000 pyiqa-0.1.7/pyiqa/archs/pieapp_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2663 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/psnr_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11184 2023-05-25 12:06:16.000000 pyiqa-0.1.7/pyiqa/archs/ssim_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    14811 2023-02-22 14:19:42.000000 pyiqa-0.1.7/pyiqa/archs/tres_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    29869 2023-04-01 05:17:21.000000 pyiqa-0.1.7/pyiqa/archs/uranker_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    18900 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/vif_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     9938 2023-05-25 15:06:40.000000 pyiqa-0.1.7/pyiqa/archs/vsi_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6508 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/wadiqam_arch.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/data/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4472 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4164 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/ava_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4390 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/bapps_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1812 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/data_sampler.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13252 2022-09-01 10:56:27.000000 pyiqa-0.1.7/pyiqa/data/data_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2678 2023-02-23 14:39:44.000000 pyiqa-0.1.7/pyiqa/data/flive_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3325 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/general_fr_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2726 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/general_nr_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2560 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/livechallenge_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7728 2022-09-01 10:54:53.000000 pyiqa-0.1.7/pyiqa/data/multiscale_trans_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4849 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/pieapp_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3201 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/pipal_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3131 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/prefetch_dataloader.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13759 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/transforms.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7891 2023-06-16 06:39:56.000000 pyiqa-0.1.7/pyiqa/default_model_configs.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/losses/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      716 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/losses/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4348 2022-09-01 10:48:31.000000 pyiqa-0.1.7/pyiqa/losses/iqa_losses.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2903 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/losses/loss_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7448 2022-09-01 10:47:19.000000 pyiqa-0.1.7/pyiqa/losses/losses.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/matlab_utils/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      529 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/matlab_utils/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    10201 2023-03-29 12:41:27.000000 pyiqa-0.1.7/pyiqa/matlab_utils/functions.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2581 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/matlab_utils/math_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12829 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/matlab_utils/resize.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     8057 2023-05-25 19:10:31.000000 pyiqa-0.1.7/pyiqa/matlab_utils/scfpyr_util.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/metrics/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      566 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/metrics/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2041 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/metrics/correlation_coefficient.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      270 2022-09-01 10:44:09.000000 pyiqa-0.1.7/pyiqa/metrics/other_metrics.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/models/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1007 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/models/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5767 2022-09-01 10:41:30.000000 pyiqa-0.1.7/pyiqa/models/bapps_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16067 2022-09-01 10:43:19.000000 pyiqa-0.1.7/pyiqa/models/base_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1737 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/models/dbcnn_model.py
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     8143 2023-01-11 18:50:33.000000 pyiqa-0.1.7/pyiqa/models/general_iqa_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1190 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/models/hypernet_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3166 2023-05-25 17:07:55.000000 pyiqa-0.1.7/pyiqa/models/inference_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3956 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/models/lr_scheduler.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2227 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/models/nima_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2302 2022-09-01 10:41:22.000000 pyiqa-0.1.7/pyiqa/models/pieapp_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     9300 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/models/sr_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      975 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/models/wadiqam_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1720 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/test.py
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    11007 2023-01-11 18:50:33.000000 pyiqa-0.1.7/pyiqa/train.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2405 2022-09-01 11:01:29.000000 pyiqa-0.1.7/pyiqa/train_nsplits.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/utils/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      934 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7621 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/color_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2608 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/dist_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3345 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/download_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6017 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/file_client.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7261 2022-10-26 05:47:49.000000 pyiqa-0.1.7/pyiqa/utils/img_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7123 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/lmdb_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7139 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/logger.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4767 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/misc.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6474 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/options.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2185 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/registry.py
--rwxr-xr-x   0 cfchen   (25144) cfchen   (25144)      128 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/version.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa.egg-info/
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    12231 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa.egg-info/PKG-INFO
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     2739 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa.egg-info/SOURCES.txt
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)        1 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa.egg-info/dependency_links.txt
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)      170 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa.egg-info/requires.txt
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)        6 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa.egg-info/top_level.txt
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)      169 2023-03-29 17:32:51.000000 pyiqa-0.1.7/requirements.txt
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      333 2023-06-23 11:59:10.000000 pyiqa-0.1.7/setup.cfg
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3478 2023-03-29 17:15:09.000000 pyiqa-0.1.7/setup.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-10-09 06:59:09.000000 pyiqa-0.1.8/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    21165 2022-08-14 08:39:50.000000 pyiqa-0.1.8/LICENSE
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1717 2022-09-23 04:11:05.000000 pyiqa-0.1.8/LICENSE_NTU-S-Lab
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)       41 2022-08-14 08:39:50.000000 pyiqa-0.1.8/MANIFEST.in
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    13756 2023-10-09 06:59:09.000000 pyiqa-0.1.8/PKG-INFO
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12882 2023-10-09 06:04:04.000000 pyiqa-0.1.8/README.md
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)        6 2023-10-09 06:37:07.000000 pyiqa-0.1.8/VERSION
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-10-09 06:59:07.000000 pyiqa-0.1.8/pyiqa/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      322 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2137 2023-03-05 10:38:17.000000 pyiqa-0.1.8/pyiqa/api_helpers.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-10-09 06:59:08.000000 pyiqa-0.1.8/pyiqa/archs/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      881 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/archs/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7900 2023-10-01 15:23:33.000000 pyiqa-0.1.8/pyiqa/archs/ahiq_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5187 2023-08-19 08:39:08.000000 pyiqa-0.1.8/pyiqa/archs/arch_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7339 2023-10-01 15:23:35.000000 pyiqa-0.1.8/pyiqa/archs/brisque_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12397 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/archs/ckdn_arch.py
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    25846 2023-08-04 07:06:24.000000 pyiqa-0.1.8/pyiqa/archs/clip_model.py
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     6636 2023-04-01 05:18:41.000000 pyiqa-0.1.8/pyiqa/archs/clipiqa_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1471 2023-09-30 13:43:43.000000 pyiqa-0.1.8/pyiqa/archs/clipscore_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2425 2023-08-06 15:32:56.000000 pyiqa-0.1.8/pyiqa/archs/cnniqa_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      387 2022-12-21 06:18:18.000000 pyiqa-0.1.8/pyiqa/archs/constants.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6202 2023-08-07 11:19:04.000000 pyiqa-0.1.8/pyiqa/archs/dbcnn_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5215 2023-07-10 08:42:20.000000 pyiqa-0.1.8/pyiqa/archs/dists_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1453 2023-06-16 07:14:54.000000 pyiqa-0.1.8/pyiqa/archs/entropy_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11009 2023-04-18 12:09:31.000000 pyiqa-0.1.8/pyiqa/archs/fid_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    18043 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/archs/fsim_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7101 2023-09-25 14:11:38.000000 pyiqa-0.1.8/pyiqa/archs/func_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3471 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/archs/gmsd_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7125 2023-08-06 15:34:59.000000 pyiqa-0.1.8/pyiqa/archs/hypernet_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12026 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/archs/inception.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    23872 2023-04-01 05:20:23.000000 pyiqa-0.1.8/pyiqa/archs/iqt_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1675 2023-08-19 08:40:38.000000 pyiqa-0.1.8/pyiqa/archs/laion_aes_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    14542 2023-07-10 08:34:30.000000 pyiqa-0.1.8/pyiqa/archs/lpips_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11210 2023-09-12 06:01:17.000000 pyiqa-0.1.8/pyiqa/archs/mad_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6828 2023-08-06 13:43:07.000000 pyiqa-0.1.8/pyiqa/archs/maniqa_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16367 2023-07-10 09:09:22.000000 pyiqa-0.1.8/pyiqa/archs/maniqa_swin.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13556 2023-08-18 05:37:46.000000 pyiqa-0.1.8/pyiqa/archs/musiq_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3721 2023-08-06 13:09:26.000000 pyiqa-0.1.8/pyiqa/archs/nima_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    19945 2023-06-01 04:20:40.000000 pyiqa-0.1.8/pyiqa/archs/niqe_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7047 2023-08-18 05:18:13.000000 pyiqa-0.1.8/pyiqa/archs/nlpd_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16411 2023-08-18 05:17:36.000000 pyiqa-0.1.8/pyiqa/archs/nrqm_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2877 2023-07-10 08:43:09.000000 pyiqa-0.1.8/pyiqa/archs/paq2piq_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5467 2022-12-21 06:09:37.000000 pyiqa-0.1.8/pyiqa/archs/pieapp_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2663 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/archs/psnr_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11184 2023-05-25 12:06:16.000000 pyiqa-0.1.8/pyiqa/archs/ssim_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    23972 2023-08-15 08:31:22.000000 pyiqa-0.1.8/pyiqa/archs/stlpips_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    18158 2023-10-09 05:57:21.000000 pyiqa-0.1.8/pyiqa/archs/topiq_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    31486 2023-09-26 12:12:06.000000 pyiqa-0.1.8/pyiqa/archs/topiq_swin.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    14233 2023-08-06 14:00:05.000000 pyiqa-0.1.8/pyiqa/archs/tres_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    29869 2023-04-01 05:17:21.000000 pyiqa-0.1.8/pyiqa/archs/uranker_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    18900 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/archs/vif_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     9938 2023-05-25 15:06:40.000000 pyiqa-0.1.8/pyiqa/archs/vsi_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6508 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/archs/wadiqam_arch.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-10-09 06:59:08.000000 pyiqa-0.1.8/pyiqa/data/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4472 2022-09-01 10:53:45.000000 pyiqa-0.1.8/pyiqa/data/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3119 2023-08-06 12:16:31.000000 pyiqa-0.1.8/pyiqa/data/ava_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3574 2023-08-06 12:22:39.000000 pyiqa-0.1.8/pyiqa/data/bapps_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3072 2023-10-08 12:53:45.000000 pyiqa-0.1.8/pyiqa/data/base_iqa_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1812 2022-09-01 10:53:45.000000 pyiqa-0.1.8/pyiqa/data/data_sampler.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13252 2022-09-01 10:56:27.000000 pyiqa-0.1.8/pyiqa/data/data_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2891 2023-08-06 12:11:02.000000 pyiqa-0.1.8/pyiqa/data/general_fr_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      933 2023-10-08 11:28:52.000000 pyiqa-0.1.8/pyiqa/data/general_nr_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      966 2023-08-06 11:49:13.000000 pyiqa-0.1.8/pyiqa/data/livechallenge_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7728 2022-09-01 10:54:53.000000 pyiqa-0.1.8/pyiqa/data/multiscale_trans_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3701 2023-08-06 12:49:45.000000 pyiqa-0.1.8/pyiqa/data/pieapp_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2588 2023-10-09 05:46:46.000000 pyiqa-0.1.8/pyiqa/data/piq_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3131 2022-09-01 10:53:45.000000 pyiqa-0.1.8/pyiqa/data/prefetch_dataloader.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13722 2023-08-15 11:16:32.000000 pyiqa-0.1.8/pyiqa/data/transforms.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    10823 2023-10-09 05:57:32.000000 pyiqa-0.1.8/pyiqa/default_model_configs.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-10-09 06:59:08.000000 pyiqa-0.1.8/pyiqa/losses/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      716 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/losses/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4348 2022-09-01 10:48:31.000000 pyiqa-0.1.8/pyiqa/losses/iqa_losses.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2903 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/losses/loss_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7448 2022-09-01 10:47:19.000000 pyiqa-0.1.8/pyiqa/losses/losses.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-10-09 06:59:08.000000 pyiqa-0.1.8/pyiqa/matlab_utils/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      656 2023-08-18 05:21:08.000000 pyiqa-0.1.8/pyiqa/matlab_utils/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    10188 2023-09-25 14:11:36.000000 pyiqa-0.1.8/pyiqa/matlab_utils/functions.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2581 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/matlab_utils/math_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3094 2023-08-18 05:20:44.000000 pyiqa-0.1.8/pyiqa/matlab_utils/padding.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12829 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/matlab_utils/resize.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     8057 2023-05-25 19:10:31.000000 pyiqa-0.1.8/pyiqa/matlab_utils/scfpyr_util.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-10-09 06:59:08.000000 pyiqa-0.1.8/pyiqa/metrics/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      566 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/metrics/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2041 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/metrics/correlation_coefficient.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      270 2022-09-01 10:44:09.000000 pyiqa-0.1.8/pyiqa/metrics/other_metrics.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-10-09 06:59:09.000000 pyiqa-0.1.8/pyiqa/models/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1007 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/models/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5767 2022-09-01 10:41:30.000000 pyiqa-0.1.8/pyiqa/models/bapps_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16067 2022-09-01 10:43:19.000000 pyiqa-0.1.8/pyiqa/models/base_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1737 2022-08-14 08:39:50.000000 pyiqa-0.1.8/pyiqa/models/dbcnn_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1584 2023-08-05 13:22:02.000000 pyiqa-0.1.8/pyiqa/models/distiqa_model.py
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     9808 2023-10-08 12:02:58.000000 pyiqa-0.1.8/pyiqa/models/general_iqa_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1190 2022-08-14 08:39:51.000000 pyiqa-0.1.8/pyiqa/models/hypernet_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3186 2023-09-29 14:21:10.000000 pyiqa-0.1.8/pyiqa/models/inference_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3956 2022-08-14 08:39:51.000000 pyiqa-0.1.8/pyiqa/models/lr_scheduler.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2302 2022-09-01 10:41:22.000000 pyiqa-0.1.8/pyiqa/models/pieapp_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      975 2022-08-14 08:39:51.000000 pyiqa-0.1.8/pyiqa/models/wadiqam_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1720 2022-08-14 08:39:51.000000 pyiqa-0.1.8/pyiqa/test.py
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    11542 2023-10-08 09:55:32.000000 pyiqa-0.1.8/pyiqa/train.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2405 2022-09-01 11:01:29.000000 pyiqa-0.1.8/pyiqa/train_nsplits.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-10-09 06:59:09.000000 pyiqa-0.1.8/pyiqa/utils/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1098 2023-08-06 09:40:33.000000 pyiqa-0.1.8/pyiqa/utils/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7621 2022-08-14 08:39:51.000000 pyiqa-0.1.8/pyiqa/utils/color_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2608 2022-08-14 08:39:51.000000 pyiqa-0.1.8/pyiqa/utils/dist_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3345 2022-08-14 08:39:51.000000 pyiqa-0.1.8/pyiqa/utils/download_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6017 2022-08-14 08:39:51.000000 pyiqa-0.1.8/pyiqa/utils/file_client.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7133 2023-08-15 11:16:08.000000 pyiqa-0.1.8/pyiqa/utils/img_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7123 2022-08-14 08:39:51.000000 pyiqa-0.1.8/pyiqa/utils/lmdb_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7139 2022-08-14 08:39:51.000000 pyiqa-0.1.8/pyiqa/utils/logger.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4767 2022-08-14 08:39:51.000000 pyiqa-0.1.8/pyiqa/utils/misc.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6474 2022-08-14 08:39:51.000000 pyiqa-0.1.8/pyiqa/utils/options.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2185 2022-08-14 08:39:51.000000 pyiqa-0.1.8/pyiqa/utils/registry.py
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)      128 2023-10-09 06:59:06.000000 pyiqa-0.1.8/pyiqa/version.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-10-09 06:59:07.000000 pyiqa-0.1.8/pyiqa.egg-info/
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    13756 2023-10-09 06:59:06.000000 pyiqa-0.1.8/pyiqa.egg-info/PKG-INFO
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     2858 2023-10-09 06:59:06.000000 pyiqa-0.1.8/pyiqa.egg-info/SOURCES.txt
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)        1 2023-10-09 06:59:06.000000 pyiqa-0.1.8/pyiqa.egg-info/dependency_links.txt
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)      170 2023-10-09 06:59:06.000000 pyiqa-0.1.8/pyiqa.egg-info/requires.txt
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)        6 2023-10-09 06:59:06.000000 pyiqa-0.1.8/pyiqa.egg-info/top_level.txt
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)      169 2023-09-26 12:13:23.000000 pyiqa-0.1.8/requirements.txt
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      333 2023-10-09 06:59:09.000000 pyiqa-0.1.8/setup.cfg
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3478 2023-03-29 17:15:09.000000 pyiqa-0.1.8/setup.py
```

### Comparing `pyiqa-0.1.7/LICENSE` & `pyiqa-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/LICENSE_NTU-S-Lab` & `pyiqa-0.1.8/LICENSE_NTU-S-Lab`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/PKG-INFO` & `pyiqa-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiqa
-Version: 0.1.7
+Version: 0.1.8
 Summary: PyTorch Toolbox for Image Quality Assessment
 Home-page: https://github.com/chaofengc/IQA-PyTorch
 Author: Chaofeng Chen
 Author-email: chaofenghust@gmail.com
 License: UNKNOWN
 Keywords: image quality assessment,pytorch
 Platform: UNKNOWN
@@ -18,25 +18,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE_NTU-S-Lab
 
-# PyTorch Toolbox for Image Quality Assessment
+# <img align="left" width="100" height="100" src="docs/pyiqa_logo.jpg"> PyTorch Toolbox for Image Quality Assessment
 
-An IQA toolbox with pure python and pytorch. Please refer to [Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-Quality-Assessment) for a comprehensive survey of IQA methods, as well as download links for IQA datasets.
+An IQA toolbox with pure python and pytorch. Please refer to [Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-Quality-Assessment) for a comprehensive survey of IQA methods and download links for IQA datasets.
 
 <a href="https://colab.research.google.com/drive/14J3KoyrjJ6R531DsdOy5Bza5xfeMODi6?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="google colab logo"></a> 
 [![PyPI](https://img.shields.io/pypi/v/pyiqa)](https://pypi.org/project/pyiqa/)
 ![visitors](https://visitor-badge.laobi.icu/badge?page_id=chaofengc/IQA-PyTorch) 
+[![Documentation Status](https://readthedocs.org/projects/iqa-pytorch/badge/?version=latest)](https://iqa-pytorch.readthedocs.io/en/latest/?badge=latest)
 [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/chaofengc/Awesome-Image-Quality-Assessment)
 [![Citation](https://img.shields.io/badge/Citation-bibtex-green)](https://github.com/chaofengc/IQA-PyTorch/blob/main/README.md#bookmark_tabs-citation)
 
-![demo](demo.gif)
+![demo](docs/demo.gif)
 
 - [:open\_book: Introduction](#open_book-introduction)
 - [:zap: Quick Start](#zap-quick-start)
   - [Dependencies and Installation](#dependencies-and-installation)
   - [Basic Usage](#basic-usage)
 - [:1st\_place\_medal: Benchmark Performances and Model Zoo](#1st_place_medal-benchmark-performances-and-model-zoo)
   - [Results Calibration](#results-calibration)
@@ -44,36 +45,42 @@
   - [Benchmark Performance with Provided Script](#benchmark-performance-with-provided-script)
 - [:hammer\_and\_wrench: Train](#hammer_and_wrench-train)
   - [Dataset Preparation](#dataset-preparation)
   - [Example Train Script](#example-trai-script)
  
 ## :open_book: Introduction
 
-This is a image quality assessment toolbox with **pure python and pytorch**. We provide reimplementation of many mainstream full reference (FR) and no reference (NR) metrics (results are calibrated with official matlab scripts if exist). **With GPU acceleration, most of our implementations are much faster than Matlab.** Please refer to the [Model Cards](docs/ModelCard.md) and [Dataset Cards](docs/Dataset_Preparation.md) for all supported methods and datasets.
+This is a image quality assessment toolbox with **pure python and pytorch**. We provide reimplementation of many mainstream full reference (FR) and no reference (NR) metrics (results are calibrated with official matlab scripts if exist). **With GPU acceleration, most of our implementations are much faster than Matlab.** Please refer to the following documents for details:  
+
+<div align="center">
+
+📦 [Model Cards](docs/ModelCard.md)  |  🗃️ [Dataset Cards](docs/Dataset_Preparation.md) 
+
+</div>
 
 ---
 
 ### :triangular_flag_on_post: Updates/Changelog
-
+- **Oct 09, 2023**. Add datasets: [PIQ2023](https://github.com/DXOMARK-Research/PIQ2023), [GFIQA](http://database.mmsp-kn.de/gfiqa-20k-database.html). Add metric `topiq_nr-face`. 
+- **Aug 15, 2023**. Add `st-lpips` and `laion_aes`. Refer to official repo at [ShiftTolerant-LPIPS](https://github.com/abhijay9/ShiftTolerant-LPIPS) and [improved-aesthetic-predictor](https://github.com/christophschuhmann/improved-aesthetic-predictor)
+- **Aug 05, 2023**. Add our work [TOPIQ](https://arxiv.org/abs/2308.03060) with remarkable performance on almost all benchmarks via efficient Resnet50 backbone. Use it with `topiq_fr, topiq_nr, topiq_iaa` for Full-Reference, No-Reference and Aesthetic assessment respectively.
 - **March 30, 2023**. Add [URanker](https://github.com/RQ-Wu/UnderwaterRanker) for IQA of under water images. 
 - **March 29, 2023**. :rotating_light: Hot fix of NRQM & PI. 
 - **March 25, 2023**. Add TreS, HyperIQA, CNNIQA, CLIPIQA.
-- **Sep 1, 2022**. 1) Add pretrained models for MANIQA and AHIQ. 2) Add dataset interface for pieapp and PIPAL.
-- **June 3, 2022**. Add FID metric. See [clean-fid](https://github.com/GaParmar/clean-fid) for more details.
-- **March 11, 2022**. Add pretrained DBCNN, NIMA, and official model of PieAPP, paq2piq.
 - [**More**](docs/history_changelog.md)
 
 ---
 
 ## :zap: Quick Start
 
 ### Dependencies and Installation
 - Ubuntu >= 18.04
 - Python >= 3.8
-- Pytorch >= 1.10
+- PyTorch >= 1.12
+- Torchvision >= 0.13
 - CUDA >= 10.2 (if use GPU)
 ```
 # Install with pip
 pip install pyiqa
 
 # Install latest github version
 pip uninstall pyiqa # if have older version installed already 
@@ -140,30 +147,35 @@
 
 Please refer to the [results calibration](./ResultsCalibra/ResultsCalibra.md) to verify the correctness of the python implementations compared with official scripts in matlab or python.
 
 ### Performance Evaluation Protocol
 
 **We use official models for evaluation if available.** Otherwise, we use the following settings to train and evaluate different models for simplicity and consistency:
 
-| Metric Type   | Train     | Test                                       | Results                                                  |
+| Metric Type   | Train     | Test                                       | Results                                                  | 
 | ------------- | --------- | ------------------------------------------ | -------------------------------------------------------- |
 | FR            | KADID-10k | CSIQ, LIVE, TID2008, TID2013               | [FR benchmark results](tests/FR_benchmark_results.csv)   |
-| NR            | KonIQ-10k | LIVEC, KonIQ-10k (official split), TID2013 | [NR benchmark results](tests/NR_benchmark_results.csv)   |
+| NR            | KonIQ-10k | LIVEC, KonIQ-10k (official split), TID2013, SPAQ | [NR benchmark results](tests/NR_benchmark_results.csv)   |
 | Aesthetic IQA | AVA       | AVA (official split)                       | [IAA benchmark results](tests/IAA_benchmark_results.csv) |
 
+Results are calculated with:
+- **PLCC without any correction**. Although test time value correction is common in IQA papers, we want to use the original value in our benchmark.
+- **Full image single input.** We use multi-patch testing only when it is necessary for the model to work.
+
 Basically, we use the largest existing datasets for training, and cross dataset evaluation performance for fair comparison. The following models do not provide official weights, and are retrained by our scripts:
 
-| Metric Type   | Model Names                   |
+| Metric Type   | Reproduced Models |
 | ------------- | ----------------------------- |
 | FR            |                               |
 | NR            | `cnniqa`, `dbcnn`, `hyperiqa` |
 | Aesthetic IQA | `nima`, `nima-vgg16-ava`      |
 
-Notes:
-- Due to optimized training process, performance of some retrained approaches may be higher than original paper.
+**Important Notes:**
+- Due to optimized training process, performance of some retrained approaches may be different with original paper.
+- Results of all **retrained models by ours** are normalized to [0, 1] and change to higher better for convenience.
 - Results of KonIQ-10k, AVA are both tested with official split.
 - NIMA is only applicable to AVA dataset now. We use `inception_resnet_v2` for default `nima`.
 - MUSIQ is not included in the IAA benchmark because we do not have train/split information of the official model.
 
 ### Benchmark Performance with Provided Script
 
 Here is an example script to get performance benchmark on different datasets:
@@ -181,26 +193,26 @@
 ```
 
 ## :hammer_and_wrench: Train
 
 ### Dataset Preparation
 
 - You only need to unzip downloaded datasets from official website without any extra operation. And then make soft links of these dataset folder under `datasets/` folder. Download links are provided in [Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-Quality-Assessment).
-- We provide common interface to load these datasets with the prepared meta information files and train/val/test split files, which can be downloaded from [download_link](https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/data_info_files.tgz) and extract them to `datasets/` folder.
+- We provide common interface to load these datasets with the prepared meta information files and train/val/test split files, which can be downloaded from [download_link](https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/meta_info.tgz) and extract them to `datasets/` folder.
 
 You may also use the following commands:
 
 ```
 mkdir datasets && cd datasets
 
 # make soft links of your dataset
 ln -sf your/dataset/path datasetname
 
 # download meta info files and train split files
-wget https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/data_info_files.tgz
+wget https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/meta_info.tgz
 tar -xvf data_info_files.tgz
 ```
 
 Examples to specific dataset options can be found in `./options/default_dataset_opt.yml`. Details of the dataloader inferface and meta information files can be found in [Dataset Preparation](docs/Dataset_Preparation.md)
 
 ### Example Train Script
 
@@ -233,14 +245,26 @@
   title={{IQA-PyTorch}: PyTorch Toolbox for Image Quality Assessment},
   author={Chaofeng Chen and Jiadi Mo},
   year={2022},
   howpublished = "[Online]. Available: \url{https://github.com/chaofengc/IQA-PyTorch}"
 }
 ```
 
+Please also consider to cite our new work `TOPIQ` if it is useful to you:
+```
+@misc{chen2023topiq,
+      title={TOPIQ: A Top-down Approach from Semantics to Distortions for Image Quality Assessment}, 
+      author={Chaofeng Chen and Jiadi Mo and Jingwen Hou and Haoning Wu and Liang Liao and Wenxiu Sun and Qiong Yan and Weisi Lin},
+      year={2023},
+      eprint={2308.03060},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+}
+``` 
+
 ## :heart: Acknowledgement
 
 The code architecture is borrowed from [BasicSR](https://github.com/xinntao/BasicSR). Several implementations are taken from: [IQA-optimization](https://github.com/dingkeyan93/IQA-optimization), [Image-Quality-Assessment-Toolbox](https://github.com/RyanXingQL/Image-Quality-Assessment-Toolbox), [piq](https://github.com/photosynthesis-team/piq), [piqa](https://github.com/francois-rozet/piqa), [clean-fid](https://github.com/GaParmar/clean-fid)
 
 We also thanks the following public repositories: [MUSIQ](https://github.com/google-research/google-research/tree/master/musiq), [DBCNN](https://github.com/zwx8981/DBCNN-PyTorch), [NIMA](https://github.com/kentsyx/Neural-IMage-Assessment), [HyperIQA](https://github.com/SSL92/hyperIQA), [CNNIQA](https://github.com/lidq92/CNNIQA), [WaDIQaM](https://github.com/lidq92/WaDIQaM), [PieAPP](https://github.com/prashnani/PerceptualImageError), [paq2piq](https://github.com/baidut/paq2piq), [MANIQA](https://github.com/IIGROUP/MANIQA) 
 
 ## :e-mail: Contact
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,77 +1,86 @@
-Metadata-Version: 2.1 Name: pyiqa Version: 0.1.7 Summary: PyTorch Toolbox for
+Metadata-Version: 2.1 Name: pyiqa Version: 0.1.8 Summary: PyTorch Toolbox for
 Image Quality Assessment Home-page: https://github.com/chaofengc/IQA-PyTorch
 Author: Chaofeng Chen Author-email: chaofenghust@gmail.com License: UNKNOWN
 Keywords: image quality assessment,pytorch Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE License-File: LICENSE_NTU-S-Lab # PyTorch Toolbox for Image Quality
-Assessment An IQA toolbox with pure python and pytorch. Please refer to
-[Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-
-Quality-Assessment) for a comprehensive survey of IQA methods, as well as
-download links for IQA datasets. _[_g_o_o_g_l_e_ _c_o_l_a_b_ _l_o_g_o_][![PyPI](https://
-img.shields.io/pypi/v/pyiqa)](https://pypi.org/project/pyiqa/) ![visitors]
+LICENSE License-File: LICENSE_NTU-S-Lab # [docs/pyiqa_logo.jpg]PyTorch Toolbox
+for Image Quality Assessment An IQA toolbox with pure python and pytorch.
+Please refer to [Awesome-Image-Quality-Assessment](https://github.com/
+chaofengc/Awesome-Image-Quality-Assessment) for a comprehensive survey of IQA
+methods and download links for IQA datasets. _[_g_o_o_g_l_e_ _c_o_l_a_b_ _l_o_g_o_][![PyPI](https:
+//img.shields.io/pypi/v/pyiqa)](https://pypi.org/project/pyiqa/) ![visitors]
 (https://visitor-badge.laobi.icu/badge?page_id=chaofengc/IQA-PyTorch) [!
-[Awesome](https://cdn.rawgit.com/sindresorhus/awesome/
+[Documentation Status](https://readthedocs.org/projects/iqa-pytorch/badge/
+?version=latest)](https://iqa-pytorch.readthedocs.io/en/latest/?badge=latest)
+[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/
 d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/
 chaofengc/Awesome-Image-Quality-Assessment) [![Citation](https://
 img.shields.io/badge/Citation-bibtex-green)](https://github.com/chaofengc/IQA-
-PyTorch/blob/main/README.md#bookmark_tabs-citation) ![demo](demo.gif) - [:
+PyTorch/blob/main/README.md#bookmark_tabs-citation) ![demo](docs/demo.gif) - [:
 open\_book: Introduction](#open_book-introduction) - [:zap: Quick Start](#zap-
 quick-start) - [Dependencies and Installation](#dependencies-and-installation)
 - [Basic Usage](#basic-usage) - [:1st\_place\_medal: Benchmark Performances and
 Model Zoo](#1st_place_medal-benchmark-performances-and-model-zoo) - [Results
 Calibration](#results-calibration) - [Performance Evaluation Protocol]
 (#performance-evaluation-protocol) - [Benchmark Performance with Provided
 Script](#benchmark-performance-with-provided-script) - [:hammer\_and\_wrench:
 Train](#hammer_and_wrench-train) - [Dataset Preparation](#dataset-preparation)
 - [Example Train Script](#example-trai-script) ## :open_book: Introduction This
 is a image quality assessment toolbox with **pure python and pytorch**. We
 provide reimplementation of many mainstream full reference (FR) and no
 reference (NR) metrics (results are calibrated with official matlab scripts if
 exist). **With GPU acceleration, most of our implementations are much faster
-than Matlab.** Please refer to the [Model Cards](docs/ModelCard.md) and
-[Dataset Cards](docs/Dataset_Preparation.md) for all supported methods and
-datasets. --- ### :triangular_flag_on_post: Updates/Changelog - **March 30,
-2023**. Add [URanker](https://github.com/RQ-Wu/UnderwaterRanker) for IQA of
-under water images. - **March 29, 2023**. :rotating_light: Hot fix of NRQM &
-PI. - **March 25, 2023**. Add TreS, HyperIQA, CNNIQA, CLIPIQA. - **Sep 1,
-2022**. 1) Add pretrained models for MANIQA and AHIQ. 2) Add dataset interface
-for pieapp and PIPAL. - **June 3, 2022**. Add FID metric. See [clean-fid]
-(https://github.com/GaParmar/clean-fid) for more details. - **March 11, 2022**.
-Add pretrained DBCNN, NIMA, and official model of PieAPP, paq2piq. - [**More**]
-(docs/history_changelog.md) --- ## :zap: Quick Start ### Dependencies and
-Installation - Ubuntu >= 18.04 - Python >= 3.8 - Pytorch >= 1.10 - CUDA >= 10.2
-(if use GPU) ``` # Install with pip pip install pyiqa # Install latest github
-version pip uninstall pyiqa # if have older version installed already pip
-install git+https://github.com/chaofengc/IQA-PyTorch.git # Install with git
-clone git clone https://github.com/chaofengc/IQA-PyTorch.git cd IQA-PyTorch pip
-install -r requirements.txt python setup.py develop ``` ### Basic Usage ```
-import pyiqa import torch # list all available metrics print(pyiqa.list_models
-()) device = torch.device("cuda") if torch.cuda.is_available() else
-torch.device("cpu") # create metric with default setting iqa_metric =
-pyiqa.create_metric('lpips', device=device) # Note that gradient propagation is
-disabled by default. set as_loss=True to enable it as a loss function. iqa_loss
-= pyiqa.create_metric('lpips', device=device, as_loss=True) # create metric
-with custom setting iqa_metric = pyiqa.create_metric('psnr',
-test_y_channel=True, color_space='ycbcr').to(device) # check if lower better or
-higher better print(iqa_metric.lower_better) # example for iqa score inference
-# Tensor inputs, img_tensor_x/y: (N, 3, H, W), RGB, 0 ~ 1 score_fr = iqa_metric
-(img_tensor_x, img_tensor_y) score_nr = iqa_metric(img_tensor_x) # img path as
-inputs. score_fr = iqa_metric('./ResultsCalibra/dist_dir/I03.bmp', './
-ResultsCalibra/ref_dir/I03.bmp') # For FID metric, use directory or precomputed
-statistics as inputs # refer to clean-fid for more details: https://github.com/
-GaParmar/clean-fid fid_metric = pyiqa.create_metric('fid') score = fid_metric
-('./ResultsCalibra/dist_dir/', './ResultsCalibra/ref_dir') score = fid_metric
-('./ResultsCalibra/dist_dir/', dataset_name="FFHQ", dataset_res=1024,
+than Matlab.** Please refer to the following documents for details:
+     ð¦ [Model Cards](docs/ModelCard.md) | ðï¸ [Dataset Cards](docs/
+                            Dataset_Preparation.md)
+--- ### :triangular_flag_on_post: Updates/Changelog - **Oct 09, 2023**. Add
+datasets: [PIQ2023](https://github.com/DXOMARK-Research/PIQ2023), [GFIQA](http:
+//database.mmsp-kn.de/gfiqa-20k-database.html). Add metric `topiq_nr-face`. -
+**Aug 15, 2023**. Add `st-lpips` and `laion_aes`. Refer to official repo at
+[ShiftTolerant-LPIPS](https://github.com/abhijay9/ShiftTolerant-LPIPS) and
+[improved-aesthetic-predictor](https://github.com/christophschuhmann/improved-
+aesthetic-predictor) - **Aug 05, 2023**. Add our work [TOPIQ](https://
+arxiv.org/abs/2308.03060) with remarkable performance on almost all benchmarks
+via efficient Resnet50 backbone. Use it with `topiq_fr, topiq_nr, topiq_iaa`
+for Full-Reference, No-Reference and Aesthetic assessment respectively. -
+**March 30, 2023**. Add [URanker](https://github.com/RQ-Wu/UnderwaterRanker)
+for IQA of under water images. - **March 29, 2023**. :rotating_light: Hot fix
+of NRQM & PI. - **March 25, 2023**. Add TreS, HyperIQA, CNNIQA, CLIPIQA. -
+[**More**](docs/history_changelog.md) --- ## :zap: Quick Start ### Dependencies
+and Installation - Ubuntu >= 18.04 - Python >= 3.8 - PyTorch >= 1.12 -
+Torchvision >= 0.13 - CUDA >= 10.2 (if use GPU) ``` # Install with pip pip
+install pyiqa # Install latest github version pip uninstall pyiqa # if have
+older version installed already pip install git+https://github.com/chaofengc/
+IQA-PyTorch.git # Install with git clone git clone https://github.com/
+chaofengc/IQA-PyTorch.git cd IQA-PyTorch pip install -r requirements.txt python
+setup.py develop ``` ### Basic Usage ``` import pyiqa import torch # list all
+available metrics print(pyiqa.list_models()) device = torch.device("cuda") if
+torch.cuda.is_available() else torch.device("cpu") # create metric with default
+setting iqa_metric = pyiqa.create_metric('lpips', device=device) # Note that
+gradient propagation is disabled by default. set as_loss=True to enable it as a
+loss function. iqa_loss = pyiqa.create_metric('lpips', device=device,
+as_loss=True) # create metric with custom setting iqa_metric =
+pyiqa.create_metric('psnr', test_y_channel=True, color_space='ycbcr').to
+(device) # check if lower better or higher better print
+(iqa_metric.lower_better) # example for iqa score inference # Tensor inputs,
+img_tensor_x/y: (N, 3, H, W), RGB, 0 ~ 1 score_fr = iqa_metric(img_tensor_x,
+img_tensor_y) score_nr = iqa_metric(img_tensor_x) # img path as inputs.
+score_fr = iqa_metric('./ResultsCalibra/dist_dir/I03.bmp', './ResultsCalibra/
+ref_dir/I03.bmp') # For FID metric, use directory or precomputed statistics as
+inputs # refer to clean-fid for more details: https://github.com/GaParmar/
+clean-fid fid_metric = pyiqa.create_metric('fid') score = fid_metric('./
+ResultsCalibra/dist_dir/', './ResultsCalibra/ref_dir') score = fid_metric('./
+ResultsCalibra/dist_dir/', dataset_name="FFHQ", dataset_res=1024,
 dataset_split="trainval70k") ``` #### Example Test script Example test script
 with input directory/images and reference directory/images. ``` # example for
 FR metric with dirs python inference_iqa.py -m LPIPS[or lpips] -i ./
 ResultsCalibra/dist_dir[dist_img] -r ./ResultsCalibra/ref_dir[ref_img] #
 example for NR metric with single image python inference_iqa.py -m brisque -
 i ./ResultsCalibra/dist_dir/I03.bmp ``` ## :1st_place_medal: Benchmark
 Performances and Model Zoo ### Results Calibration Please refer to the [results
@@ -80,74 +89,83 @@
 ### Performance Evaluation Protocol **We use official models for evaluation if
 available.** Otherwise, we use the following settings to train and evaluate
 different models for simplicity and consistency: | Metric Type | Train | Test |
 Results | | ------------- | --------- | ---------------------------------------
 --- | -------------------------------------------------------- | | FR | KADID-
 10k | CSIQ, LIVE, TID2008, TID2013 | [FR benchmark results](tests/
 FR_benchmark_results.csv) | | NR | KonIQ-10k | LIVEC, KonIQ-10k (official
-split), TID2013 | [NR benchmark results](tests/NR_benchmark_results.csv) | |
-Aesthetic IQA | AVA | AVA (official split) | [IAA benchmark results](tests/
-IAA_benchmark_results.csv) | Basically, we use the largest existing datasets
-for training, and cross dataset evaluation performance for fair comparison. The
-following models do not provide official weights, and are retrained by our
-scripts: | Metric Type | Model Names | | ------------- | ----------------------
-------- | | FR | | | NR | `cnniqa`, `dbcnn`, `hyperiqa` | | Aesthetic IQA |
-`nima`, `nima-vgg16-ava` | Notes: - Due to optimized training process,
-performance of some retrained approaches may be higher than original paper. -
-Results of KonIQ-10k, AVA are both tested with official split. - NIMA is only
-applicable to AVA dataset now. We use `inception_resnet_v2` for default `nima`.
-- MUSIQ is not included in the IAA benchmark because we do not have train/split
-information of the official model. ### Benchmark Performance with Provided
-Script Here is an example script to get performance benchmark on different
-datasets: ``` # NOTE: this script will test ALL specified metrics on ALL
-specified datasets # Test default metrics on default datasets python
-benchmark_results.py -m psnr ssim -d csiq tid2013 tid2008 # Test with your own
-options python benchmark_results.py -m psnr --data_opt options/
-example_benchmark_data_opts.yml python benchmark_results.py --metric_opt
-options/example_benchmark_metric_opts.yml tid2013 tid2008 python
+split), TID2013, SPAQ | [NR benchmark results](tests/NR_benchmark_results.csv)
+| | Aesthetic IQA | AVA | AVA (official split) | [IAA benchmark results](tests/
+IAA_benchmark_results.csv) | Results are calculated with: - **PLCC without any
+correction**. Although test time value correction is common in IQA papers, we
+want to use the original value in our benchmark. - **Full image single input.**
+We use multi-patch testing only when it is necessary for the model to work.
+Basically, we use the largest existing datasets for training, and cross dataset
+evaluation performance for fair comparison. The following models do not provide
+official weights, and are retrained by our scripts: | Metric Type | Reproduced
+Models | | ------------- | ----------------------------- | | FR | | | NR |
+`cnniqa`, `dbcnn`, `hyperiqa` | | Aesthetic IQA | `nima`, `nima-vgg16-ava` |
+**Important Notes:** - Due to optimized training process, performance of some
+retrained approaches may be different with original paper. - Results of all
+**retrained models by ours** are normalized to [0, 1] and change to higher
+better for convenience. - Results of KonIQ-10k, AVA are both tested with
+official split. - NIMA is only applicable to AVA dataset now. We use
+`inception_resnet_v2` for default `nima`. - MUSIQ is not included in the IAA
+benchmark because we do not have train/split information of the official model.
+### Benchmark Performance with Provided Script Here is an example script to get
+performance benchmark on different datasets: ``` # NOTE: this script will test
+ALL specified metrics on ALL specified datasets # Test default metrics on
+default datasets python benchmark_results.py -m psnr ssim -d csiq tid2013
+tid2008 # Test with your own options python benchmark_results.py -m psnr --
+data_opt options/example_benchmark_data_opts.yml python benchmark_results.py --
+metric_opt options/example_benchmark_metric_opts.yml tid2013 tid2008 python
 benchmark_results.py --metric_opt options/example_benchmark_metric_opts.yml --
 data_opt options/example_benchmark_data_opts.yml ``` ## :hammer_and_wrench:
 Train ### Dataset Preparation - You only need to unzip downloaded datasets from
 official website without any extra operation. And then make soft links of these
 dataset folder under `datasets/` folder. Download links are provided in
 [Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-
 Quality-Assessment). - We provide common interface to load these datasets with
 the prepared meta information files and train/val/test split files, which can
 be downloaded from [download_link](https://github.com/chaofengc/IQA-PyTorch/
-releases/download/v0.1-weights/data_info_files.tgz) and extract them to
-`datasets/` folder. You may also use the following commands: ``` mkdir datasets
-&& cd datasets # make soft links of your dataset ln -sf your/dataset/path
-datasetname # download meta info files and train split files wget https://
-github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/
-data_info_files.tgz tar -xvf data_info_files.tgz ``` Examples to specific
-dataset options can be found in `./options/default_dataset_opt.yml`. Details of
-the dataloader inferface and meta information files can be found in [Dataset
-Preparation](docs/Dataset_Preparation.md) ### Example Train Script Example to
-train DBCNN on LIVEChallenge dataset ``` # train for single experiment python
-pyiqa/train.py -opt options/train/DBCNN/train_DBCNN.yml # train N splits for
-small datasets python pyiqa/train_nsplits.py -opt options/train/DBCNN/
-train_DBCNN.yml ``` ## :beers: Contribution Any contributions to this
-repository are greatly appreciated. Please follow the [contribution
-instructions](docs/Instruction.md) for contribution guidance. ## :scroll:
-License This work is licensed under a [NTU S-Lab License](https://github.com/
-chaofengc/IQA-PyTorch/blob/main/LICENSE_NTU-S-Lab) and _C_r_e_a_t_i_v_e_ _C_o_m_m_o_n_s
-_A_t_t_r_i_b_u_t_i_o_n_-_N_o_n_C_o_m_m_e_r_c_i_a_l_-_S_h_a_r_e_A_l_i_k_e_ _4_._0_ _I_n_t_e_r_n_a_t_i_o_n_a_l_ _L_i_c_e_n_s_e. _[_C_r_e_a_t_i_v_e
-_C_o_m_m_o_n_s_ _L_i_c_e_n_s_e_]## :bookmark_tabs: Citation If you find our codes helpful to
-your research, please consider to use the following citation: ``` @misc{pyiqa,
-title={{IQA-PyTorch}: PyTorch Toolbox for Image Quality Assessment}, author=
-{Chaofeng Chen and Jiadi Mo}, year={2022}, howpublished = "[Online]. Available:
-\url{https://github.com/chaofengc/IQA-PyTorch}" } ``` ## :heart:
-Acknowledgement The code architecture is borrowed from [BasicSR](https://
-github.com/xinntao/BasicSR). Several implementations are taken from: [IQA-
-optimization](https://github.com/dingkeyan93/IQA-optimization), [Image-Quality-
-Assessment-Toolbox](https://github.com/RyanXingQL/Image-Quality-Assessment-
-Toolbox), [piq](https://github.com/photosynthesis-team/piq), [piqa](https://
-github.com/francois-rozet/piqa), [clean-fid](https://github.com/GaParmar/clean-
-fid) We also thanks the following public repositories: [MUSIQ](https://
-github.com/google-research/google-research/tree/master/musiq), [DBCNN](https://
-github.com/zwx8981/DBCNN-PyTorch), [NIMA](https://github.com/kentsyx/Neural-
-IMage-Assessment), [HyperIQA](https://github.com/SSL92/hyperIQA), [CNNIQA]
-(https://github.com/lidq92/CNNIQA), [WaDIQaM](https://github.com/lidq92/
-WaDIQaM), [PieAPP](https://github.com/prashnani/PerceptualImageError),
-[paq2piq](https://github.com/baidut/paq2piq), [MANIQA](https://github.com/
-IIGROUP/MANIQA) ## :e-mail: Contact If you have any questions, please email
-`chaofenghust@gmail.com`
+releases/download/v0.1-weights/meta_info.tgz) and extract them to `datasets/
+` folder. You may also use the following commands: ``` mkdir datasets && cd
+datasets # make soft links of your dataset ln -sf your/dataset/path datasetname
+# download meta info files and train split files wget https://github.com/
+chaofengc/IQA-PyTorch/releases/download/v0.1-weights/meta_info.tgz tar -xvf
+data_info_files.tgz ``` Examples to specific dataset options can be found in
+`./options/default_dataset_opt.yml`. Details of the dataloader inferface and
+meta information files can be found in [Dataset Preparation](docs/
+Dataset_Preparation.md) ### Example Train Script Example to train DBCNN on
+LIVEChallenge dataset ``` # train for single experiment python pyiqa/train.py -
+opt options/train/DBCNN/train_DBCNN.yml # train N splits for small datasets
+python pyiqa/train_nsplits.py -opt options/train/DBCNN/train_DBCNN.yml ``` ## :
+beers: Contribution Any contributions to this repository are greatly
+appreciated. Please follow the [contribution instructions](docs/Instruction.md)
+for contribution guidance. ## :scroll: License This work is licensed under a
+[NTU S-Lab License](https://github.com/chaofengc/IQA-PyTorch/blob/main/
+LICENSE_NTU-S-Lab) and _C_r_e_a_t_i_v_e_ _C_o_m_m_o_n_s_ _A_t_t_r_i_b_u_t_i_o_n_-_N_o_n_C_o_m_m_e_r_c_i_a_l_-_S_h_a_r_e_A_l_i_k_e
+_4_._0_ _I_n_t_e_r_n_a_t_i_o_n_a_l_ _L_i_c_e_n_s_e. _[_C_r_e_a_t_i_v_e_ _C_o_m_m_o_n_s_ _L_i_c_e_n_s_e_]## :bookmark_tabs:
+Citation If you find our codes helpful to your research, please consider to use
+the following citation: ``` @misc{pyiqa, title={{IQA-PyTorch}: PyTorch Toolbox
+for Image Quality Assessment}, author={Chaofeng Chen and Jiadi Mo}, year=
+{2022}, howpublished = "[Online]. Available: \url{https://github.com/chaofengc/
+IQA-PyTorch}" } ``` Please also consider to cite our new work `TOPIQ` if it is
+useful to you: ``` @misc{chen2023topiq, title={TOPIQ: A Top-down Approach from
+Semantics to Distortions for Image Quality Assessment}, author={Chaofeng Chen
+and Jiadi Mo and Jingwen Hou and Haoning Wu and Liang Liao and Wenxiu Sun and
+Qiong Yan and Weisi Lin}, year={2023}, eprint={2308.03060}, archivePrefix=
+{arXiv}, primaryClass={cs.CV} } ``` ## :heart: Acknowledgement The code
+architecture is borrowed from [BasicSR](https://github.com/xinntao/BasicSR).
+Several implementations are taken from: [IQA-optimization](https://github.com/
+dingkeyan93/IQA-optimization), [Image-Quality-Assessment-Toolbox](https://
+github.com/RyanXingQL/Image-Quality-Assessment-Toolbox), [piq](https://
+github.com/photosynthesis-team/piq), [piqa](https://github.com/francois-rozet/
+piqa), [clean-fid](https://github.com/GaParmar/clean-fid) We also thanks the
+following public repositories: [MUSIQ](https://github.com/google-research/
+google-research/tree/master/musiq), [DBCNN](https://github.com/zwx8981/DBCNN-
+PyTorch), [NIMA](https://github.com/kentsyx/Neural-IMage-Assessment),
+[HyperIQA](https://github.com/SSL92/hyperIQA), [CNNIQA](https://github.com/
+lidq92/CNNIQA), [WaDIQaM](https://github.com/lidq92/WaDIQaM), [PieAPP](https://
+github.com/prashnani/PerceptualImageError), [paq2piq](https://github.com/
+baidut/paq2piq), [MANIQA](https://github.com/IIGROUP/MANIQA) ## :e-mail:
+Contact If you have any questions, please email `chaofenghust@gmail.com`
```

### Comparing `pyiqa-0.1.7/README.md` & `pyiqa-0.1.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# PyTorch Toolbox for Image Quality Assessment
+# <img align="left" width="100" height="100" src="docs/pyiqa_logo.jpg"> PyTorch Toolbox for Image Quality Assessment
 
-An IQA toolbox with pure python and pytorch. Please refer to [Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-Quality-Assessment) for a comprehensive survey of IQA methods, as well as download links for IQA datasets.
+An IQA toolbox with pure python and pytorch. Please refer to [Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-Quality-Assessment) for a comprehensive survey of IQA methods and download links for IQA datasets.
 
 <a href="https://colab.research.google.com/drive/14J3KoyrjJ6R531DsdOy5Bza5xfeMODi6?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="google colab logo"></a> 
 [![PyPI](https://img.shields.io/pypi/v/pyiqa)](https://pypi.org/project/pyiqa/)
 ![visitors](https://visitor-badge.laobi.icu/badge?page_id=chaofengc/IQA-PyTorch) 
+[![Documentation Status](https://readthedocs.org/projects/iqa-pytorch/badge/?version=latest)](https://iqa-pytorch.readthedocs.io/en/latest/?badge=latest)
 [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/chaofengc/Awesome-Image-Quality-Assessment)
 [![Citation](https://img.shields.io/badge/Citation-bibtex-green)](https://github.com/chaofengc/IQA-PyTorch/blob/main/README.md#bookmark_tabs-citation)
 
-![demo](demo.gif)
+![demo](docs/demo.gif)
 
 - [:open\_book: Introduction](#open_book-introduction)
 - [:zap: Quick Start](#zap-quick-start)
   - [Dependencies and Installation](#dependencies-and-installation)
   - [Basic Usage](#basic-usage)
 - [:1st\_place\_medal: Benchmark Performances and Model Zoo](#1st_place_medal-benchmark-performances-and-model-zoo)
   - [Results Calibration](#results-calibration)
@@ -20,36 +21,42 @@
   - [Benchmark Performance with Provided Script](#benchmark-performance-with-provided-script)
 - [:hammer\_and\_wrench: Train](#hammer_and_wrench-train)
   - [Dataset Preparation](#dataset-preparation)
   - [Example Train Script](#example-trai-script)
  
 ## :open_book: Introduction
 
-This is a image quality assessment toolbox with **pure python and pytorch**. We provide reimplementation of many mainstream full reference (FR) and no reference (NR) metrics (results are calibrated with official matlab scripts if exist). **With GPU acceleration, most of our implementations are much faster than Matlab.** Please refer to the [Model Cards](docs/ModelCard.md) and [Dataset Cards](docs/Dataset_Preparation.md) for all supported methods and datasets.
+This is a image quality assessment toolbox with **pure python and pytorch**. We provide reimplementation of many mainstream full reference (FR) and no reference (NR) metrics (results are calibrated with official matlab scripts if exist). **With GPU acceleration, most of our implementations are much faster than Matlab.** Please refer to the following documents for details:  
+
+<div align="center">
+
+📦 [Model Cards](docs/ModelCard.md)  |  🗃️ [Dataset Cards](docs/Dataset_Preparation.md) 
+
+</div>
 
 ---
 
 ### :triangular_flag_on_post: Updates/Changelog
-
+- **Oct 09, 2023**. Add datasets: [PIQ2023](https://github.com/DXOMARK-Research/PIQ2023), [GFIQA](http://database.mmsp-kn.de/gfiqa-20k-database.html). Add metric `topiq_nr-face`. 
+- **Aug 15, 2023**. Add `st-lpips` and `laion_aes`. Refer to official repo at [ShiftTolerant-LPIPS](https://github.com/abhijay9/ShiftTolerant-LPIPS) and [improved-aesthetic-predictor](https://github.com/christophschuhmann/improved-aesthetic-predictor)
+- **Aug 05, 2023**. Add our work [TOPIQ](https://arxiv.org/abs/2308.03060) with remarkable performance on almost all benchmarks via efficient Resnet50 backbone. Use it with `topiq_fr, topiq_nr, topiq_iaa` for Full-Reference, No-Reference and Aesthetic assessment respectively.
 - **March 30, 2023**. Add [URanker](https://github.com/RQ-Wu/UnderwaterRanker) for IQA of under water images. 
 - **March 29, 2023**. :rotating_light: Hot fix of NRQM & PI. 
 - **March 25, 2023**. Add TreS, HyperIQA, CNNIQA, CLIPIQA.
-- **Sep 1, 2022**. 1) Add pretrained models for MANIQA and AHIQ. 2) Add dataset interface for pieapp and PIPAL.
-- **June 3, 2022**. Add FID metric. See [clean-fid](https://github.com/GaParmar/clean-fid) for more details.
-- **March 11, 2022**. Add pretrained DBCNN, NIMA, and official model of PieAPP, paq2piq.
 - [**More**](docs/history_changelog.md)
 
 ---
 
 ## :zap: Quick Start
 
 ### Dependencies and Installation
 - Ubuntu >= 18.04
 - Python >= 3.8
-- Pytorch >= 1.10
+- PyTorch >= 1.12
+- Torchvision >= 0.13
 - CUDA >= 10.2 (if use GPU)
 ```
 # Install with pip
 pip install pyiqa
 
 # Install latest github version
 pip uninstall pyiqa # if have older version installed already 
@@ -116,30 +123,35 @@
 
 Please refer to the [results calibration](./ResultsCalibra/ResultsCalibra.md) to verify the correctness of the python implementations compared with official scripts in matlab or python.
 
 ### Performance Evaluation Protocol
 
 **We use official models for evaluation if available.** Otherwise, we use the following settings to train and evaluate different models for simplicity and consistency:
 
-| Metric Type   | Train     | Test                                       | Results                                                  |
+| Metric Type   | Train     | Test                                       | Results                                                  | 
 | ------------- | --------- | ------------------------------------------ | -------------------------------------------------------- |
 | FR            | KADID-10k | CSIQ, LIVE, TID2008, TID2013               | [FR benchmark results](tests/FR_benchmark_results.csv)   |
-| NR            | KonIQ-10k | LIVEC, KonIQ-10k (official split), TID2013 | [NR benchmark results](tests/NR_benchmark_results.csv)   |
+| NR            | KonIQ-10k | LIVEC, KonIQ-10k (official split), TID2013, SPAQ | [NR benchmark results](tests/NR_benchmark_results.csv)   |
 | Aesthetic IQA | AVA       | AVA (official split)                       | [IAA benchmark results](tests/IAA_benchmark_results.csv) |
 
+Results are calculated with:
+- **PLCC without any correction**. Although test time value correction is common in IQA papers, we want to use the original value in our benchmark.
+- **Full image single input.** We use multi-patch testing only when it is necessary for the model to work.
+
 Basically, we use the largest existing datasets for training, and cross dataset evaluation performance for fair comparison. The following models do not provide official weights, and are retrained by our scripts:
 
-| Metric Type   | Model Names                   |
+| Metric Type   | Reproduced Models |
 | ------------- | ----------------------------- |
 | FR            |                               |
 | NR            | `cnniqa`, `dbcnn`, `hyperiqa` |
 | Aesthetic IQA | `nima`, `nima-vgg16-ava`      |
 
-Notes:
-- Due to optimized training process, performance of some retrained approaches may be higher than original paper.
+**Important Notes:**
+- Due to optimized training process, performance of some retrained approaches may be different with original paper.
+- Results of all **retrained models by ours** are normalized to [0, 1] and change to higher better for convenience.
 - Results of KonIQ-10k, AVA are both tested with official split.
 - NIMA is only applicable to AVA dataset now. We use `inception_resnet_v2` for default `nima`.
 - MUSIQ is not included in the IAA benchmark because we do not have train/split information of the official model.
 
 ### Benchmark Performance with Provided Script
 
 Here is an example script to get performance benchmark on different datasets:
@@ -157,26 +169,26 @@
 ```
 
 ## :hammer_and_wrench: Train
 
 ### Dataset Preparation
 
 - You only need to unzip downloaded datasets from official website without any extra operation. And then make soft links of these dataset folder under `datasets/` folder. Download links are provided in [Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-Quality-Assessment).
-- We provide common interface to load these datasets with the prepared meta information files and train/val/test split files, which can be downloaded from [download_link](https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/data_info_files.tgz) and extract them to `datasets/` folder.
+- We provide common interface to load these datasets with the prepared meta information files and train/val/test split files, which can be downloaded from [download_link](https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/meta_info.tgz) and extract them to `datasets/` folder.
 
 You may also use the following commands:
 
 ```
 mkdir datasets && cd datasets
 
 # make soft links of your dataset
 ln -sf your/dataset/path datasetname
 
 # download meta info files and train split files
-wget https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/data_info_files.tgz
+wget https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/meta_info.tgz
 tar -xvf data_info_files.tgz
 ```
 
 Examples to specific dataset options can be found in `./options/default_dataset_opt.yml`. Details of the dataloader inferface and meta information files can be found in [Dataset Preparation](docs/Dataset_Preparation.md)
 
 ### Example Train Script
 
@@ -209,14 +221,26 @@
   title={{IQA-PyTorch}: PyTorch Toolbox for Image Quality Assessment},
   author={Chaofeng Chen and Jiadi Mo},
   year={2022},
   howpublished = "[Online]. Available: \url{https://github.com/chaofengc/IQA-PyTorch}"
 }
 ```
 
+Please also consider to cite our new work `TOPIQ` if it is useful to you:
+```
+@misc{chen2023topiq,
+      title={TOPIQ: A Top-down Approach from Semantics to Distortions for Image Quality Assessment}, 
+      author={Chaofeng Chen and Jiadi Mo and Jingwen Hou and Haoning Wu and Liang Liao and Wenxiu Sun and Qiong Yan and Weisi Lin},
+      year={2023},
+      eprint={2308.03060},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+}
+``` 
+
 ## :heart: Acknowledgement
 
 The code architecture is borrowed from [BasicSR](https://github.com/xinntao/BasicSR). Several implementations are taken from: [IQA-optimization](https://github.com/dingkeyan93/IQA-optimization), [Image-Quality-Assessment-Toolbox](https://github.com/RyanXingQL/Image-Quality-Assessment-Toolbox), [piq](https://github.com/photosynthesis-team/piq), [piqa](https://github.com/francois-rozet/piqa), [clean-fid](https://github.com/GaParmar/clean-fid)
 
 We also thanks the following public repositories: [MUSIQ](https://github.com/google-research/google-research/tree/master/musiq), [DBCNN](https://github.com/zwx8981/DBCNN-PyTorch), [NIMA](https://github.com/kentsyx/Neural-IMage-Assessment), [HyperIQA](https://github.com/SSL92/hyperIQA), [CNNIQA](https://github.com/lidq92/CNNIQA), [WaDIQaM](https://github.com/lidq92/WaDIQaM), [PieAPP](https://github.com/prashnani/PerceptualImageError), [paq2piq](https://github.com/baidut/paq2piq), [MANIQA](https://github.com/IIGROUP/MANIQA) 
 
 ## :e-mail: Contact
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,50 +1,59 @@
-# PyTorch Toolbox for Image Quality Assessment An IQA toolbox with pure python
-and pytorch. Please refer to [Awesome-Image-Quality-Assessment](https://
-github.com/chaofengc/Awesome-Image-Quality-Assessment) for a comprehensive
-survey of IQA methods, as well as download links for IQA datasets. _[_g_o_o_g_l_e
-_c_o_l_a_b_ _l_o_g_o_][![PyPI](https://img.shields.io/pypi/v/pyiqa)](https://pypi.org/
-project/pyiqa/) ![visitors](https://visitor-badge.laobi.icu/
-badge?page_id=chaofengc/IQA-PyTorch) [![Awesome](https://cdn.rawgit.com/
-sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)]
-(https://github.com/chaofengc/Awesome-Image-Quality-Assessment) [![Citation]
-(https://img.shields.io/badge/Citation-bibtex-green)](https://github.com/
-chaofengc/IQA-PyTorch/blob/main/README.md#bookmark_tabs-citation) ![demo]
-(demo.gif) - [:open\_book: Introduction](#open_book-introduction) - [:zap:
-Quick Start](#zap-quick-start) - [Dependencies and Installation](#dependencies-
-and-installation) - [Basic Usage](#basic-usage) - [:1st\_place\_medal:
-Benchmark Performances and Model Zoo](#1st_place_medal-benchmark-performances-
-and-model-zoo) - [Results Calibration](#results-calibration) - [Performance
-Evaluation Protocol](#performance-evaluation-protocol) - [Benchmark Performance
-with Provided Script](#benchmark-performance-with-provided-script) - [:
-hammer\_and\_wrench: Train](#hammer_and_wrench-train) - [Dataset Preparation]
-(#dataset-preparation) - [Example Train Script](#example-trai-script) ## :
-open_book: Introduction This is a image quality assessment toolbox with **pure
-python and pytorch**. We provide reimplementation of many mainstream full
-reference (FR) and no reference (NR) metrics (results are calibrated with
-official matlab scripts if exist). **With GPU acceleration, most of our
-implementations are much faster than Matlab.** Please refer to the [Model
-Cards](docs/ModelCard.md) and [Dataset Cards](docs/Dataset_Preparation.md) for
-all supported methods and datasets. --- ### :triangular_flag_on_post: Updates/
-Changelog - **March 30, 2023**. Add [URanker](https://github.com/RQ-Wu/
-UnderwaterRanker) for IQA of under water images. - **March 29, 2023**. :
-rotating_light: Hot fix of NRQM & PI. - **March 25, 2023**. Add TreS, HyperIQA,
-CNNIQA, CLIPIQA. - **Sep 1, 2022**. 1) Add pretrained models for MANIQA and
-AHIQ. 2) Add dataset interface for pieapp and PIPAL. - **June 3, 2022**. Add
-FID metric. See [clean-fid](https://github.com/GaParmar/clean-fid) for more
-details. - **March 11, 2022**. Add pretrained DBCNN, NIMA, and official model
-of PieAPP, paq2piq. - [**More**](docs/history_changelog.md) --- ## :zap: Quick
-Start ### Dependencies and Installation - Ubuntu >= 18.04 - Python >= 3.8 -
-Pytorch >= 1.10 - CUDA >= 10.2 (if use GPU) ``` # Install with pip pip install
-pyiqa # Install latest github version pip uninstall pyiqa # if have older
-version installed already pip install git+https://github.com/chaofengc/IQA-
-PyTorch.git # Install with git clone git clone https://github.com/chaofengc/
-IQA-PyTorch.git cd IQA-PyTorch pip install -r requirements.txt python setup.py
-develop ``` ### Basic Usage ``` import pyiqa import torch # list all available
-metrics print(pyiqa.list_models()) device = torch.device("cuda") if
+# [docs/pyiqa_logo.jpg]PyTorch Toolbox for Image Quality Assessment An IQA
+toolbox with pure python and pytorch. Please refer to [Awesome-Image-Quality-
+Assessment](https://github.com/chaofengc/Awesome-Image-Quality-Assessment) for
+a comprehensive survey of IQA methods and download links for IQA datasets.
+_[_g_o_o_g_l_e_ _c_o_l_a_b_ _l_o_g_o_][![PyPI](https://img.shields.io/pypi/v/pyiqa)](https://
+pypi.org/project/pyiqa/) ![visitors](https://visitor-badge.laobi.icu/
+badge?page_id=chaofengc/IQA-PyTorch) [![Documentation Status](https://
+readthedocs.org/projects/iqa-pytorch/badge/?version=latest)](https://iqa-
+pytorch.readthedocs.io/en/latest/?badge=latest) [![Awesome](https://
+cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/
+media/badge.svg)](https://github.com/chaofengc/Awesome-Image-Quality-
+Assessment) [![Citation](https://img.shields.io/badge/Citation-bibtex-green)]
+(https://github.com/chaofengc/IQA-PyTorch/blob/main/README.md#bookmark_tabs-
+citation) ![demo](docs/demo.gif) - [:open\_book: Introduction](#open_book-
+introduction) - [:zap: Quick Start](#zap-quick-start) - [Dependencies and
+Installation](#dependencies-and-installation) - [Basic Usage](#basic-usage) -
+[:1st\_place\_medal: Benchmark Performances and Model Zoo](#1st_place_medal-
+benchmark-performances-and-model-zoo) - [Results Calibration](#results-
+calibration) - [Performance Evaluation Protocol](#performance-evaluation-
+protocol) - [Benchmark Performance with Provided Script](#benchmark-
+performance-with-provided-script) - [:hammer\_and\_wrench: Train]
+(#hammer_and_wrench-train) - [Dataset Preparation](#dataset-preparation) -
+[Example Train Script](#example-trai-script) ## :open_book: Introduction This
+is a image quality assessment toolbox with **pure python and pytorch**. We
+provide reimplementation of many mainstream full reference (FR) and no
+reference (NR) metrics (results are calibrated with official matlab scripts if
+exist). **With GPU acceleration, most of our implementations are much faster
+than Matlab.** Please refer to the following documents for details:
+     ð¦ [Model Cards](docs/ModelCard.md) | ðï¸ [Dataset Cards](docs/
+                            Dataset_Preparation.md)
+--- ### :triangular_flag_on_post: Updates/Changelog - **Oct 09, 2023**. Add
+datasets: [PIQ2023](https://github.com/DXOMARK-Research/PIQ2023), [GFIQA](http:
+//database.mmsp-kn.de/gfiqa-20k-database.html). Add metric `topiq_nr-face`. -
+**Aug 15, 2023**. Add `st-lpips` and `laion_aes`. Refer to official repo at
+[ShiftTolerant-LPIPS](https://github.com/abhijay9/ShiftTolerant-LPIPS) and
+[improved-aesthetic-predictor](https://github.com/christophschuhmann/improved-
+aesthetic-predictor) - **Aug 05, 2023**. Add our work [TOPIQ](https://
+arxiv.org/abs/2308.03060) with remarkable performance on almost all benchmarks
+via efficient Resnet50 backbone. Use it with `topiq_fr, topiq_nr, topiq_iaa`
+for Full-Reference, No-Reference and Aesthetic assessment respectively. -
+**March 30, 2023**. Add [URanker](https://github.com/RQ-Wu/UnderwaterRanker)
+for IQA of under water images. - **March 29, 2023**. :rotating_light: Hot fix
+of NRQM & PI. - **March 25, 2023**. Add TreS, HyperIQA, CNNIQA, CLIPIQA. -
+[**More**](docs/history_changelog.md) --- ## :zap: Quick Start ### Dependencies
+and Installation - Ubuntu >= 18.04 - Python >= 3.8 - PyTorch >= 1.12 -
+Torchvision >= 0.13 - CUDA >= 10.2 (if use GPU) ``` # Install with pip pip
+install pyiqa # Install latest github version pip uninstall pyiqa # if have
+older version installed already pip install git+https://github.com/chaofengc/
+IQA-PyTorch.git # Install with git clone git clone https://github.com/
+chaofengc/IQA-PyTorch.git cd IQA-PyTorch pip install -r requirements.txt python
+setup.py develop ``` ### Basic Usage ``` import pyiqa import torch # list all
+available metrics print(pyiqa.list_models()) device = torch.device("cuda") if
 torch.cuda.is_available() else torch.device("cpu") # create metric with default
 setting iqa_metric = pyiqa.create_metric('lpips', device=device) # Note that
 gradient propagation is disabled by default. set as_loss=True to enable it as a
 loss function. iqa_loss = pyiqa.create_metric('lpips', device=device,
 as_loss=True) # create metric with custom setting iqa_metric =
 pyiqa.create_metric('psnr', test_y_channel=True, color_space='ycbcr').to
 (device) # check if lower better or higher better print
@@ -69,74 +78,83 @@
 ### Performance Evaluation Protocol **We use official models for evaluation if
 available.** Otherwise, we use the following settings to train and evaluate
 different models for simplicity and consistency: | Metric Type | Train | Test |
 Results | | ------------- | --------- | ---------------------------------------
 --- | -------------------------------------------------------- | | FR | KADID-
 10k | CSIQ, LIVE, TID2008, TID2013 | [FR benchmark results](tests/
 FR_benchmark_results.csv) | | NR | KonIQ-10k | LIVEC, KonIQ-10k (official
-split), TID2013 | [NR benchmark results](tests/NR_benchmark_results.csv) | |
-Aesthetic IQA | AVA | AVA (official split) | [IAA benchmark results](tests/
-IAA_benchmark_results.csv) | Basically, we use the largest existing datasets
-for training, and cross dataset evaluation performance for fair comparison. The
-following models do not provide official weights, and are retrained by our
-scripts: | Metric Type | Model Names | | ------------- | ----------------------
-------- | | FR | | | NR | `cnniqa`, `dbcnn`, `hyperiqa` | | Aesthetic IQA |
-`nima`, `nima-vgg16-ava` | Notes: - Due to optimized training process,
-performance of some retrained approaches may be higher than original paper. -
-Results of KonIQ-10k, AVA are both tested with official split. - NIMA is only
-applicable to AVA dataset now. We use `inception_resnet_v2` for default `nima`.
-- MUSIQ is not included in the IAA benchmark because we do not have train/split
-information of the official model. ### Benchmark Performance with Provided
-Script Here is an example script to get performance benchmark on different
-datasets: ``` # NOTE: this script will test ALL specified metrics on ALL
-specified datasets # Test default metrics on default datasets python
-benchmark_results.py -m psnr ssim -d csiq tid2013 tid2008 # Test with your own
-options python benchmark_results.py -m psnr --data_opt options/
-example_benchmark_data_opts.yml python benchmark_results.py --metric_opt
-options/example_benchmark_metric_opts.yml tid2013 tid2008 python
+split), TID2013, SPAQ | [NR benchmark results](tests/NR_benchmark_results.csv)
+| | Aesthetic IQA | AVA | AVA (official split) | [IAA benchmark results](tests/
+IAA_benchmark_results.csv) | Results are calculated with: - **PLCC without any
+correction**. Although test time value correction is common in IQA papers, we
+want to use the original value in our benchmark. - **Full image single input.**
+We use multi-patch testing only when it is necessary for the model to work.
+Basically, we use the largest existing datasets for training, and cross dataset
+evaluation performance for fair comparison. The following models do not provide
+official weights, and are retrained by our scripts: | Metric Type | Reproduced
+Models | | ------------- | ----------------------------- | | FR | | | NR |
+`cnniqa`, `dbcnn`, `hyperiqa` | | Aesthetic IQA | `nima`, `nima-vgg16-ava` |
+**Important Notes:** - Due to optimized training process, performance of some
+retrained approaches may be different with original paper. - Results of all
+**retrained models by ours** are normalized to [0, 1] and change to higher
+better for convenience. - Results of KonIQ-10k, AVA are both tested with
+official split. - NIMA is only applicable to AVA dataset now. We use
+`inception_resnet_v2` for default `nima`. - MUSIQ is not included in the IAA
+benchmark because we do not have train/split information of the official model.
+### Benchmark Performance with Provided Script Here is an example script to get
+performance benchmark on different datasets: ``` # NOTE: this script will test
+ALL specified metrics on ALL specified datasets # Test default metrics on
+default datasets python benchmark_results.py -m psnr ssim -d csiq tid2013
+tid2008 # Test with your own options python benchmark_results.py -m psnr --
+data_opt options/example_benchmark_data_opts.yml python benchmark_results.py --
+metric_opt options/example_benchmark_metric_opts.yml tid2013 tid2008 python
 benchmark_results.py --metric_opt options/example_benchmark_metric_opts.yml --
 data_opt options/example_benchmark_data_opts.yml ``` ## :hammer_and_wrench:
 Train ### Dataset Preparation - You only need to unzip downloaded datasets from
 official website without any extra operation. And then make soft links of these
 dataset folder under `datasets/` folder. Download links are provided in
 [Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-
 Quality-Assessment). - We provide common interface to load these datasets with
 the prepared meta information files and train/val/test split files, which can
 be downloaded from [download_link](https://github.com/chaofengc/IQA-PyTorch/
-releases/download/v0.1-weights/data_info_files.tgz) and extract them to
-`datasets/` folder. You may also use the following commands: ``` mkdir datasets
-&& cd datasets # make soft links of your dataset ln -sf your/dataset/path
-datasetname # download meta info files and train split files wget https://
-github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/
-data_info_files.tgz tar -xvf data_info_files.tgz ``` Examples to specific
-dataset options can be found in `./options/default_dataset_opt.yml`. Details of
-the dataloader inferface and meta information files can be found in [Dataset
-Preparation](docs/Dataset_Preparation.md) ### Example Train Script Example to
-train DBCNN on LIVEChallenge dataset ``` # train for single experiment python
-pyiqa/train.py -opt options/train/DBCNN/train_DBCNN.yml # train N splits for
-small datasets python pyiqa/train_nsplits.py -opt options/train/DBCNN/
-train_DBCNN.yml ``` ## :beers: Contribution Any contributions to this
-repository are greatly appreciated. Please follow the [contribution
-instructions](docs/Instruction.md) for contribution guidance. ## :scroll:
-License This work is licensed under a [NTU S-Lab License](https://github.com/
-chaofengc/IQA-PyTorch/blob/main/LICENSE_NTU-S-Lab) and _C_r_e_a_t_i_v_e_ _C_o_m_m_o_n_s
-_A_t_t_r_i_b_u_t_i_o_n_-_N_o_n_C_o_m_m_e_r_c_i_a_l_-_S_h_a_r_e_A_l_i_k_e_ _4_._0_ _I_n_t_e_r_n_a_t_i_o_n_a_l_ _L_i_c_e_n_s_e. _[_C_r_e_a_t_i_v_e
-_C_o_m_m_o_n_s_ _L_i_c_e_n_s_e_]## :bookmark_tabs: Citation If you find our codes helpful to
-your research, please consider to use the following citation: ``` @misc{pyiqa,
-title={{IQA-PyTorch}: PyTorch Toolbox for Image Quality Assessment}, author=
-{Chaofeng Chen and Jiadi Mo}, year={2022}, howpublished = "[Online]. Available:
-\url{https://github.com/chaofengc/IQA-PyTorch}" } ``` ## :heart:
-Acknowledgement The code architecture is borrowed from [BasicSR](https://
-github.com/xinntao/BasicSR). Several implementations are taken from: [IQA-
-optimization](https://github.com/dingkeyan93/IQA-optimization), [Image-Quality-
-Assessment-Toolbox](https://github.com/RyanXingQL/Image-Quality-Assessment-
-Toolbox), [piq](https://github.com/photosynthesis-team/piq), [piqa](https://
-github.com/francois-rozet/piqa), [clean-fid](https://github.com/GaParmar/clean-
-fid) We also thanks the following public repositories: [MUSIQ](https://
-github.com/google-research/google-research/tree/master/musiq), [DBCNN](https://
-github.com/zwx8981/DBCNN-PyTorch), [NIMA](https://github.com/kentsyx/Neural-
-IMage-Assessment), [HyperIQA](https://github.com/SSL92/hyperIQA), [CNNIQA]
-(https://github.com/lidq92/CNNIQA), [WaDIQaM](https://github.com/lidq92/
-WaDIQaM), [PieAPP](https://github.com/prashnani/PerceptualImageError),
-[paq2piq](https://github.com/baidut/paq2piq), [MANIQA](https://github.com/
-IIGROUP/MANIQA) ## :e-mail: Contact If you have any questions, please email
-`chaofenghust@gmail.com`
+releases/download/v0.1-weights/meta_info.tgz) and extract them to `datasets/
+` folder. You may also use the following commands: ``` mkdir datasets && cd
+datasets # make soft links of your dataset ln -sf your/dataset/path datasetname
+# download meta info files and train split files wget https://github.com/
+chaofengc/IQA-PyTorch/releases/download/v0.1-weights/meta_info.tgz tar -xvf
+data_info_files.tgz ``` Examples to specific dataset options can be found in
+`./options/default_dataset_opt.yml`. Details of the dataloader inferface and
+meta information files can be found in [Dataset Preparation](docs/
+Dataset_Preparation.md) ### Example Train Script Example to train DBCNN on
+LIVEChallenge dataset ``` # train for single experiment python pyiqa/train.py -
+opt options/train/DBCNN/train_DBCNN.yml # train N splits for small datasets
+python pyiqa/train_nsplits.py -opt options/train/DBCNN/train_DBCNN.yml ``` ## :
+beers: Contribution Any contributions to this repository are greatly
+appreciated. Please follow the [contribution instructions](docs/Instruction.md)
+for contribution guidance. ## :scroll: License This work is licensed under a
+[NTU S-Lab License](https://github.com/chaofengc/IQA-PyTorch/blob/main/
+LICENSE_NTU-S-Lab) and _C_r_e_a_t_i_v_e_ _C_o_m_m_o_n_s_ _A_t_t_r_i_b_u_t_i_o_n_-_N_o_n_C_o_m_m_e_r_c_i_a_l_-_S_h_a_r_e_A_l_i_k_e
+_4_._0_ _I_n_t_e_r_n_a_t_i_o_n_a_l_ _L_i_c_e_n_s_e. _[_C_r_e_a_t_i_v_e_ _C_o_m_m_o_n_s_ _L_i_c_e_n_s_e_]## :bookmark_tabs:
+Citation If you find our codes helpful to your research, please consider to use
+the following citation: ``` @misc{pyiqa, title={{IQA-PyTorch}: PyTorch Toolbox
+for Image Quality Assessment}, author={Chaofeng Chen and Jiadi Mo}, year=
+{2022}, howpublished = "[Online]. Available: \url{https://github.com/chaofengc/
+IQA-PyTorch}" } ``` Please also consider to cite our new work `TOPIQ` if it is
+useful to you: ``` @misc{chen2023topiq, title={TOPIQ: A Top-down Approach from
+Semantics to Distortions for Image Quality Assessment}, author={Chaofeng Chen
+and Jiadi Mo and Jingwen Hou and Haoning Wu and Liang Liao and Wenxiu Sun and
+Qiong Yan and Weisi Lin}, year={2023}, eprint={2308.03060}, archivePrefix=
+{arXiv}, primaryClass={cs.CV} } ``` ## :heart: Acknowledgement The code
+architecture is borrowed from [BasicSR](https://github.com/xinntao/BasicSR).
+Several implementations are taken from: [IQA-optimization](https://github.com/
+dingkeyan93/IQA-optimization), [Image-Quality-Assessment-Toolbox](https://
+github.com/RyanXingQL/Image-Quality-Assessment-Toolbox), [piq](https://
+github.com/photosynthesis-team/piq), [piqa](https://github.com/francois-rozet/
+piqa), [clean-fid](https://github.com/GaParmar/clean-fid) We also thanks the
+following public repositories: [MUSIQ](https://github.com/google-research/
+google-research/tree/master/musiq), [DBCNN](https://github.com/zwx8981/DBCNN-
+PyTorch), [NIMA](https://github.com/kentsyx/Neural-IMage-Assessment),
+[HyperIQA](https://github.com/SSL92/hyperIQA), [CNNIQA](https://github.com/
+lidq92/CNNIQA), [WaDIQaM](https://github.com/lidq92/WaDIQaM), [PieAPP](https://
+github.com/prashnani/PerceptualImageError), [paq2piq](https://github.com/
+baidut/paq2piq), [MANIQA](https://github.com/IIGROUP/MANIQA) ## :e-mail:
+Contact If you have any questions, please email `chaofenghust@gmail.com`
```

### Comparing `pyiqa-0.1.7/pyiqa/api_helpers.py` & `pyiqa-0.1.8/pyiqa/api_helpers.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/__init__.py` & `pyiqa-0.1.8/pyiqa/archs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/ahiq_arch.py` & `pyiqa-0.1.8/pyiqa/archs/ahiq_arch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,27 @@
-from pyexpat import model
+import timm
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from torchvision.ops.deform_conv import DeformConv2d
-import numpy as np
-
-import timm
+from timm.models.resnet import Bottleneck
 from timm.models.vision_transformer import Block
-from timm.models.resnet import BasicBlock, Bottleneck
+from torchvision.ops.deform_conv import DeformConv2d
 
+from pyiqa.archs.arch_util import (
+    load_file_from_url,
+    load_pretrained_network,
+    random_crop,
+)
 from pyiqa.utils.registry import ARCH_REGISTRY
-from pyiqa.archs.arch_util import load_pretrained_network, default_init_weights, to_2tuple, ExactPadding2d, load_file_from_url
-
 
 default_model_urls = {
-    'pipal': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/AHIQ_vit_p8_epoch33-da3ea303.pth'
+    "pipal": "https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/AHIQ_vit_p8_epoch33-da3ea303.pth"
 }
 
 
-def random_crop(x, y, crop_size, crop_num):
-    b, c, h, w = x.shape
-    ch, cw = to_2tuple(crop_size)
-
-    crops_x = []
-    crops_y = []
-    for i in range(crop_num):
-        sh = np.random.randint(0, h - ch)
-        sw = np.random.randint(0, w - cw)
-        crops_x.append(x[..., sh: sh + ch, sw: sw + cw])
-        crops_y.append(y[..., sh: sh + ch, sw: sw + cw])
-    crops_x = torch.stack(crops_x, dim=1)
-    crops_y = torch.stack(crops_y, dim=1)
-    return crops_x.reshape(b * crop_num, c, ch, cw), crops_y.reshape(b * crop_num, c, ch, cw)
-
-
 class SaveOutput:
     def __init__(self):
         self.outputs = {}
 
     def __call__(self, module, module_in, module_out):
         if module_out.device in self.outputs.keys():
             self.outputs[module_out.device].append(module_out)
@@ -45,28 +29,46 @@
             self.outputs[module_out.device] = [module_out]
 
     def clear(self, device):
         self.outputs[device] = []
 
 
 class DeformFusion(nn.Module):
-    def __init__(self, patch_size=8, in_channels=768 * 5, cnn_channels=256 * 3, out_channels=256 * 3):
+    def __init__(
+        self,
+        patch_size=8,
+        in_channels=768 * 5,
+        cnn_channels=256 * 3,
+        out_channels=256 * 3,
+    ):
         super().__init__()
-        #in_channels, out_channels, kernel_size, stride, padding
+        # in_channels, out_channels, kernel_size, stride, padding
         self.d_hidn = 512
         if patch_size == 8:
             stride = 1
         else:
             stride = 2
         self.conv_offset = nn.Conv2d(in_channels, 2 * 3 * 3, 3, 1, 1)
         self.deform = DeformConv2d(cnn_channels, out_channels, 3, 1, 1)
         self.conv1 = nn.Sequential(
-            nn.Conv2d(in_channels=out_channels, out_channels=self.d_hidn, kernel_size=3, padding=1, stride=2),
+            nn.Conv2d(
+                in_channels=out_channels,
+                out_channels=self.d_hidn,
+                kernel_size=3,
+                padding=1,
+                stride=2,
+            ),
             nn.ReLU(),
-            nn.Conv2d(in_channels=self.d_hidn, out_channels=out_channels, kernel_size=3, padding=1, stride=stride)
+            nn.Conv2d(
+                in_channels=self.d_hidn,
+                out_channels=out_channels,
+                kernel_size=3,
+                padding=1,
+                stride=stride,
+            ),
         )
 
     def forward(self, cnn_feat, vit_feat):
         vit_feat = F.interpolate(vit_feat, size=cnn_feat.shape[-2:], mode="nearest")
         offset = self.conv_offset(vit_feat)
         deform_feat = self.deform(cnn_feat, offset)
         deform_feat = self.conv1(deform_feat)
@@ -76,26 +78,29 @@
 
 class Pixel_Prediction(nn.Module):
     def __init__(self, inchannels=768 * 5 + 256 * 3, outchannels=256, d_hidn=1024):
         super().__init__()
         self.d_hidn = d_hidn
         self.down_channel = nn.Conv2d(inchannels, outchannels, kernel_size=1)
         self.feat_smoothing = nn.Sequential(
-            nn.Conv2d(in_channels=256 * 3, out_channels=self.d_hidn, kernel_size=3, padding=1),
+            nn.Conv2d(
+                in_channels=256 * 3, out_channels=self.d_hidn, kernel_size=3, padding=1
+            ),
             nn.ReLU(),
-            nn.Conv2d(in_channels=self.d_hidn, out_channels=512, kernel_size=3, padding=1)
+            nn.Conv2d(
+                in_channels=self.d_hidn, out_channels=512, kernel_size=3, padding=1
+            ),
         )
 
         self.conv1 = nn.Sequential(
             nn.Conv2d(in_channels=512, out_channels=256, kernel_size=3, padding=1),
-            nn.ReLU()
+            nn.ReLU(),
         )
         self.conv_attent = nn.Sequential(
-            nn.Conv2d(in_channels=256, out_channels=1, kernel_size=1),
-            nn.Sigmoid()
+            nn.Conv2d(in_channels=256, out_channels=1, kernel_size=1), nn.Sigmoid()
         )
         self.conv = nn.Sequential(
             nn.Conv2d(in_channels=256, out_channels=1, kernel_size=1),
         )
 
     def forward(self, f_dis, f_ref, cnn_dis, cnn_ref):
         f_dis = torch.cat((f_dis, cnn_dis), 1)
@@ -112,45 +117,48 @@
         pred = (f * w).sum(dim=-1).sum(dim=-1) / w.sum(dim=-1).sum(dim=-1)
 
         return pred
 
 
 @ARCH_REGISTRY.register()
 class AHIQ(nn.Module):
-    def __init__(self,
-                 num_crop=20,
-                 crop_size=224,
-                 default_mean=[0.485, 0.456, 0.406],
-                 default_std=[0.229, 0.224, 0.225],
-                 pretrained=True,
-                 pretrained_model_path=None,
-                 ):
+    def __init__(
+        self,
+        num_crop=20,
+        crop_size=224,
+        default_mean=[0.485, 0.456, 0.406],
+        default_std=[0.229, 0.224, 0.225],
+        pretrained=True,
+        pretrained_model_path=None,
+    ):
         super().__init__()
 
-        self.resnet50 = timm.create_model('resnet50', pretrained=True)
-        self.vit = timm.create_model('vit_base_patch8_224', pretrained=True)
+        self.resnet50 = timm.create_model("resnet50", pretrained=True)
+        self.vit = timm.create_model("vit_base_patch8_224", pretrained=True)
         self.fix_network(self.resnet50)
         self.fix_network(self.vit)
 
         self.deform_net = DeformFusion()
         self.regressor = Pixel_Prediction()
 
         # register hook to get intermediate features
         self.init_saveoutput()
 
         self.default_mean = torch.Tensor(default_mean).view(1, 3, 1, 1)
         self.default_std = torch.Tensor(default_std).view(1, 3, 1, 1)
 
         if pretrained_model_path is not None:
-            load_pretrained_network(self, pretrained_model_path, True, weight_keys='params')
+            load_pretrained_network(
+                self, pretrained_model_path, True, weight_keys="params"
+            )
         elif pretrained:
-            weight_path = load_file_from_url(default_model_urls['pipal'])
+            weight_path = load_file_from_url(default_model_urls["pipal"])
             checkpoint = torch.load(weight_path)
-            self.regressor.load_state_dict(checkpoint['regressor_model_state_dict'])
-            self.deform_net.load_state_dict(checkpoint['deform_net_model_state_dict'])
+            self.regressor.load_state_dict(checkpoint["regressor_model_state_dict"])
+            self.deform_net.load_state_dict(checkpoint["deform_net_model_state_dict"])
 
         self.eps = 1e-12
         self.crops = num_crop
         self.crop_size = crop_size
 
     def init_saveoutput(self):
         self.save_output = SaveOutput()
@@ -178,28 +186,28 @@
             (
                 self.save_output.outputs[x.device][0][:, 1:, :],
                 self.save_output.outputs[x.device][1][:, 1:, :],
                 self.save_output.outputs[x.device][2][:, 1:, :],
                 self.save_output.outputs[x.device][3][:, 1:, :],
                 self.save_output.outputs[x.device][4][:, 1:, :],
             ),
-            dim=2
+            dim=2,
         )
         self.save_output.clear(x.device)
         return feat
 
     def get_resnet_feature(self, x):
         self.resnet50(x)
         feat = torch.cat(
             (
                 self.save_output.outputs[x.device][0],
                 self.save_output.outputs[x.device][1],
                 self.save_output.outputs[x.device][2],
             ),
-            dim=1
+            dim=1,
         )
         self.save_output.clear(x.device)
         return feat
 
     def regress_score(self, dis, ref):
         self.resnet50.eval()
         self.vit.eval()
@@ -223,14 +231,14 @@
 
         return score
 
     def forward(self, x, y):
         bsz = x.shape[0]
 
         if self.crops > 1 and not self.training:
-            x, y = random_crop(x, y, self.crop_size, self.crops)
+            x, y = random_crop([x, y], self.crop_size, self.crops)
             score = self.regress_score(x, y)
             score = score.reshape(bsz, self.crops, 1)
             score = score.mean(dim=1)
         else:
             score = self.regress_score(x, y)
         return score
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/arch_util.py` & `pyiqa-0.1.8/pyiqa/archs/arch_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from collections import OrderedDict
-import math
 import collections.abc
 from itertools import repeat
 import numpy as np
-from typing import Tuple
 
 import torch
 from torch import nn as nn
 from torch.nn import functional as F
 from torch.nn import init as init
 from torch.nn.modules.batchnorm import _BatchNorm
+import torchvision.transforms as T
 
+from .constants import OPENAI_CLIP_MEAN, OPENAI_CLIP_STD
 from pyiqa.utils.download_util import load_file_from_url
 
+
 # --------------------------------------------
 # IQA utils
 # --------------------------------------------
 
 
 def dist_to_mos(dist_score: torch.Tensor) -> torch.Tensor:
     """Convert distribution prediction to mos score.
@@ -30,41 +31,92 @@
     """
     num_classes = dist_score.shape[-1]
     mos_score = dist_score * torch.arange(1, num_classes + 1).to(dist_score)
     mos_score = mos_score.sum(dim=-1, keepdim=True)
     return mos_score
 
 
+def random_crop(input_list, crop_size, crop_num):
+    if not isinstance(input_list, collections.abc.Sequence):
+        input_list = [input_list]
+
+    b, c, h, w = input_list[0].shape
+    ch, cw = to_2tuple(crop_size)
+
+    if min(h, w) <= crop_size:
+        scale_factor = (crop_size + 1) / min(h, w)
+        input_list = [
+            F.interpolate(x, scale_factor=scale_factor, mode="bilinear")
+            for x in input_list
+        ]
+        b, c, h, w = input_list[0].shape
+
+    crops_list = [[] for i in range(len(input_list))]
+    for i in range(crop_num):
+        sh = np.random.randint(0, h - ch + 1)
+        sw = np.random.randint(0, w - cw + 1)
+        for j in range(len(input_list)):
+            crops_list[j].append(input_list[j][..., sh : sh + ch, sw : sw + cw])
+
+    for i in range(len(crops_list)):
+        crops_list[i] = torch.stack(crops_list[i], dim=1).reshape(
+            b * crop_num, c, ch, cw
+        )
+
+    if len(crops_list) == 1:
+        crops_list = crops_list[0]
+    return crops_list
+
+
+def clip_preprocess_tensor(x: torch.Tensor, model):
+    """clip preprocess function with tensor input.
+
+    NOTE: Results are slightly different with original preprocess function with PIL image input, because of differences in resize function.
+    """
+    # Bicubic interpolation
+    x = (x * 255).byte()
+    x = T.functional.resize(
+        x,
+        model.visual.input_resolution,
+        interpolation=T.InterpolationMode.BICUBIC,
+        antialias=True,
+    )
+    # Center crop
+    x = T.functional.center_crop(x, model.visual.input_resolution)
+    x = x.float() / 255.0
+    x = T.functional.normalize(x, OPENAI_CLIP_MEAN, OPENAI_CLIP_STD)
+    return x
+
+
 # --------------------------------------------
 # Common utils
 # --------------------------------------------
 
 
 def clean_state_dict(state_dict):
     # 'clean' checkpoint by removing .module prefix from state dict if it exists from parallel training
     cleaned_state_dict = OrderedDict()
     for k, v in state_dict.items():
-        name = k[7:] if k.startswith('module.') else k
+        name = k[7:] if k.startswith("module.") else k
         cleaned_state_dict[name] = v
     return cleaned_state_dict
 
 
 def load_pretrained_network(net, model_path, strict=True, weight_keys=None):
-    if model_path.startswith('https://') or model_path.startswith('http://'):
+    if model_path.startswith("https://") or model_path.startswith("http://"):
         model_path = load_file_from_url(model_path)
-    print(f'Loading pretrained model {net.__class__.__name__} from {model_path}')
-    state_dict = torch.load(model_path, map_location=torch.device('cpu'))
+    print(f"Loading pretrained model {net.__class__.__name__} from {model_path}")
+    state_dict = torch.load(model_path, map_location=torch.device("cpu"))
     if weight_keys is not None:
         state_dict = state_dict[weight_keys]
     state_dict = clean_state_dict(state_dict)
     net.load_state_dict(state_dict, strict=strict)
 
 
 def _ntuple(n):
-
     def parse(x):
         if isinstance(x, collections.abc.Iterable):
             return x
         return tuple(repeat(x, n))
 
     return parse
 
@@ -102,77 +154,7 @@
                 m.weight.data *= scale
                 if m.bias is not None:
                     m.bias.data.fill_(bias_fill)
             elif isinstance(m, _BatchNorm):
                 init.constant_(m.weight, 1)
                 if m.bias is not None:
                     m.bias.data.fill_(bias_fill)
-
-
-def symm_pad(im: torch.Tensor, padding: Tuple[int, int, int, int]):
-    """Symmetric padding same as tensorflow.
-    Ref: https://discuss.pytorch.org/t/symmetric-padding/19866/3
-    """
-    h, w = im.shape[-2:]
-    left, right, top, bottom = padding
-
-    x_idx = np.arange(-left, w + right)
-    y_idx = np.arange(-top, h + bottom)
-
-    def reflect(x, minx, maxx):
-        """ Reflects an array around two points making a triangular waveform that ramps up
-        and down,  allowing for pad lengths greater than the input length """
-        rng = maxx - minx
-        double_rng = 2 * rng
-        mod = np.fmod(x - minx, double_rng)
-        normed_mod = np.where(mod < 0, mod + double_rng, mod)
-        out = np.where(normed_mod >= rng, double_rng - normed_mod, normed_mod) + minx
-        return np.array(out, dtype=x.dtype)
-
-    x_pad = reflect(x_idx, -0.5, w - 0.5)
-    y_pad = reflect(y_idx, -0.5, h - 0.5)
-    xx, yy = np.meshgrid(x_pad, y_pad)
-    return im[..., yy, xx]
-
-
-def excact_padding_2d(x, kernel, stride=1, dilation=1, mode='same'):
-    assert len(x.shape) == 4, f'Only support 4D tensor input, but got {x.shape}'
-    kernel = to_2tuple(kernel)
-    stride = to_2tuple(stride)
-    dilation = to_2tuple(dilation)
-    b, c, h, w = x.shape
-    h2 = math.ceil(h / stride[0])
-    w2 = math.ceil(w / stride[1])
-    pad_row = (h2 - 1) * stride[0] + (kernel[0] - 1) * dilation[0] + 1 - h
-    pad_col = (w2 - 1) * stride[1] + (kernel[1] - 1) * dilation[1] + 1 - w
-    pad_l, pad_r, pad_t, pad_b = (pad_col // 2, pad_col - pad_col // 2, pad_row // 2, pad_row - pad_row // 2)
-
-    mode = mode if mode != 'same' else 'constant'
-    if mode != 'symmetric':
-        x = F.pad(x, (pad_l, pad_r, pad_t, pad_b), mode=mode)
-    elif mode == 'symmetric':
-        x = symm_pad(x, (pad_l, pad_r, pad_t, pad_b))
-
-    return x
-
-
-class ExactPadding2d(nn.Module):
-    r"""This function calculate exact padding values for 4D tensor inputs,
-    and support the same padding mode as tensorflow.
-
-    Args:
-        kernel (int or tuple): kernel size.
-        stride (int or tuple): stride size.
-        dilation (int or tuple): dilation size, default with 1.
-        mode (srt): padding mode can be ('same', 'symmetric', 'replicate', 'circular')
-
-    """
-
-    def __init__(self, kernel, stride=1, dilation=1, mode='same'):
-        super().__init__()
-        self.kernel = to_2tuple(kernel)
-        self.stride = to_2tuple(stride)
-        self.dilation = to_2tuple(dilation)
-        self.mode = mode
-
-    def forward(self, x):
-        return excact_padding_2d(x, self.kernel, self.stride, self.dilation, self.mode)
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/brisque_arch.py` & `pyiqa-0.1.8/pyiqa/archs/brisque_arch.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,15 @@
                  pretrained_model_path: str = None) -> None:
         super().__init__()
         self.kernel_size = kernel_size
 
         # This check might look redundant because kernel size is checked within the brisque function anyway.
         # However, this check allows to fail fast when the loss is being initialised and training has not been started.
         assert kernel_size % 2 == 1, f'Kernel size must be odd, got [{kernel_size}]'
+        assert test_y_channel, f'Only [test_y_channel=True] is supported for current BRISQUE model, which is taken directly from official codes: https://github.com/utlive/BRISQUE.'
 
         self.kernel_sigma = kernel_sigma
         self.test_y_channel = test_y_channel
         if pretrained_model_path is not None:
             self.pretrained_model_path = pretrained_model_path
         else:
             self.pretrained_model_path = load_file_from_url(default_model_urls['url'])
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/ckdn_arch.py` & `pyiqa-0.1.8/pyiqa/archs/ckdn_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/clip_model.py` & `pyiqa-0.1.8/pyiqa/archs/clip_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -278,25 +278,47 @@
         # residual layers
         self._inplanes = width  # this is a *mutable* variable used during construction
         self.layer1 = self._make_layer(width, layers[0])
         self.layer2 = self._make_layer(width * 2, layers[1], stride=2)
         self.layer3 = self._make_layer(width * 4, layers[2], stride=2)
         self.layer4 = self._make_layer(width * 8, layers[3], stride=2)
 
+        self.feature_dim_list = [width, width * 4, width * 8, width * 16, width * 32]
+
         embed_dim = width * 32  # the ResNet feature dimension
         self.attnpool = AttentionPool2d(input_resolution // 32, embed_dim, heads, output_dim)
 
     def _make_layer(self, planes, blocks, stride=1):
         layers = [Bottleneck(self._inplanes, planes, stride)]
 
         self._inplanes = planes * Bottleneck.expansion
         for _ in range(1, blocks):
             layers.append(Bottleneck(self._inplanes, planes))
 
         return nn.Sequential(*layers)
+    
+    def forward_features(self, x, return_token=False, pos_embedding=False):
+        def stem(x):
+            for conv, bn in [(self.conv1, self.bn1), (self.conv2, self.bn2), (self.conv3, self.bn3)]:
+                x = self.relu(bn(conv(x)))
+            x = self.avgpool(x)
+            return x
+        
+        x = x.type(self.conv1.weight.dtype)
+        x = stem(x)
+        feat_list = [x]
+        x = self.layer1(x)
+        feat_list += [x]
+        x = self.layer2(x)
+        feat_list += [x]
+        x = self.layer3(x)
+        feat_list += [x]
+        x = self.layer4(x)
+        feat_list += [x]
+        return feat_list
 
     def forward(self, x, return_token=False, pos_embedding=False):
         def stem(x):
             for conv, bn in [(self.conv1, self.bn1), (self.conv2, self.bn2), (self.conv3, self.bn3)]:
                 x = self.relu(bn(conv(x)))
             x = self.avgpool(x)
             return x
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/clipiqa_arch.py` & `pyiqa-0.1.8/pyiqa/archs/clipiqa_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/cnniqa_arch.py` & `pyiqa-0.1.8/pyiqa/archs/cnniqa_arch.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import torch.nn as nn
 import torch.nn.functional as F
 from pyiqa.utils.registry import ARCH_REGISTRY
 from pyiqa.archs.arch_util import load_pretrained_network
 
 
 default_model_urls = {
-    'koniq10k': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/CNNIQA_koniq10k-fd89516f.pth'
+    'koniq10k': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/CNNIQA_koniq10k-e6f14c91.pth'
 }
 
 
 @ARCH_REGISTRY.register()
 class CNNIQA(nn.Module):
     r"""CNNIQA model.
     Args:
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/dbcnn_arch.py` & `pyiqa-0.1.8/pyiqa/archs/dbcnn_arch.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 default_model_urls = {
     'csiq': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/DBCNN_CSIQ-8677d071.pth',
     'tid2008': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/DBCNN_TID2008-4b47c5d1.pth',
     'tid2013': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/DBCNN_TID2013-485d021d.pth',
     'live': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/DBCNN_LIVE-97262bf4.pth',
     'livec': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/DBCNN_LIVEC-83f6dad3.pth',
     'livem': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/DBCNN_LIVEM-698474e3.pth',
-    'koniq': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/DBCNN_KonIQ10k-254e8241.pth',
+    'koniq': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/DBCNN_KonIQ10k-2de81c0a.pth',
+    'scnn': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/DBCNN_scnn-7ea73d75.pth',
 }
 
 
 class SCNN(nn.Module):
     """Network branch for synthetic distortions.
     Args:
         use_bn (Boolean): Whether to use batch normalization.
@@ -110,19 +111,18 @@
         pretrained_model_path=None,
         default_mean=[0.485, 0.456, 0.406],
         default_std=[0.229, 0.224, 0.225],
     ):
         super(DBCNN, self).__init__()
 
         # Convolution and pooling layers of VGG-16.
-        self.features1 = torchvision.models.vgg16(pretrained=True).features
+        self.features1 = torchvision.models.vgg16(weights='IMAGENET1K_V1').features
         self.features1 = nn.Sequential(*list(self.features1.children())[:-1])
         scnn = SCNN(use_bn=use_bn)
-        if pretrained_scnn_path is not None:
-            load_pretrained_network(scnn, pretrained_scnn_path)
+        load_pretrained_network(scnn, default_model_urls['scnn'])
 
         self.features2 = scnn.features
 
         # Linear classifier.
         self.fc = torch.nn.Linear(512 * 128, 1)
 
         self.default_mean = torch.Tensor(default_mean).view(1, 3, 1, 1)
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/dists_arch.py` & `pyiqa-0.1.8/pyiqa/archs/dists_arch.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     '''
 
     def __init__(self, pretrained=True, pretrained_model_path=None, **kwargs):
         """Refer to offical code https://github.com/dingkeyan93/DISTS
         """
         super(DISTS, self).__init__()
-        vgg_pretrained_features = models.vgg16(pretrained=True).features
+        vgg_pretrained_features = models.vgg16(weights='IMAGENET1K_V1').features
         self.stage1 = torch.nn.Sequential()
         self.stage2 = torch.nn.Sequential()
         self.stage3 = torch.nn.Sequential()
         self.stage4 = torch.nn.Sequential()
         self.stage5 = torch.nn.Sequential()
         for x in range(0, 4):
             self.stage1.add_module(str(x), vgg_pretrained_features[x])
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/entropy_arch.py` & `pyiqa-0.1.8/pyiqa/archs/entropy_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/fid_arch.py` & `pyiqa-0.1.8/pyiqa/archs/fid_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/fsim_arch.py` & `pyiqa-0.1.8/pyiqa/archs/fsim_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/func_util.py` & `pyiqa-0.1.8/pyiqa/archs/func_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from typing import Tuple
 import torch
 import torch.nn.functional as F
 
 from pyiqa.utils.color_util import to_y_channel
-from pyiqa.matlab_utils import fspecial, imfilter
-from .arch_util import excact_padding_2d
+from pyiqa.matlab_utils import fspecial, imfilter, exact_padding_2d
+
 
 EPS = torch.finfo(torch.float32).eps
 
 
-def preprocess_rgb(x, test_y_channel, data_range=1., color_space='yiq'):
+def preprocess_rgb(x, test_y_channel, data_range: int = 1, color_space="yiq"):
     if test_y_channel and x.shape[1] == 3:
         x = to_y_channel(x, data_range, color_space)
     else:
         x = x * data_range
+
+    # use rounded uint8 value to make the input image same as MATLAB
+    if data_range == 255:
         x = x - x.detach() + x.round()
     return x
 
 
-def extract_2d_patches(x, kernel, stride=1, dilation=1, padding='same'):
+def extract_2d_patches(x, kernel, stride=1, dilation=1, padding="same"):
     """
     Ref: https://stackoverflow.com/a/65886666
     """
     b, c, h, w = x.shape
-    if padding != 'none':
-        x = excact_padding_2d(x, kernel, stride, dilation, mode=padding)
+    if padding != "none":
+        x = exact_padding_2d(x, kernel, stride, dilation, mode=padding)
 
     # Extract patches
     patches = F.unfold(x, kernel, dilation, stride=stride)
     b, _, pnum = patches.shape
     patches = patches.transpose(1, 2).reshape(b, pnum, c, kernel, kernel)
     return patches
 
@@ -50,69 +53,72 @@
         x (torch.Tensor): should be non-negative
     """
     EPS = torch.finfo(x.dtype).eps
     return torch.sqrt(x + EPS)
 
 
 def diff_round(x: torch.Tensor) -> torch.Tensor:
-    r"""Differentiable round.
-    """
+    r"""Differentiable round."""
     return x - x.detach() + x.round()
 
 
-def normalize_img_with_guass(img: torch.Tensor,
-                             kernel_size: int = 7,
-                             sigma: float = 7. / 6,
-                             C: int = 1,
-                             padding: str = 'same'):
-
+def normalize_img_with_guass(
+    img: torch.Tensor,
+    kernel_size: int = 7,
+    sigma: float = 7.0 / 6,
+    C: int = 1,
+    padding: str = "same",
+):
     kernel = fspecial(kernel_size, sigma, 1).to(img)
     mu = imfilter(img, kernel, padding=padding)
     std = imfilter(img**2, kernel, padding=padding)
     sigma = safe_sqrt((std - mu**2).abs())
     img_normalized = (img - mu) / (sigma + C)
     return img_normalized
 
 
 # Gradient operator kernels
 def scharr_filter() -> torch.Tensor:
     r"""Utility function that returns a normalized 3x3 Scharr kernel in X direction
     Returns:
         kernel: Tensor with shape (1, 3, 3)
     """
-    return torch.tensor([[[-3., 0., 3.], [-10., 0., 10.], [-3., 0., 3.]]]) / 16
+    return torch.tensor([[[-3.0, 0.0, 3.0], [-10.0, 0.0, 10.0], [-3.0, 0.0, 3.0]]]) / 16
 
 
 def gradient_map(x: torch.Tensor, kernels: torch.Tensor) -> torch.Tensor:
-    r""" Compute gradient map for a given tensor and stack of kernels.
+    r"""Compute gradient map for a given tensor and stack of kernels.
     Args:
         x: Tensor with shape (N, C, H, W).
         kernels: Stack of tensors for gradient computation with shape (k_N, k_H, k_W)
     Returns:
         Gradients of x per-channel with shape (N, C, H, W)
     """
     padding = kernels.size(-1) // 2
     grads = torch.nn.functional.conv2d(x, kernels.to(x), padding=padding)
     return safe_sqrt(torch.sum(grads**2, dim=-3, keepdim=True))
 
 
-def similarity_map(map_x: torch.Tensor, map_y: torch.Tensor, constant: float, alpha: float = 0.0) -> torch.Tensor:
-    r""" Compute similarity_map between two tensors using Dice-like equation.
+def similarity_map(
+    map_x: torch.Tensor, map_y: torch.Tensor, constant: float, alpha: float = 0.0
+) -> torch.Tensor:
+    r"""Compute similarity_map between two tensors using Dice-like equation.
     Args:
         map_x: Tensor with map to be compared
         map_y: Tensor with map to be compared
         constant: Used for numerical stability
         alpha: Masking coefficient. Substracts - `alpha` * map_x * map_y from denominator and nominator
     """
-    return (2.0 * map_x * map_y - alpha * map_x * map_y + constant) / \
-           (map_x ** 2 + map_y ** 2 - alpha * map_x * map_y + constant + EPS)
+    return (2.0 * map_x * map_y - alpha * map_x * map_y + constant) / (
+        map_x**2 + map_y**2 - alpha * map_x * map_y + constant + EPS
+    )
 
 
 def ifftshift(x: torch.Tensor) -> torch.Tensor:
-    r""" Similar to np.fft.ifftshift but applies to PyTorch Tensors"""
+    r"""Similar to np.fft.ifftshift but applies to PyTorch Tensors"""
     shift = [-(ax // 2) for ax in x.size()]
     return torch.roll(x, shift, tuple(range(len(shift))))
 
 
 def get_meshgrid(size: Tuple[int, int]) -> torch.Tensor:
     r"""Return coordinate grid matrices centered at zero point.
     Args:
@@ -127,67 +133,87 @@
 
     if size[1] % 2:
         # Odd
         y = torch.arange(-(size[1] - 1) / 2, size[1] / 2) / (size[1] - 1)
     else:
         # Even
         y = torch.arange(-size[1] / 2, size[1] / 2) / size[1]
-    return torch.meshgrid(x, y, indexing='ij')
+    return torch.meshgrid(x, y, indexing="ij")
 
 
 def estimate_ggd_param(x: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
     """Estimate general gaussian distribution.
 
     Args:
         x (Tensor): shape (b, 1, h, w)
     """
     gamma = torch.arange(0.2, 10 + 0.001, 0.001).to(x)
-    r_table = (torch.lgamma(1. / gamma) + torch.lgamma(3. / gamma) - 2 * torch.lgamma(2. / gamma)).exp()
+    r_table = (
+        torch.lgamma(1.0 / gamma)
+        + torch.lgamma(3.0 / gamma)
+        - 2 * torch.lgamma(2.0 / gamma)
+    ).exp()
     r_table = r_table.repeat(x.size(0), 1)
 
     sigma_sq = x.pow(2).mean(dim=(-1, -2))
     sigma = sigma_sq.sqrt().squeeze(dim=-1)
 
-    assert not torch.isclose(sigma, torch.zeros_like(sigma)).all(), \
-        'Expected image with non zero variance of pixel values'
+    assert not torch.isclose(
+        sigma, torch.zeros_like(sigma)
+    ).all(), "Expected image with non zero variance of pixel values"
 
     E = x.abs().mean(dim=(-1, -2))
     rho = sigma_sq / E**2
 
     indexes = (rho - r_table).abs().argmin(dim=-1)
     solution = gamma[indexes]
     return solution, sigma
 
 
-def estimate_aggd_param(block: torch.Tensor, return_sigma=False) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+def estimate_aggd_param(
+    block: torch.Tensor, return_sigma=False
+) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
     """Estimate AGGD (Asymmetric Generalized Gaussian Distribution) parameters.
     Args:
         block (Tensor): Image block with shape (b, 1, h, w).
     Returns:
         Tensor: alpha, beta_l and beta_r for the AGGD distribution
         (Estimating the parames in Equation 7 in the paper).
     """
     gam = torch.arange(0.2, 10 + 0.001, 0.001).to(block)
-    r_gam = (2 * torch.lgamma(2. / gam) - (torch.lgamma(1. / gam) + torch.lgamma(3. / gam))).exp()
+    r_gam = (
+        2 * torch.lgamma(2.0 / gam)
+        - (torch.lgamma(1.0 / gam) + torch.lgamma(3.0 / gam))
+    ).exp()
     r_gam = r_gam.repeat(block.shape[0], 1)
 
     mask_left = block < 0
     mask_right = block > 0
     count_left = mask_left.sum(dim=(-1, -2), dtype=torch.float32)
     count_right = mask_right.sum(dim=(-1, -2), dtype=torch.float32)
 
     left_std = torch.sqrt((block * mask_left).pow(2).sum(dim=(-1, -2)) / (count_left))
-    right_std = torch.sqrt((block * mask_right).pow(2).sum(dim=(-1, -2)) / (count_right))
+    right_std = torch.sqrt(
+        (block * mask_right).pow(2).sum(dim=(-1, -2)) / (count_right)
+    )
 
     gammahat = left_std / right_std
     rhat = block.abs().mean(dim=(-1, -2)).pow(2) / block.pow(2).mean(dim=(-1, -2))
-    rhatnorm = (rhat * (gammahat.pow(3) + 1) * (gammahat + 1)) / (gammahat.pow(2) + 1).pow(2)
+    rhatnorm = (rhat * (gammahat.pow(3) + 1) * (gammahat + 1)) / (
+        gammahat.pow(2) + 1
+    ).pow(2)
     array_position = (r_gam - rhatnorm).abs().argmin(dim=-1)
 
     alpha = gam[array_position]
-    beta_l = left_std.squeeze(-1) * (torch.lgamma(1 / alpha) - torch.lgamma(3 / alpha)).exp().sqrt()
-    beta_r = right_std.squeeze(-1) * (torch.lgamma(1 / alpha) - torch.lgamma(3 / alpha)).exp().sqrt()
+    beta_l = (
+        left_std.squeeze(-1)
+        * (torch.lgamma(1 / alpha) - torch.lgamma(3 / alpha)).exp().sqrt()
+    )
+    beta_r = (
+        right_std.squeeze(-1)
+        * (torch.lgamma(1 / alpha) - torch.lgamma(3 / alpha)).exp().sqrt()
+    )
 
     if return_sigma:
         return alpha, left_std.squeeze(-1), right_std.squeeze(-1)
     else:
         return alpha, beta_l, beta_r
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/gmsd_arch.py` & `pyiqa-0.1.8/pyiqa/archs/gmsd_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/hypernet_arch.py` & `pyiqa-0.1.8/pyiqa/archs/hypernet_arch.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import torch.nn as nn
 import timm
 from pyiqa.utils.registry import ARCH_REGISTRY
 from pyiqa.archs.arch_util import load_pretrained_network
 
 
 default_model_urls = {
-    'resnet50-koniq': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/HyperIQA-resnet50-koniq10k-48579ec9.pth', 
+    'resnet50-koniq': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/HyperIQA-resnet50-koniq10k-c96c41b1.pth',
 }
 
 
 @ARCH_REGISTRY.register()
 class HyperNet(nn.Module):
     """HyperNet Model.
     Args:
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/inception.py` & `pyiqa-0.1.8/pyiqa/archs/inception.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/iqt_arch.py` & `pyiqa-0.1.8/pyiqa/archs/iqt_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/lpips_arch.py` & `pyiqa-0.1.8/pyiqa/archs/lpips_arch.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,15 @@
         return out
 
 
 class alexnet(torch.nn.Module):
 
     def __init__(self, requires_grad=False, pretrained=True):
         super(alexnet, self).__init__()
-        alexnet_pretrained_features = models.alexnet(pretrained=pretrained).features
+        alexnet_pretrained_features = models.alexnet(weights='IMAGENET1K_V1').features
         self.slice1 = torch.nn.Sequential()
         self.slice2 = torch.nn.Sequential()
         self.slice3 = torch.nn.Sequential()
         self.slice4 = torch.nn.Sequential()
         self.slice5 = torch.nn.Sequential()
         self.N_slices = 5
         for x in range(2):
@@ -299,15 +299,15 @@
         return out
 
 
 class vgg16(torch.nn.Module):
 
     def __init__(self, requires_grad=False, pretrained=True):
         super(vgg16, self).__init__()
-        vgg_pretrained_features = models.vgg16(pretrained=pretrained).features
+        vgg_pretrained_features = models.vgg16(weights='IMAGENET1K_V1').features
         self.slice1 = torch.nn.Sequential()
         self.slice2 = torch.nn.Sequential()
         self.slice3 = torch.nn.Sequential()
         self.slice4 = torch.nn.Sequential()
         self.slice5 = torch.nn.Sequential()
         self.N_slices = 5
         for x in range(4):
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/mad_arch.py` & `pyiqa-0.1.8/pyiqa/archs/mad_arch.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,29 +268,32 @@
         test_y_channel: bool, whether to use y channel on ycbcr which mimics official matlab code.
     References:
         Larson, Eric Cooper, and Damon Michael Chandler. "Most apparent distortion: full-reference
         image quality assessment and the role of strategy." Journal of electronic imaging 19, no. 1
         (2010): 011006.
     """
 
-    def __init__(self, channels=3, test_y_channel=True):
+    def __init__(self, channels=3, test_y_channel=False):
         super(MAD, self).__init__()
         self.channels = channels
         self.test_y_channel = test_y_channel
 
     def mad(self, ref, dst):
         r"""Compute MAD for a batch of images.
         Args:
             ref: An reference tensor. Shape :math:`(N, C, H, W)`.
             dst: A distortion tensor. Shape :math:`(N, C, H, W)`.
         """
         if self.test_y_channel and ref.shape[1] == 3:
             ref = to_y_channel(ref, 255.)
             dst = to_y_channel(dst, 255.)
             self.channels = 1
+        else:
+            ref = ref * 255
+            dst = dst * 255
 
         HI = hi_index(ref, dst)
         LO = lo_index(ref, dst)
         thresh1 = 2.55
         thresh2 = 3.35
         b1 = math.exp(-thresh1 / thresh2)
         b2 = 1 / (math.log(10) * thresh2)
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/maniqa_arch.py` & `pyiqa-0.1.8/pyiqa/archs/maniqa_arch.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,34 +15,23 @@
 from timm.models.vision_transformer import Block
 from .constants import IMAGENET_INCEPTION_MEAN, IMAGENET_INCEPTION_STD
 from .maniqa_swin import SwinTransformer
 from torch import nn
 from einops import rearrange
 
 from pyiqa.utils.registry import ARCH_REGISTRY
-from pyiqa.archs.arch_util import load_pretrained_network
+from pyiqa.archs.arch_util import load_pretrained_network, random_crop
 
 default_model_urls = {
     'pipal': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/MANIQA_PIPAL-ae6d356b.pth',
     'koniq': 'https://github.com/IIGROUP/MANIQA/releases/download/Koniq10k/ckpt_koniq10k.pt',
     'kadid': 'https://github.com/IIGROUP/MANIQA/releases/download/Kadid10k/ckpt_kadid10k.pt',
 }
 
 
-def random_crop(x, sample_size=224, sample_num=8):
-    b, c, h, w = x.shape
-    th = tw = sample_size
-    cropped_x = []
-    for s in range(sample_num):
-        i = torch.randint(0, h - th + 1, size=(1, )).item()
-        j = torch.randint(0, w - tw + 1, size=(1, )).item()
-        cropped_x.append(x[:, :, i:i + th, j:j + tw])
-    cropped_x = torch.stack(cropped_x, dim=1)
-    return cropped_x
-
 
 class TABlock(nn.Module):
     def __init__(self, dim, drop=0.1):
         super().__init__()
         self.c_q = nn.Linear(dim, dim)
         self.c_k = nn.Linear(dim, dim)
         self.c_v = nn.Linear(dim, dim)
@@ -165,22 +154,20 @@
         x9 = save_output.outputs[9][:, 1:]
         x = torch.cat((x6, x7, x8, x9), dim=2)
         return x
 
     def forward(self, x):
 
         x = (x - self.default_mean.to(x)) / self.default_std.to(x)
+        bsz = x.shape[0]
 
         if self.training:
-            x_patches = random_crop(x, sample_size=224, sample_num=1)
+            x = random_crop(x, crop_size=224, crop_num=1)
         else:
-            x_patches = random_crop(x, sample_size=224, sample_num=self.test_sample)
-
-        bsz, num_patches, c, psz, psz = x_patches.shape
-        x = x_patches.reshape(bsz * num_patches, c, psz, psz)
+            x = random_crop(x, crop_size=224, crop_num=self.test_sample)
 
         _x = self.vit(x)
         x = self.extract_feature(self.save_output)
         self.save_output.outputs.clear()
 
         # stage 1
         x = rearrange(x, 'b (h w) c -> b c (h w)', h=self.input_size, w=self.input_size)
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/maniqa_swin.py` & `pyiqa-0.1.8/pyiqa/archs/maniqa_swin.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         # define a parameter table of relative position bias
         self.relative_position_bias_table = nn.Parameter(
             torch.zeros((2 * window_size[0] - 1) * (2 * window_size[1] - 1), num_heads))  # 2*Wh-1 * 2*Ww-1, nH
 
         # get pair-wise relative position index for each token inside the window
         coords_h = torch.arange(self.window_size[0])
         coords_w = torch.arange(self.window_size[1])
-        coords = torch.stack(torch.meshgrid([coords_h, coords_w]))  # 2, Wh, Ww
+        coords = torch.stack(torch.meshgrid([coords_h, coords_w], indexing='ij'))  # 2, Wh, Ww
         coords_flatten = torch.flatten(coords, 1)  # 2, Wh*Ww
         relative_coords = coords_flatten[:, :, None] - coords_flatten[:, None, :]  # 2, Wh*Ww, Wh*Ww
         relative_coords = relative_coords.permute(1, 2, 0).contiguous()  # Wh*Ww, Wh*Ww, 2
         relative_coords[:, :, 0] += self.window_size[0] - 1  # shift to start from 0
         relative_coords[:, :, 1] += self.window_size[1] - 1
         relative_coords[:, :, 0] *= 2 * self.window_size[1] - 1
         relative_position_index = relative_coords.sum(-1)  # Wh*Ww, Wh*Ww
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/musiq_arch.py` & `pyiqa-0.1.8/pyiqa/archs/musiq_arch.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 """
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from .arch_util import dist_to_mos, load_pretrained_network
-from .arch_util import ExactPadding2d, excact_padding_2d
+from pyiqa.matlab_utils import ExactPadding2d, exact_padding_2d 
 from pyiqa.utils.registry import ARCH_REGISTRY
 from pyiqa.data.multiscale_trans_util import get_multiscale_patches
 
 default_model_urls = {
     'ava':
     'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/musiq_ava_ckpt-e8d3f067.pth',
     'koniq10k':
@@ -32,15 +32,15 @@
 class StdConv(nn.Conv2d):
     """
     Reference: https://github.com/joe-siyuan-qiao/WeightStandardization
     """
 
     def forward(self, x):
         # implement same padding
-        x = excact_padding_2d(x, self.kernel_size, self.stride, mode='same')
+        x = exact_padding_2d(x, self.kernel_size, self.stride, mode='same')
         weight = self.weight
         weight = weight - weight.mean((1, 2, 3), keepdim=True)
         weight = weight / (weight.std((1, 2, 3), keepdim=True) + 1e-5)
         return F.conv2d(x, weight, self.bias, self.stride)
 
 
 class Bottleneck(nn.Module):
@@ -340,17 +340,19 @@
         else:
             self.head = nn.Linear(hidden_size, num_class)
 
         if pretrained_model_path is not None:
             load_pretrained_network(self, pretrained_model_path, True)
 
     def forward(self, x, return_mos=True, return_dist=False):
+
         # normalize inputs to [-1, 1] as the official code
-        x = (x - 0.5) * 2
-        x = get_multiscale_patches(x, **self.data_preprocess_opts)
+        if not self.training:
+            x = (x - 0.5) * 2
+            x = get_multiscale_patches(x, **self.data_preprocess_opts)
 
         assert len(x.shape) in [3, 4]
         if len(x.shape) == 4:
             b, num_crops, seq_len, dim = x.shape
             x = x.reshape(b * num_crops, seq_len, dim)
         else:
             b, seq_len, dim = x.shape
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/nima_arch.py` & `pyiqa-0.1.8/pyiqa/archs/nima_arch.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 Modified by: Chaofeng Chen (https://github.com/chaofengc)
 
 """
 
 import torch
 import torch.nn as nn
 import timm
-from timm.data import IMAGENET_INCEPTION_MEAN, IMAGENET_INCEPTION_STD
 from pyiqa.utils.registry import ARCH_REGISTRY
 from pyiqa.archs.arch_util import dist_to_mos, load_pretrained_network
 
+
 default_model_urls = {
     'vgg16-ava': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/NIMA_VGG16_ava-dc4e8265.pth',
     'inception_resnet_v2-ava': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/NIMA_InceptionV2_ava-b0c77c00.pth',
 }
 
 
 @ARCH_REGISTRY.register()
@@ -42,44 +42,37 @@
     def __init__(
         self,
         base_model_name='vgg16',
         num_classes=10,
         dropout_rate=0.,
         pretrained=True,
         pretrained_model_path=None,
-        default_mean=[0.485, 0.456, 0.406],
-        default_std=[0.229, 0.224, 0.225],
     ):
         super(NIMA, self).__init__()
         self.base_model = timm.create_model(base_model_name, pretrained=True, features_only=True)
-
-        # set output number of classes
-        num_classes = 10 if 'ava' in pretrained else num_classes
         
         self.global_pool = nn.AdaptiveAvgPool2d(1)
         in_ch = self.base_model.feature_info.channels()[-1]
         self.num_classes = num_classes
 
         self.classifier = [nn.Flatten(),
                            nn.Dropout(p=dropout_rate),
                            nn.Linear(in_features=in_ch, out_features=num_classes),
                            ]
         if num_classes > 1:
             self.classifier.append(nn.Softmax(dim=-1))
         self.classifier = nn.Sequential(*self.classifier)
 
-        if 'inception' in base_model_name:
-            default_mean = IMAGENET_INCEPTION_MEAN
-            default_std = IMAGENET_INCEPTION_STD
-
+        default_mean = self.base_model.pretrained_cfg['mean']
+        default_std = self.base_model.pretrained_cfg['std']
         self.default_mean = torch.Tensor(default_mean).view(1, 3, 1, 1)
         self.default_std = torch.Tensor(default_std).view(1, 3, 1, 1)
         
         if pretrained and pretrained_model_path is None:
-            url_key = f'{base_model_name}-{pretrained}'
+            url_key = f'{base_model_name}-ava'
             load_pretrained_network(self, default_model_urls[url_key], True, weight_keys='params')
         elif pretrained_model_path is not None:
             load_pretrained_network(self, pretrained_model_path, True, weight_keys='params')
 
     def preprocess(self, x):
         x = (x - self.default_mean.to(x)) / self.default_std.to(x)
         return x
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/niqe_arch.py` & `pyiqa-0.1.8/pyiqa/archs/niqe_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/nlpd_arch.py` & `pyiqa-0.1.8/pyiqa/archs/nlpd_arch.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import torch.nn as nn
 import torch.nn.functional as F
 import numpy as np
 import torchvision.transforms.functional as tf
 
 from pyiqa.archs.ssim_arch import to_y_channel
 from pyiqa.utils.registry import ARCH_REGISTRY
-from pyiqa.archs.arch_util import ExactPadding2d
+from pyiqa.matlab_utils import ExactPadding2d
 
 LAPLACIAN_FILTER = np.array([[0.0025, 0.0125, 0.0200, 0.0125, 0.0025], [0.0125, 0.0625, 0.1000, 0.0625, 0.0125],
                              [0.0200, 0.1000, 0.1600, 0.1000, 0.0200], [0.0125, 0.0625, 0.1000, 0.0625, 0.0125],
                              [0.0025, 0.0125, 0.0200, 0.0125, 0.0025]],
                             dtype=np.float32)
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/nrqm_arch.py` & `pyiqa-0.1.8/pyiqa/archs/nrqm_arch.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 import torch
 from torch import Tensor
 import torch.nn.functional as F
 
 from pyiqa.utils.registry import ARCH_REGISTRY
 from pyiqa.utils.color_util import to_y_channel
 from pyiqa.utils.download_util import load_file_from_url
-from pyiqa.matlab_utils import imresize, fspecial, SCFpyr_PyTorch, dct2d, im2col
+from pyiqa.matlab_utils import imresize, fspecial, SCFpyr_PyTorch, dct2d, im2col, ExactPadding2d
 from pyiqa.archs.func_util import extract_2d_patches
 from pyiqa.archs.ssim_arch import ssim as ssim_func
-from pyiqa.archs.arch_util import ExactPadding2d
 from pyiqa.archs.niqe_arch import NIQE
 from warnings import warn
 
 default_model_urls = {'url': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/NRQM_model.mat'}
 
 
 def get_guass_pyramid(x: Tensor, scale: int = 2):
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/paq2piq_arch.py` & `pyiqa-0.1.8/pyiqa/archs/paq2piq_arch.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 @ARCH_REGISTRY.register()
 class PAQ2PIQ(nn.Module):
 
     def __init__(self, backbone='resnet18', pretrained=True, pretrained_model_path=None):
         super(PAQ2PIQ, self).__init__()
 
         if backbone == 'resnet18':
-            model = tv.models.resnet18(pretrained=False)
+            model = tv.models.resnet18(weights='IMAGENET1K_V1')
             cut = -2
             spatial_scale = 1 / 32
 
         self.blk_size = 20, 20
 
         self.model_type = self.__class__.__name__
         self.body = nn.Sequential(*list(model.children())[:cut])
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/pieapp_arch.py` & `pyiqa-0.1.8/pyiqa/archs/pieapp_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/psnr_arch.py` & `pyiqa-0.1.8/pyiqa/archs/psnr_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/ssim_arch.py` & `pyiqa-0.1.8/pyiqa/archs/ssim_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/tres_arch.py` & `pyiqa-0.1.8/pyiqa/archs/tres_arch.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,39 +16,23 @@
 import torch.nn as nn
 from torch import Tensor
 import torch.nn.functional as F
 import torchvision.models as models
 
 from .arch_util import load_pretrained_network
 from pyiqa.utils.registry import ARCH_REGISTRY
+from .arch_util import random_crop
 
 
 default_model_urls = {
     'koniq': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/tres_koniq-f0502926.pth',
     'flive': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/tres_flive-09b0de5b.pth',
 }
 
 
-def random_crop(x, sample_size=224, sample_num=8):
-    b, c, h, w = x.shape
-    if min(h, w) <= sample_size:
-        scale_factor = (sample_size + 1) / min(h, w)
-        x = F.interpolate(x, scale_factor=scale_factor, mode='bicubic')
-        b, c, h, w = x.shape
-
-    th = tw = sample_size
-    cropped_x = []
-    for s in range(sample_num):
-        i = torch.randint(0, h - th + 1, size=(1, )).item()
-        j = torch.randint(0, w - tw + 1, size=(1, )).item()
-        cropped_x.append(x[:, :, i:i + th, j:j + tw])
-    cropped_x = torch.stack(cropped_x, dim=1)
-    return cropped_x
-
-
 def _get_activation_fn(activation):
     """Return an activation function given a string"""
     if activation == "relu":
         return F.relu
     if activation == "gelu":
         return F.gelu
     if activation == "glu":
@@ -261,24 +245,24 @@
         self.L2pooling_l1 = L2pooling(channels=256)
         self.L2pooling_l2 = L2pooling(channels=512)
         self.L2pooling_l3 = L2pooling(channels=1024)
         self.L2pooling_l4 = L2pooling(channels=2048)
 
         if network == 'resnet50':
             dim_modelt = 3840
-            self.model = models.resnet50(pretrained=True)
+            self.model = models.resnet50(weights='IMAGENET1K_V1')
         elif network == 'resnet34':
-            self.model = models.resnet34(pretrained=True)
+            self.model = models.resnet34(weights='IMAGENET1K_V1')
             dim_modelt = 960
             self.L2pooling_l1 = L2pooling(channels=64)
             self.L2pooling_l2 = L2pooling(channels=128)
             self.L2pooling_l3 = L2pooling(channels=256)
             self.L2pooling_l4 = L2pooling(channels=512)
         elif network == 'resnet18':
-            self.model = models.resnet18(pretrained=True)
+            self.model = models.resnet18(weights='IMAGENET1K_V1')
             dim_modelt = 960
             self.L2pooling_l1 = L2pooling(channels=64)
             self.L2pooling_l2 = L2pooling(channels=128)
             self.L2pooling_l3 = L2pooling(channels=256)
             self.L2pooling_l4 = L2pooling(channels=512)
 
         self.dim_modelt = dim_modelt
@@ -333,22 +317,22 @@
         x = torch.flatten(x, 1)
         x = model.fc(x)
 
         return x, l1, l2, l3, l4
 
     def forward(self, x):
         x = (x - self.default_mean.to(x)) / self.default_std.to(x)
+        bsz = x.shape[0]
 
         if self.training:
-            x = random_crop(x, sample_size=224, sample_num=1)
+            x = random_crop(x, 224, 1)
+            num_patches = 1
         else:
-            x = random_crop(x, sample_size=224, sample_num=self.test_sample)
-
-        bsz, num_patches, c, psz, psz = x.shape
-        x = x.reshape(bsz * num_patches, c, psz, psz)
+            x = random_crop(x, 224, self.test_sample)
+            num_patches = self.test_sample
 
         self.pos_enc_1 = self.position_embedding(torch.ones(1, self.dim_modelt, 7, 7).to(x))
         self.pos_enc = self.pos_enc_1.repeat(x.shape[0], 1, 1, 1).contiguous()
 
         out, layer1, layer2, layer3, layer4 = self.forward_backbone(self.model, x)
 
         layer1_t = self.avg8(self.drop2d(self.L2pooling_l1(F.normalize(layer1, dim=1, p=2))))
```

### Comparing `pyiqa-0.1.7/pyiqa/archs/uranker_arch.py` & `pyiqa-0.1.8/pyiqa/archs/uranker_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/vif_arch.py` & `pyiqa-0.1.8/pyiqa/archs/vif_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/vsi_arch.py` & `pyiqa-0.1.8/pyiqa/archs/vsi_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/archs/wadiqam_arch.py` & `pyiqa-0.1.8/pyiqa/archs/wadiqam_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/data/__init__.py` & `pyiqa-0.1.8/pyiqa/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/data/ava_dataset.py` & `pyiqa-0.1.8/pyiqa/data/ava_dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,63 @@
 import numpy as np
 import pickle
 from PIL import Image
-import cv2
 import os
-import random
-import itertools
 
 import torch
 from torch.utils import data as data
-import torchvision.transforms as tf
 
-from pyiqa.data.transforms import transform_mapping
 from pyiqa.utils.registry import DATASET_REGISTRY
 import pandas as pd
 
+from .base_iqa_dataset import BaseIQADataset 
+
 # avoid possible image read error in AVA dataset 
 from PIL import ImageFile
 ImageFile.LOAD_TRUNCATED_IMAGES = True
 
 @DATASET_REGISTRY.register()
-class AVADataset(data.Dataset):
+class AVADataset(BaseIQADataset):
     """AVA dataset, proposed by
 
     Murray, Naila, Luca Marchesotti, and Florent Perronnin. 
     "AVA: A large-scale database for aesthetic visual analysis." 
     In 2012 IEEE conference on computer vision and pattern recognition (CVPR), pp. 2408-2415. IEEE, 2012.
     
     Args:
         opt (dict): Config for train datasets with the following keys:
             phase (str): 'train' or 'val'.
     """
 
-    def __init__(self, opt):
-        super(AVADataset, self).__init__()
-        self.opt = opt
-
+    def init_path_mos(self, opt):
         target_img_folder = opt['dataroot_target']
         self.dataroot = target_img_folder
         self.paths_mos = pd.read_csv(opt['meta_info_file']).values.tolist()
-
+    
+    def get_split(self, opt):
         # read train/val/test splits
         split_file_path = opt.get('split_file', None)
         if split_file_path:
             split_index = opt.get('split_index', 1)
             with open(opt['split_file'], 'rb') as f:
                 split_dict = pickle.load(f)
             
             # use val_num for validation 
-            val_num = 2000
+            val_num = opt.get('val_num', 2000)
             train_split = split_dict[split_index]['train'] 
             val_split = split_dict[split_index]['val'] 
             train_split = train_split + val_split[:-val_num]
             val_split = val_split[-val_num:]
             split_dict[split_index]['train'] = train_split
             split_dict[split_index]['val'] = val_split 
 
-            if opt.get('override_phase', None) is None:
-                splits = split_dict[split_index][opt['phase']]
-            else:
-                splits = split_dict[split_index][opt['override_phase']]
-            
+            splits = split_dict[split_index][self.phase]
             self.paths_mos = [self.paths_mos[i] for i in splits] 
-        
-        self.mean_mos = np.array([item[1] for item in self.paths_mos]).mean()
 
-        # self.paths_mos.sort(key=lambda x: x[1])
-        # n = 32
-        # n = 4
-        # tmp_list = [self.paths_mos[i: i + n] for i in range(0, len(self.paths_mos), n)]
-        # random.shuffle(tmp_list)
-        # self.paths_mos = list(itertools.chain.from_iterable(tmp_list))
-
-        transform_list = []
-        augment_dict = opt.get('augment', None)
-        if augment_dict is not None:
-            for k, v in augment_dict.items():
-                transform_list += transform_mapping(k, v)
-
-        img_range = opt.get('img_range', 1.0)
-        transform_list += [
-                tf.ToTensor(),
-                tf.Lambda(lambda x: x * img_range),
-                ]
-        self.trans = tf.Compose(transform_list)
+        self.mean_mos = np.array([item[1] for item in self.paths_mos]).mean()
 
     def __getitem__(self, index):
 
         img_path = os.path.join(self.dataroot, self.paths_mos[index][0])
         mos_label = self.paths_mos[index][1]
         mos_dist = self.paths_mos[index][2:12]
         img_pil = Image.open(img_path).convert('RGB')
@@ -100,10 +71,7 @@
         if self.opt.get('list_imgs', False):
             tmp_tensor = torch.zeros((img_tensor.shape[0], 800, 800)) 
             h, w = img_tensor.shape[1:]
             tmp_tensor[..., :h, :w] = img_tensor
             return {'img': tmp_tensor, 'mos_label': mos_label_tensor, 'mos_dist': mos_dist_tensor, 'org_size': torch.tensor([height, width]), 'img_path': img_path, 'mean_mos': torch.tensor(self.mean_mos)}
         else:
             return {'img': img_tensor, 'img2': img_tensor2, 'mos_label': mos_label_tensor, 'mos_dist': mos_dist_tensor, 'org_size': torch.tensor([height, width]), 'img_path': img_path, 'mean_mos': torch.tensor(self.mean_mos)}
-
-    def __len__(self):
-        return len(self.paths_mos)
```

### Comparing `pyiqa-0.1.7/pyiqa/data/data_sampler.py` & `pyiqa-0.1.8/pyiqa/data/data_sampler.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/data/data_util.py` & `pyiqa-0.1.8/pyiqa/data/data_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/data/flive_dataset.py` & `pyiqa-0.1.8/pyiqa/data/piq_dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,71 @@
-import numpy as np
-import pickle
+import torch
+import os
+import csv
 from PIL import Image
-import cv2
 
-import torch
-from torch.utils import data as data
-import torchvision.transforms as tf
-from torchvision.transforms.functional import normalize
-
-from pyiqa.data.data_util import read_meta_info_file
-from pyiqa.data.transforms import transform_mapping
-from pyiqa.utils import FileClient, imfrombytes, img2tensor
+from pyiqa.data.data_util import read_meta_info_file 
 from pyiqa.utils.registry import DATASET_REGISTRY
+from pyiqa.utils import get_root_logger
+from .general_nr_dataset import GeneralNRDataset
 
 
 @DATASET_REGISTRY.register()
-class FLIVEDataset(data.Dataset):
+class PIQDataset(GeneralNRDataset):
     """General No Reference dataset with meta info file.
-
-    Args:
-        opt (dict): Config for train datasets with the following keys:
-            phase (str): 'train' or 'val'.
     """
+    def init_path_mos(self, opt):
+        logger = get_root_logger()
+        target_img_folder = opt['dataroot_target']
+        attr = opt.get('attribute', 'Overall')
 
-    def __init__(self, opt):
-        super(FLIVEDataset, self).__init__()
-        self.opt = opt
+        assert attr in ['Details', 'Exposure', 'Overall'], f'attribute should be in [Details, Exposure, Overall], got {attr}'
 
-        target_img_folder = opt['dataroot_target']
-        self.paths_mos = read_meta_info_file(target_img_folder, opt['meta_info_file'])
+        logger.info(f'Training on PIQ2023 dataset with attribute [{attr}]')
 
-        # read train/val/test splits
-        split_file_path = opt.get('split_file', None)
-        if split_file_path:
-            split_index = opt.get('split_index', 1)
-            with open(opt['split_file'], 'rb') as f:
-                split_dict = pickle.load(f)
-                if opt.get('override_phase', None) is None:
-                    splits = split_dict[split_index][opt['phase']]
-                else:
-                    splits = split_dict[split_index][opt['override_phase']]
-
-            self.paths_mos = [self.paths_mos[i] for i in splits]
-
-        dmos_max = opt.get('dmos_max', 0.)
-        if dmos_max:
-            self.use_dmos = True
-            self.dmos_max = opt.get('dmos_max')
-        else:
-            self.use_dmos = False
-        self.mos_max = opt.get('mos_max', 1.)
-
-        transform_list = []
-        augment_dict = opt.get('augment', None)
-        if augment_dict is not None:
-            for k, v in augment_dict.items():
-                transform_list += transform_mapping(k, v)
-
-        self.img_range = opt.get('img_range', 1.0)
-        transform_list += [
-            tf.ToTensor(),
-        ]
-        self.trans = tf.Compose(transform_list)
+        with open(opt['meta_info_file'], 'r') as fin:
+            csvreader = csv.reader(fin)
+            name_mos = list(csvreader)[1:]
+        
+        self.paths_mos = name_mos
+
+        self.paths_mos = []
+        for item in name_mos:
+            if attr in item[0]:
+                item[0] = os.path.join(target_img_folder, item[0])
+                self.paths_mos.append(item)
+    
+    def get_split(self, opt):
+        """Get split for PIQ2023 dataset:
+            1: device split
+            2: scene split 
+        """
+        logger = get_root_logger()
+        split_index = opt.get('split_index', None)
+        if split_index is not None:
+            assert split_index in [1, 2], f'split indexes should be, 1: device split; 2: scene split'
+            assert self.phase in ['train', 'test'], f'PIQDataset has no {self.phase} split'
+            
+            logger.info(f'Training on PIQ2023 dataset with split [{split_index}](1: device split; 2: scene split)')
+
+            new_paths_mos = []
+            for item in self.paths_mos:
+                if self.phase == 'train' and item[split_index - 3] == 'Train':
+                    new_paths_mos.append(item)
+                elif self.phase == 'test' and item[split_index - 3] == 'Test':
+                    new_paths_mos.append(item)
+            
+            self.paths_mos = new_paths_mos
 
     def __getitem__(self, index):
 
         img_path = self.paths_mos[index][0]
-        mos_label = self.paths_mos[index][1]
+        mos_label = float(self.paths_mos[index][1])
         img_pil = Image.open(img_path).convert('RGB')
 
         img_tensor = self.trans(img_pil) * self.img_range
-        if self.use_dmos:
-            mos_label = self.dmos_max - mos_label
-        else:
-            mos_label = mos_label / self.mos_max
         mos_label_tensor = torch.Tensor([mos_label])
 
-        return {'img': img_tensor, 'mos_label': mos_label_tensor, 'img_path': img_path}
-
-    def __len__(self):
-        return len(self.paths_mos)
+        scene_idx = int(self.paths_mos[index][-4])
+                
+        return {'img': img_tensor, 'mos_label': mos_label_tensor, 'img_path': img_path, 'scene_idx': scene_idx}
+
```

### Comparing `pyiqa-0.1.7/pyiqa/data/general_fr_dataset.py` & `pyiqa-0.1.8/pyiqa/data/general_fr_dataset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,70 @@
-import numpy as np
-import pickle
 from PIL import Image
 
 import torch
 from torch.utils import data as data
 import torchvision.transforms as tf
-from torchvision.transforms.functional import normalize
 
 from pyiqa.data.data_util import read_meta_info_file 
-from pyiqa.data.transforms import transform_mapping, augment, PairedToTensor
-from pyiqa.utils import FileClient, imfrombytes, img2tensor
+from pyiqa.data.transforms import transform_mapping, PairedToTensor
 from pyiqa.utils.registry import DATASET_REGISTRY
 
+from .base_iqa_dataset import BaseIQADataset
 
 @DATASET_REGISTRY.register()
-class GeneralFRDataset(data.Dataset):
+class GeneralFRDataset(BaseIQADataset):
     """General Full Reference dataset with meta info file.
-    
-    Args:
-        opt (dict): Config for train datasets with the following keys:
-            phase (str): 'train' or 'val'.
     """
-
-    def __init__(self, opt):
-        super(GeneralFRDataset, self).__init__()
-        self.opt = opt
-
-        if opt.get('override_phase', None) is None:
-            self.phase = opt['phase']
-        else:
-            self.phase = opt['override_phase']
-
+    
+    def init_path_mos(self, opt):
         target_img_folder = opt['dataroot_target']
         ref_img_folder = opt.get('dataroot_ref', None)
         self.paths_mos = read_meta_info_file(target_img_folder, opt['meta_info_file'], mode='fr', ref_dir=ref_img_folder) 
 
-        # read train/val/test splits
-        split_file_path = opt.get('split_file', None)
-        if split_file_path:
-            split_index = opt.get('split_index', 1)
-            with open(opt['split_file'], 'rb') as f:
-                split_dict = pickle.load(f)
-                splits = split_dict[split_index][self.phase]
-            self.paths_mos = [self.paths_mos[i] for i in splits] 
-        
-        dmos_max = opt.get('dmos_max', 0.)
-        if dmos_max:
-            self.use_dmos = True
-            self.dmos_max = opt.get('dmos_max') 
-        else:
-            self.use_dmos = False
-        
-        self.mos_max = opt.get('mos_max', 1.)
-
+    def get_transforms(self, opt):
         # do paired transform first and then do common transform
         paired_transform_list = []
         augment_dict = opt.get('augment', None)
         if augment_dict is not None:
             for k, v in augment_dict.items():
                 paired_transform_list += transform_mapping(k, v)
         self.paired_trans = tf.Compose(paired_transform_list)
 
         common_transform_list = []
         self.img_range = opt.get('img_range', 1.0)
         common_transform_list += [
                 PairedToTensor(),
                 ]
         self.common_trans = tf.Compose(common_transform_list)
+    
+    def mos_normalize(self, opt):
+        mos_range = opt.get('mos_range', None)
+        mos_lower_better = opt.get('lower_better', None)
+        mos_normalize = opt.get('mos_normalize', False)
+
+        if mos_normalize:
+            assert mos_range is not None and mos_lower_better is not None, 'mos_range and mos_lower_better should be provided when mos_normalize is True'
+
+            def normalize(mos_label):
+                mos_label = (mos_label - mos_range[0]) / (mos_range[1] - mos_range[0])
+                if mos_lower_better:
+                    mos_label = 1 - mos_label
+                return mos_label
 
+            self.paths_mos = [item[:2] + [normalize(item[2])] for item in self.paths_mos]
+            self.logger.info(f'mos_label is normalized from {mos_range}, lower_better[{mos_lower_better}] to [0, 1], higher better.')
 
     def __getitem__(self, index):
 
         ref_path = self.paths_mos[index][0]
         img_path = self.paths_mos[index][1]
         mos_label = self.paths_mos[index][2]
         img_pil = Image.open(img_path).convert('RGB')
         ref_pil = Image.open(ref_path).convert('RGB')
         
         img_pil, ref_pil = self.paired_trans([img_pil, ref_pil])
 
         img_tensor = self.common_trans(img_pil) * self.img_range
         ref_tensor = self.common_trans(ref_pil) * self.img_range
-        if self.use_dmos:
-            mos_label = (self.dmos_max - mos_label) / self.dmos_max
-        else:
-            mos_label /= self.mos_max
         mos_label_tensor = torch.Tensor([mos_label])
         
         return {'img': img_tensor, 'ref_img': ref_tensor, 'mos_label': mos_label_tensor, 'img_path': img_path, 'ref_img_path': ref_path}
-
-    def __len__(self):
-        return len(self.paths_mos)
```

### Comparing `pyiqa-0.1.7/pyiqa/data/livechallenge_dataset.py` & `pyiqa-0.1.8/pyiqa/data/base_iqa_dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,90 @@
-import numpy as np
 import pickle
-from PIL import Image
-import os
 
-import torch
 from torch.utils import data as data
 import torchvision.transforms as tf
-from torchvision.transforms.functional import normalize
 
 from pyiqa.data.data_util import read_meta_info_file
-from pyiqa.data.transforms import transform_mapping, augment
-from pyiqa.utils import FileClient, imfrombytes, img2tensor
-from pyiqa.utils.registry import DATASET_REGISTRY
+from pyiqa.data.transforms import transform_mapping, PairedToTensor
+from pyiqa.utils import get_root_logger
 
 
-@DATASET_REGISTRY.register()
-class LIVEChallengeDataset(data.Dataset):
-    """The LIVE Challenge Dataset introduced by
-
-    D. Ghadiyaram and A.C. Bovik, 
-    "Massive Online Crowdsourced Study of Subjective and Objective Picture Quality," 
-    IEEE Transactions on Image Processing, 2016
-    url: https://live.ece.utexas.edu/research/ChallengeDB/index.html 
+class BaseIQADataset(data.Dataset):
+    """General No Reference dataset with meta info file.
     
     Args:
         opt (dict): Config for train datasets with the following keys:
             phase (str): 'train' or 'val'.
     """
 
     def __init__(self, opt):
-        super(LIVEChallengeDataset, self).__init__()
         self.opt = opt
+        self.logger = get_root_logger()
 
-        target_img_folder = os.path.join(opt['dataroot_target'], 'Images')
+        if opt.get('override_phase', None) is None:
+            self.phase = opt['phase']
+        else:
+            self.phase = opt['override_phase']
+
+        # initialize datasets
+        self.init_path_mos(opt)
+
+        # mos normalization
+        self.mos_normalize(opt)
+
+        # read train/val/test splits
+        self.get_split(opt)
+
+        # get transforms       
+        self.get_transforms(opt)
+            
+    def init_path_mos(self, opt):
+        target_img_folder = opt['dataroot_target']
         self.paths_mos = read_meta_info_file(target_img_folder, opt['meta_info_file']) 
-        # remove first 7 training images as previous works
-        self.paths_mos = self.paths_mos[7:] 
 
+    def get_split(self, opt):
         # read train/val/test splits
         split_file_path = opt.get('split_file', None)
         if split_file_path:
             split_index = opt.get('split_index', 1)
             with open(opt['split_file'], 'rb') as f:
                 split_dict = pickle.load(f)
-                splits = split_dict[split_index][opt['phase']]
+                splits = split_dict[split_index][self.phase]
             self.paths_mos = [self.paths_mos[i] for i in splits] 
+    
+    def mos_normalize(self, opt):
+        mos_range = opt.get('mos_range', None)
+        mos_lower_better = opt.get('lower_better', None)
+        mos_normalize = opt.get('mos_normalize', False)
+
+        if mos_normalize:
+            assert mos_range is not None and mos_lower_better is not None, 'mos_range and mos_lower_better should be provided when mos_normalize is True'
+
+            def normalize(mos_label):
+                mos_label = (mos_label - mos_range[0]) / (mos_range[1] - mos_range[0])
+                # convert to higher better if lower better is true
+                if mos_lower_better:
+                    mos_label = 1 - mos_label
+                return mos_label
+
+            for item in self.paths_mos:
+                item[1] = normalize(float(item[1]))
+            self.logger.info(f'mos_label is normalized from {mos_range}, lower_better[{mos_lower_better}] to [0, 1], lower_better[False(higher better)].')
 
+    def get_transforms(self, opt):
         transform_list = []
         augment_dict = opt.get('augment', None)
         if augment_dict is not None:
             for k, v in augment_dict.items():
                 transform_list += transform_mapping(k, v)
 
-        img_range = opt.get('img_range', 1.0)
+        self.img_range = opt.get('img_range', 1.0)
         transform_list += [
-                tf.ToTensor(),
-                tf.Lambda(lambda x: x * img_range),
+                PairedToTensor(),
                 ]
         self.trans = tf.Compose(transform_list)
 
     def __getitem__(self, index):
-
-        img_path = self.paths_mos[index][0]
-        mos_label = self.paths_mos[index][1]
-        img_pil = Image.open(img_path)
-
-        img_tensor = self.trans(img_pil)
-        mos_label_tensor = torch.Tensor([mos_label])
-        
-        return {'img': img_tensor, 'mos_label': mos_label_tensor, 'img_path': img_path}
+        pass
 
     def __len__(self):
         return len(self.paths_mos)
```

### Comparing `pyiqa-0.1.7/pyiqa/data/multiscale_trans_util.py` & `pyiqa-0.1.8/pyiqa/data/multiscale_trans_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/data/pieapp_dataset.py` & `pyiqa-0.1.8/pyiqa/data/bapps_dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,98 @@
-import numpy as np
 import pickle
 from PIL import Image
 import os
 
 import torch
 from torch.utils import data as data
-import torchvision.transforms as tf
-from torchvision.transforms.functional import normalize
 
-from pyiqa.data.data_util import read_meta_info_file 
-from pyiqa.data.transforms import transform_mapping, augment, PairedToTensor
-from pyiqa.utils import FileClient, imfrombytes, img2tensor
 from pyiqa.utils.registry import DATASET_REGISTRY
+from .base_iqa_dataset import BaseIQADataset 
 
 import pandas as pd
 
 
 @DATASET_REGISTRY.register()
-class PieAPPDataset(data.Dataset):
-    """The PieAPP Dataset introduced by:
+class BAPPSDataset(BaseIQADataset):
+    """The BAPPS Dataset introduced by:
 
-    Prashnani, Ekta and Cai, Hong and Mostofi, Yasamin and Sen, Pradeep
-    PieAPP: Perceptual Image-Error Assessment Through Pairwise Preference
+    Zhang, Richard and Isola, Phillip and Efros, Alexei A and Shechtman, Eli and Wang, Oliver
+    The Unreasonable Effectiveness of Deep Features as a Perceptual Metric.
     CVPR2018
-    url: http://civc.ucsb.edu/graphics/Papers/CVPR2018_PieAPP/
+    url: https://github.com/richzhang/PerceptualSimilarity
     
     Args:
         opt (dict): Config for train datasets with the following keys:
             phase (str): 'train' or 'val'.
+        mode (str):
+            - 2afc: load 2afc triplet data
+            - jnd: load jnd pair data
     """
 
-    def __init__(self, opt):
-        super(PieAPPDataset, self).__init__()
-        self.opt = opt
-
-        target_img_folder = opt['dataroot_target']
-        self.dataroot = target_img_folder
-
+    def init_path_mos(self, opt):
         if opt.get('override_phase', None) is None:
-            self.phase = opt['phase']
+            self.phase = opt['phase'] 
         else:
-            self.phase = opt['override_phase']
+            self.phase = opt['override_phase'] 
 
-        if self.phase == "test":
-            metadata = pd.read_csv(opt['meta_info_file'], usecols=['ref_img_path', 'dist_imgB_path', 'per_img score for dist_imgB'])
-        else:
-            metadata = pd.read_csv(opt['meta_info_file'])
-        self.paths_mos = metadata.values.tolist()
+        self.dataset_mode = opt.get('mode', '2afc')
 
+        target_img_folder = opt['dataroot_target']
+        self.dataroot = target_img_folder
+
+        self.paths_mos = pd.read_csv(opt['meta_info_file']).values.tolist()
+    
+    def get_split(self, opt):
+        val_types = opt.get('val_types', None)
         # read train/val/test splits
         split_file_path = opt.get('split_file', None)
         if split_file_path:
             split_index = opt.get('split_index', 1)
             with open(opt['split_file'], 'rb') as f:
                 split_dict = pickle.load(f)
                 splits = split_dict[split_index][self.phase]
             self.paths_mos = [self.paths_mos[i] for i in splits] 
-        
-        # remove duplicates
-        if self.phase == 'test':
-            temp = []
-            [temp.append(item) for item in self.paths_mos if not item in temp]
-            self.paths_mos = temp
-        
-        # do paired transform first and then do common transform
-        paired_transform_list = []
-        augment_dict = opt.get('augment', None)
-        if augment_dict is not None:
-            for k, v in augment_dict.items():
-                paired_transform_list += transform_mapping(k, v)
-        self.paired_trans = tf.Compose(paired_transform_list)
-
-        common_transform_list = []
-        self.img_range = opt.get('img_range', 1.0)
-        common_transform_list += [
-                PairedToTensor(),
-                ]
-        self.common_trans = tf.Compose(common_transform_list)
 
+        if self.dataset_mode == '2afc':
+            self.paths_mos = [x for x in self.paths_mos if x[0] != 'jnd']
+        elif self.dataset_mode == 'jnd':
+            self.paths_mos = [x for x in self.paths_mos if x[0] == 'jnd']
+        
+        if val_types is not None:
+            tmp_paths_mos = []
+            for item in self.paths_mos:
+                for vt in val_types:
+                    if vt in item[1]:
+                        tmp_paths_mos.append(item)
+            self.paths_mos = tmp_paths_mos
         
     def __getitem__(self, index):
+        is_jnd_data = self.paths_mos[index][0] == 'jnd'
+        distA_path = os.path.join(self.dataroot, self.paths_mos[index][1])
+        distB_path = os.path.join(self.dataroot, self.paths_mos[index][2])
 
-        ref_path = os.path.join(self.dataroot, self.paths_mos[index][0])
-        if self.phase == "test":
-            distB_path = os.path.join(self.dataroot, self.paths_mos[index][1])
-        else:
-            distA_path = os.path.join(self.dataroot, self.paths_mos[index][1])
-            distB_path = os.path.join(self.dataroot, self.paths_mos[index][2])
-        
+        distA_pil = Image.open(distA_path).convert('RGB')
         distB_pil = Image.open(distB_path).convert('RGB')
-        ref_img_pil = Image.open(ref_path).convert('RGB')
 
-        if self.phase != 'test':
-            distA_pil = Image.open(distA_path).convert('RGB')
+        score = self.paths_mos[index][3]
+        # original 0 means prefer p0, transfer to probability of p0
+        mos_label_tensor = torch.Tensor([score]) 
+
+        if not is_jnd_data:
+            ref_path = os.path.join(self.dataroot, self.paths_mos[index][0])
+            ref_img_pil = Image.open(ref_path).convert('RGB')
 
-            distA_pil, distB_pil, ref_img_pil = self.paired_trans([distA_pil, distB_pil, ref_img_pil])
-
-            distA_tensor, distB_tensor, ref_tensor = self.common_trans([distA_pil, distB_pil, ref_img_pil])
+            distA_tensor, distB_tensor, ref_tensor = self.trans([distA_pil, distB_pil, ref_img_pil])
         else:
-            distB_pil, ref_img_pil = self.paired_trans([distB_pil, ref_img_pil])
-            distB_tensor, ref_tensor = self.common_trans([distB_pil, ref_img_pil])
+            distA_tensor, distB_tensor = self.trans([distA_pil, distB_pil])
 
-        if self.phase == 'train':
-            score = self.paths_mos[index][4]
-            mos_label_tensor = torch.Tensor([score])
-            distB_score = torch.Tensor([-1])
-        elif self.phase == 'val':
-            score = self.paths_mos[index][4]
-            mos_label_tensor = torch.Tensor([score])
-            distB_score = torch.Tensor([-1])
-        elif self.phase == 'test':
-            per_img_score = self.paths_mos[index][2]
-            distB_score = torch.Tensor([per_img_score])
-        
-        if self.phase == 'test':
-            return {'img': distB_tensor, 'ref_img': ref_tensor, 'mos_label': distB_score, 
-                    'img_path': distB_path, 'ref_img_path': ref_path}
+        if not is_jnd_data:
+
+            return {'ref_img': ref_tensor, 'distB_img': distB_tensor, 'distA_img': distA_tensor, 
+                    'mos_label': mos_label_tensor,  
+                    'img_path': ref_path, 'distB_path': distB_path, 'distA_path': distA_path}
         else:
-            return {'distB_img': distB_tensor, 'ref_img': ref_tensor, 'distA_img': distA_tensor, 
-                    'mos_label': mos_label_tensor, 'distB_per_img_score': distB_score, 
-                    'distB_path': distB_path, 'ref_img_path': ref_path, 'distA_path': distA_path}
 
-    def __len__(self):
-        return len(self.paths_mos)
+            return {'distB_img': distB_tensor, 'distA_img': distA_tensor, 
+                'mos_label': mos_label_tensor,  
+                'distB_path': distB_path, 'distA_path': distA_path}
+
```

### Comparing `pyiqa-0.1.7/pyiqa/data/prefetch_dataloader.py` & `pyiqa-0.1.8/pyiqa/data/prefetch_dataloader.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/data/transforms.py` & `pyiqa-0.1.8/pyiqa/data/transforms.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,56 +40,56 @@
         return [ChangeColorSpace(args)]
     elif key == 'totensor' and args:
         return [PairedToTensor()]
     else:
         return []
 
 
-def _check_pair(x):
+def _is_pair(x):
     if isinstance(x, (tuple, list)) and len(x) >= 2:
         return True
 
 
 class PairedToTensor(tf.ToTensor):
     """Pair version of center crop"""
     def to_tensor(self, x):
         if isinstance(x, torch.Tensor):
             return x
         else:
-            return F.to_tensor(x)
+            return super().__call__(x)
 
     def __call__(self, imgs):
-        if _check_pair(imgs):
+        if _is_pair(imgs):
             for i in range(len(imgs)):
                 imgs[i] = self.to_tensor(imgs[i])
             return imgs 
         else:
             return self.to_tensor(imgs) 
 
 
 class ChangeColorSpace:
     """Pair version of center crop"""
     def __init__(self, to_colorspace):
         self.aug_op = iaa.color.ChangeColorspace(to_colorspace)
 
     def __call__(self, imgs):
-        if _check_pair(imgs):
+        if _is_pair(imgs):
             for i in range(len(imgs)):
                 tmpimg = self.aug_op.augment_image(np.array(imgs[i]))
                 imgs[i] = Image.fromarray(tmpimg)
             return imgs 
         else:
             imgs = self.aug_op.augment_image(np.array(imgs))
             return Image.fromarray(imgs)
 
 
 class PairedCenterCrop(tf.CenterCrop):
     """Pair version of center crop"""
     def forward(self, imgs):
-        if _check_pair(imgs):
+        if _is_pair(imgs):
             for i in range(len(imgs)):
                 imgs[i] = super().forward(imgs[i])
             return imgs
         elif isinstance(imgs, Image.Image):
             return super().forward(imgs)
 
 
@@ -107,30 +107,30 @@
         # pad the height if needed
         if self.pad_if_needed and height < self.size[0]:
             padding = [0, self.size[0] - height]
             img = F.pad(img, padding, self.fill, self.padding_mode)
         return img
 
     def forward(self, imgs):
-        if _check_pair(imgs):
+        if _is_pair(imgs):
             i, j, h, w = self.get_params(imgs[0], self.size)
             for i in range(len(imgs)):
                 img = self._pad(imgs[i]) 
                 img = F.crop(img, i, j, h, w)
                 imgs[i] = img
             return imgs
         elif isinstance(imgs, Image.Image):
             return super().forward(imgs)
 
 
 class PairedRandomErasing(tf.RandomErasing):
     """Pair version of random erasing"""
 
     def forward(self, imgs):
-        if _check_pair(imgs):
+        if _is_pair(imgs):
             if torch.rand(1) < self.p:
                 # cast self.value to script acceptable type
                 if isinstance(self.value, (int, float)):
                     value = [self.value]
                 elif isinstance(self.value, str):
                     value = None
                 elif isinstance(self.value, tuple):
@@ -151,27 +151,27 @@
         elif isinstance(imgs, Image.Image):
             return super().forward(imgs)
 
 
 class PairedRandomHorizontalFlip(tf.RandomHorizontalFlip):
     """Pair version of random hflip"""
     def forward(self, imgs):
-        if _check_pair(imgs):
+        if _is_pair(imgs):
             if torch.rand(1) < self.p:
                 for i in range(len(imgs)):
                     imgs[i] = F.hflip(imgs[i])
             return imgs
         elif isinstance(imgs, Image.Image):
             return super().forward(imgs)
 
 
 class PairedRandomVerticalFlip(tf.RandomVerticalFlip):
     """Pair version of random hflip"""
     def forward(self, imgs):
-        if _check_pair(imgs):
+        if _is_pair(imgs):
             if torch.rand(1) < self.p:
                 for i in range(len(imgs)):
                     imgs[i] = F.vflip(imgs[i])
             return imgs
         elif isinstance(imgs, Image.Image):
             return super().forward(imgs)
 
@@ -180,40 +180,40 @@
 class PairedRandomRot90(torch.nn.Module):
     """Pair version of random hflip"""
     def __init__(self, p=0.5):
         super().__init__()
         self.p = p
 
     def forward(self, imgs):
-        if _check_pair(imgs):
+        if _is_pair(imgs):
             if torch.rand(1) < self.p:
                 for i in range(len(imgs)):
                     imgs[i] = F.rotate(imgs[i], 90)
             return imgs
         elif isinstance(imgs, Image.Image):
             if torch.rand(1) < self.p:
                 imgs = F.rotate(imgs, 90)
             return imgs
 
 
 class PairedResize(tf.Resize):
     """Pair version of resize"""
     def forward(self, imgs):
-        if _check_pair(imgs):
+        if _is_pair(imgs):
             for i in range(len(imgs)):
                 imgs[i] = super().forward(imgs[i])
             return imgs
         elif isinstance(imgs, Image.Image): 
             return super().forward(imgs)
 
 
 class PairedAdaptiveResize(tf.Resize):
     """ARP preserved resize when necessary"""
     def forward(self, imgs):
-        if _check_pair(imgs):
+        if _is_pair(imgs):
             for i in range(len(imgs)):
                 tmpimg = imgs[i]
                 min_size = min(tmpimg.size)
                 if min_size < self.size:
                     tmpimg = super().forward(tmpimg)
                 imgs[i] = tmpimg
             return imgs
@@ -234,15 +234,15 @@
         self.size_range = size_range
         if not (isinstance(size_range, Sequence) and len(size_range) == 2):
             raise TypeError(f"size_range should be sequence with 2 int. Got {size_range} with {type(size_range)}")
 
     def forward(self, imgs):
         min_size, max_size = sorted(self.size_range)
         target_size = random.randint(min_size, max_size)
-        if _check_pair(imgs):
+        if _is_pair(imgs):
             for i in range(len(imgs)):
                 imgs[i] = F.resize(imgs[i], target_size, self.interpolation)
             return imgs
         elif isinstance(imgs, Image.Image): 
             return F.resize(imgs, target_size, self.interpolation)
 
 
@@ -256,15 +256,15 @@
         if not (isinstance(size_range, Sequence) and len(size_range) == 2):
             raise TypeError(f"size_range should be sequence with 2 int. Got {size_range} with {type(size_range)}")
 
     def forward(self, imgs):
         min_size, max_size = sorted(self.size_range)
         target_size = random.randint(min_size, max_size)
         target_size = (target_size, target_size)
-        if _check_pair(imgs):
+        if _is_pair(imgs):
             for i in range(len(imgs)):
                 imgs[i] = F.resize(imgs[i], target_size, self.interpolation)
             return imgs
         elif isinstance(imgs, Image.Image): 
             return F.resize(imgs, target_size, self.interpolation)
 
 
@@ -282,15 +282,15 @@
         assert th >= h and tw >= w, f'Target size {self.target_size} should be larger than image size ({h}, {w})'
         pad_row = th - h 
         pad_col = tw - w
         pad_l, pad_r, pad_t, pad_b = (pad_col//2, pad_col - pad_col//2, pad_row//2, pad_row - pad_row//2)
         return (pad_l, pad_t, pad_r, pad_b)
 
     def forward(self, imgs):
-        if _check_pair(imgs):
+        if _is_pair(imgs):
             for i in range(len(imgs)):
                 padding = self.get_padding(imgs[i])
                 imgs[i] = F.pad(imgs[i], padding, self.fill, self.padding_mode)
             return imgs
         elif isinstance(imgs, Image.Image): 
             padding = self.get_padding(imgs)
             imgs = F.pad(imgs, padding, self.fill, self.padding_mode)
```

### Comparing `pyiqa-0.1.7/pyiqa/default_model_configs.py` & `pyiqa-0.1.8/pyiqa/default_model_configs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from collections import OrderedDict
 
-IMAGENET_DEFAULT_MEAN = (0.485, 0.456, 0.406)
-IMAGENET_DEFAULT_STD = (0.229, 0.224, 0.225)
-
 DEFAULT_CONFIGS = OrderedDict({
     'ahiq': {
         'metric_opts': {
             'type': 'AHIQ',
         },
         'metric_mode': 'FR',
     },
@@ -30,14 +27,32 @@
             'type': 'LPIPS',
             'net': 'vgg',
             'version': '0.1',
         },
         'metric_mode': 'FR',
         'lower_better': True,
     },
+    'stlpips': {
+        'metric_opts': {
+            'type': 'STLPIPS',
+            'net': 'alex',
+            'variant': 'shift_tolerant',
+        },
+        'metric_mode': 'FR',
+        'lower_better': True,
+    },
+    'stlpips-vgg': {
+        'metric_opts': {
+            'type': 'STLPIPS',
+            'net': 'vgg',
+            'variant': 'shift_tolerant',
+        },
+        'metric_mode': 'FR',
+        'lower_better': True,
+    },
     'dists': {
         'metric_opts': {
             'type': 'DISTS',
         },
         'metric_mode': 'FR',
         'lower_better': True,
     },
@@ -125,15 +140,14 @@
             'test_y_channel': True,
         },
         'metric_mode': 'FR',
     },
     'mad': {
         'metric_opts': {
             'type': 'MAD',
-            'test_y_channel': True,
         },
         'metric_mode': 'FR',
         'lower_better': True,
     },
     # =============================================================
     'niqe': {
         'metric_opts': {
@@ -212,23 +226,23 @@
             'pretrained': 'spaq'
         },
         'metric_mode': 'NR',
     },
     'nima': {
         'metric_opts': {
             'type': 'NIMA',
-            'pretrained': 'ava',
+            'num_classes': 10,
             'base_model_name': 'inception_resnet_v2',
         },
         'metric_mode': 'NR',
     },
     'nima-vgg16-ava': {
         'metric_opts': {
             'type': 'NIMA',
-            'pretrained': 'ava',
+            'num_classes': 10,
             'base_model_name': 'vgg16',
         },
         'metric_mode': 'NR',
     },
     'pieapp': {
         'metric_opts': {
             'type': 'PieAPP',
@@ -249,29 +263,38 @@
         },
         'metric_mode': 'NR',
     },
     'fid': {
         'metric_opts': {
             'type': 'FID',
         },
-        'metric_mode': 'NR'
+        'metric_mode': 'NR',
+        'lower_better': True,
     },
     'maniqa': {
         'metric_opts': {
             'type': 'MANIQA',
+            'train_dataset': 'koniq',
         },
         'metric_mode': 'NR',
     },
     'maniqa-koniq': {
         'metric_opts': {
             'type': 'MANIQA',
             'train_dataset': 'koniq',
         },
         'metric_mode': 'NR',
     },
+    'maniqa-pipal': {
+        'metric_opts': {
+            'type': 'MANIQA',
+            'train_dataset': 'pipal',
+        },
+        'metric_mode': 'NR',
+    },
     'maniqa-kadid': {
         'metric_opts': {
             'type': 'MANIQA',
             'train_dataset': 'kadid',
         },
         'metric_mode': 'NR',
     },
@@ -339,16 +362,102 @@
         },
         'metric_mode': 'NR',
     },
     'clipscore': {
         'metric_opts': {
             'type': 'CLIPScore',
         },
-        'metric_mode': 'NR', # Caption image similarity
+        'metric_mode': 'NR',  # Caption image similarity
     },
     'entropy': {
         'metric_opts': {
             'type': 'Entropy',
         },
         'metric_mode': 'NR',
+    },
+    'topiq_nr': {
+        'metric_opts': {
+            'type': 'CFANet',
+            'semantic_model_name': 'resnet50',
+            'model_name': 'cfanet_nr_koniq_res50',
+            'use_ref': False,
+        },
+        'metric_mode': 'NR',
+    },
+    'topiq_nr-flive': {
+        'metric_opts': {
+            'type': 'CFANet',
+            'semantic_model_name': 'resnet50',
+            'model_name': 'cfanet_nr_flive_res50',
+            'use_ref': False,
+        },
+        'metric_mode': 'NR',
+    },
+    'topiq_nr-spaq': {
+        'metric_opts': {
+            'type': 'CFANet',
+            'semantic_model_name': 'resnet50',
+            'model_name': 'cfanet_nr_spaq_res50',
+            'use_ref': False,
+        },
+        'metric_mode': 'NR',
+    },
+    'topiq_nr-face': {
+        'metric_opts': {
+            'type': 'CFANet',
+            'semantic_model_name': 'resnet50',
+            'model_name': 'topiq_nr_gfiqa_res50',
+            'use_ref': False,
+            'test_img_size': 512,
+        },
+        'metric_mode': 'NR',
+    },
+    'topiq_fr': {
+        'metric_opts': {
+            'type': 'CFANet',
+            'semantic_model_name': 'resnet50',
+            'model_name': 'cfanet_fr_kadid_res50',
+            'use_ref': True,
+        },
+        'metric_mode': 'FR',
+    },
+    'topiq_fr-pipal': {
+        'metric_opts': {
+            'type': 'CFANet',
+            'semantic_model_name': 'resnet50',
+            'model_name': 'cfanet_fr_pipal_res50',
+            'use_ref': True,
+        },
+        'metric_mode': 'FR',
+    },
+    'topiq_iaa': {
+        'metric_opts': {
+            'type': 'CFANet',
+            'semantic_model_name': 'swin_base_patch4_window12_384',
+            'model_name': 'cfanet_iaa_ava_swin',
+            'use_ref': False,
+            'inter_dim': 512,
+            'num_heads': 8,
+            'num_class': 10,
+        },
+        'metric_mode': 'NR',
+    },
+    'topiq_iaa_res50': {
+        'metric_opts': {
+            'type': 'CFANet',
+            'semantic_model_name': 'resnet50',
+            'model_name': 'cfanet_iaa_ava_res50',
+            'use_ref': False,
+            'inter_dim': 512,
+            'num_heads': 8,
+            'num_class': 10,
+            'test_img_size': 384,
+        },
+        'metric_mode': 'NR',
+    },
+    'laion_aes': {
+        'metric_opts': {
+            'type': 'LAIONAes',
+        },
+        'metric_mode': 'NR',
     }
 })
```

### Comparing `pyiqa-0.1.7/pyiqa/losses/__init__.py` & `pyiqa-0.1.8/pyiqa/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/losses/iqa_losses.py` & `pyiqa-0.1.8/pyiqa/losses/iqa_losses.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/losses/loss_util.py` & `pyiqa-0.1.8/pyiqa/losses/loss_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/losses/losses.py` & `pyiqa-0.1.8/pyiqa/losses/losses.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/matlab_utils/__init__.py` & `pyiqa-0.1.8/pyiqa/matlab_utils/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,22 +4,27 @@
 Note: to enable GPU acceleration, all functions take batched tensors as inputs,
 and return batched results.
 
 """
 from .resize import imresize
 from .functions import *
 from .scfpyr_util import SCFpyr_PyTorch
+from .padding import ExactPadding2d, exact_padding_2d, symm_pad
+
 
 __all__ = [
     'imresize',
     'fspecial',
     'SCFpyr_PyTorch',
     'imfilter',
     'dct2d',
     'conv2d',
     'filter2',
     'fitweibull',
     'nancov',
     'nanmean',
     'im2col',
     'blockproc',
+    'ExactPadding2d',
+    'exact_padding_2d',
+    'symm_pad',
 ]
```

### Comparing `pyiqa-0.1.7/pyiqa/matlab_utils/functions.py` & `pyiqa-0.1.8/pyiqa/matlab_utils/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 import numpy as np
 import torch
 import torch.nn.functional as F
-from pyiqa.archs.arch_util import ExactPadding2d, to_2tuple, symm_pad
+from .padding import ExactPadding2d, to_2tuple, symm_pad
 
 
 def fspecial(size=None, sigma=None, channels=1, filter_type='gaussian'):
     r""" Function same as 'fspecial' in MATLAB, only support gaussian now.
     Args:
         size (int or tuple): size of window
         sigma (float): sigma of gaussian
```

### Comparing `pyiqa-0.1.7/pyiqa/matlab_utils/math_util.py` & `pyiqa-0.1.8/pyiqa/matlab_utils/math_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/matlab_utils/resize.py` & `pyiqa-0.1.8/pyiqa/matlab_utils/resize.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/matlab_utils/scfpyr_util.py` & `pyiqa-0.1.8/pyiqa/matlab_utils/scfpyr_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/metrics/__init__.py` & `pyiqa-0.1.8/pyiqa/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/metrics/correlation_coefficient.py` & `pyiqa-0.1.8/pyiqa/metrics/correlation_coefficient.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/models/__init__.py` & `pyiqa-0.1.8/pyiqa/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/models/bapps_model.py` & `pyiqa-0.1.8/pyiqa/models/bapps_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/models/base_model.py` & `pyiqa-0.1.8/pyiqa/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/models/dbcnn_model.py` & `pyiqa-0.1.8/pyiqa/models/dbcnn_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/models/general_iqa_model.py` & `pyiqa-0.1.8/pyiqa/models/general_iqa_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,33 +52,73 @@
 
         # set up optimizers and schedulers
         self.setup_optimizers()
         self.setup_schedulers()
 
     def setup_optimizers(self):
         train_opt = self.opt['train']
+        optim_opt = train_opt['optim']
+
+        param_dict = {k: v for k, v in self.net.named_parameters()}
+        param_keys = list(param_dict.keys())
+        # set different lr for different modules if needed, e.g., lr_backbone, lr_head
+        lr_keys = [i for i in optim_opt.keys() if i.startswith('lr_')]
+
         optim_params = []
-        for k, v in self.net.named_parameters():
-            if v.requires_grad:
-                optim_params.append(v)
-            else:
+        for key in lr_keys:
+            if key.startswith('lr_'):
+                module_key = key.replace('lr_', '')
+                logger = get_root_logger()
+                logger.info(f'Set optimizer for {module_key} with lr: {optim_opt[key]}, weight_decay: {optim_opt.get(f"weight_decay_{module_key}", 0.)}')
+
+                optim_params.append({
+                    'params': [param_dict[k] for k in param_keys if module_key in k and param_dict[k].requires_grad],
+                    'lr': optim_opt.pop(key, 0.),
+                    'weight_decay': optim_opt.pop(f'weight_decay_{module_key}', 0.),
+                })
+
+                # should use param_keys[:] to avoid iteration error
+                for k in param_keys[:]:
+                    if module_key in k:
+                        param_keys.remove(k)
+        
+        # append the rest of the parameters
+        optim_params.append({
+            'params': [param_dict[k] for k in param_keys if param_dict[k].requires_grad],
+        })
+
+        # log params that will not be optimized
+        for k, v in param_dict.items():
+            if not v.requires_grad:
                 logger = get_root_logger()
                 logger.warning(f'Params {k} will not be optimized.')
+        
+        # remove blank param list
+        for k in optim_params:
+            if len(k['params']) == 0:
+                optim_params.remove(k)
 
         optim_type = train_opt['optim'].pop('type')
         self.optimizer = self.get_optimizer(optim_type, optim_params, **train_opt['optim'])
         self.optimizers.append(self.optimizer)
-
+    
     def feed_data(self, data):
         self.img_input = data['img'].to(self.device)
 
         if 'mos_label' in data:
             self.gt_mos = data['mos_label'].to(self.device)
 
-        self.use_ref = self.opt['train'].get('use_ref', False)
+        if 'ref_img' in data:
+            self.use_ref = True
+            self.ref_input = data['ref_img'].to(self.device)
+        else:
+            self.use_ref = False
+
+        if 'use_ref' in self.opt['train']:
+            self.use_ref = self.opt['train']['use_ref']
 
     def net_forward(self, net):
         if self.use_ref:
             return net(self.img_input, self.ref_input)
         else:
             return net(self.img_input)
```

### Comparing `pyiqa-0.1.7/pyiqa/models/hypernet_model.py` & `pyiqa-0.1.8/pyiqa/models/hypernet_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/models/inference_model.py` & `pyiqa-0.1.8/pyiqa/models/inference_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,19 @@
 
         with torch.set_grad_enabled(self.as_loss):
 
             if 'fid' in self.metric_name:
                 output = self.net(target, ref, device=self.device, **kwargs)
             else:
                 if not torch.is_tensor(target):
-                    target = imread2tensor(target)
+                    target = imread2tensor(target, rgb=True)
                     target = target.unsqueeze(0)
                     if self.metric_mode == 'FR':
                         assert ref is not None, 'Please specify reference image for Full Reference metric'
-                        ref = imread2tensor(ref)
+                        ref = imread2tensor(ref, rgb=True)
                         ref = ref.unsqueeze(0)
 
                 if self.metric_mode == 'FR':
                     output = self.net(target.to(self.device), ref.to(self.device), **kwargs)
                 elif self.metric_mode == 'NR':
                     output = self.net(target.to(self.device), **kwargs)
```

### Comparing `pyiqa-0.1.7/pyiqa/models/lr_scheduler.py` & `pyiqa-0.1.8/pyiqa/models/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/models/nima_model.py` & `pyiqa-0.1.8/pyiqa/models/distiqa_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,41 +3,23 @@
 
 from pyiqa.metrics import calculate_metric
 from pyiqa.utils.registry import MODEL_REGISTRY
 from .general_iqa_model import GeneralIQAModel
 
 
 @MODEL_REGISTRY.register()
-class NIMAModel(GeneralIQAModel):
+class DistIQAModel(GeneralIQAModel):
     """General module to train an IQA network."""
 
     def feed_data(self, data):
         self.img_input = data['img'].to(self.device)
         self.gt_mos = data['mos_label'].to(self.device)
         self.gt_mos_dist = data['mos_dist'].to(self.device)
         self.use_ref = False
 
-    def setup_optimizers(self):
-        train_opt = self.opt['train']
-        optim_opt = train_opt['optim']
-        optim_params = [
-            {
-                'params': self.get_bare_model(self.net).base_model.parameters(),
-                'lr': optim_opt.pop('lr_basemodel'),
-            },
-            {
-                'params': self.get_bare_model(self.net).classifier.parameters(),
-                'lr': optim_opt.pop('lr_classifier'),
-            },
-        ]
-
-        optim_type = optim_opt.pop('type')
-        self.optimizer = self.get_optimizer(optim_type, optim_params, **optim_opt)
-        self.optimizers.append(self.optimizer)
-
     def test(self):
         self.net.eval()
         with torch.no_grad():
             self.output_score = self.net(self.img_input, return_mos=True, return_dist=False)
         self.net.train()
 
     def optimize_parameters(self, current_iter):
```

### Comparing `pyiqa-0.1.7/pyiqa/models/pieapp_model.py` & `pyiqa-0.1.8/pyiqa/models/pieapp_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/models/wadiqam_model.py` & `pyiqa-0.1.8/pyiqa/models/wadiqam_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/test.py` & `pyiqa-0.1.8/pyiqa/test.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/train.py` & `pyiqa-0.1.8/pyiqa/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import datetime
 import logging
 import math
 import time
 import torch
 import os
+import tarfile
 from os import path as osp
 
 from pyiqa.data import build_dataloader, build_dataset
 from pyiqa.data.data_sampler import EnlargedSampler
 from pyiqa.data.prefetch_dataloader import CPUPrefetcher, CUDAPrefetcher
 from pyiqa.models import build_model
 from pyiqa.utils import (AvgTimer, MessageLogger, check_resume, get_env_info, get_root_logger, get_time_str,
-                           init_tb_logger, init_wandb_logger, make_exp_dirs, mkdir_and_rename, scandir)
+                           init_tb_logger, init_wandb_logger, make_exp_dirs, mkdir_and_rename, scandir, load_file_from_url)
 from pyiqa.utils.options import copy_opt_file, dict2str, parse_options
 
 
 def init_tb_loggers(opt):
     # initialize wandb logger before tensorboard logger to allow proper sync
     if (opt['logger'].get('wandb') is not None) and (opt['logger']['wandb'].get('project')
                                                      is not None) and ('debug' not in opt['name']):
@@ -24,14 +25,22 @@
     tb_logger = None
     if opt['logger'].get('use_tb_logger') and 'debug' not in opt['name']:
         tb_logger = init_tb_logger(log_dir=osp.join(opt['root_path'], 'tb_logger', opt['name']))
     return tb_logger
 
 
 def create_train_val_dataloader(opt, logger):
+    # download meta informatioin for datasets if needed
+    if not os.path.exists(f"{opt['root_path']}/datasets/meta_info"):
+        logger.info('Downloading meta information for datasets.')
+        os.makedirs(f"{opt['root_path']}/datasets", exist_ok=True)
+        file_path = load_file_from_url('https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/meta_info.tgz', f"{opt['root_path']}/datasets")
+        metainfo_file = tarfile.open(file_path, mode='r|gz')
+        metainfo_file.extractall(f"{opt['root_path']}/datasets")
+
     # create train and val dataloaders
     train_loader, val_loaders = None, []
     for phase, dataset_opt in opt['datasets'].items():
         if phase == 'train':
             dataset_enlarge_ratio = dataset_opt.get('dataset_enlarge_ratio', 1)
             train_set = build_dataset(dataset_opt)
             train_sampler = EnlargedSampler(train_set, opt['world_size'], opt['rank'], dataset_enlarge_ratio, dataset_opt.get('use_shuffle', True))
@@ -207,16 +216,15 @@
 
             if current_iter % opt['logger']['save_latest_freq'] == 0:
                 logger.info('Saving latest models and training states.')
                 model.save(epoch, -1) 
 
             # validation
             if opt.get('val') is not None and (current_iter % opt['val']['val_freq'] == 0):
-                if len(val_loaders) > 1:
-                    logger.warning('Multiple validation datasets are *only* supported by SRModel.')
+                logger.info(f'{len(val_loaders)} validation datasets are used for validation.')
                 for val_loader in val_loaders:
                     model.validation(val_loader, current_iter, tb_logger, opt['val']['save_img'])
 
             data_timer.start()
             iter_timer.start()
             train_data = prefetcher.next()
         # end of iter
```

### Comparing `pyiqa-0.1.7/pyiqa/train_nsplits.py` & `pyiqa-0.1.8/pyiqa/train_nsplits.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/utils/__init__.py` & `pyiqa-0.1.8/pyiqa/utils/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .file_client import FileClient
 from .img_util import crop_border, imfrombytes, img2tensor, imwrite, tensor2img, imread2tensor
 from .logger import AvgTimer, MessageLogger, get_env_info, get_root_logger, init_tb_logger, init_wandb_logger
 from .misc import check_resume, get_time_str, make_exp_dirs, mkdir_and_rename, scandir, set_random_seed, sizeof_fmt
+from .download_util import download_file_from_google_drive, load_file_from_url
 
 from .color_util import rgb2ycbcr, ycbcr2rgb
 
 __all__ = [
     # file_client.py
     'FileClient',
     # img_util.py
@@ -29,8 +30,11 @@
     'make_exp_dirs',
     'scandir',
     'check_resume',
     'sizeof_fmt',
     # color util
     'rgb2ycbcr',
     'ycbcr2rgb',
+    # download util
+    'download_file_from_google_drive',
+    'load_file_from_url',
 ]
```

### Comparing `pyiqa-0.1.7/pyiqa/utils/color_util.py` & `pyiqa-0.1.8/pyiqa/utils/color_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/utils/dist_util.py` & `pyiqa-0.1.8/pyiqa/utils/dist_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/utils/download_util.py` & `pyiqa-0.1.8/pyiqa/utils/download_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/utils/file_client.py` & `pyiqa-0.1.8/pyiqa/utils/file_client.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/utils/img_util.py` & `pyiqa-0.1.8/pyiqa/utils/img_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,16 @@
 from torchvision.utils import make_grid
 import io
 
 from PIL import Image
 import torchvision.transforms.functional as TF
 
 
-IMG_EXTENSIONS = [
-    '.jpg', '.JPG', '.jpeg', '.JPEG',
-    '.png', '.PNG', '.ppm', '.PPM', '.bmp', '.BMP',
-    '.tif', '.TIF', '.tiff', '.TIFF',
-]
-
-
 def is_image_file(filename):
-    return any(filename.endswith(extension) for extension in IMG_EXTENSIONS)
+    return any(filename.lower().endswith(extension) for extension in Image.registered_extensions())
 
 
 def imread2tensor(img_source, rgb=False):
     """Read image to tensor.
 
     Args:
         img_source (str, bytes, or PIL.Image): image filepath string, image contents as a bytearray or a PIL Image instance
```

### Comparing `pyiqa-0.1.7/pyiqa/utils/lmdb_util.py` & `pyiqa-0.1.8/pyiqa/utils/lmdb_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/utils/logger.py` & `pyiqa-0.1.8/pyiqa/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/utils/misc.py` & `pyiqa-0.1.8/pyiqa/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/utils/options.py` & `pyiqa-0.1.8/pyiqa/utils/options.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa/utils/registry.py` & `pyiqa-0.1.8/pyiqa/utils/registry.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.7/pyiqa.egg-info/PKG-INFO` & `pyiqa-0.1.8/pyiqa.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiqa
-Version: 0.1.7
+Version: 0.1.8
 Summary: PyTorch Toolbox for Image Quality Assessment
 Home-page: https://github.com/chaofengc/IQA-PyTorch
 Author: Chaofeng Chen
 Author-email: chaofenghust@gmail.com
 License: UNKNOWN
 Keywords: image quality assessment,pytorch
 Platform: UNKNOWN
@@ -18,25 +18,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE_NTU-S-Lab
 
-# PyTorch Toolbox for Image Quality Assessment
+# <img align="left" width="100" height="100" src="docs/pyiqa_logo.jpg"> PyTorch Toolbox for Image Quality Assessment
 
-An IQA toolbox with pure python and pytorch. Please refer to [Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-Quality-Assessment) for a comprehensive survey of IQA methods, as well as download links for IQA datasets.
+An IQA toolbox with pure python and pytorch. Please refer to [Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-Quality-Assessment) for a comprehensive survey of IQA methods and download links for IQA datasets.
 
 <a href="https://colab.research.google.com/drive/14J3KoyrjJ6R531DsdOy5Bza5xfeMODi6?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="google colab logo"></a> 
 [![PyPI](https://img.shields.io/pypi/v/pyiqa)](https://pypi.org/project/pyiqa/)
 ![visitors](https://visitor-badge.laobi.icu/badge?page_id=chaofengc/IQA-PyTorch) 
+[![Documentation Status](https://readthedocs.org/projects/iqa-pytorch/badge/?version=latest)](https://iqa-pytorch.readthedocs.io/en/latest/?badge=latest)
 [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/chaofengc/Awesome-Image-Quality-Assessment)
 [![Citation](https://img.shields.io/badge/Citation-bibtex-green)](https://github.com/chaofengc/IQA-PyTorch/blob/main/README.md#bookmark_tabs-citation)
 
-![demo](demo.gif)
+![demo](docs/demo.gif)
 
 - [:open\_book: Introduction](#open_book-introduction)
 - [:zap: Quick Start](#zap-quick-start)
   - [Dependencies and Installation](#dependencies-and-installation)
   - [Basic Usage](#basic-usage)
 - [:1st\_place\_medal: Benchmark Performances and Model Zoo](#1st_place_medal-benchmark-performances-and-model-zoo)
   - [Results Calibration](#results-calibration)
@@ -44,36 +45,42 @@
   - [Benchmark Performance with Provided Script](#benchmark-performance-with-provided-script)
 - [:hammer\_and\_wrench: Train](#hammer_and_wrench-train)
   - [Dataset Preparation](#dataset-preparation)
   - [Example Train Script](#example-trai-script)
  
 ## :open_book: Introduction
 
-This is a image quality assessment toolbox with **pure python and pytorch**. We provide reimplementation of many mainstream full reference (FR) and no reference (NR) metrics (results are calibrated with official matlab scripts if exist). **With GPU acceleration, most of our implementations are much faster than Matlab.** Please refer to the [Model Cards](docs/ModelCard.md) and [Dataset Cards](docs/Dataset_Preparation.md) for all supported methods and datasets.
+This is a image quality assessment toolbox with **pure python and pytorch**. We provide reimplementation of many mainstream full reference (FR) and no reference (NR) metrics (results are calibrated with official matlab scripts if exist). **With GPU acceleration, most of our implementations are much faster than Matlab.** Please refer to the following documents for details:  
+
+<div align="center">
+
+📦 [Model Cards](docs/ModelCard.md)  |  🗃️ [Dataset Cards](docs/Dataset_Preparation.md) 
+
+</div>
 
 ---
 
 ### :triangular_flag_on_post: Updates/Changelog
-
+- **Oct 09, 2023**. Add datasets: [PIQ2023](https://github.com/DXOMARK-Research/PIQ2023), [GFIQA](http://database.mmsp-kn.de/gfiqa-20k-database.html). Add metric `topiq_nr-face`. 
+- **Aug 15, 2023**. Add `st-lpips` and `laion_aes`. Refer to official repo at [ShiftTolerant-LPIPS](https://github.com/abhijay9/ShiftTolerant-LPIPS) and [improved-aesthetic-predictor](https://github.com/christophschuhmann/improved-aesthetic-predictor)
+- **Aug 05, 2023**. Add our work [TOPIQ](https://arxiv.org/abs/2308.03060) with remarkable performance on almost all benchmarks via efficient Resnet50 backbone. Use it with `topiq_fr, topiq_nr, topiq_iaa` for Full-Reference, No-Reference and Aesthetic assessment respectively.
 - **March 30, 2023**. Add [URanker](https://github.com/RQ-Wu/UnderwaterRanker) for IQA of under water images. 
 - **March 29, 2023**. :rotating_light: Hot fix of NRQM & PI. 
 - **March 25, 2023**. Add TreS, HyperIQA, CNNIQA, CLIPIQA.
-- **Sep 1, 2022**. 1) Add pretrained models for MANIQA and AHIQ. 2) Add dataset interface for pieapp and PIPAL.
-- **June 3, 2022**. Add FID metric. See [clean-fid](https://github.com/GaParmar/clean-fid) for more details.
-- **March 11, 2022**. Add pretrained DBCNN, NIMA, and official model of PieAPP, paq2piq.
 - [**More**](docs/history_changelog.md)
 
 ---
 
 ## :zap: Quick Start
 
 ### Dependencies and Installation
 - Ubuntu >= 18.04
 - Python >= 3.8
-- Pytorch >= 1.10
+- PyTorch >= 1.12
+- Torchvision >= 0.13
 - CUDA >= 10.2 (if use GPU)
 ```
 # Install with pip
 pip install pyiqa
 
 # Install latest github version
 pip uninstall pyiqa # if have older version installed already 
@@ -140,30 +147,35 @@
 
 Please refer to the [results calibration](./ResultsCalibra/ResultsCalibra.md) to verify the correctness of the python implementations compared with official scripts in matlab or python.
 
 ### Performance Evaluation Protocol
 
 **We use official models for evaluation if available.** Otherwise, we use the following settings to train and evaluate different models for simplicity and consistency:
 
-| Metric Type   | Train     | Test                                       | Results                                                  |
+| Metric Type   | Train     | Test                                       | Results                                                  | 
 | ------------- | --------- | ------------------------------------------ | -------------------------------------------------------- |
 | FR            | KADID-10k | CSIQ, LIVE, TID2008, TID2013               | [FR benchmark results](tests/FR_benchmark_results.csv)   |
-| NR            | KonIQ-10k | LIVEC, KonIQ-10k (official split), TID2013 | [NR benchmark results](tests/NR_benchmark_results.csv)   |
+| NR            | KonIQ-10k | LIVEC, KonIQ-10k (official split), TID2013, SPAQ | [NR benchmark results](tests/NR_benchmark_results.csv)   |
 | Aesthetic IQA | AVA       | AVA (official split)                       | [IAA benchmark results](tests/IAA_benchmark_results.csv) |
 
+Results are calculated with:
+- **PLCC without any correction**. Although test time value correction is common in IQA papers, we want to use the original value in our benchmark.
+- **Full image single input.** We use multi-patch testing only when it is necessary for the model to work.
+
 Basically, we use the largest existing datasets for training, and cross dataset evaluation performance for fair comparison. The following models do not provide official weights, and are retrained by our scripts:
 
-| Metric Type   | Model Names                   |
+| Metric Type   | Reproduced Models |
 | ------------- | ----------------------------- |
 | FR            |                               |
 | NR            | `cnniqa`, `dbcnn`, `hyperiqa` |
 | Aesthetic IQA | `nima`, `nima-vgg16-ava`      |
 
-Notes:
-- Due to optimized training process, performance of some retrained approaches may be higher than original paper.
+**Important Notes:**
+- Due to optimized training process, performance of some retrained approaches may be different with original paper.
+- Results of all **retrained models by ours** are normalized to [0, 1] and change to higher better for convenience.
 - Results of KonIQ-10k, AVA are both tested with official split.
 - NIMA is only applicable to AVA dataset now. We use `inception_resnet_v2` for default `nima`.
 - MUSIQ is not included in the IAA benchmark because we do not have train/split information of the official model.
 
 ### Benchmark Performance with Provided Script
 
 Here is an example script to get performance benchmark on different datasets:
@@ -181,26 +193,26 @@
 ```
 
 ## :hammer_and_wrench: Train
 
 ### Dataset Preparation
 
 - You only need to unzip downloaded datasets from official website without any extra operation. And then make soft links of these dataset folder under `datasets/` folder. Download links are provided in [Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-Quality-Assessment).
-- We provide common interface to load these datasets with the prepared meta information files and train/val/test split files, which can be downloaded from [download_link](https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/data_info_files.tgz) and extract them to `datasets/` folder.
+- We provide common interface to load these datasets with the prepared meta information files and train/val/test split files, which can be downloaded from [download_link](https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/meta_info.tgz) and extract them to `datasets/` folder.
 
 You may also use the following commands:
 
 ```
 mkdir datasets && cd datasets
 
 # make soft links of your dataset
 ln -sf your/dataset/path datasetname
 
 # download meta info files and train split files
-wget https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/data_info_files.tgz
+wget https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/meta_info.tgz
 tar -xvf data_info_files.tgz
 ```
 
 Examples to specific dataset options can be found in `./options/default_dataset_opt.yml`. Details of the dataloader inferface and meta information files can be found in [Dataset Preparation](docs/Dataset_Preparation.md)
 
 ### Example Train Script
 
@@ -233,14 +245,26 @@
   title={{IQA-PyTorch}: PyTorch Toolbox for Image Quality Assessment},
   author={Chaofeng Chen and Jiadi Mo},
   year={2022},
   howpublished = "[Online]. Available: \url{https://github.com/chaofengc/IQA-PyTorch}"
 }
 ```
 
+Please also consider to cite our new work `TOPIQ` if it is useful to you:
+```
+@misc{chen2023topiq,
+      title={TOPIQ: A Top-down Approach from Semantics to Distortions for Image Quality Assessment}, 
+      author={Chaofeng Chen and Jiadi Mo and Jingwen Hou and Haoning Wu and Liang Liao and Wenxiu Sun and Qiong Yan and Weisi Lin},
+      year={2023},
+      eprint={2308.03060},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+}
+``` 
+
 ## :heart: Acknowledgement
 
 The code architecture is borrowed from [BasicSR](https://github.com/xinntao/BasicSR). Several implementations are taken from: [IQA-optimization](https://github.com/dingkeyan93/IQA-optimization), [Image-Quality-Assessment-Toolbox](https://github.com/RyanXingQL/Image-Quality-Assessment-Toolbox), [piq](https://github.com/photosynthesis-team/piq), [piqa](https://github.com/francois-rozet/piqa), [clean-fid](https://github.com/GaParmar/clean-fid)
 
 We also thanks the following public repositories: [MUSIQ](https://github.com/google-research/google-research/tree/master/musiq), [DBCNN](https://github.com/zwx8981/DBCNN-PyTorch), [NIMA](https://github.com/kentsyx/Neural-IMage-Assessment), [HyperIQA](https://github.com/SSL92/hyperIQA), [CNNIQA](https://github.com/lidq92/CNNIQA), [WaDIQaM](https://github.com/lidq92/WaDIQaM), [PieAPP](https://github.com/prashnani/PerceptualImageError), [paq2piq](https://github.com/baidut/paq2piq), [MANIQA](https://github.com/IIGROUP/MANIQA) 
 
 ## :e-mail: Contact
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,77 +1,86 @@
-Metadata-Version: 2.1 Name: pyiqa Version: 0.1.7 Summary: PyTorch Toolbox for
+Metadata-Version: 2.1 Name: pyiqa Version: 0.1.8 Summary: PyTorch Toolbox for
 Image Quality Assessment Home-page: https://github.com/chaofengc/IQA-PyTorch
 Author: Chaofeng Chen Author-email: chaofenghust@gmail.com License: UNKNOWN
 Keywords: image quality assessment,pytorch Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE License-File: LICENSE_NTU-S-Lab # PyTorch Toolbox for Image Quality
-Assessment An IQA toolbox with pure python and pytorch. Please refer to
-[Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-
-Quality-Assessment) for a comprehensive survey of IQA methods, as well as
-download links for IQA datasets. _[_g_o_o_g_l_e_ _c_o_l_a_b_ _l_o_g_o_][![PyPI](https://
-img.shields.io/pypi/v/pyiqa)](https://pypi.org/project/pyiqa/) ![visitors]
+LICENSE License-File: LICENSE_NTU-S-Lab # [docs/pyiqa_logo.jpg]PyTorch Toolbox
+for Image Quality Assessment An IQA toolbox with pure python and pytorch.
+Please refer to [Awesome-Image-Quality-Assessment](https://github.com/
+chaofengc/Awesome-Image-Quality-Assessment) for a comprehensive survey of IQA
+methods and download links for IQA datasets. _[_g_o_o_g_l_e_ _c_o_l_a_b_ _l_o_g_o_][![PyPI](https:
+//img.shields.io/pypi/v/pyiqa)](https://pypi.org/project/pyiqa/) ![visitors]
 (https://visitor-badge.laobi.icu/badge?page_id=chaofengc/IQA-PyTorch) [!
-[Awesome](https://cdn.rawgit.com/sindresorhus/awesome/
+[Documentation Status](https://readthedocs.org/projects/iqa-pytorch/badge/
+?version=latest)](https://iqa-pytorch.readthedocs.io/en/latest/?badge=latest)
+[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/
 d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/
 chaofengc/Awesome-Image-Quality-Assessment) [![Citation](https://
 img.shields.io/badge/Citation-bibtex-green)](https://github.com/chaofengc/IQA-
-PyTorch/blob/main/README.md#bookmark_tabs-citation) ![demo](demo.gif) - [:
+PyTorch/blob/main/README.md#bookmark_tabs-citation) ![demo](docs/demo.gif) - [:
 open\_book: Introduction](#open_book-introduction) - [:zap: Quick Start](#zap-
 quick-start) - [Dependencies and Installation](#dependencies-and-installation)
 - [Basic Usage](#basic-usage) - [:1st\_place\_medal: Benchmark Performances and
 Model Zoo](#1st_place_medal-benchmark-performances-and-model-zoo) - [Results
 Calibration](#results-calibration) - [Performance Evaluation Protocol]
 (#performance-evaluation-protocol) - [Benchmark Performance with Provided
 Script](#benchmark-performance-with-provided-script) - [:hammer\_and\_wrench:
 Train](#hammer_and_wrench-train) - [Dataset Preparation](#dataset-preparation)
 - [Example Train Script](#example-trai-script) ## :open_book: Introduction This
 is a image quality assessment toolbox with **pure python and pytorch**. We
 provide reimplementation of many mainstream full reference (FR) and no
 reference (NR) metrics (results are calibrated with official matlab scripts if
 exist). **With GPU acceleration, most of our implementations are much faster
-than Matlab.** Please refer to the [Model Cards](docs/ModelCard.md) and
-[Dataset Cards](docs/Dataset_Preparation.md) for all supported methods and
-datasets. --- ### :triangular_flag_on_post: Updates/Changelog - **March 30,
-2023**. Add [URanker](https://github.com/RQ-Wu/UnderwaterRanker) for IQA of
-under water images. - **March 29, 2023**. :rotating_light: Hot fix of NRQM &
-PI. - **March 25, 2023**. Add TreS, HyperIQA, CNNIQA, CLIPIQA. - **Sep 1,
-2022**. 1) Add pretrained models for MANIQA and AHIQ. 2) Add dataset interface
-for pieapp and PIPAL. - **June 3, 2022**. Add FID metric. See [clean-fid]
-(https://github.com/GaParmar/clean-fid) for more details. - **March 11, 2022**.
-Add pretrained DBCNN, NIMA, and official model of PieAPP, paq2piq. - [**More**]
-(docs/history_changelog.md) --- ## :zap: Quick Start ### Dependencies and
-Installation - Ubuntu >= 18.04 - Python >= 3.8 - Pytorch >= 1.10 - CUDA >= 10.2
-(if use GPU) ``` # Install with pip pip install pyiqa # Install latest github
-version pip uninstall pyiqa # if have older version installed already pip
-install git+https://github.com/chaofengc/IQA-PyTorch.git # Install with git
-clone git clone https://github.com/chaofengc/IQA-PyTorch.git cd IQA-PyTorch pip
-install -r requirements.txt python setup.py develop ``` ### Basic Usage ```
-import pyiqa import torch # list all available metrics print(pyiqa.list_models
-()) device = torch.device("cuda") if torch.cuda.is_available() else
-torch.device("cpu") # create metric with default setting iqa_metric =
-pyiqa.create_metric('lpips', device=device) # Note that gradient propagation is
-disabled by default. set as_loss=True to enable it as a loss function. iqa_loss
-= pyiqa.create_metric('lpips', device=device, as_loss=True) # create metric
-with custom setting iqa_metric = pyiqa.create_metric('psnr',
-test_y_channel=True, color_space='ycbcr').to(device) # check if lower better or
-higher better print(iqa_metric.lower_better) # example for iqa score inference
-# Tensor inputs, img_tensor_x/y: (N, 3, H, W), RGB, 0 ~ 1 score_fr = iqa_metric
-(img_tensor_x, img_tensor_y) score_nr = iqa_metric(img_tensor_x) # img path as
-inputs. score_fr = iqa_metric('./ResultsCalibra/dist_dir/I03.bmp', './
-ResultsCalibra/ref_dir/I03.bmp') # For FID metric, use directory or precomputed
-statistics as inputs # refer to clean-fid for more details: https://github.com/
-GaParmar/clean-fid fid_metric = pyiqa.create_metric('fid') score = fid_metric
-('./ResultsCalibra/dist_dir/', './ResultsCalibra/ref_dir') score = fid_metric
-('./ResultsCalibra/dist_dir/', dataset_name="FFHQ", dataset_res=1024,
+than Matlab.** Please refer to the following documents for details:
+     ð¦ [Model Cards](docs/ModelCard.md) | ðï¸ [Dataset Cards](docs/
+                            Dataset_Preparation.md)
+--- ### :triangular_flag_on_post: Updates/Changelog - **Oct 09, 2023**. Add
+datasets: [PIQ2023](https://github.com/DXOMARK-Research/PIQ2023), [GFIQA](http:
+//database.mmsp-kn.de/gfiqa-20k-database.html). Add metric `topiq_nr-face`. -
+**Aug 15, 2023**. Add `st-lpips` and `laion_aes`. Refer to official repo at
+[ShiftTolerant-LPIPS](https://github.com/abhijay9/ShiftTolerant-LPIPS) and
+[improved-aesthetic-predictor](https://github.com/christophschuhmann/improved-
+aesthetic-predictor) - **Aug 05, 2023**. Add our work [TOPIQ](https://
+arxiv.org/abs/2308.03060) with remarkable performance on almost all benchmarks
+via efficient Resnet50 backbone. Use it with `topiq_fr, topiq_nr, topiq_iaa`
+for Full-Reference, No-Reference and Aesthetic assessment respectively. -
+**March 30, 2023**. Add [URanker](https://github.com/RQ-Wu/UnderwaterRanker)
+for IQA of under water images. - **March 29, 2023**. :rotating_light: Hot fix
+of NRQM & PI. - **March 25, 2023**. Add TreS, HyperIQA, CNNIQA, CLIPIQA. -
+[**More**](docs/history_changelog.md) --- ## :zap: Quick Start ### Dependencies
+and Installation - Ubuntu >= 18.04 - Python >= 3.8 - PyTorch >= 1.12 -
+Torchvision >= 0.13 - CUDA >= 10.2 (if use GPU) ``` # Install with pip pip
+install pyiqa # Install latest github version pip uninstall pyiqa # if have
+older version installed already pip install git+https://github.com/chaofengc/
+IQA-PyTorch.git # Install with git clone git clone https://github.com/
+chaofengc/IQA-PyTorch.git cd IQA-PyTorch pip install -r requirements.txt python
+setup.py develop ``` ### Basic Usage ``` import pyiqa import torch # list all
+available metrics print(pyiqa.list_models()) device = torch.device("cuda") if
+torch.cuda.is_available() else torch.device("cpu") # create metric with default
+setting iqa_metric = pyiqa.create_metric('lpips', device=device) # Note that
+gradient propagation is disabled by default. set as_loss=True to enable it as a
+loss function. iqa_loss = pyiqa.create_metric('lpips', device=device,
+as_loss=True) # create metric with custom setting iqa_metric =
+pyiqa.create_metric('psnr', test_y_channel=True, color_space='ycbcr').to
+(device) # check if lower better or higher better print
+(iqa_metric.lower_better) # example for iqa score inference # Tensor inputs,
+img_tensor_x/y: (N, 3, H, W), RGB, 0 ~ 1 score_fr = iqa_metric(img_tensor_x,
+img_tensor_y) score_nr = iqa_metric(img_tensor_x) # img path as inputs.
+score_fr = iqa_metric('./ResultsCalibra/dist_dir/I03.bmp', './ResultsCalibra/
+ref_dir/I03.bmp') # For FID metric, use directory or precomputed statistics as
+inputs # refer to clean-fid for more details: https://github.com/GaParmar/
+clean-fid fid_metric = pyiqa.create_metric('fid') score = fid_metric('./
+ResultsCalibra/dist_dir/', './ResultsCalibra/ref_dir') score = fid_metric('./
+ResultsCalibra/dist_dir/', dataset_name="FFHQ", dataset_res=1024,
 dataset_split="trainval70k") ``` #### Example Test script Example test script
 with input directory/images and reference directory/images. ``` # example for
 FR metric with dirs python inference_iqa.py -m LPIPS[or lpips] -i ./
 ResultsCalibra/dist_dir[dist_img] -r ./ResultsCalibra/ref_dir[ref_img] #
 example for NR metric with single image python inference_iqa.py -m brisque -
 i ./ResultsCalibra/dist_dir/I03.bmp ``` ## :1st_place_medal: Benchmark
 Performances and Model Zoo ### Results Calibration Please refer to the [results
@@ -80,74 +89,83 @@
 ### Performance Evaluation Protocol **We use official models for evaluation if
 available.** Otherwise, we use the following settings to train and evaluate
 different models for simplicity and consistency: | Metric Type | Train | Test |
 Results | | ------------- | --------- | ---------------------------------------
 --- | -------------------------------------------------------- | | FR | KADID-
 10k | CSIQ, LIVE, TID2008, TID2013 | [FR benchmark results](tests/
 FR_benchmark_results.csv) | | NR | KonIQ-10k | LIVEC, KonIQ-10k (official
-split), TID2013 | [NR benchmark results](tests/NR_benchmark_results.csv) | |
-Aesthetic IQA | AVA | AVA (official split) | [IAA benchmark results](tests/
-IAA_benchmark_results.csv) | Basically, we use the largest existing datasets
-for training, and cross dataset evaluation performance for fair comparison. The
-following models do not provide official weights, and are retrained by our
-scripts: | Metric Type | Model Names | | ------------- | ----------------------
-------- | | FR | | | NR | `cnniqa`, `dbcnn`, `hyperiqa` | | Aesthetic IQA |
-`nima`, `nima-vgg16-ava` | Notes: - Due to optimized training process,
-performance of some retrained approaches may be higher than original paper. -
-Results of KonIQ-10k, AVA are both tested with official split. - NIMA is only
-applicable to AVA dataset now. We use `inception_resnet_v2` for default `nima`.
-- MUSIQ is not included in the IAA benchmark because we do not have train/split
-information of the official model. ### Benchmark Performance with Provided
-Script Here is an example script to get performance benchmark on different
-datasets: ``` # NOTE: this script will test ALL specified metrics on ALL
-specified datasets # Test default metrics on default datasets python
-benchmark_results.py -m psnr ssim -d csiq tid2013 tid2008 # Test with your own
-options python benchmark_results.py -m psnr --data_opt options/
-example_benchmark_data_opts.yml python benchmark_results.py --metric_opt
-options/example_benchmark_metric_opts.yml tid2013 tid2008 python
+split), TID2013, SPAQ | [NR benchmark results](tests/NR_benchmark_results.csv)
+| | Aesthetic IQA | AVA | AVA (official split) | [IAA benchmark results](tests/
+IAA_benchmark_results.csv) | Results are calculated with: - **PLCC without any
+correction**. Although test time value correction is common in IQA papers, we
+want to use the original value in our benchmark. - **Full image single input.**
+We use multi-patch testing only when it is necessary for the model to work.
+Basically, we use the largest existing datasets for training, and cross dataset
+evaluation performance for fair comparison. The following models do not provide
+official weights, and are retrained by our scripts: | Metric Type | Reproduced
+Models | | ------------- | ----------------------------- | | FR | | | NR |
+`cnniqa`, `dbcnn`, `hyperiqa` | | Aesthetic IQA | `nima`, `nima-vgg16-ava` |
+**Important Notes:** - Due to optimized training process, performance of some
+retrained approaches may be different with original paper. - Results of all
+**retrained models by ours** are normalized to [0, 1] and change to higher
+better for convenience. - Results of KonIQ-10k, AVA are both tested with
+official split. - NIMA is only applicable to AVA dataset now. We use
+`inception_resnet_v2` for default `nima`. - MUSIQ is not included in the IAA
+benchmark because we do not have train/split information of the official model.
+### Benchmark Performance with Provided Script Here is an example script to get
+performance benchmark on different datasets: ``` # NOTE: this script will test
+ALL specified metrics on ALL specified datasets # Test default metrics on
+default datasets python benchmark_results.py -m psnr ssim -d csiq tid2013
+tid2008 # Test with your own options python benchmark_results.py -m psnr --
+data_opt options/example_benchmark_data_opts.yml python benchmark_results.py --
+metric_opt options/example_benchmark_metric_opts.yml tid2013 tid2008 python
 benchmark_results.py --metric_opt options/example_benchmark_metric_opts.yml --
 data_opt options/example_benchmark_data_opts.yml ``` ## :hammer_and_wrench:
 Train ### Dataset Preparation - You only need to unzip downloaded datasets from
 official website without any extra operation. And then make soft links of these
 dataset folder under `datasets/` folder. Download links are provided in
 [Awesome-Image-Quality-Assessment](https://github.com/chaofengc/Awesome-Image-
 Quality-Assessment). - We provide common interface to load these datasets with
 the prepared meta information files and train/val/test split files, which can
 be downloaded from [download_link](https://github.com/chaofengc/IQA-PyTorch/
-releases/download/v0.1-weights/data_info_files.tgz) and extract them to
-`datasets/` folder. You may also use the following commands: ``` mkdir datasets
-&& cd datasets # make soft links of your dataset ln -sf your/dataset/path
-datasetname # download meta info files and train split files wget https://
-github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/
-data_info_files.tgz tar -xvf data_info_files.tgz ``` Examples to specific
-dataset options can be found in `./options/default_dataset_opt.yml`. Details of
-the dataloader inferface and meta information files can be found in [Dataset
-Preparation](docs/Dataset_Preparation.md) ### Example Train Script Example to
-train DBCNN on LIVEChallenge dataset ``` # train for single experiment python
-pyiqa/train.py -opt options/train/DBCNN/train_DBCNN.yml # train N splits for
-small datasets python pyiqa/train_nsplits.py -opt options/train/DBCNN/
-train_DBCNN.yml ``` ## :beers: Contribution Any contributions to this
-repository are greatly appreciated. Please follow the [contribution
-instructions](docs/Instruction.md) for contribution guidance. ## :scroll:
-License This work is licensed under a [NTU S-Lab License](https://github.com/
-chaofengc/IQA-PyTorch/blob/main/LICENSE_NTU-S-Lab) and _C_r_e_a_t_i_v_e_ _C_o_m_m_o_n_s
-_A_t_t_r_i_b_u_t_i_o_n_-_N_o_n_C_o_m_m_e_r_c_i_a_l_-_S_h_a_r_e_A_l_i_k_e_ _4_._0_ _I_n_t_e_r_n_a_t_i_o_n_a_l_ _L_i_c_e_n_s_e. _[_C_r_e_a_t_i_v_e
-_C_o_m_m_o_n_s_ _L_i_c_e_n_s_e_]## :bookmark_tabs: Citation If you find our codes helpful to
-your research, please consider to use the following citation: ``` @misc{pyiqa,
-title={{IQA-PyTorch}: PyTorch Toolbox for Image Quality Assessment}, author=
-{Chaofeng Chen and Jiadi Mo}, year={2022}, howpublished = "[Online]. Available:
-\url{https://github.com/chaofengc/IQA-PyTorch}" } ``` ## :heart:
-Acknowledgement The code architecture is borrowed from [BasicSR](https://
-github.com/xinntao/BasicSR). Several implementations are taken from: [IQA-
-optimization](https://github.com/dingkeyan93/IQA-optimization), [Image-Quality-
-Assessment-Toolbox](https://github.com/RyanXingQL/Image-Quality-Assessment-
-Toolbox), [piq](https://github.com/photosynthesis-team/piq), [piqa](https://
-github.com/francois-rozet/piqa), [clean-fid](https://github.com/GaParmar/clean-
-fid) We also thanks the following public repositories: [MUSIQ](https://
-github.com/google-research/google-research/tree/master/musiq), [DBCNN](https://
-github.com/zwx8981/DBCNN-PyTorch), [NIMA](https://github.com/kentsyx/Neural-
-IMage-Assessment), [HyperIQA](https://github.com/SSL92/hyperIQA), [CNNIQA]
-(https://github.com/lidq92/CNNIQA), [WaDIQaM](https://github.com/lidq92/
-WaDIQaM), [PieAPP](https://github.com/prashnani/PerceptualImageError),
-[paq2piq](https://github.com/baidut/paq2piq), [MANIQA](https://github.com/
-IIGROUP/MANIQA) ## :e-mail: Contact If you have any questions, please email
-`chaofenghust@gmail.com`
+releases/download/v0.1-weights/meta_info.tgz) and extract them to `datasets/
+` folder. You may also use the following commands: ``` mkdir datasets && cd
+datasets # make soft links of your dataset ln -sf your/dataset/path datasetname
+# download meta info files and train split files wget https://github.com/
+chaofengc/IQA-PyTorch/releases/download/v0.1-weights/meta_info.tgz tar -xvf
+data_info_files.tgz ``` Examples to specific dataset options can be found in
+`./options/default_dataset_opt.yml`. Details of the dataloader inferface and
+meta information files can be found in [Dataset Preparation](docs/
+Dataset_Preparation.md) ### Example Train Script Example to train DBCNN on
+LIVEChallenge dataset ``` # train for single experiment python pyiqa/train.py -
+opt options/train/DBCNN/train_DBCNN.yml # train N splits for small datasets
+python pyiqa/train_nsplits.py -opt options/train/DBCNN/train_DBCNN.yml ``` ## :
+beers: Contribution Any contributions to this repository are greatly
+appreciated. Please follow the [contribution instructions](docs/Instruction.md)
+for contribution guidance. ## :scroll: License This work is licensed under a
+[NTU S-Lab License](https://github.com/chaofengc/IQA-PyTorch/blob/main/
+LICENSE_NTU-S-Lab) and _C_r_e_a_t_i_v_e_ _C_o_m_m_o_n_s_ _A_t_t_r_i_b_u_t_i_o_n_-_N_o_n_C_o_m_m_e_r_c_i_a_l_-_S_h_a_r_e_A_l_i_k_e
+_4_._0_ _I_n_t_e_r_n_a_t_i_o_n_a_l_ _L_i_c_e_n_s_e. _[_C_r_e_a_t_i_v_e_ _C_o_m_m_o_n_s_ _L_i_c_e_n_s_e_]## :bookmark_tabs:
+Citation If you find our codes helpful to your research, please consider to use
+the following citation: ``` @misc{pyiqa, title={{IQA-PyTorch}: PyTorch Toolbox
+for Image Quality Assessment}, author={Chaofeng Chen and Jiadi Mo}, year=
+{2022}, howpublished = "[Online]. Available: \url{https://github.com/chaofengc/
+IQA-PyTorch}" } ``` Please also consider to cite our new work `TOPIQ` if it is
+useful to you: ``` @misc{chen2023topiq, title={TOPIQ: A Top-down Approach from
+Semantics to Distortions for Image Quality Assessment}, author={Chaofeng Chen
+and Jiadi Mo and Jingwen Hou and Haoning Wu and Liang Liao and Wenxiu Sun and
+Qiong Yan and Weisi Lin}, year={2023}, eprint={2308.03060}, archivePrefix=
+{arXiv}, primaryClass={cs.CV} } ``` ## :heart: Acknowledgement The code
+architecture is borrowed from [BasicSR](https://github.com/xinntao/BasicSR).
+Several implementations are taken from: [IQA-optimization](https://github.com/
+dingkeyan93/IQA-optimization), [Image-Quality-Assessment-Toolbox](https://
+github.com/RyanXingQL/Image-Quality-Assessment-Toolbox), [piq](https://
+github.com/photosynthesis-team/piq), [piqa](https://github.com/francois-rozet/
+piqa), [clean-fid](https://github.com/GaParmar/clean-fid) We also thanks the
+following public repositories: [MUSIQ](https://github.com/google-research/
+google-research/tree/master/musiq), [DBCNN](https://github.com/zwx8981/DBCNN-
+PyTorch), [NIMA](https://github.com/kentsyx/Neural-IMage-Assessment),
+[HyperIQA](https://github.com/SSL92/hyperIQA), [CNNIQA](https://github.com/
+lidq92/CNNIQA), [WaDIQaM](https://github.com/lidq92/WaDIQaM), [PieAPP](https://
+github.com/prashnani/PerceptualImageError), [paq2piq](https://github.com/
+baidut/paq2piq), [MANIQA](https://github.com/IIGROUP/MANIQA) ## :e-mail:
+Contact If you have any questions, please email `chaofenghust@gmail.com`
```

### Comparing `pyiqa-0.1.7/pyiqa.egg-info/SOURCES.txt` & `pyiqa-0.1.8/pyiqa.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -34,69 +34,73 @@
 pyiqa/archs/fid_arch.py
 pyiqa/archs/fsim_arch.py
 pyiqa/archs/func_util.py
 pyiqa/archs/gmsd_arch.py
 pyiqa/archs/hypernet_arch.py
 pyiqa/archs/inception.py
 pyiqa/archs/iqt_arch.py
+pyiqa/archs/laion_aes_arch.py
 pyiqa/archs/lpips_arch.py
 pyiqa/archs/mad_arch.py
 pyiqa/archs/maniqa_arch.py
 pyiqa/archs/maniqa_swin.py
 pyiqa/archs/musiq_arch.py
 pyiqa/archs/nima_arch.py
 pyiqa/archs/niqe_arch.py
 pyiqa/archs/nlpd_arch.py
 pyiqa/archs/nrqm_arch.py
 pyiqa/archs/paq2piq_arch.py
 pyiqa/archs/pieapp_arch.py
 pyiqa/archs/psnr_arch.py
 pyiqa/archs/ssim_arch.py
+pyiqa/archs/stlpips_arch.py
+pyiqa/archs/topiq_arch.py
+pyiqa/archs/topiq_swin.py
 pyiqa/archs/tres_arch.py
 pyiqa/archs/uranker_arch.py
 pyiqa/archs/vif_arch.py
 pyiqa/archs/vsi_arch.py
 pyiqa/archs/wadiqam_arch.py
 pyiqa/data/__init__.py
 pyiqa/data/ava_dataset.py
 pyiqa/data/bapps_dataset.py
+pyiqa/data/base_iqa_dataset.py
 pyiqa/data/data_sampler.py
 pyiqa/data/data_util.py
-pyiqa/data/flive_dataset.py
 pyiqa/data/general_fr_dataset.py
 pyiqa/data/general_nr_dataset.py
 pyiqa/data/livechallenge_dataset.py
 pyiqa/data/multiscale_trans_util.py
 pyiqa/data/pieapp_dataset.py
-pyiqa/data/pipal_dataset.py
+pyiqa/data/piq_dataset.py
 pyiqa/data/prefetch_dataloader.py
 pyiqa/data/transforms.py
 pyiqa/losses/__init__.py
 pyiqa/losses/iqa_losses.py
 pyiqa/losses/loss_util.py
 pyiqa/losses/losses.py
 pyiqa/matlab_utils/__init__.py
 pyiqa/matlab_utils/functions.py
 pyiqa/matlab_utils/math_util.py
+pyiqa/matlab_utils/padding.py
 pyiqa/matlab_utils/resize.py
 pyiqa/matlab_utils/scfpyr_util.py
 pyiqa/metrics/__init__.py
 pyiqa/metrics/correlation_coefficient.py
 pyiqa/metrics/other_metrics.py
 pyiqa/models/__init__.py
 pyiqa/models/bapps_model.py
 pyiqa/models/base_model.py
 pyiqa/models/dbcnn_model.py
+pyiqa/models/distiqa_model.py
 pyiqa/models/general_iqa_model.py
 pyiqa/models/hypernet_model.py
 pyiqa/models/inference_model.py
 pyiqa/models/lr_scheduler.py
-pyiqa/models/nima_model.py
 pyiqa/models/pieapp_model.py
-pyiqa/models/sr_model.py
 pyiqa/models/wadiqam_model.py
 pyiqa/utils/__init__.py
 pyiqa/utils/color_util.py
 pyiqa/utils/dist_util.py
 pyiqa/utils/download_util.py
 pyiqa/utils/file_client.py
 pyiqa/utils/img_util.py
```

### Comparing `pyiqa-0.1.7/setup.py` & `pyiqa-0.1.8/setup.py`

 * *Files identical despite different names*

