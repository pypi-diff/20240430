# Comparing `tmp/nkululeko-0.83.1.tar.gz` & `tmp/nkululeko-0.83.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.83.1.tar", last modified: Fri Apr 26 07:11:47 2024, max compression
+gzip compressed data, was "nkululeko-0.83.2.tar", last modified: Mon Apr 29 13:55:35 2024, max compression
```

## Comparing `nkululeko-0.83.1.tar` & `nkululeko-0.83.2.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.591673 nkululeko-0.83.1/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17352 2024-04-25 14:01:58.000000 nkululeko-0.83.1/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.83.1/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36080 2024-04-26 07:11:47.591673 nkululeko-0.83.1/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17457 2024-04-24 09:02:29.000000 nkululeko-0.83.1/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/aesdd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.83.1/data/aesdd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/androids/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.83.1/data/androids/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/androids_orig/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.83.1/data/androids_orig/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/androids_test/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.83.1/data/androids_test/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/ased/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.83.1/data/ased/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/asvp-esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.83.1/data/asvp-esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/baved/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.83.1/data/baved/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/cafe/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.83.1/data/cafe/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/clac/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.83.1/data/clac/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/cmu-mosei/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.83.1/data/cmu-mosei/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.83.1/data/demos/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/ekorpus/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.83.1/data/ekorpus/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/emns/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.83.1/data/emns/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/emofilm/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.83.1/data/emofilm/convert_to_16k.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.83.1/data/emofilm/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/emorynlp/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.83.1/data/emorynlp/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/emov-db/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.83.1/data/emov-db/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/emovo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.83.1/data/emovo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/emozionalmente/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.83.1/data/emozionalmente/create.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/enterface/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.83.1/data/enterface/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.83.1/data/esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/gerparas/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.83.1/data/gerparas/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/iemocap/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.83.1/data/iemocap/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/jl/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.83.1/data/jl/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/jtes/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.83.1/data/jtes/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/meld/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.83.1/data/meld/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/mesd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.83.1/data/mesd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/mess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.83.1/data/mess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/mlendsnd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.83.1/data/mlendsnd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/msp-improv/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.83.1/data/msp-improv/process_database2.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/msp-podcast/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.83.1/data/msp-podcast/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/oreau2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.83.1/data/oreau2/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/data/portuguese/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.83.1/data/portuguese/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/data/ravdess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.83.1/data/ravdess/process_database.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.83.1/data/ravdess/process_database_speaker.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/data/savee/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.83.1/data/savee/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/data/shemo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.83.1/data/shemo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/data/subesco/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.83.1/data/subesco/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/data/tess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.83.1/data/tess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/data/thorsten-emotional/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.83.1/data/thorsten-emotional/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/data/urdu/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.83.1/data/urdu/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/data/vivae/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.83.1/data/vivae/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/docs/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/docs/source/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.83.1/docs/source/conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/meta/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/meta/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.83.1/meta/demos/demo_best_model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.83.1/meta/demos/my_experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.83.1/meta/demos/my_experiment_local.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.83.1/meta/demos/plot_faster_anim.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.83.1/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.83.1/nkululeko/aug_train.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.83.1/nkululeko/augment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/nkululeko/augmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.83.1/nkululeko/augmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.83.1/nkululeko/augmenting/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.83.1/nkululeko/augmenting/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.83.1/nkululeko/augmenting/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.83.1/nkululeko/augmenting/resampler.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/nkululeko/autopredict/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.83.1/nkululeko/autopredict/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.83.1/nkululeko/autopredict/ap_age.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.83.1/nkululeko/autopredict/ap_arousal.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.83.1/nkululeko/autopredict/ap_dominance.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.83.1/nkululeko/autopredict/ap_gender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.83.1/nkululeko/autopredict/ap_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.83.1/nkululeko/autopredict/ap_pesq.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.83.1/nkululeko/autopredict/ap_sdr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.83.1/nkululeko/autopredict/ap_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.83.1/nkululeko/autopredict/ap_stoi.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.83.1/nkululeko/autopredict/ap_valence.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.83.1/nkululeko/autopredict/estimate_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.83.1/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-04-25 14:02:12.000000 nkululeko-0.83.1/nkululeko/constants.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.583673 nkululeko-0.83.1/nkululeko/data/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.83.1/nkululeko/data/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.83.1/nkululeko/data/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3884 2024-04-24 12:41:45.000000 nkululeko-0.83.1/nkululeko/data/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3264 2024-04-22 09:09:10.000000 nkululeko-0.83.1/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.83.1/nkululeko/demo_feats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4755 2024-04-22 09:09:10.000000 nkululeko-0.83.1/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    29605 2024-04-25 13:53:08.000000 nkululeko-0.83.1/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2310 2024-04-22 09:09:10.000000 nkululeko-0.83.1/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.83.1/nkululeko/export.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.587673 nkululeko-0.83.1/nkululeko/feat_extract/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.83.1/nkululeko/feat_extract/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3346 2024-04-16 13:29:59.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_agender_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11399 2024-01-24 16:15:03.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_auddim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_hubert.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3978 2024-04-24 10:46:37.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_spectra.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_spkrec.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4528 2024-04-23 10:02:24.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_squim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3319 2024-04-23 09:16:18.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5285 2024-04-23 09:16:18.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_wavlm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4533 2024-04-23 11:35:51.000000 nkululeko-0.83.1/nkululeko/feat_extract/feats_whisper.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1448 2024-04-23 09:16:18.000000 nkululeko-0.83.1/nkululeko/feat_extract/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.83.1/nkululeko/feat_extract/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.83.1/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.83.1/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.83.1/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      453 2024-02-28 17:38:08.000000 nkululeko-0.83.1/nkululeko/glob_conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.587673 nkululeko-0.83.1/nkululeko/losses/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.83.1/nkululeko/losses/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.83.1/nkululeko/losses/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.83.1/nkululeko/losses/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9288 2024-04-25 13:02:38.000000 nkululeko-0.83.1/nkululeko/modelrunner.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.587673 nkululeko-0.83.1/nkululeko/models/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.83.1/nkululeko/models/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11569 2024-04-17 13:01:47.000000 nkululeko-0.83.1/nkululeko/models/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      378 2023-12-23 10:35:03.000000 nkululeko-0.83.1/nkululeko/models/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9726 2024-04-16 11:54:29.000000 nkululeko-0.83.1/nkululeko/models/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      645 2023-09-26 13:42:48.000000 nkululeko-0.83.1/nkululeko/models/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      573 2023-09-07 11:38:13.000000 nkululeko-0.83.1/nkululeko/models/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      580 2023-09-07 11:38:09.000000 nkululeko-0.83.1/nkululeko/models/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      392 2023-12-19 13:57:23.000000 nkululeko-0.83.1/nkululeko/models/model_lin_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9107 2024-04-16 11:54:31.000000 nkululeko-0.83.1/nkululeko/models/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10083 2024-04-16 13:48:13.000000 nkululeko-0.83.1/nkululeko/models/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      914 2024-04-17 12:17:54.000000 nkululeko-0.83.1/nkululeko/models/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      699 2024-03-21 10:56:18.000000 nkululeko-0.83.1/nkululeko/models/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      390 2023-09-07 11:38:37.000000 nkululeko-0.83.1/nkululeko/models/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      397 2023-09-07 11:38:33.000000 nkululeko-0.83.1/nkululeko/models/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 10:21:07.000000 nkululeko-0.83.1/nkululeko/models/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      227 2023-12-14 15:14:23.000000 nkululeko-0.83.1/nkululeko/models/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.83.1/nkululeko/multidb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.83.1/nkululeko/nkuluflag.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.83.1/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23025 2024-02-01 14:55:26.000000 nkululeko-0.83.1/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.83.1/nkululeko/predict.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.587673 nkululeko-0.83.1/nkululeko/reporting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.83.1/nkululeko/reporting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.83.1/nkululeko/reporting/defines.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.83.1/nkululeko/reporting/latex_writer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.83.1/nkululeko/reporting/report.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.83.1/nkululeko/reporting/report_item.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12841 2024-04-25 13:02:38.000000 nkululeko-0.83.1/nkululeko/reporting/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.83.1/nkululeko/reporting/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2287 2024-04-22 09:09:10.000000 nkululeko-0.83.1/nkululeko/resample.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.83.1/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.83.1/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.83.1/nkululeko/segment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.587673 nkululeko-0.83.1/nkululeko/segmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.83.1/nkululeko/segmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.83.1/nkululeko/segmenting/seg_inaspeechsegmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.83.1/nkululeko/segmenting/seg_silero.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.83.1/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.83.1/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.83.1/nkululeko/test_predictor.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.587673 nkululeko-0.83.1/nkululeko/utils/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.83.1/nkululeko/utils/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.83.1/nkululeko/utils/files.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.83.1/nkululeko/utils/stats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12330 2024-03-21 11:06:05.000000 nkululeko-0.83.1/nkululeko/utils/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.587673 nkululeko-0.83.1/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36080 2024-04-26 07:11:47.000000 nkululeko-0.83.1/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5073 2024-04-26 07:11:47.000000 nkululeko-0.83.1/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-04-26 07:11:47.000000 nkululeko-0.83.1/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-04-26 07:11:47.000000 nkululeko-0.83.1/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-04-26 07:11:47.000000 nkululeko-0.83.1/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.83.1/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-04-26 07:11:47.591673 nkululeko-0.83.1/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.83.1/setup.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.579673 nkululeko-0.83.1/venv/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-26 07:11:47.587673 nkululeko-0.83.1/venv/bin/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.83.1/venv/bin/activate_this.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.142839 nkululeko-0.83.2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17430 2024-04-29 13:37:24.000000 nkululeko-0.83.2/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.83.2/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36158 2024-04-29 13:55:35.142839 nkululeko-0.83.2/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17457 2024-04-24 09:02:29.000000 nkululeko-0.83.2/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.130839 nkululeko-0.83.2/data/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/aesdd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.83.2/data/aesdd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/androids/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.83.2/data/androids/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/androids_orig/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.83.2/data/androids_orig/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/androids_test/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.83.2/data/androids_test/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/ased/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.83.2/data/ased/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/asvp-esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.83.2/data/asvp-esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/baved/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.83.2/data/baved/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/cafe/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.83.2/data/cafe/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/clac/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.83.2/data/clac/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/cmu-mosei/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.83.2/data/cmu-mosei/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.83.2/data/demos/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/ekorpus/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.83.2/data/ekorpus/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/emns/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.83.2/data/emns/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/emofilm/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.83.2/data/emofilm/convert_to_16k.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.83.2/data/emofilm/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/emorynlp/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.83.2/data/emorynlp/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/emov-db/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.83.2/data/emov-db/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/emovo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.83.2/data/emovo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/emozionalmente/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.83.2/data/emozionalmente/create.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/enterface/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.83.2/data/enterface/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.83.2/data/esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/gerparas/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.83.2/data/gerparas/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/iemocap/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.83.2/data/iemocap/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/jl/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.83.2/data/jl/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/jtes/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.83.2/data/jtes/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/meld/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.83.2/data/meld/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/mesd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.83.2/data/mesd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/mess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.83.2/data/mess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/mlendsnd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.83.2/data/mlendsnd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/msp-improv/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.83.2/data/msp-improv/process_database2.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/msp-podcast/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.83.2/data/msp-podcast/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/oreau2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.83.2/data/oreau2/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/portuguese/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.83.2/data/portuguese/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/ravdess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.83.2/data/ravdess/process_database.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.83.2/data/ravdess/process_database_speaker.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/savee/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.83.2/data/savee/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/shemo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.83.2/data/shemo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/subesco/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.83.2/data/subesco/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/tess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.83.2/data/tess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/thorsten-emotional/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.83.2/data/thorsten-emotional/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/urdu/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.83.2/data/urdu/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/data/vivae/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.83.2/data/vivae/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.130839 nkululeko-0.83.2/docs/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/docs/source/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.83.2/docs/source/conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.130839 nkululeko-0.83.2/meta/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/meta/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.83.2/meta/demos/demo_best_model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.83.2/meta/demos/my_experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.83.2/meta/demos/my_experiment_local.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.83.2/meta/demos/plot_faster_anim.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.138839 nkululeko-0.83.2/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.83.2/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.83.2/nkululeko/aug_train.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.83.2/nkululeko/augment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.138839 nkululeko-0.83.2/nkululeko/augmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.83.2/nkululeko/augmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.83.2/nkululeko/augmenting/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.83.2/nkululeko/augmenting/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.83.2/nkululeko/augmenting/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.83.2/nkululeko/augmenting/resampler.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.138839 nkululeko-0.83.2/nkululeko/autopredict/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.83.2/nkululeko/autopredict/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.83.2/nkululeko/autopredict/ap_age.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.83.2/nkululeko/autopredict/ap_arousal.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.83.2/nkululeko/autopredict/ap_dominance.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.83.2/nkululeko/autopredict/ap_gender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.83.2/nkululeko/autopredict/ap_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.83.2/nkululeko/autopredict/ap_pesq.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.83.2/nkululeko/autopredict/ap_sdr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.83.2/nkululeko/autopredict/ap_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.83.2/nkululeko/autopredict/ap_stoi.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.83.2/nkululeko/autopredict/ap_valence.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.83.2/nkululeko/autopredict/estimate_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.83.2/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-04-29 13:37:24.000000 nkululeko-0.83.2/nkululeko/constants.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.138839 nkululeko-0.83.2/nkululeko/data/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.83.2/nkululeko/data/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.83.2/nkululeko/data/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3884 2024-04-24 12:41:45.000000 nkululeko-0.83.2/nkululeko/data/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3264 2024-04-22 09:09:10.000000 nkululeko-0.83.2/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.83.2/nkululeko/demo_feats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4755 2024-04-22 09:09:10.000000 nkululeko-0.83.2/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    29728 2024-04-29 13:37:24.000000 nkululeko-0.83.2/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2310 2024-04-22 09:09:10.000000 nkululeko-0.83.2/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.83.2/nkululeko/export.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.142839 nkululeko-0.83.2/nkululeko/feat_extract/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.83.2/nkululeko/feat_extract/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3424 2024-04-29 13:37:24.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11399 2024-01-24 16:15:03.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_auddim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_hubert.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3978 2024-04-24 10:46:37.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_spectra.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_spkrec.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4617 2024-04-29 13:37:24.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_squim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3319 2024-04-23 09:16:18.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5268 2024-04-29 13:37:24.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_wavlm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4576 2024-04-29 13:37:24.000000 nkululeko-0.83.2/nkululeko/feat_extract/feats_whisper.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1448 2024-04-23 09:16:18.000000 nkululeko-0.83.2/nkululeko/feat_extract/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.83.2/nkululeko/feat_extract/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.83.2/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.83.2/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.83.2/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      453 2024-02-28 17:38:08.000000 nkululeko-0.83.2/nkululeko/glob_conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.142839 nkululeko-0.83.2/nkululeko/losses/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.83.2/nkululeko/losses/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.83.2/nkululeko/losses/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.83.2/nkululeko/losses/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9288 2024-04-25 13:02:38.000000 nkululeko-0.83.2/nkululeko/modelrunner.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.142839 nkululeko-0.83.2/nkululeko/models/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.83.2/nkululeko/models/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11569 2024-04-17 13:01:47.000000 nkululeko-0.83.2/nkululeko/models/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      378 2023-12-23 10:35:03.000000 nkululeko-0.83.2/nkululeko/models/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10002 2024-04-29 13:37:24.000000 nkululeko-0.83.2/nkululeko/models/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      645 2023-09-26 13:42:48.000000 nkululeko-0.83.2/nkululeko/models/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      573 2023-09-07 11:38:13.000000 nkululeko-0.83.2/nkululeko/models/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      580 2023-09-07 11:38:09.000000 nkululeko-0.83.2/nkululeko/models/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      392 2023-12-19 13:57:23.000000 nkululeko-0.83.2/nkululeko/models/model_lin_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9471 2024-04-29 13:37:24.000000 nkululeko-0.83.2/nkululeko/models/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10290 2024-04-29 13:37:24.000000 nkululeko-0.83.2/nkululeko/models/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      914 2024-04-17 12:17:54.000000 nkululeko-0.83.2/nkululeko/models/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      699 2024-03-21 10:56:18.000000 nkululeko-0.83.2/nkululeko/models/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      390 2023-09-07 11:38:37.000000 nkululeko-0.83.2/nkululeko/models/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      397 2023-09-07 11:38:33.000000 nkululeko-0.83.2/nkululeko/models/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 10:21:07.000000 nkululeko-0.83.2/nkululeko/models/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      227 2023-12-14 15:14:23.000000 nkululeko-0.83.2/nkululeko/models/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.83.2/nkululeko/multidb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.83.2/nkululeko/nkuluflag.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.83.2/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23276 2024-04-29 13:37:24.000000 nkululeko-0.83.2/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.83.2/nkululeko/predict.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.142839 nkululeko-0.83.2/nkululeko/reporting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.83.2/nkululeko/reporting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.83.2/nkululeko/reporting/defines.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.83.2/nkululeko/reporting/latex_writer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.83.2/nkululeko/reporting/report.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.83.2/nkululeko/reporting/report_item.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12841 2024-04-25 13:02:38.000000 nkululeko-0.83.2/nkululeko/reporting/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.83.2/nkululeko/reporting/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2287 2024-04-22 09:09:10.000000 nkululeko-0.83.2/nkululeko/resample.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.83.2/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.83.2/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.83.2/nkululeko/segment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.142839 nkululeko-0.83.2/nkululeko/segmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.83.2/nkululeko/segmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.83.2/nkululeko/segmenting/seg_inaspeechsegmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.83.2/nkululeko/segmenting/seg_silero.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.83.2/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.83.2/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.83.2/nkululeko/test_predictor.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.142839 nkululeko-0.83.2/nkululeko/utils/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.83.2/nkululeko/utils/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.83.2/nkululeko/utils/files.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.83.2/nkululeko/utils/stats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12330 2024-03-21 11:06:05.000000 nkululeko-0.83.2/nkululeko/utils/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.142839 nkululeko-0.83.2/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36158 2024-04-29 13:55:35.000000 nkululeko-0.83.2/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5073 2024-04-29 13:55:35.000000 nkululeko-0.83.2/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-04-29 13:55:35.000000 nkululeko-0.83.2/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-04-29 13:55:35.000000 nkululeko-0.83.2/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-04-29 13:55:35.000000 nkululeko-0.83.2/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.83.2/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-04-29 13:55:35.142839 nkululeko-0.83.2/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.83.2/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.134839 nkululeko-0.83.2/venv/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-29 13:55:35.142839 nkululeko-0.83.2/venv/bin/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.83.2/venv/bin/activate_this.py
```

### Comparing `nkululeko-0.83.1/CHANGELOG.md` & `nkululeko-0.83.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.83.2
+--------------
+* added default cuda if present and not stated
+
 Version 0.83.1
 --------------
 * add test module to nkuluflag
 
 Version 0.83.0
 --------------
 * test module now prints out reports
```

### Comparing `nkululeko-0.83.1/LICENSE` & `nkululeko-0.83.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/PKG-INFO` & `nkululeko-0.83.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.83.1
+Version: 0.83.2
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -329,14 +329,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.83.2
+--------------
+* added default cuda if present and not stated
+
 Version 0.83.1
 --------------
 * add test module to nkuluflag
 
 Version 0.83.0
 --------------
 * test module now prints out reports
```

### Comparing `nkululeko-0.83.1/README.md` & `nkululeko-0.83.2/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/aesdd/process_database.py` & `nkululeko-0.83.2/data/aesdd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/androids/process_database.py` & `nkululeko-0.83.2/data/androids/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/androids_orig/process_database.py` & `nkululeko-0.83.2/data/androids_orig/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/androids_test/process_database.py` & `nkululeko-0.83.2/data/androids_test/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/ased/process_database.py` & `nkululeko-0.83.2/data/ased/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/asvp-esd/process_database.py` & `nkululeko-0.83.2/data/asvp-esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/baved/process_database.py` & `nkululeko-0.83.2/data/baved/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/cafe/process_database.py` & `nkululeko-0.83.2/data/cafe/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/clac/process_database.py` & `nkululeko-0.83.2/data/clac/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/cmu-mosei/process_database.py` & `nkululeko-0.83.2/data/cmu-mosei/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/demos/process_database.py` & `nkululeko-0.83.2/data/demos/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/ekorpus/process_database.py` & `nkululeko-0.83.2/data/ekorpus/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/emns/process_database.py` & `nkululeko-0.83.2/data/emns/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/emofilm/convert_to_16k.py` & `nkululeko-0.83.2/data/emofilm/convert_to_16k.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/emofilm/process_database.py` & `nkululeko-0.83.2/data/emofilm/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/emorynlp/process_database.py` & `nkululeko-0.83.2/data/emorynlp/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/emov-db/process_database.py` & `nkululeko-0.83.2/data/emov-db/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/emovo/process_database.py` & `nkululeko-0.83.2/data/emovo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/emozionalmente/create.py` & `nkululeko-0.83.2/data/emozionalmente/create.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/enterface/process_database.py` & `nkululeko-0.83.2/data/enterface/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/esd/process_database.py` & `nkululeko-0.83.2/data/esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/gerparas/process_database.py` & `nkululeko-0.83.2/data/gerparas/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/iemocap/process_database.py` & `nkululeko-0.83.2/data/iemocap/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/jl/process_database.py` & `nkululeko-0.83.2/data/jl/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/jtes/process_database.py` & `nkululeko-0.83.2/data/jtes/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/meld/process_database.py` & `nkululeko-0.83.2/data/meld/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/mesd/process_database.py` & `nkululeko-0.83.2/data/mesd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/mess/process_database.py` & `nkululeko-0.83.2/data/mess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/mlendsnd/process_database.py` & `nkululeko-0.83.2/data/mlendsnd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/msp-improv/process_database2.py` & `nkululeko-0.83.2/data/msp-improv/process_database2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/msp-podcast/process_database.py` & `nkululeko-0.83.2/data/msp-podcast/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/oreau2/process_database.py` & `nkululeko-0.83.2/data/oreau2/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/portuguese/process_database.py` & `nkululeko-0.83.2/data/portuguese/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/ravdess/process_database.py` & `nkululeko-0.83.2/data/ravdess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/ravdess/process_database_speaker.py` & `nkululeko-0.83.2/data/ravdess/process_database_speaker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/savee/process_database.py` & `nkululeko-0.83.2/data/savee/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/shemo/process_database.py` & `nkululeko-0.83.2/data/shemo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/subesco/process_database.py` & `nkululeko-0.83.2/data/subesco/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/tess/process_database.py` & `nkululeko-0.83.2/data/tess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/thorsten-emotional/process_database.py` & `nkululeko-0.83.2/data/thorsten-emotional/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/urdu/process_database.py` & `nkululeko-0.83.2/data/urdu/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/data/vivae/process_database.py` & `nkululeko-0.83.2/data/vivae/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/docs/source/conf.py` & `nkululeko-0.83.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/meta/demos/demo_best_model.py` & `nkululeko-0.83.2/meta/demos/demo_best_model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/meta/demos/my_experiment.py` & `nkululeko-0.83.2/meta/demos/my_experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/meta/demos/my_experiment_local.py` & `nkululeko-0.83.2/meta/demos/my_experiment_local.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/meta/demos/plot_faster_anim.py` & `nkululeko-0.83.2/meta/demos/plot_faster_anim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/aug_train.py` & `nkululeko-0.83.2/nkululeko/aug_train.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/augment.py` & `nkululeko-0.83.2/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/augmenting/augmenter.py` & `nkululeko-0.83.2/nkululeko/augmenting/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/augmenting/randomsplicer.py` & `nkululeko-0.83.2/nkululeko/augmenting/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/augmenting/randomsplicing.py` & `nkululeko-0.83.2/nkululeko/augmenting/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/augmenting/resampler.py` & `nkululeko-0.83.2/nkululeko/augmenting/resampler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/autopredict/ap_age.py` & `nkululeko-0.83.2/nkululeko/autopredict/ap_age.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/autopredict/ap_arousal.py` & `nkululeko-0.83.2/nkululeko/autopredict/ap_arousal.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/autopredict/ap_dominance.py` & `nkululeko-0.83.2/nkululeko/autopredict/ap_dominance.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/autopredict/ap_gender.py` & `nkululeko-0.83.2/nkululeko/autopredict/ap_gender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/autopredict/ap_mos.py` & `nkululeko-0.83.2/nkululeko/autopredict/ap_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/autopredict/ap_pesq.py` & `nkululeko-0.83.2/nkululeko/autopredict/ap_pesq.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/autopredict/ap_sdr.py` & `nkululeko-0.83.2/nkululeko/autopredict/ap_sdr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/autopredict/ap_snr.py` & `nkululeko-0.83.2/nkululeko/autopredict/ap_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/autopredict/ap_stoi.py` & `nkululeko-0.83.2/nkululeko/autopredict/ap_stoi.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/autopredict/ap_valence.py` & `nkululeko-0.83.2/nkululeko/autopredict/ap_valence.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/autopredict/estimate_snr.py` & `nkululeko-0.83.2/nkululeko/autopredict/estimate_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/cacheddataset.py` & `nkululeko-0.83.2/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/data/dataset.py` & `nkululeko-0.83.2/nkululeko/data/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/data/dataset_csv.py` & `nkululeko-0.83.2/nkululeko/data/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/demo.py` & `nkululeko-0.83.2/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/demo_feats.py` & `nkululeko-0.83.2/nkululeko/demo_feats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/demo_predictor.py` & `nkululeko-0.83.2/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/experiment.py` & `nkululeko-0.83.2/nkululeko/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -675,17 +675,20 @@
         test_predictor = TestPredictor(
             model, self.df_test, self.label_encoder, result_name
         )
         result = test_predictor.predict_and_store()
         return result
 
     def load(self, filename):
-        f = open(filename, "rb")
-        tmp_dict = pickle.load(f)
-        f.close()
+        try:
+            f = open(filename, "rb")
+            tmp_dict = pickle.load(f)
+            f.close()
+        except EOFError as eof:
+            self.util.error(f"can't open file {filename}: {eof}")
         self.__dict__.update(tmp_dict)
         glob_conf.set_labels(self.labels)
 
     def save(self, filename):
         if self.runmgr.modelrunner.model.is_ann():
             self.runmgr.modelrunner.model = None
             self.util.warn(
```

### Comparing `nkululeko-0.83.1/nkululeko/explore.py` & `nkululeko-0.83.2/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/export.py` & `nkululeko-0.83.2/nkululeko/export.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_agender.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_agender_agender.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_agender_agender.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,19 @@
         model_url = "https://zenodo.org/record/7761387/files/w2v2-L-robust-6-age-gender.25c844af-1.1.1.zip"
         model_root = self.util.config_val(
             "FEATS", "agender.model", "./audmodel_agender/"
         )
         if not os.path.isdir(model_root):
             cache_root = audeer.mkdir("cache")
             model_root = audeer.mkdir(model_root)
-            archive_path = audeer.download_url(model_url, cache_root, verbose=True)
+            archive_path = audeer.download_url(
+                model_url, cache_root, verbose=True)
             audeer.extract_archive(archive_path, model_root)
-        device = self.util.config_val("MODEL", "device", "cpu")
+        cuda = "cuda" if torch.cuda.is_available() else "cpu"
+        device = self.util.config_val("MODEL", "device", cuda)
         self.model = audonnx.load(model_root, device=device)
         #        pytorch_total_params = sum(p.numel() for p in self.model.parameters())
         # self.util.debug(
         #     f"initialized agender model with {pytorch_total_params} parameters in total"
         # )
         self.util.debug("initialized agender model")
         self.model_loaded = True
```

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_analyser.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_auddim.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_auddim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_audmodel.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_clap.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_hubert.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_hubert.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_import.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_mld.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_mos.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_opensmile.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_oxbow.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_praat.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_snr.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_spectra.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_spectra.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_spkrec.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_spkrec.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_squim.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_squim.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,20 +24,25 @@
 
 from nkululeko.feat_extract.featureset import Featureset
 import nkululeko.glob_conf as glob_conf
 from nkululeko.utils.util import Util
 
 
 class SquimSet(Featureset):
-    """Class to predict SQUIM features"""
+    """Class to predict SQUIM features."""
 
     def __init__(self, name, data_df, feats_type):
-        """Constructor. is_train is needed to distinguish from test/dev sets, because they use the codebook from the training"""
+        """Constructor.
+
+        Is_train is needed to distinguish from test/dev sets,
+        because they use the codebook from the training.
+        """
         super().__init__(name, data_df, feats_type)
-        self.device = self.util.config_val("MODEL", "device", "cpu")
+        cuda = "cuda" if torch.cuda.is_available() else "cpu"
+        self.device = self.util.config_val("MODEL", "device", cuda)
         self.model_initialized = False
 
     def init_model(self):
         # load model
         self.util.debug("loading model...")
         self.objective_model = SQUIM_OBJECTIVE.get_model()
         pytorch_total_params = sum(p.numel() for p in self.objective_model.parameters())
```

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_trill.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_wav2vec2.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_wav2vec2.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,19 @@
 import nkululeko.glob_conf as glob_conf
 
 
 class Wav2vec2(Featureset):
     """Class to extract wav2vec2 embeddings"""
 
     def __init__(self, name, data_df, feat_type):
-        """Constructor. is_train is needed to distinguish from test/dev sets, because they use the codebook from the training"""
+        """Constructor.
+
+        If_train is needed to distinguish from test/dev sets,
+        because they use the codebook from the training
+        """
         super().__init__(name, data_df, feat_type)
         cuda = "cuda" if torch.cuda.is_available() else "cpu"
         self.device = self.util.config_val("MODEL", "device", cuda)
         self.model_initialized = False
         if feat_type == "wav2vec2":
             self.feat_type = "wav2vec2-large-robust-ft-swbd-300h"
         else:
@@ -35,32 +39,30 @@
         # load model
         self.util.debug("loading wav2vec2 model...")
         model_path = self.util.config_val(
             "FEATS", "wav2vec2.model", f"facebook/{self.feat_type}"
         )
         config = transformers.AutoConfig.from_pretrained(model_path)
         layer_num = config.num_hidden_layers
-        hidden_layer = int(self.util.config_val(
-            "FEATS", "wav2vec2.layer", "0"))
+        hidden_layer = int(self.util.config_val("FEATS", "wav2vec2.layer", "0"))
         config.num_hidden_layers = layer_num - hidden_layer
         self.util.debug(f"using hidden layer #{config.num_hidden_layers}")
         self.processor = Wav2Vec2FeatureExtractor.from_pretrained(model_path)
         self.model = Wav2Vec2Model.from_pretrained(model_path, config=config).to(
             self.device
         )
         print(f"intialized Wav2vec model on {self.device}")
         self.model.eval()
         self.model_initialized = True
 
     def extract(self):
         """Extract the features or load them from disk if present."""
         store = self.util.get_path("store")
         storage = f"{store}{self.name}.pkl"
-        extract = self.util.config_val(
-            "FEATS", "needs_feature_extraction", False)
+        extract = self.util.config_val("FEATS", "needs_feature_extraction", False)
         no_reuse = eval(self.util.config_val("FEATS", "no_reuse", "False"))
         if extract or no_reuse or not os.path.isfile(storage):
             if not self.model_initialized:
                 self.init_model()
             self.util.debug(
                 "extracting wav2vec2 embeddings, this might take a while..."
             )
@@ -73,16 +75,15 @@
                     frame_offset=int(start.total_seconds() * 16000),
                     num_frames=int((end - start).total_seconds() * 16000),
                 )
                 assert sampling_rate == 16000, f"got {sampling_rate} instead of 16000"
                 emb = self.get_embeddings(signal, sampling_rate, file)
                 emb_series[idx] = emb
             # print(f"emb_series shape: {emb_series.shape}")
-            self.df = pd.DataFrame(
-                emb_series.values.tolist(), index=self.data_df.index)
+            self.df = pd.DataFrame(emb_series.values.tolist(), index=self.data_df.index)
             # print(f"df shape: {self.df.shape}")
             self.df.to_pickle(storage)
             try:
                 glob_conf.config["DATA"]["needs_feature_extraction"] = "false"
             except KeyError:
                 pass
         else:
```

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_wavlm.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_wavlm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feats_whisper.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feats_whisper.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,27 +28,30 @@
 
     def init_model(self):
         # load model
         self.util.debug("loading whisper model...")
         model_name = f"openai/{self.feat_type}"
         self.model = WhisperModel.from_pretrained(model_name).to(self.device)
         print(f"intialized Whisper model on {self.device}")
-        self.feature_extractor = AutoFeatureExtractor.from_pretrained(model_name)
+        self.feature_extractor = AutoFeatureExtractor.from_pretrained(
+            model_name)
         self.model_initialized = True
 
     def extract(self):
         """Extract the features or load them from disk if present."""
         store = self.util.get_path("store")
         storage = f"{store}{self.name}.pkl"
-        extract = self.util.config_val("FEATS", "needs_feature_extraction", False)
+        extract = self.util.config_val(
+            "FEATS", "needs_feature_extraction", False)
         no_reuse = eval(self.util.config_val("FEATS", "no_reuse", "False"))
         if extract or no_reuse or not os.path.isfile(storage):
             if not self.model_initialized:
                 self.init_model()
-            self.util.debug("extracting whisper embeddings, this might take a while...")
+            self.util.debug(
+                "extracting whisper embeddings, this might take a while...")
             emb_series = []
             for (file, start, end), _ in audeer.progress_bar(
                 self.data_df.iterrows(),
                 total=len(self.data_df),
                 desc=f"Running whisper on {len(self.data_df)} audiofiles",
             ):
                 if end == pd.NaT:
```

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/featureset.py` & `nkululeko-0.83.2/nkululeko/feat_extract/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feat_extract/feinberg_praat.py` & `nkululeko-0.83.2/nkululeko/feat_extract/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/feature_extractor.py` & `nkululeko-0.83.2/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/file_checker.py` & `nkululeko-0.83.2/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/filter_data.py` & `nkululeko-0.83.2/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/losses/loss_ccc.py` & `nkululeko-0.83.2/nkululeko/losses/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/losses/loss_softf1loss.py` & `nkululeko-0.83.2/nkululeko/losses/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/modelrunner.py` & `nkululeko-0.83.2/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/models/model.py` & `nkululeko-0.83.2/nkululeko/models/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/models/model_cnn.py` & `nkululeko-0.83.2/nkululeko/models/model_cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import torchvision.transforms as transforms
 from torch.utils.data import Dataset
 import ast
 import numpy as np
 from sklearn.metrics import recall_score
 from collections import OrderedDict
 from PIL import Image
+from traitlets import default
 
 from nkululeko.utils.util import Util
 import nkululeko.glob_conf as glob_conf
 from nkululeko.models.model import Model
 from nkululeko.reporting.reporter import Reporter
 from nkululeko.losses.loss_softf1loss import SoftF1Loss
 
@@ -44,14 +45,15 @@
             self.criterion = SoftF1Loss(
                 num_classes=self.class_num, weight=None, epsilon=1e-7
             )
         else:
             self.util.error(f"unknown loss function: {criterion}")
         self.util.debug(f"using model with cross entropy loss function")
         # set up the model
+        # cuda = "cuda" if torch.cuda.is_available() else "cpu"
         self.device = self.util.config_val("MODEL", "device", "cpu")
         try:
             layers_string = glob_conf.config["MODEL"]["layers"]
         except KeyError as ke:
             self.util.error(f"Please provide MODEL layers: {ke}")
         self.util.debug(f"using layers {layers_string}")
         layers = ast.literal_eval(layers_string)
@@ -80,15 +82,16 @@
                 transforms.ToTensor()
                 # transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))
             ]
         )
         train_set = self.Dataset_image(
             feats_train, df_train, self.target, transformations
         )
-        test_set = self.Dataset_image(feats_test, df_test, self.target, transformations)
+        test_set = self.Dataset_image(
+            feats_test, df_test, self.target, transformations)
         # Define data loaders
         self.trainloader = torch.utils.data.DataLoader(
             train_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
@@ -133,15 +136,16 @@
         self.set_testdata(df_test, feats_test)
 
     def train(self):
         self.model.train()
         losses = []
         for images, labels in self.trainloader:
             logits = self.model(images.to(self.device))
-            loss = self.criterion(logits, labels.to(self.device, dtype=torch.int64))
+            loss = self.criterion(logits, labels.to(
+                self.device, dtype=torch.int64))
             losses.append(loss.item())
             self.optimizer.zero_grad()
             loss.backward()
             self.optimizer.step()
         self.loss = (np.asarray(losses)).mean()
 
     def evaluate_model(self, model, loader, device):
@@ -161,22 +165,24 @@
                     logits[start_index:end_index, :],
                     labels.to(self.device, dtype=torch.int64),
                 )
                 losses.append(loss.item())
 
         self.loss_eval = (np.asarray(losses)).mean()
         predictions = logits.argmax(dim=1)
-        uar = recall_score(targets.numpy(), predictions.numpy(), average="macro")
+        uar = recall_score(
+            targets.numpy(), predictions.numpy(), average="macro")
         return uar, targets, predictions
 
     def predict(self):
         _, truths, predictions = self.evaluate_model(
             self.model, self.testloader, self.device
         )
-        uar, _, _ = self.evaluate_model(self.model, self.trainloader, self.device)
+        uar, _, _ = self.evaluate_model(
+            self.model, self.trainloader, self.device)
         report = Reporter(truths, predictions, self.run, self.epoch)
         try:
             report.result.loss = self.loss
         except AttributeError:  # if the model was loaded from disk the loss is unknown
             pass
         try:
             report.result.loss_eval = self.loss_eval
@@ -205,28 +211,30 @@
         torch.save(self.model.state_dict(), self.store_path)
 
     def load(self, run, epoch):
         self.set_id(run, epoch)
         dir = self.util.get_path("model_dir")
         # name = f'{self.util.get_exp_name()}_{run}_{epoch:03d}.model'
         name = f"{self.util.get_exp_name(only_train=True)}_{self.run}_{self.epoch:03d}.model"
-        self.device = self.util.config_val("MODEL", "device", "cpu")
+        cuda = "cuda" if torch.cuda.is_available() else "cpu"
+        self.device = self.util.config_val("MODEL", "device", cuda)
         layers = ast.literal_eval(glob_conf.config["MODEL"]["layers"])
         self.store_path = dir + name
         drop = self.util.config_val("MODEL", "drop", False)
         if drop:
             self.util.debug(f"loading: dropout set to: {drop}")
         self.model = myCNN(layers, self.class_num).to(self.device)
         self.model.load_state_dict(torch.load(self.store_path))
         self.model.eval()
 
     def load_path(self, path, run, epoch):
         self.set_id(run, epoch)
         with open(path, "rb") as handle:
-            self.device = self.util.config_val("MODEL", "device", "cpu")
+            cuda = "cuda" if torch.cuda.is_available() else "cpu"
+            self.device = self.util.config_val("MODEL", "device", cuda)
             layers = ast.literal_eval(glob_conf.config["MODEL"]["layers"])
             self.store_path = path
             drop = self.util.config_val("MODEL", "drop", False)
             if drop:
                 self.util.debug(f"dropout set to: {drop}")
             self.model = self.MLP(
                 self.feats_train.shape[1], layers, self.class_num, drop
```

### Comparing `nkululeko-0.83.1/nkululeko/models/model_gmm.py` & `nkululeko-0.83.2/nkululeko/models/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/models/model_knn.py` & `nkululeko-0.83.2/nkululeko/models/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/models/model_knn_reg.py` & `nkululeko-0.83.2/nkululeko/models/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/models/model_mlp.py` & `nkululeko-0.83.2/nkululeko/models/model_mlp.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,16 +30,17 @@
         elif criterion == "f1":
             self.criterion = SoftF1Loss(
                 num_classes=self.class_num, weight=None, epsilon=1e-7
             )
         else:
             self.util.error(f"unknown loss function: {criterion}")
         self.util.debug(f"using model with cross entropy loss function")
-        # set up the model
-        self.device = self.util.config_val("MODEL", "device", "cpu")
+        # set up the model, use GPU if availabe
+        cuda = "cuda" if torch.cuda.is_available() else "cpu"
+        self.device = self.util.config_val("MODEL", "device", cuda)
         try:
             layers_string = glob_conf.config["MODEL"]["layers"]
         except KeyError as ke:
             self.util.error(f"Please provide MODEL layers: {ke}")
         self.util.debug(f"using layers {layers_string}")
         layers = ast.literal_eval(layers_string)
         # with dropout?
@@ -82,15 +83,16 @@
         self.testloader = self.get_loader(feats_test, df_test, False)
 
     def train(self):
         self.model.train()
         losses = []
         for features, labels in self.trainloader:
             logits = self.model(features.to(self.device))
-            loss = self.criterion(logits, labels.to(self.device, dtype=torch.int64))
+            loss = self.criterion(logits, labels.to(
+                self.device, dtype=torch.int64))
             losses.append(loss.item())
             self.optimizer.zero_grad()
             loss.backward()
             self.optimizer.step()
         self.loss = (np.asarray(losses)).mean()
 
     def evaluate_model(self, model, loader, device):
@@ -110,22 +112,24 @@
                     logits[start_index:end_index, :].to(device),
                     labels.to(device, dtype=torch.int64),
                 )
                 losses.append(loss.item())
 
         self.loss_eval = (np.asarray(losses)).mean()
         predictions = logits.argmax(dim=1)
-        uar = recall_score(targets.numpy(), predictions.numpy(), average="macro")
+        uar = recall_score(
+            targets.numpy(), predictions.numpy(), average="macro")
         return uar, targets, predictions
 
     def predict(self):
         _, truths, predictions = self.evaluate_model(
             self.model, self.testloader, self.device
         )
-        uar, _, _ = self.evaluate_model(self.model, self.trainloader, self.device)
+        uar, _, _ = self.evaluate_model(
+            self.model, self.trainloader, self.device)
         report = Reporter(truths, predictions, self.run, self.epoch)
         try:
             report.result.loss = self.loss
         except AttributeError:  # if the model was loaded from disk the loss is unknown
             pass
         try:
             report.result.loss_eval = self.loss_eval
@@ -175,14 +179,17 @@
     def predict_sample(self, features):
         """Predict one sample"""
         with torch.no_grad():
             features = torch.from_numpy(features)
             features = np.reshape(features, (-1, 1)).T
             logits = self.model(features.to(self.device))
             # logits = self.model(features)
+        # if tensor conver to cpu
+        if isinstance(logits, torch.Tensor):
+            logits = logits.cpu()
         a = logits.numpy()
         res = {}
         for i in range(len(a[0])):
             res[i] = a[0][i]
         return res
 
     def store(self):
@@ -192,30 +199,32 @@
         pass
 
     def load(self, run, epoch):
         self.set_id(run, epoch)
         dir = self.util.get_path("model_dir")
         # name = f'{self.util.get_exp_name()}_{run}_{epoch:03d}.model'
         name = f"{self.util.get_exp_name(only_train=True)}_{self.run}_{self.epoch:03d}.model"
-        self.device = self.util.config_val("MODEL", "device", "cpu")
+        cuda = "cuda" if torch.cuda.is_available() else "cpu"
+        self.device = self.util.config_val("MODEL", "device", cuda)
         layers = ast.literal_eval(glob_conf.config["MODEL"]["layers"])
         self.store_path = dir + name
         drop = self.util.config_val("MODEL", "drop", False)
         if drop:
             self.util.debug(f"loading: dropout set to: {drop}")
         self.model = self.MLP(
             self.feats_train.shape[1], layers, self.class_num, drop
         ).to(self.device)
         self.model.load_state_dict(torch.load(self.store_path))
         self.model.eval()
 
     def load_path(self, path, run, epoch):
         self.set_id(run, epoch)
         with open(path, "rb") as handle:
-            self.device = self.util.config_val("MODEL", "device", "cpu")
+            cuda = "cuda" if torch.cuda.is_available() else "cpu"
+            self.device = self.util.config_val("MODEL", "device", cuda)
             layers = ast.literal_eval(glob_conf.config["MODEL"]["layers"])
             self.store_path = path
             drop = self.util.config_val("MODEL", "drop", False)
             if drop:
                 self.util.debug(f"dropout set to: {drop}")
             self.model = self.MLP(
                 self.feats_train.shape[1], layers, self.class_num, drop
```

### Comparing `nkululeko-0.83.1/nkululeko/models/model_mlp_regression.py` & `nkululeko-0.83.2/nkululeko/models/model_mlp_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import numpy as np
 import torch
 
 from audmetric import concordance_cc
 from audmetric import mean_absolute_error
 from audmetric import mean_squared_error
+from traitlets import default
 
 import nkululeko.glob_conf as glob_conf
 from nkululeko.losses.loss_ccc import ConcordanceCorCoeff
 from nkululeko.models.model import Model
 from nkululeko.reporting.reporter import Reporter
 
 
@@ -36,25 +37,27 @@
             self.criterion = torch.nn.L1Loss()
         elif criterion == "1-ccc":
             self.criterion = ConcordanceCorCoeff()
         else:
             self.util.error(f"unknown loss function: {criterion}")
         self.util.debug(f"training model with {criterion} loss function")
         # set up the model
-        self.device = self.util.config_val("MODEL", "device", "cpu")
+        cuda = "cuda" if torch.cuda.is_available() else "cpu"
+        self.device = self.util.config_val("MODEL", "device", cuda)
         layers_string = glob_conf.config["MODEL"]["layers"]
         self.util.debug(f"using layers {layers_string}")
         try:
             layers = ast.literal_eval(layers_string)
         except KeyError as ke:
             self.util.error(f"Please provide MODEL layers: {ke}")
         drop = self.util.config_val("MODEL", "drop", False)
         if drop:
             self.util.debug(f"training with dropout: {drop}")
-        self.model = self.MLP(feats_train.shape[1], layers, 1, drop).to(self.device)
+        self.model = self.MLP(
+            feats_train.shape[1], layers, 1, drop).to(self.device)
         self.learning_rate = float(
             self.util.config_val("MODEL", "learning_rate", 0.0001)
         )
         # set up regularization
         self.optimizer = torch.optim.Adam(
             self.model.parameters(), lr=self.learning_rate
         )
@@ -89,16 +92,18 @@
         )
         return loss
 
     def predict(self):
         _, truths, predictions = self.evaluate_model(
             self.model, self.testloader, self.device
         )
-        result, _, _ = self.evaluate_model(self.model, self.trainloader, self.device)
-        report = Reporter(truths.numpy(), predictions.numpy(), self.run, self.epoch)
+        result, _, _ = self.evaluate_model(
+            self.model, self.trainloader, self.device)
+        report = Reporter(truths.numpy(), predictions.numpy(),
+                          self.run, self.epoch)
         try:
             report.result.loss = self.loss
         except AttributeError:  # if the model was loaded from disk the loss is unknown
             pass
         try:
             report.result.loss_eval = self.loss_eval
         except AttributeError:  # if the model was loaded from disk the loss is unknown
@@ -124,17 +129,19 @@
             self.label = label
 
         def __len__(self):
             return len(self.df)
 
         def __getitem__(self, item):
             index = self.df.index[item]
-            features = self.df_features.loc[index, :].values.astype("float32").squeeze()
+            features = self.df_features.loc[index, :].values.astype(
+                "float32").squeeze()
             labels = (
-                np.array([self.df.loc[index, self.label]]).astype("float32").squeeze()
+                np.array([self.df.loc[index, self.label]]
+                         ).astype("float32").squeeze()
             )
             return features, labels
 
     class MLP(torch.nn.Module):
         def __init__(self, i, layers, o, drop):
             super().__init__()
             sorted_layers = sorted(layers.items(), key=lambda x: x[1])
@@ -183,15 +190,16 @@
         losses = []
         with torch.no_grad():
             for index, (features, labels) in enumerate(loader):
                 start_index = index * loader.batch_size
                 end_index = (index + 1) * loader.batch_size
                 if end_index > len(loader.dataset):
                     end_index = len(loader.dataset)
-                logits[start_index:end_index] = model(features.to(device)).reshape(-1)
+                logits[start_index:end_index] = model(
+                    features.to(device)).reshape(-1)
                 targets[start_index:end_index] = labels
                 loss = self.criterion(
                     logits[start_index:end_index].to(
                         device,
                     ),
                     labels.to(device),
                 )
```

### Comparing `nkululeko-0.83.1/nkululeko/models/model_svm.py` & `nkululeko-0.83.2/nkululeko/models/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/models/model_svr.py` & `nkululeko-0.83.2/nkululeko/models/model_svr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/multidb.py` & `nkululeko-0.83.2/nkululeko/multidb.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/nkuluflag.py` & `nkululeko-0.83.2/nkululeko/nkuluflag.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/nkululeko.py` & `nkululeko-0.83.2/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/plots.py` & `nkululeko-0.83.2/nkululeko/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         df_speakers = pd.DataFrame()
         pd.options.mode.chained_assignment = None  # default='warn'
         for s in df.speaker.unique():
             df_speaker = df[df.speaker == s]
             df_speaker["samplenum"] = df_speaker.shape[0]
             df_speakers = pd.concat([df_speakers, df_speaker.head(1)])
         # plot the distribution of samples per speaker
-        fig_dir = self.util.get_path("fig_dir") + "../"  # one up because of the runs
+        # one up because of the runs
+        fig_dir = self.util.get_path("fig_dir") + "../"
         self.util.debug(f"plotting samples per speaker")
         if "gender" in df_speakers:
             filename = f"samples_value_counts"
             ax = (
                 df_speakers.groupby("samplenum")["gender"]
                 .value_counts()
                 .unstack()
@@ -133,43 +134,46 @@
                         )
                 else:
                     if self.util.is_categorical(df[att1]):
                         ax, caption = self._plotcatcont(
                             df, att1, class_label, att1, type_s
                         )
                     else:
-                        ax, caption = self._plot2cont(df, class_label, att1, type_s)
+                        ax, caption = self._plot2cont(
+                            df, class_label, att1, type_s)
                 self._save_plot(
                     ax,
                     caption,
                     f"Correlation of {self.target} and {att[0]}",
                     filename,
                     type_s,
                 )
                 # fig.clear()           # avoid error
             elif len(att) == 2:
                 att1 = att[0]
                 att2 = att[1]
                 if att1 == self.target or att2 == self.target:
-                    self.util.debug(f"no need to correlate {self.target} with itself")
+                    self.util.debug(
+                        f"no need to correlate {self.target} with itself")
                     return
                 if att1 not in df:
                     self.util.error(f"unknown feature: {att1}")
                 if att2 not in df:
                     self.util.error(f"unknown feature: {att2}")
                 att1, df = self._check_binning(att1, df)
                 att2, df = self._check_binning(att2, df)
                 self.util.debug(f"plotting {att}")
                 filename = f"{att1}-{att2}"
                 filename = f"{self.target}-{filename}"
                 if self.util.is_categorical(df["class_label"]):
                     if self.util.is_categorical(df[att1]):
                         if self.util.is_categorical(df[att2]):
                             # class_label = cat, att1 = cat, att2 = cat
-                            ax, caption = self._plot2cat(df, att1, att2, att1, type_s)
+                            ax, caption = self._plot2cat(
+                                df, att1, att2, att1, type_s)
                         else:
                             # class_label = cat, att1 = cat, att2 = cont
                             ax, caption = self._plotcatcont(
                                 df, att1, att2, att1, type_s
                             )
                     else:
                         if self.util.is_categorical(df[att2]):
@@ -182,42 +186,45 @@
                             ax, caption = self._plot2cont_cat(
                                 df, att1, att2, "class_label", type_s
                             )
                 else:  # class_label is continuous
                     if self.util.is_categorical(df[att1]):
                         if self.util.is_categorical(df[att2]):
                             # class_label = cont, att1 = cat, att2 = cat
-                            ax, caption = self._plot2cat(df, att1, att2, att1, type_s)
+                            ax, caption = self._plot2cat(
+                                df, att1, att2, att1, type_s)
                         else:
                             # class_label = cont, att1 = cat, att2 = cont
                             ax, caption = self._plot2cont_cat(
                                 df, att2, "class_label", att1, type_s
                             )
                     else:
                         if self.util.is_categorical(df[att2]):
                             # class_label = cont, att1 = cont, att2 = cat
                             ax, caption = self._plot2cont_cat(
                                 df, att1, "class_label", att2, type_s
                             )
                         else:
                             # class_label = cont, att1 = cont, att2 = cont
-                            ax, caption = self._plot2cont(df, att1, att2, type_s)
+                            ax, caption = self._plot2cont(
+                                df, att1, att2, type_s)
 
                 self._save_plot(
                     ax, caption, f"Correlation of {att1} and {att2}", filename, type_s
                 )
 
             else:
                 self.util.error(
                     "plot value counts: the plot distribution descriptor for"
                     f" {att} has more than 2 values. Perhaps you forgot to state a list of lists?"
                 )
 
     def _save_plot(self, ax, caption, header, filename, type_s):
-        fig_dir = self.util.get_path("fig_dir") + "../"  # one up because of the runs
+        # one up because of the runs
+        fig_dir = self.util.get_path("fig_dir") + "../"
         fig = ax.figure
         # avoid warning
         # plt.tight_layout()
         img_path = f"{fig_dir}{filename}_{type_s}.{self.format}"
         plt.savefig(img_path)
         plt.close(fig)
         # fig.clear()   # avoid error
@@ -227,15 +234,16 @@
                 header,
                 caption,
                 img_path,
             )
         )
 
     def _check_binning(self, att, df):
-        bin_reals_att = eval(self.util.config_val("EXPL", f"{att}.bin_reals", "False"))
+        bin_reals_att = eval(self.util.config_val(
+            "EXPL", f"{att}.bin_reals", "False"))
         if bin_reals_att:
             self.util.debug(f"binning continuous variable {att} to categories")
             att_new = f"{att}_binned"
             df[att_new] = self.util.continuous_to_categorical(df[att]).values
             att = att_new
         return att, df
 
@@ -301,15 +309,16 @@
             .plot(kind="bar", stacked=True, title=caption, rot=0)
         )
         ax.set_ylabel(f"number of {ylab}")
         ax.set_xlabel(xlab)
         return ax, caption
 
     def plot_durations(self, df, filename, sample_selection, caption=""):
-        fig_dir = self.util.get_path("fig_dir") + "../"  # one up because of the runs
+        # one up because of the runs
+        fig_dir = self.util.get_path("fig_dir") + "../"
         try:
             ax = sns.histplot(df, x="duration", hue="class_label", kde=True)
         except AttributeError as ae:
             self.util.warn(ae)
             ax = sns.histplot(df, x="duration", kde=True)
         min = self.util.to_3_digits(df.duration.min())
         max = self.util.to_3_digits(df.duration.max())
@@ -329,15 +338,16 @@
                 title,
                 img_path,
             )
         )
 
     def describe_df(self, name, df, target, filename):
         """Make a stacked barplot of samples and speakers per sex and target values. speaker, gender and target columns must be present"""
-        fig_dir = self.util.get_path("fig_dir") + "../"  # one up because of the runs
+        fig_dir = self.util.get_path(
+            "fig_dir") + "../"  # one up because of the runs
         sampl_num = df.shape[0]
         sex_col = "gender"
         if target == "gender":
             sex_col = "class_label"
         if self.util.exp_is_classification() and target != "gender":
             target = "class_label"
         if df.is_labeled:
@@ -376,16 +386,18 @@
                     "",
                     img_path,
                 )
             )
 
     def scatter_plot(self, feats, label_df, label, dimred_type):
         dim_num = int(self.util.config_val("EXPL", "scatter.dim", 2))
-        fig_dir = self.util.get_path("fig_dir") + "../"  # one up because of the runs
-        sample_selection = self.util.config_val("EXPL", "sample_selection", "all")
+        # one up because of the runs
+        fig_dir = self.util.get_path("fig_dir") + "../"
+        sample_selection = self.util.config_val(
+            "EXPL", "sample_selection", "all")
         filename = f"{label}_{self.util.get_feattype_name()}_{sample_selection}_{dimred_type}_{str(dim_num)}d"
         filename = f"{fig_dir}{filename}.{self.format}"
         self.util.debug(f"computing {dimred_type}, this might take a while...")
         data = None
         labels = label_df[label]
         if dimred_type == "tsne":
             data = self.getTsne(feats, dim_num)
@@ -419,15 +431,16 @@
                 y,
                 feats.index,
                 columns=columns,
             )
 
         if dim_num == 2:
             plot_data = np.vstack((data.T, labels)).T
-            plot_df = pd.DataFrame(data=plot_data, columns=("Dim_1", "Dim_2", "label"))
+            plot_df = pd.DataFrame(
+                data=plot_data, columns=("Dim_1", "Dim_2", "label"))
             # plt.tight_layout()
             ax = (
                 sns.FacetGrid(plot_df, hue="label", height=6)
                 .map(plt.scatter, "Dim_1", "Dim_2")
                 .add_legend()
             )
         elif dim_num == 3:
@@ -511,15 +524,16 @@
         )
         tsne_data = model.fit_transform(feats)
         return tsne_data
 
     def plot_feature(self, title, feature, label, df_labels, df_features):
         # remove fullstops in the name
         feature_name = feature.replace(".", "-")
-        fig_dir = self.util.get_path("fig_dir") + "../"  # one up because of the runs
+        # one up because of the runs
+        fig_dir = self.util.get_path("fig_dir") + "../"
         filename = f"{fig_dir}feat_dist_{title}_{feature_name}.{self.format}"
         if self.util.is_categorical(df_labels[label]):
             df_plot = pd.DataFrame(
                 {label: df_labels[label], feature: df_features[feature]}
             )
             ax = sns.violinplot(data=df_plot, x=label, y=feature)
             label = self.util.config_val("DATA", "target", "class_label")
@@ -550,15 +564,16 @@
 
         ax = plt.gca()
         ax.figure.set_size_inches(100, 60)
         #        tree.plot_tree(model, ax = ax)
         tree.plot_tree(model, feature_names=list(features.columns), ax=ax)
         # plt.tight_layout()
         # print(ax)
-        fig_dir = self.util.get_path("fig_dir") + "../"  # one up because of the runs
+        # one up because of the runs
+        fig_dir = self.util.get_path("fig_dir") + "../"
         exp_name = self.util.get_exp_name(only_data=True)
         format = self.util.config_val("PLOT", "format", "png")
         filename = f"{fig_dir}{exp_name}EXPL_tree-plot.{format}"
         fig = ax.figure
         fig.savefig(filename)
         fig.clear()
         plt.close(fig)
```

### Comparing `nkululeko-0.83.1/nkululeko/predict.py` & `nkululeko-0.83.2/nkululeko/predict.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/reporting/defines.py` & `nkululeko-0.83.2/nkululeko/reporting/defines.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/reporting/latex_writer.py` & `nkululeko-0.83.2/nkululeko/reporting/latex_writer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/reporting/report.py` & `nkululeko-0.83.2/nkululeko/reporting/report.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/reporting/report_item.py` & `nkululeko-0.83.2/nkululeko/reporting/report_item.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/reporting/reporter.py` & `nkululeko-0.83.2/nkululeko/reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/reporting/result.py` & `nkululeko-0.83.2/nkululeko/reporting/result.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/resample.py` & `nkululeko-0.83.2/nkululeko/resample.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/runmanager.py` & `nkululeko-0.83.2/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/scaler.py` & `nkululeko-0.83.2/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/segment.py` & `nkululeko-0.83.2/nkululeko/segment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/segmenting/seg_inaspeechsegmenter.py` & `nkululeko-0.83.2/nkululeko/segmenting/seg_inaspeechsegmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/segmenting/seg_silero.py` & `nkululeko-0.83.2/nkululeko/segmenting/seg_silero.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/syllable_nuclei.py` & `nkululeko-0.83.2/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/test.py` & `nkululeko-0.83.2/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/test_predictor.py` & `nkululeko-0.83.2/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/utils/files.py` & `nkululeko-0.83.2/nkululeko/utils/files.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/utils/stats.py` & `nkululeko-0.83.2/nkululeko/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko/utils/util.py` & `nkululeko-0.83.2/nkululeko/utils/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.83.2/nkululeko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.83.1
+Version: 0.83.2
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -329,14 +329,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.83.2
+--------------
+* added default cuda if present and not stated
+
 Version 0.83.1
 --------------
 * add test module to nkuluflag
 
 Version 0.83.0
 --------------
 * test module now prints out reports
```

### Comparing `nkululeko-0.83.1/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.83.2/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/setup.cfg` & `nkululeko-0.83.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nkululeko-0.83.1/venv/bin/activate_this.py` & `nkululeko-0.83.2/venv/bin/activate_this.py`

 * *Files identical despite different names*

