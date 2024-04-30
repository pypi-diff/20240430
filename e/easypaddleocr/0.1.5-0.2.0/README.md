# Comparing `tmp/easypaddleocr-0.1.5.tar.gz` & `tmp/easypaddleocr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypaddleocr-0.1.5.tar", last modified: Sat Apr 27 15:41:53 2024, max compression
+gzip compressed data, was "easypaddleocr-0.2.0.tar", last modified: Tue Apr 30 08:25:23 2024, max compression
```

## Comparing `easypaddleocr-0.1.5.tar` & `easypaddleocr-0.2.0.tar`

### file list

```diff
@@ -1,130 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.475957 easypaddleocr-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-27 15:41:53.475957 easypaddleocr-0.1.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.455958 easypaddleocr-0.1.5/easypaddleocr/
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/infer_cls_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/infer_det_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/infer_rec_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/infer_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/tools_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.459957 easypaddleocr-0.1.5/easypaddleocr/torchocr/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.459957 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/collate_fn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.463957 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/ColorJitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/abinet_aug.py
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/ct_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    28635 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/drrg_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/east_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    20193 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/fce_aug.py
--rw-r--r--   0 runner    (1001) docker     (127)    25842 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/fce_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)    44263 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/label_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/make_border_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/make_pse_gt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/make_shrink_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    40691 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/pg_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/randaugment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/random_crop_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    26725 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/rec_img_aug.py
--rw-r--r--   0 runner    (1001) docker     (127)    28698 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/sast_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/ssl_img_aug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/table_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.463957 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/text_image_aug/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/text_image_aug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/text_image_aug/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/text_image_aug/warp_mls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/multi_scale_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/pgnet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/pubtab_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/data/simple_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.463957 easypaddleocr-0.1.5/easypaddleocr/torchocr/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/engine/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.463957 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.463957 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/architectures/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/architectures/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/architectures/distillation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.467957 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/det_mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/det_resnet_vd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_hgnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_lcnetv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_mv1_enhance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_nrtr_mtb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_resnet_31.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_resnet_vd.py
--rw-r--r--   0 runner    (1001) docker     (127)    19956 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_svtrnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.467957 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/cls_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/det_db_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/multiheadAttention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/rec_att_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/rec_ctc_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/rec_multi_head.py
--rw-r--r--   0 runner    (1001) docker     (127)    25935 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/rec_nrtr_head.py
--rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/rec_sar_head.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.467957 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/necks/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/necks/db_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/necks/intracl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/necks/rnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.471957 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/transforms/tps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.471957 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/cls_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/ct_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/db_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/drrg_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/east_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/fce_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/locality_aware_nms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/pg_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/picodet_postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.471957 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/pse_postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/pse_postprocess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.471957 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/pse_postprocess/pse/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/pse_postprocess/pse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/pse_postprocess/pse/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/pse_postprocess/pse_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    37952 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/rec_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    13048 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/sast_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/table_postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.475957 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/ckpt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.475957 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/e2e_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/e2e_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/e2e_utils/extract_batchsize.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/e2e_utils/extract_textpoint_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)    21466 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/e2e_utils/extract_textpoint_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/e2e_utils/pgnet_pp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/e2e_utils/visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/gen_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/poly_nms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/easypaddleocr/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:41:53.475957 easypaddleocr-0.1.5/easypaddleocr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-27 15:41:53.000000 easypaddleocr-0.1.5/easypaddleocr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-27 15:41:53.000000 easypaddleocr-0.1.5/easypaddleocr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 15:41:53.000000 easypaddleocr-0.1.5/easypaddleocr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-27 15:41:53.000000 easypaddleocr-0.1.5/easypaddleocr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 15:41:53.000000 easypaddleocr-0.1.5/easypaddleocr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-27 15:41:49.000000 easypaddleocr-0.1.5/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 15:41:53.475957 easypaddleocr-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.798332 easypaddleocr-0.2.0/easypaddleocr/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/base_ocr_v20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/predict_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/predict_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18529 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/predict_rec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/predict_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.798332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.798332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.798332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/gen_table_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14205 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.798332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.798332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/architectures/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/architectures/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.802332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_resnet_vd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_resnet_vd_sast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/e2e_resnet_vd_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_hgnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_lcnetv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14852 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_lcnetv3_bak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_mv1_enhance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_nrtr_mtb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_31.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_vd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19950 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_svtrnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_vitstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/table_mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/table_resnet_vd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.806332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/cls_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_db_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_east_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_fce_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_pse_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_sast_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/e2e_pg_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/multiheadAttention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_att_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10803 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_can_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_ctc_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_multi_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32230 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_nrtr_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13998 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_sar_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10383 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_srn_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14521 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/self_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/sr_rensnet_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/table_att_head.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.806332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13771 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/db_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/east_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12731 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/fce_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/intracl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/pg_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/sast_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/table_fpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.806332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/stn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/tbsrn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10786 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/tps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/tps_spatial_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/tsrn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/cls_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/db_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/east_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8031 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/fce_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/locality_aware_nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pg_postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27043 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/rec_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/sast_postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/extract_batchsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/extract_textpoint_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22223 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/extract_textpoint_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/pgnet_pp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/poly_nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18308 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/easypaddleocr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 08:25:23.000000 easypaddleocr-0.2.0/easypaddleocr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-30 08:25:23.000000 easypaddleocr-0.2.0/easypaddleocr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:25:23.000000 easypaddleocr-0.2.0/easypaddleocr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-30 08:25:23.000000 easypaddleocr-0.2.0/easypaddleocr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 08:25:23.000000 easypaddleocr-0.2.0/easypaddleocr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/setup.cfg
```

### Comparing `easypaddleocr-0.1.5/LICENCE` & `easypaddleocr-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.5/PKG-INFO` & `easypaddleocr-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypaddleocr
-Version: 0.1.5
+Version: 0.2.0
 Summary: A simple, optional tool for PaddleOCR Detection, direction classification and recognition on CPU and GPU using torch.
 Author: pk5ls20, hv0905
 Project-URL: Code, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Documentation, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Download, https://pypi.org/project/easypaddleocr
 Project-URL: Homepage, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Issues, https://github.com/pk5ls20/EasyPaddleOCR/issues
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/__init__.py` & `easypaddleocr-0.2.0/easypaddleocr/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,64 @@
-import cv2
 import numpy as np
 import torch
 from huggingface_hub import hf_hub_download
 from loguru import logger
-
-from .infer_system import InferSystem
+from .predict_system import PredictSystem
 
 
 class EasyPaddleOCR:
-    def __init__(self, use_angle_cls=False, devices="auto", needWarmUp=False, warmup_size=(640, 640), **kwargs):
+    def __init__(self, use_angle_cls=False, devices="auto", needWarmUp=False,
+                 warmup_size=(640, 640), drop_score=0.5, **kwargs):
         """
         Initialize EasyPaddleOCR object with specified parameters.
         :param use_angle_cls: Whether to use angle classifier. This is used to detect text that is 180' rotated.
         :param devices: Device to use in pytorch. "auto" for auto-detect, "cpu" for cpu, "cuda" for cuda.
         :param needWarmUp: Whether to warm up the model. This will take some time.
         :param warmup_size: Size of the image to use in warm up. Please specify the **MAX** image size you want to
         inference with in this parameter when possible. This can reduce the usage of VMEM.
         :param kwargs: other parameters to pass to InferSystem. See original PaddleOCR documentation for more details.
         """
         self._modelFileKeys = ["det_model_path", "rec_model_path", "cls_model_path",
-                               "det_model_config_path", "rec_model_config_path", "cls_model_config_path",
-                               "character_dict_path"]
+                               "det_model_config_path", "rec_model_config_path", "character_dict_path"]
         self._modelFilePaths = {key: kwargs.get(key, None) for key in self._modelFileKeys}
-        self._devices = devices
-        if self._devices == "auto":
-            self._devices = "cuda" if torch.cuda.is_available() else "cpu"
-        logger.info(f"Using device: {self._devices}")
+        if devices == "auto":
+            self._use_gpu = True if torch.cuda.is_available() else False
+        else:
+            self._use_gpu = True if devices == "cuda" else False
+        logger.info(f"Using device: {devices}")
         self._download_file(self._modelFilePaths)
-        self.use_angle_cls = use_angle_cls
-        self.ocr = InferSystem(use_angle_cls=self.use_angle_cls,
-                               det_model_config=self._modelFilePaths["det_model_config_path"],
-                               det_model_name=self._modelFilePaths["det_model_path"],
-                               rec_model_config=self._modelFilePaths["rec_model_config_path"],
-                               rec_model_name=self._modelFilePaths["rec_model_path"],
-                               cls_model_config=self._modelFilePaths["cls_model_config_path"],
-                               cls_model_name=self._modelFilePaths["cls_model_path"],
-                               character_dict_path=self._modelFilePaths["character_dict_path"],
-                               drop_score=kwargs.get("drop_score", 0.5),
-                               det_box_type=kwargs.get("det_box_type", "quad"),
-                               save_crop_res=kwargs.get("save_crop_res", False),
-                               crop_res_save_dir=kwargs.get("crop_res_save_dir", "./output"),
-                               devices=self._devices)
+        self.ocr = PredictSystem(use_angle_cls=use_angle_cls,
+                                 det_yaml_path=self._modelFilePaths["det_model_config_path"],
+                                 det_model_path=self._modelFilePaths["det_model_path"],
+                                 rec_yaml_path=self._modelFilePaths["rec_model_config_path"],
+                                 rec_model_path=self._modelFilePaths["rec_model_path"],
+                                 cls_model_path=self._modelFilePaths["cls_model_path"],
+                                 rec_char_dict_path=self._modelFilePaths["character_dict_path"],
+                                 drop_score=drop_score,
+                                 use_gpu=self._use_gpu)
         self.needWarmUp = needWarmUp
         self._warm_up(warmup_size) if self.needWarmUp else None
 
     @staticmethod
     def _download_file(fileDict):
         config_default_dict = {
-            "det_model_path": "pt/ch_PP-OCRv4_det_server_train/best_accuracy.pth",
-            "rec_model_path": "pt/ch_PP-OCRv4_rec_server_train/best_accuracy.pth",
-            "cls_model_path": "pt/cls/best_accuracy.pth",
-            "det_model_config_path": "configs/det/ch_PP-OCRv4/ch_PP-OCRv4_det_teacher.yml",
-            "rec_model_config_path": "configs/rec/PP-OCRv4/ch_PP-OCRv4_rec_hgnet.yml",
-            "cls_model_config_path": "configs/cls/cls_mv3.yml",
+            "det_model_path": "PaddleOCR2Pytorch/ch_ptocr_v4_det_infer.pth",
+            "rec_model_path": "PaddleOCR2Pytorch/ch_ptocr_v4_rec_infer.pth",
+            "cls_model_path": "PaddleOCR2Pytorch/ch_ptocr_mobile_v2.0_cls_infer.pth",
+            "det_model_config_path": "PaddleOCR2Pytorch/configs/det/ch_PP-OCRv4/ch_PP-OCRv4_det_student.yml",
+            "rec_model_config_path": "PaddleOCR2Pytorch/configs/rec/PP-OCRv4/ch_PP-OCRv4_rec.yml",
             "character_dict_path": "ppocr_keys_v1.txt"
         }
         for key, val in fileDict.items():
             if not val:
                 logger.warning(f"Unspecified {key[:-5]}, using default value {config_default_dict[key]}")
                 fileDict[key] = hf_hub_download(repo_id="pk5ls20/PaddleModel", filename=config_default_dict[key])
+        logger.info(fileDict)
 
     def _warm_up(self, warmup_size):
         logger.info("Warm up started")
         assert (isinstance(warmup_size, (list, tuple)) and
                 len(warmup_size) == 2), "warmup_size must be tuple or list with 2 elems."
         img = np.random.uniform(0, 255, [warmup_size[0], warmup_size[1], 3]).astype(np.uint8)
         for i in range(10):
             _ = self.ocr(img)
         logger.info("Warm up finished")
-
-
-if __name__ == '__main__':
-    ocr = EasyPaddleOCR(use_angle_cls=True, needWarmUp=True)
-    image_path = r'C:\Users\pk5ls\Desktop\PytorchOCR\img\1_normal_1.jpeg'
-    image = cv2.imread(image_path)
-    image_ndarray = np.array(image)
-    print(ocr.ocr(image_ndarray))
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/infer_system.py` & `easypaddleocr-0.2.0/easypaddleocr/predict_system.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,120 +1,113 @@
-import os
+import time
+
 import cv2
 import copy
-import time
-import logging
-from .tools_utility import get_minarea_rect_crop, get_rotate_crop_image
-from .torchocr.utils.logging import get_logger
-from .infer_det_class import TextDetector
-from .infer_rec_class import TextRecognizer
-from .infer_cls_class import TextClassifier
+import numpy as np
 
-logger = get_logger()
+from .predict_rec import TextRecognizer
+from .predict_det import TextDetector
+from .predict_cls import TextClassifier
+from .config import Config
 
 
-class InferSystem:
+class PredictSystem:
     def __init__(self, **kwargs):
-        if not kwargs.get("show_log", None):
-            logger.setLevel(logging.WARNING)
-        self.use_angle_cls = kwargs.get("use_angle_cls", False)
-        self.text_detector = TextDetector(
-            kwargs.get("det_model_config"),
-            kwargs.get("det_model_name"),
-            kwargs.get("devices")
-        )
-        self.text_recognizer = TextRecognizer(
-            kwargs.get("rec_model_config"),
-            kwargs.get("rec_model_name"),
-            kwargs.get("character_dict_path"),
-            kwargs.get("devices")
-        )
+        self.args = Config(**kwargs)
+        self.text_detector = TextDetector(self.args)
+        self.text_recognizer = TextRecognizer(self.args)
+        self.use_angle_cls = self.args.use_angle_cls
+        self.drop_score = self.args.drop_score
         if self.use_angle_cls:
-            self.text_classifier = TextClassifier(
-                kwargs.get("cls_model_config"),
-                kwargs.get("cls_model_name"),
-                kwargs.get("devices")
-            )
-        self.drop_score = kwargs.get("drop_score", 0.5)
-        self.det_box_type = kwargs.get("det_box_type", "quad")
-        self.save_crop_res = kwargs.get("save_crop_res", False)
-        self.crop_res_save_dir = kwargs.get("crop_res_save_dir", "./output")
-        self.crop_image_res_index = 0
+            self.text_classifier = TextClassifier(self.args)
 
-    def __call__(self, input_img, cls=True):
+    def __call__(self, img: np.ndarray) -> (list[np.ndarray], list[tuple], dict):
         time_dict = {'det': 0, 'rec': 0, 'cls': 0, 'all': 0}
-        if input_img is None:
-            logger.debug("no valid image provided")
-            return None, None, time_dict
+        ori_im = img.copy()
         start = time.time()
-        ori_im = input_img.copy()
-        dt_boxes, elapse = self.text_detector(input_img)  # 进入位置检测器
+        dt_boxes, elapse = self.text_detector(img)
         time_dict['det'] = elapse
         if dt_boxes is None:
-            logger.debug("no dt_boxes found, elapsed : {}".format(elapse))
+            # logger.debug("no dt_boxes found, elapsed : {}".format(elapse))
             end = time.time()
             time_dict['all'] = end - start
             return None, None, time_dict
         else:
-            logger.debug("dt_boxes num : {}, elapsed : {}".format(len(dt_boxes), elapse))
+            pass
+            # logger.debug("dt_boxes num : {}, elapsed : {}".format(len(dt_boxes), elapse))
         img_crop_list = []
-        dt_boxes = self.sorted_boxes(dt_boxes)
+        dt_boxes = sorted_boxes(dt_boxes)
         for bno in range(len(dt_boxes)):
             tmp_box = copy.deepcopy(dt_boxes[bno])
-            if self.det_box_type == "quad":
-                img_crop = get_rotate_crop_image(ori_im, tmp_box)
-            else:
-                img_crop = get_minarea_rect_crop(ori_im, tmp_box)
+            img_crop = self.get_rotate_crop_image(ori_im, tmp_box)
             img_crop_list.append(img_crop)
-        if self.use_angle_cls and cls:
+        if self.use_angle_cls:
             img_crop_list, angle_list, elapse = self.text_classifier(img_crop_list)
             time_dict['cls'] = elapse
-            logger.debug("cls num  : {}, elapsed : {}".format(
-                len(img_crop_list), elapse))
-        rec_res, elapse = self.text_recognizer(img_crop_list)  # 进入文字识别器
+            # logger.debug("cls num  : {}, elapse : {}".format(len(img_crop_list), elapse))
+        rec_res, elapse = self.text_recognizer(img_crop_list)
         time_dict['rec'] = elapse
-        logger.debug("rec_res num  : {}, elapsed : {}".format(len(rec_res), elapse))
-        if self.save_crop_res:
-            self.draw_crop_rec_res(self.crop_res_save_dir, img_crop_list, rec_res)
+        # logger.debug("rec_res num  : {}, elapse : {}".format(len(rec_res), elapse))
         filter_boxes, filter_rec_res = [], []
-        for box, rec_result in zip(dt_boxes, rec_res):
-            text, score = rec_result
+        for box, rec_reuslt in zip(dt_boxes, rec_res):
+            text, score = rec_reuslt
             if score >= self.drop_score:
                 filter_boxes.append(box)
-                filter_rec_res.append(rec_result)
+                filter_rec_res.append(rec_reuslt)
         end = time.time()
         time_dict['all'] = end - start
         return filter_boxes, filter_rec_res, time_dict
 
     @staticmethod
-    def sorted_boxes(dt_boxes):
+    def get_rotate_crop_image(img, points):
         """
-        Sort text boxes in order from top to bottom, left to right
-        args:
-            dt_boxes(array):detected text boxes with shape [4, 2]
-        return:
-            sorted boxes(array) with shape [4, 2]
+        img_height, img_width = img.shape[0:2]
+        left = int(np.min(points[:, 0]))
+        right = int(np.max(points[:, 0]))
+        top = int(np.min(points[:, 1]))
+        bottom = int(np.max(points[:, 1]))
+        img_crop = img[top:bottom, left:right, :].copy()
+        points[:, 0] = points[:, 0] - left
+        points[:, 1] = points[:, 1] - top
         """
-        num_boxes = dt_boxes.shape[0]
-        sorted_boxes = sorted(dt_boxes, key=lambda x: (x[0][1], x[0][0]))
-        _boxes = list(sorted_boxes)
-        for i in range(num_boxes - 1):
-            for j in range(i, -1, -1):
-                if abs(_boxes[j + 1][0][1] - _boxes[j][0][1]) < 10 and \
-                        (_boxes[j + 1][0][0] < _boxes[j][0][0]):
-                    tmp = _boxes[j]
-                    _boxes[j] = _boxes[j + 1]
-                    _boxes[j + 1] = tmp
-                else:
-                    break
-        return _boxes
-
-    def draw_crop_rec_res(self, output_dir, img_crop_list, rec_res):
-        os.makedirs(output_dir, exist_ok=True)
-        bbox_num = len(img_crop_list)
-        for bno in range(bbox_num):
-            cv2.imwrite(
-                os.path.join(output_dir,
-                             f"mg_crop_{bno + self.crop_image_res_index}.jpg"),
-                img_crop_list[bno])
-            logger.debug(f"{bno}, {rec_res[bno]}")
-        self.crop_image_res_index += bbox_num
+        img_crop_width = int(
+            max(
+                np.linalg.norm(points[0] - points[1]),
+                np.linalg.norm(points[2] - points[3])))
+        img_crop_height = int(
+            max(
+                np.linalg.norm(points[0] - points[3]),
+                np.linalg.norm(points[1] - points[2])))
+        pts_std = np.float32([[0, 0], [img_crop_width, 0],
+                              [img_crop_width, img_crop_height],
+                              [0, img_crop_height]])
+        M = cv2.getPerspectiveTransform(points, pts_std)
+        dst_img = cv2.warpPerspective(
+            img,
+            M, (img_crop_width, img_crop_height),
+            borderMode=cv2.BORDER_REPLICATE,
+            flags=cv2.INTER_CUBIC)
+        dst_img_height, dst_img_width = dst_img.shape[0:2]
+        if dst_img_height * 1.0 / dst_img_width >= 1.5:
+            dst_img = np.rot90(dst_img)
+        return dst_img
+
+
+def sorted_boxes(dt_boxes):
+    """
+    Sort text boxes in order from top to bottom, left to right
+    args:
+        dt_boxes(array):detected text boxes with shape [4, 2]
+    return:
+        sorted boxes(array) with shape [4, 2]
+    """
+    num_boxes = dt_boxes.shape[0]
+    _sorted_boxes = sorted(dt_boxes, key=lambda x: (x[0][1], x[0][0]))
+    _boxes = list(_sorted_boxes)
+
+    for i in range(num_boxes - 1):
+        if abs(_boxes[i + 1][0][1] - _boxes[i][0][1]) < 10 and \
+                (_boxes[i + 1][0][0] < _boxes[i][0][0]):
+            tmp = _boxes[i]
+            _boxes[i] = _boxes[i + 1]
+            _boxes[i + 1] = tmp
+    return _boxes
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/__init__.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,25 @@
-from .make_border_map import MakeBorderMap
-from .make_shrink_map import MakeShrinkMap
-from .random_crop_data import EastRandomCropData, RandomCropImgMask
-from .make_pse_gt import MakePseGt
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
+
+# from .iaa_augment import IaaAugment
+# from .make_border_map import MakeBorderMap
+# from .make_shrink_map import MakeShrinkMap
+# from .random_crop_data import EastRandomCropData, PSERandomCrop
 
-
-
-from .rec_img_aug import BaseDataAugmentation, RecAug, RecConAug, RecResizeImg, ClsResizeImg, \
-    SRNRecResizeImg, GrayRecResizeImg, SARRecResizeImg, PRENResizeImg, \
-    ABINetRecResizeImg, SVTRRecResizeImg, ABINetRecAug, VLRecResizeImg, SPINRecResizeImg, RobustScannerRecResizeImg, \
-    RFLRecResizeImg, SVTRRecAug
-from .ssl_img_aug import SSLRotateResize
-from .randaugment import RandAugment
-from .ColorJitter import ColorJitter
+# from .rec_img_aug import RecAug, RecResizeImg, ClsResizeImg
+# from .randaugment import RandAugment
 from .operators import *
-from .label_ops import *
-
-from .east_process import *
-from .sast_process import *
-from .pg_process import *
-from .table_ops import *
-
-
-from .fce_aug import *
-from .fce_targets import FCENetTargets
-from .ct_process import *
-from .drrg_targets import DRRGTargets
+# from .label_ops import *
 
+# from .east_process import *
+# from .sast_process import *
+from .gen_table_mask import *
 
 def transform(data, ops=None):
     """ transform """
     if ops is None:
         ops = []
     for op in ops:
         data = op(data)
@@ -37,23 +27,22 @@
             return None
     return data
 
 
 def create_operators(op_param_list, global_config=None):
     """
     create operators based on the config
-
     Args:
         params(list): a dict list, used to create some operators
     """
     assert isinstance(op_param_list, list), ('operator config should be a list')
     ops = []
     for operator in op_param_list:
         assert isinstance(operator,
                           dict) and len(operator) == 1, "yaml format error"
         op_name = list(operator)[0]
         param = {} if operator[op_name] is None else operator[op_name]
         if global_config is not None:
             param.update(global_config)
         op = eval(op_name)(**param)
         ops.append(op)
-    return ops
+    return ops
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/operators.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/operators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,51 @@
+"""
+# Copyright (c) 2020 PaddlePaddle Authors. All Rights Reserved
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+"""
+
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
+
 import sys
 import six
 import cv2
 import numpy as np
-import math
-from PIL import Image
 
 
 class DecodeImage(object):
     """ decode image """
 
-    def __init__(self,
-                 img_mode='RGB',
-                 channel_first=False,
-                 ignore_orientation=False,
-                 **kwargs):
+    def __init__(self, img_mode='RGB', channel_first=False, **kwargs):
         self.img_mode = img_mode
         self.channel_first = channel_first
-        self.ignore_orientation = ignore_orientation
 
     def __call__(self, data):
         img = data['image']
         if six.PY2:
             assert type(img) is str and len(
                 img) > 0, "invalid input 'img' in DecodeImage"
         else:
             assert type(img) is bytes and len(
                 img) > 0, "invalid input 'img' in DecodeImage"
         img = np.frombuffer(img, dtype='uint8')
-        if self.ignore_orientation:
-            img = cv2.imdecode(img, cv2.IMREAD_IGNORE_ORIENTATION |
-                               cv2.IMREAD_COLOR)
-        else:
-            img = cv2.imdecode(img, 1)
+        img = cv2.imdecode(img, 1)
         if img is None:
             return None
         if self.img_mode == 'GRAY':
             img = cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
         elif self.img_mode == 'RGB':
             assert img.shape[2] == 3, 'invalid shape of image[%s]' % (img.shape)
             img = img[:, :, ::-1]
@@ -43,14 +53,47 @@
         if self.channel_first:
             img = img.transpose((2, 0, 1))
 
         data['image'] = img
         return data
 
 
+class NRTRDecodeImage(object):
+    """ decode image """
+
+    def __init__(self, img_mode='RGB', channel_first=False, **kwargs):
+        self.img_mode = img_mode
+        self.channel_first = channel_first
+
+    def __call__(self, data):
+        img = data['image']
+        if six.PY2:
+            assert type(img) is str and len(
+                img) > 0, "invalid input 'img' in DecodeImage"
+        else:
+            assert type(img) is bytes and len(
+                img) > 0, "invalid input 'img' in DecodeImage"
+        img = np.frombuffer(img, dtype='uint8')
+
+        img = cv2.imdecode(img, 1)
+
+        if img is None:
+            return None
+        if self.img_mode == 'GRAY':
+            img = cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
+        elif self.img_mode == 'RGB':
+            assert img.shape[2] == 3, 'invalid shape of image[%s]' % (img.shape)
+            img = img[:, :, ::-1]
+        img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+        if self.channel_first:
+            img = img.transpose((2, 0, 1))
+        data['image'] = img
+        return data
+
+
 class NormalizeImage(object):
     """ normalize image such as substract mean, divide std
     """
 
     def __init__(self, scale=None, mean=None, std=None, order='chw', **kwargs):
         if isinstance(scale, str):
             scale = eval(scale)
@@ -109,133 +152,78 @@
     def __call__(self, data):
         data_list = []
         for key in self.keep_keys:
             data_list.append(data[key])
         return data_list
 
 
-class Pad(object):
-    def __init__(self, size=None, size_div=32, **kwargs):
-        if size is not None and not isinstance(size, (int, list, tuple)):
-            raise TypeError("Type of target_size is invalid. Now is {}".format(
-                type(size)))
-        if isinstance(size, int):
-            size = [size, size]
-        self.size = size
-        self.size_div = size_div
-
-    def __call__(self, data):
-
-        img = data['image']
-        img_h, img_w = img.shape[0], img.shape[1]
-        if self.size:
-            resize_h2, resize_w2 = self.size
-            assert (
-                img_h < resize_h2 and img_w < resize_w2
-            ), '(h, w) of target size should be greater than (img_h, img_w)'
-        else:
-            resize_h2 = max(
-                int(math.ceil(img.shape[0] / self.size_div) * self.size_div),
-                self.size_div)
-            resize_w2 = max(
-                int(math.ceil(img.shape[1] / self.size_div) * self.size_div),
-                self.size_div)
-        img = cv2.copyMakeBorder(
-            img,
-            0,
-            resize_h2 - img_h,
-            0,
-            resize_w2 - img_w,
-            cv2.BORDER_CONSTANT,
-            value=0)
-        data['image'] = img
-        return data
-
-
 class Resize(object):
     def __init__(self, size=(640, 640), **kwargs):
         self.size = size
 
     def resize_image(self, img):
         resize_h, resize_w = self.size
         ori_h, ori_w = img.shape[:2]  # (h, w, c)
         ratio_h = float(resize_h) / ori_h
         ratio_w = float(resize_w) / ori_w
         img = cv2.resize(img, (int(resize_w), int(resize_h)))
         return img, [ratio_h, ratio_w]
 
     def __call__(self, data):
         img = data['image']
-        if 'polys' in data:
-            text_polys = data['polys']
+        text_polys = data['polys']
 
         img_resize, [ratio_h, ratio_w] = self.resize_image(img)
-        if 'polys' in data:
-            new_boxes = []
-            for box in text_polys:
-                new_box = []
-                for cord in box:
-                    new_box.append([cord[0] * ratio_w, cord[1] * ratio_h])
-                new_boxes.append(new_box)
-            data['polys'] = np.array(new_boxes, dtype=np.float32)
+        new_boxes = []
+        for box in text_polys:
+            new_box = []
+            for cord in box:
+                new_box.append([cord[0] * ratio_w, cord[1] * ratio_h])
+            new_boxes.append(new_box)
         data['image'] = img_resize
+        data['polys'] = np.array(new_boxes, dtype=np.float32)
         return data
 
 
 class DetResizeForTest(object):
     def __init__(self, **kwargs):
         super(DetResizeForTest, self).__init__()
         self.resize_type = 0
-        self.keep_ratio = False
         if 'image_shape' in kwargs:
             self.image_shape = kwargs['image_shape']
             self.resize_type = 1
-            if 'keep_ratio' in kwargs:
-                self.keep_ratio = kwargs['keep_ratio']
         elif 'limit_side_len' in kwargs:
             self.limit_side_len = kwargs['limit_side_len']
             self.limit_type = kwargs.get('limit_type', 'min')
         elif 'resize_long' in kwargs:
             self.resize_type = 2
             self.resize_long = kwargs.get('resize_long', 960)
         else:
             self.limit_side_len = 736
             self.limit_type = 'min'
 
     def __call__(self, data):
         img = data['image']
         src_h, src_w, _ = img.shape
-        if sum([src_h, src_w]) < 64:
-            img = self.image_padding(img)
 
         if self.resize_type == 0:
             # img, shape = self.resize_image_type0(img)
             img, [ratio_h, ratio_w] = self.resize_image_type0(img)
         elif self.resize_type == 2:
             img, [ratio_h, ratio_w] = self.resize_image_type2(img)
         else:
             # img, shape = self.resize_image_type1(img)
             img, [ratio_h, ratio_w] = self.resize_image_type1(img)
         data['image'] = img
         data['shape'] = np.array([src_h, src_w, ratio_h, ratio_w])
         return data
 
-    def image_padding(self, im, value=0):
-        h, w, c = im.shape
-        im_pad = np.zeros((max(32, h), max(32, w), c), np.uint8) + value
-        im_pad[:h, :w, :] = im
-        return im_pad
-
     def resize_image_type1(self, img):
         resize_h, resize_w = self.image_shape
         ori_h, ori_w = img.shape[:2]  # (h, w, c)
-        if self.keep_ratio is True:
-            resize_w = ori_w * resize_h / ori_h
-            N = math.ceil(resize_w / 32)
-            resize_w = N * 32
         ratio_h = float(resize_h) / ori_h
         ratio_w = float(resize_w) / ori_w
         img = cv2.resize(img, (int(resize_w), int(resize_h)))
         # return img, np.array([ori_h, ori_w])
         return img, [ratio_h, ratio_w]
 
     def resize_image_type0(self, img):
@@ -424,80 +412,7 @@
 
     def resize_boxes(self, im, points, scale_factor):
         points = points * scale_factor
         img_shape = im.shape[:2]
         points[:, 0::2] = np.clip(points[:, 0::2], 0, img_shape[1])
         points[:, 1::2] = np.clip(points[:, 1::2], 0, img_shape[0])
         return points
-
-
-class SRResize(object):
-    def __init__(self,
-                 imgH=32,
-                 imgW=128,
-                 down_sample_scale=4,
-                 keep_ratio=False,
-                 min_ratio=1,
-                 mask=False,
-                 infer_mode=False,
-                 **kwargs):
-        self.imgH = imgH
-        self.imgW = imgW
-        self.keep_ratio = keep_ratio
-        self.min_ratio = min_ratio
-        self.down_sample_scale = down_sample_scale
-        self.mask = mask
-        self.infer_mode = infer_mode
-
-    def __call__(self, data):
-        imgH = self.imgH
-        imgW = self.imgW
-        images_lr = data["image_lr"]
-        transform2 = ResizeNormalize(
-            (imgW // self.down_sample_scale, imgH // self.down_sample_scale))
-        images_lr = transform2(images_lr)
-        data["img_lr"] = images_lr
-        if self.infer_mode:
-            return data
-
-        images_HR = data["image_hr"]
-        label_strs = data["label"]
-        transform = ResizeNormalize((imgW, imgH))
-        images_HR = transform(images_HR)
-        data["img_hr"] = images_HR
-        return data
-
-
-class ResizeNormalize(object):
-    def __init__(self, size, interpolation=Image.BICUBIC):
-        self.size = size
-        self.interpolation = interpolation
-
-    def __call__(self, img):
-        img = img.resize(self.size, self.interpolation)
-        img_numpy = np.array(img).astype("float32")
-        img_numpy = img_numpy.transpose((2, 0, 1)) / 255
-        return img_numpy
-
-
-class GrayImageChannelFormat(object):
-    """
-    format gray scale image's channel: (3,h,w) -> (1,h,w)
-    Args:
-        inverse: inverse gray image 
-    """
-
-    def __init__(self, inverse=False, **kwargs):
-        self.inverse = inverse
-
-    def __call__(self, data):
-        img = data['image']
-        img_single_channel = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
-        img_expanded = np.expand_dims(img_single_channel, 0)
-
-        if self.inverse:
-            data['image'] = np.abs(img_expanded - 1)
-        else:
-            data['image'] = img_expanded
-
-        data['src_image'] = img
-        return data
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/data/imaug/table_ops.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/gen_table_mask.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+"""
+# Copyright (c) 2020 PaddlePaddle Authors. All Rights Reserved
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+"""
+
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+from __future__ import unicode_literals
+
+import sys
+import six
 import cv2
 import numpy as np
 
 
 class GenTableMask(object):
     """ gen table mask """
 
@@ -21,20 +44,18 @@
                     project_val_array[j] += 1
         # 根据数组，获取切割点
         start_idx = 0  # 记录进入字符区的索引
         end_idx = 0  # 记录进入空白区域的索引
         in_text = False  # 是否遍历到了字符区内
         box_list = []
         for i in range(len(project_val_array)):
-            if in_text == False and project_val_array[
-                    i] > spilt_threshold:  # 进入字符区了
+            if in_text == False and project_val_array[i] > spilt_threshold:  # 进入字符区了
                 in_text = True
                 start_idx = i
-            elif project_val_array[
-                    i] <= spilt_threshold and in_text == True:  # 进入空白区了
+            elif project_val_array[i] <= spilt_threshold and in_text == True:  # 进入空白区了
                 end_idx = i
                 in_text = False
                 if end_idx - start_idx <= 2:
                     continue
                 box_list.append((start_idx, end_idx + 1))
 
         if in_text:
@@ -45,16 +66,15 @@
                 projection_map[j, i] = 0
         return box_list, projection_map
 
     def projection_cx(self, box_img):
         box_gray_img = cv2.cvtColor(box_img, cv2.COLOR_BGR2GRAY)
         h, w = box_gray_img.shape
         # 灰度图片进行二值化处理
-        ret, thresh1 = cv2.threshold(box_gray_img, 200, 255,
-                                     cv2.THRESH_BINARY_INV)
+        ret, thresh1 = cv2.threshold(box_gray_img, 200, 255, cv2.THRESH_BINARY_INV)
         # 纵向腐蚀
         if h < w:
             kernel = np.ones((2, 1), np.uint8)
             erode = cv2.erode(thresh1, kernel, iterations=1)
         else:
             erode = thresh1
         # 水平膨胀
@@ -71,20 +91,18 @@
         # 根据数组，获取切割点
         start_idx = 0  # 记录进入字符区的索引
         end_idx = 0  # 记录进入空白区域的索引
         in_text = False  # 是否遍历到了字符区内
         box_list = []
         spilt_threshold = 0
         for i in range(len(project_val_array)):
-            if in_text == False and project_val_array[
-                    i] > spilt_threshold:  # 进入字符区了
+            if in_text == False and project_val_array[i] > spilt_threshold:  # 进入字符区了
                 in_text = True
                 start_idx = i
-            elif project_val_array[
-                    i] <= spilt_threshold and in_text == True:  # 进入空白区了
+            elif project_val_array[i] <= spilt_threshold and in_text == True:  # 进入空白区了
                 end_idx = i
                 in_text = False
                 if end_idx - start_idx <= 2:
                     continue
                 box_list.append((start_idx, end_idx + 1))
 
         if in_text:
@@ -98,16 +116,15 @@
             for i, (h_start, h_end) in enumerate(box_list):
                 if i == 0:
                     h_start = 0
                 if i == len(box_list):
                     h_end = h
                 word_img = erosion[h_start:h_end + 1, :]
                 word_h, word_w = word_img.shape
-                w_split_list, w_projection_map = self.projection(word_img.T,
-                                                                 word_w, word_h)
+                w_split_list, w_projection_map = self.projection(word_img.T, word_w, word_h)
                 w_start, w_end = w_split_list[0][0], w_split_list[-1][1]
                 if h_start > 0:
                     h_start -= 1
                 h_end += 1
                 word_img = box_img[h_start:h_end + 1:, w_start:w_end + 1, :]
                 split_bbox_list.append([w_start, h_start, w_end, h_end])
         else:
@@ -149,58 +166,80 @@
                     split_bbox_list[sno][0] += left
                     split_bbox_list[sno][1] += top
                     split_bbox_list[sno][2] += left
                     split_bbox_list[sno][3] += top
 
                 for sno in range(len(split_bbox_list)):
                     left, top, right, bottom = split_bbox_list[sno]
-                    left, top, right, bottom = self.shrink_bbox(
-                        [left, top, right, bottom])
+                    left, top, right, bottom = self.shrink_bbox([left, top, right, bottom])
                     if self.mask_type == 1:
                         mask_img[top:bottom, left:right] = 1.0
                         data['mask_img'] = mask_img
                     else:
                         mask_img[top:bottom, left:right, :] = (255, 255, 255)
                         data['image'] = mask_img
         return data
 
 
 class ResizeTableImage(object):
-    def __init__(self, max_len, resize_bboxes=False, infer_mode=False,
-                 **kwargs):
+    def __init__(self, max_len, **kwargs):
         super(ResizeTableImage, self).__init__()
         self.max_len = max_len
-        self.resize_bboxes = resize_bboxes
-        self.infer_mode = infer_mode
 
-    def __call__(self, data):
-        img = data['image']
+    def get_img_bbox(self, cells):
+        bbox_list = []
+        if len(cells) == 0:
+            return bbox_list
+        cell_num = len(cells)
+        for cno in range(cell_num):
+            if "bbox" in cells[cno]:
+                bbox = cells[cno]['bbox']
+                bbox_list.append(bbox)
+        return bbox_list
+
+    def resize_img_table(self, img, bbox_list, max_len):
         height, width = img.shape[0:2]
-        ratio = self.max_len / (max(height, width) * 1.0)
+        ratio = max_len / (max(height, width) * 1.0)
         resize_h = int(height * ratio)
         resize_w = int(width * ratio)
-        resize_img = cv2.resize(img, (resize_w, resize_h))
-        if self.resize_bboxes and not self.infer_mode:
-            data['bboxes'] = data['bboxes'] * ratio
-        data['image'] = resize_img
-        data['src_img'] = img
-        data['shape'] = np.array([height, width, ratio, ratio])
+        img_new = cv2.resize(img, (resize_w, resize_h))
+        bbox_list_new = []
+        for bno in range(len(bbox_list)):
+            left, top, right, bottom = bbox_list[bno].copy()
+            left = int(left * ratio)
+            top = int(top * ratio)
+            right = int(right * ratio)
+            bottom = int(bottom * ratio)
+            bbox_list_new.append([left, top, right, bottom])
+        return img_new, bbox_list_new
+
+    def __call__(self, data):
+        img = data['image']
+        if 'cells' not in data:
+            cells = []
+        else:
+            cells = data['cells']
+        bbox_list = self.get_img_bbox(cells)
+        img_new, bbox_list_new = self.resize_img_table(img, bbox_list, self.max_len)
+        data['image'] = img_new
+        cell_num = len(cells)
+        bno = 0
+        for cno in range(cell_num):
+            if "bbox" in data['cells'][cno]:
+                data['cells'][cno]['bbox'] = bbox_list_new[bno]
+                bno += 1
         data['max_len'] = self.max_len
         return data
 
 
 class PaddingTableImage(object):
-    def __init__(self, size, **kwargs):
+    def __init__(self, **kwargs):
         super(PaddingTableImage, self).__init__()
-        self.size = size
 
     def __call__(self, data):
         img = data['image']
-        pad_h, pad_w = self.size
-        padding_img = np.zeros((pad_h, pad_w, 3), dtype=np.float32)
+        max_len = data['max_len']
+        padding_img = np.zeros((max_len, max_len, 3), dtype=np.float32)
         height, width = img.shape[0:2]
         padding_img[0:height, 0:width, :] = img.copy()
         data['image'] = padding_img
-        shape = data['shape'].tolist()
-        shape.extend([pad_h, pad_w])
-        data['shape'] = np.array(shape)
-        return data
+        return data
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/det_mobilenet_v3.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_mobilenet_v3.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+import os, sys
+import torch
 import torch.nn as nn
+import torch.nn.functional as F
 from ...modeling.common import Activation
 
 def make_divisible(v, divisor=8, min_value=None):
     if min_value is None:
         min_value = divisor
     new_v = max(min_value, int(v + divisor / 2) // divisor * divisor)
     if new_v < 0.9 * v:
@@ -15,15 +18,16 @@
                  in_channels,
                  out_channels,
                  kernel_size,
                  stride,
                  padding,
                  groups=1,
                  if_act=True,
-                 act=None):
+                 act=None,
+                 name=None):
         super(ConvBNLayer, self).__init__()
         self.if_act = if_act
         self.conv = nn.Conv2d(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=kernel_size,
             stride=stride,
@@ -93,34 +97,37 @@
         self.expand_conv = ConvBNLayer(
             in_channels=in_channels,
             out_channels=mid_channels,
             kernel_size=1,
             stride=1,
             padding=0,
             if_act=True,
-            act=act)
+            act=act,
+            name=name + "_expand")
         self.bottleneck_conv = ConvBNLayer(
             in_channels=mid_channels,
             out_channels=mid_channels,
             kernel_size=kernel_size,
             stride=stride,
             padding=int((kernel_size - 1) // 2),
             groups=mid_channels,
             if_act=True,
-            act=act)
+            act=act,
+            name=name + "_depthwise")
         if self.if_se:
             self.mid_se = SEModule(mid_channels, name=name + "_se")
         self.linear_conv = ConvBNLayer(
             in_channels=mid_channels,
             out_channels=out_channels,
             kernel_size=1,
             stride=1,
             padding=0,
             if_act=False,
-            act=None)
+            act=None,
+            name=name + "_linear")
 
     def forward(self, inputs):
         x = self.expand_conv(inputs)
         x = self.bottleneck_conv(x)
         if self.if_se:
             x = self.mid_se(x)
         x = self.linear_conv(x)
@@ -194,15 +201,16 @@
             in_channels=in_channels,
             out_channels=make_divisible(inplanes * scale),
             kernel_size=3,
             stride=2,
             padding=1,
             groups=1,
             if_act=True,
-            act='hard_swish')
+            act='hard_swish',
+            name='conv1')
 
         self.stages = nn.ModuleList()
         self.out_channels = []
         block_list = []
         i = 0
         inplanes = make_divisible(inplanes * scale)
         for (k, exp, c, se, nl, s) in cfg:
@@ -228,15 +236,16 @@
                 in_channels=inplanes,
                 out_channels=make_divisible(scale * cls_ch_squeeze),
                 kernel_size=1,
                 stride=1,
                 padding=0,
                 groups=1,
                 if_act=True,
-                act='hard_swish'))
+                act='hard_swish',
+                name='conv_last'))
         self.stages.append(nn.Sequential(*block_list))
         self.out_channels.append(make_divisible(scale * cls_ch_squeeze))
         # for i, stage in enumerate(self.stages):
         #     self.add_sublayer(sublayer=stage, name="stage{}".format(i))
 
     def forward(self, x):
         x = self.conv(x)
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/det_resnet_vd.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_resnet_vd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,32 @@
+
+
+import os, sys
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ..common import Activation
+from ...modeling.common import Activation
 import torchvision
 
 class DeformableConvV2(nn.Module):
     def __init__(self,
                  in_channels,
                  out_channels,
                  kernel_size,
                  stride=1,
+                 padding=0,
                  dilation=1,
                  groups=1,
+                 weight_attr=None,
                  bias_attr=None,
-                 skip_quant=False):
+                 lr_scale=1,
+                 regularizer=None,
+                 skip_quant=False,
+                 dcn_bias_regularizer=None,
+                 dcn_bias_lr_scale=2.):
         super(DeformableConvV2, self).__init__()
         self.offset_channel = 2 * kernel_size**2 * groups
         self.mask_channel = kernel_size**2 * groups
 
         if bias_attr:
             # in FCOS-DCN head, specifically need learning_rate and regularizer
             dcn_bias_attr = True
@@ -60,22 +69,23 @@
                  out_channels,
                  kernel_size,
                  stride=1,
                  groups=1,
                  dcn_groups=1,
                  is_vd_mode=False,
                  act=None,
+                 name=None,
                  is_dcn=False,
                  ):
         super(ConvBNLayer, self).__init__()
 
         self.is_vd_mode = is_vd_mode
         self.act = act
         self._pool2d_avg = nn.AvgPool2d(
-            kernel_size=2, stride=2, padding=0, ceil_mode=False)
+            kernel_size=2, stride=2, padding=0, ceil_mode=True)
         if not is_dcn:
             self._conv = nn.Conv2d(
                 in_channels=in_channels,
                 out_channels=out_channels,
                 kernel_size=kernel_size,
                 stride=stride,
                 padding=(kernel_size - 1) // 2,
@@ -83,14 +93,15 @@
                 bias=False)
         else:
             self._conv = DeformableConvV2(
                 in_channels=in_channels,
                 out_channels=out_channels,
                 kernel_size=kernel_size,
                 stride=stride,
+                padding=(kernel_size - 1) // 2,
                 groups=dcn_groups,
                 bias_attr=False)
 
         self._batch_norm = nn.BatchNorm2d(
             out_channels,
             track_running_stats=True,
             )
@@ -112,45 +123,50 @@
 class BottleneckBlock(nn.Module):
     def __init__(self,
                  in_channels,
                  out_channels,
                  stride,
                  shortcut=True,
                  if_first=False,
+                 name=None,
                  is_dcn=False,
                  ):
         super(BottleneckBlock, self).__init__()
 
         self.conv0 = ConvBNLayer(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=1,
-            act='relu')
+            act='relu',
+            name=name + "_branch2a")
         self.conv1 = ConvBNLayer(
             in_channels=out_channels,
             out_channels=out_channels,
             kernel_size=3,
             stride=stride,
             act='relu',
+            name=name + "_branch2b",
             is_dcn=is_dcn,
             dcn_groups=2,
         )
         self.conv2 = ConvBNLayer(
             in_channels=out_channels,
             out_channels=out_channels * 4,
             kernel_size=1,
-            act=None)
+            act=None,
+            name=name + "_branch2c")
 
         if not shortcut:
             self.short = ConvBNLayer(
                 in_channels=in_channels,
                 out_channels=out_channels * 4,
                 kernel_size=1,
                 stride=1,
-                is_vd_mode=False if if_first else True)
+                is_vd_mode=False if if_first else True,
+                name=name + "_branch1")
 
         self.shortcut = shortcut
 
     def forward(self, inputs):
         y = self.conv0(inputs)
         conv1 = self.conv1(y)
         conv2 = self.conv2(conv1)
@@ -166,36 +182,40 @@
 
 class BasicBlock(nn.Module):
     def __init__(self,
                  in_channels,
                  out_channels,
                  stride,
                  shortcut=True,
-                 if_first=False):
+                 if_first=False,
+                 name=None):
         super(BasicBlock, self).__init__()
         self.stride = stride
         self.conv0 = ConvBNLayer(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=3,
             stride=stride,
-            act='relu')
+            act='relu',
+            name=name + "_branch2a")
         self.conv1 = ConvBNLayer(
             in_channels=out_channels,
             out_channels=out_channels,
             kernel_size=3,
-            act=None)
+            act=None,
+            name=name + "_branch2b")
 
         if not shortcut:
             self.short = ConvBNLayer(
                 in_channels=in_channels,
                 out_channels=out_channels,
                 kernel_size=1,
                 stride=1,
-                is_vd_mode=False if if_first else True)
+                is_vd_mode=False if if_first else True,
+                name=name + "_branch1")
 
         self.shortcut = shortcut
 
     def forward(self, inputs):
         y = self.conv0(inputs)
         conv1 = self.conv1(y)
 
@@ -245,70 +265,90 @@
         ]
 
         self.conv1_1 = ConvBNLayer(
             in_channels=in_channels,
             out_channels=32,
             kernel_size=3,
             stride=2,
-            act='relu')
+            act='relu',
+            name="conv1_1")
         self.conv1_2 = ConvBNLayer(
             in_channels=32,
             out_channels=32,
             kernel_size=3,
             stride=1,
-            act='relu')
+            act='relu',
+            name="conv1_2")
         self.conv1_3 = ConvBNLayer(
             in_channels=32,
             out_channels=64,
             kernel_size=3,
             stride=1,
-            act='relu')
+            act='relu',
+            name="conv1_3")
         self.pool2d_max = nn.MaxPool2d(kernel_size=3, stride=2, padding=1)
 
         self.stages = nn.ModuleList()
         self.out_channels = []
         if layers >= 50:
             for block in range(len(depth)):
-                block_list = []
+                # block_list = []
+                block_list = nn.Sequential()
                 shortcut = False
                 is_dcn = self.dcn_stage[block]
                 for i in range(depth[block]):
+                    if layers in [101, 152] and block == 2:
+                        if i == 0:
+                            conv_name = "res" + str(block + 2) + "a"
+                        else:
+                            conv_name = "res" + str(block + 2) + "b" + str(i)
+                    else:
+                        conv_name = "res" + str(block + 2) + chr(97 + i)
                     bottleneck_block = BottleneckBlock(
                             in_channels=num_channels[block]
                             if i == 0 else num_filters[block] * 4,
                             out_channels=num_filters[block],
                             stride=2 if i == 0 and block != 0 else 1,
                             shortcut=shortcut,
                             if_first=block == i == 0,
+                            name=conv_name,
                             is_dcn=is_dcn,
                     )
 
                     shortcut = True
-                    block_list.append(bottleneck_block)
+                    block_list.add_module('bb_%d_%d' % (block, i), bottleneck_block)
                 if block in self.out_indices:
                     self.out_channels.append(num_filters[block] * 4)
-                self.stages.append(nn.Sequential(*block_list))
+                # self.stages.append(nn.Sequential(*block_list))
+                self.stages.append(block_list)
         else:
             for block in range(len(depth)):
-                block_list = []
+                # block_list = []
+                block_list = nn.Sequential()
                 shortcut = False
+                # is_dcn = self.dcn_stage[block]
                 for i in range(depth[block]):
+                    conv_name = "res" + str(block + 2) + chr(97 + i)
                     basic_block = BasicBlock(
                             in_channels=num_channels[block]
                             if i == 0 else num_filters[block],
                             out_channels=num_filters[block],
                             stride=2 if i == 0 and block != 0 else 1,
                             shortcut=shortcut,
-                            if_first=block == i == 0)
+                            if_first=block == i == 0,
+                            name=conv_name)
 
                     shortcut = True
-                    block_list.append(basic_block)
+                    block_list.add_module('bb_%d_%d' % (block, i), basic_block)
+                    # block_list.append(basic_block)
                 if block in self.out_indices:
                     self.out_channels.append(num_filters[block])
-                self.stages.append(nn.Sequential(*block_list))
+                self.stages.append(block_list)
+
+                # self.stages.append(nn.Sequential(*block_list))
 
 
     def forward(self, inputs):
         y = self.conv1_1(inputs)
         y = self.conv1_2(y)
         y = self.conv1_3(y)
         y = self.pool2d_max(y)
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_hgnet.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_hgnet.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_lcnetv3.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_lcnetv3_bak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ..common import Activation
+from ...modeling.common import Activation
 
 NET_CONFIG_det = {
     "blocks2":
     # k, in_c, out_c, s, use_se
         [[3, 16, 32, 1, False]],
     "blocks3": [[3, 32, 64, 2, False], [3, 64, 64, 1, False]],
     "blocks4": [[3, 64, 128, 2, False], [3, 128, 128, 1, False]],
@@ -102,15 +102,14 @@
         self.groups = groups
         self.stride = stride
         self.kernel_size = kernel_size
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.num_conv_branches = num_conv_branches
         self.padding = (kernel_size - 1) // 2
-
         self.identity = nn.BatchNorm2d(in_channels) if out_channels == in_channels and stride == 1 else None
 
         self.conv_kxk = nn.ModuleList([
             ConvBNLayer(
                 in_channels,
                 out_channels,
                 kernel_size,
@@ -122,15 +121,14 @@
         self.conv_1x1 = ConvBNLayer(
             in_channels,
             out_channels,
             1,
             stride,
             groups=groups,
             lr_mult=lr_mult) if kernel_size > 1 else None
-
         self.lab = LearnableAffineBlock(lr_mult=lr_mult, lab_lr=lab_lr)
         self.act = Act(lr_mult=lr_mult, lab_lr=lab_lr)
 
     def forward(self, x):
         # for export
         if self.is_repped:
             out = self.lab(self.reparam_conv(x))
@@ -423,14 +421,16 @@
         x = self.blocks2(x)
         x = self.blocks3(x)
         out_list.append(x)
         x = self.blocks4(x)
         out_list.append(x)
         x = self.blocks5(x)
         out_list.append(x)
+        import numpy as np
+        x = torch.Tensor(np.load('../PaddleOCR4debug/tmp.npy'))
         x = self.blocks6(x)
         out_list.append(x)
 
         if self.det:
             out_list[0] = self.layer_list[0](out_list[0])
             out_list[1] = self.layer_list[1](out_list[1])
             out_list[2] = self.layer_list[2](out_list[2])
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_mobilenet_v3.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_mobilenet_v3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+import os, sys
+import torch
 import torch.nn as nn
+import torch.nn.functional as F
+from ...modeling.common import Activation
 
 from .det_mobilenet_v3 import ResidualUnit, ConvBNLayer, make_divisible
 
 class MobileNetV3(nn.Module):
     def __init__(self,
                  in_channels=3,
                  model_name='small',
@@ -75,15 +79,16 @@
             in_channels=in_channels,
             out_channels=make_divisible(inplanes * scale),
             kernel_size=3,
             stride=2,
             padding=1,
             groups=1,
             if_act=True,
-            act='hard_swish')
+            act='hard_swish',
+            name='conv1')
         i = 0
         block_list = []
         inplanes = make_divisible(inplanes * scale)
         for (k, exp, c, se, nl, s) in cfg:
             block_list.append(
                 ResidualUnit(
                     in_channels=inplanes,
@@ -102,15 +107,16 @@
             in_channels=inplanes,
             out_channels=make_divisible(scale * cls_ch_squeeze),
             kernel_size=1,
             stride=1,
             padding=0,
             groups=1,
             if_act=True,
-            act='hard_swish')
+            act='hard_swish',
+            name='conv_last')
 
         self.pool = nn.MaxPool2d(kernel_size=2, stride=2, padding=0)
         self.out_channels = make_divisible(scale * cls_ch_squeeze)
 
     def forward(self, x):
         x = self.conv1(x)
         x = self.blocks(x)
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_mv1_enhance.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_mv1_enhance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+import os, sys
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ..common import Activation
+from ...modeling.common import Activation
 
 
 class ConvBNLayer(nn.Module):
     def __init__(self,
                  num_channels,
                  filter_size,
                  num_filters,
                  stride,
                  padding,
+                 channels=None,
                  num_groups=1,
                  act='hard_swish'):
         super(ConvBNLayer, self).__init__()
         self.act = act
         self._conv = nn.Conv2d(
             in_channels=num_channels,
             out_channels=num_filters,
@@ -46,34 +48,34 @@
                  num_groups,
                  stride,
                  scale,
                  dw_size=3,
                  padding=1,
                  use_se=False):
         super(DepthwiseSeparable, self).__init__()
+        self.use_se = use_se
         self._depthwise_conv = ConvBNLayer(
             num_channels=num_channels,
             num_filters=int(num_filters1 * scale),
             filter_size=dw_size,
             stride=stride,
             padding=padding,
             num_groups=int(num_groups * scale))
-        self._se = None
         if use_se:
             self._se = SEModule(int(num_filters1 * scale))
         self._pointwise_conv = ConvBNLayer(
             num_channels=int(num_filters1 * scale),
             filter_size=1,
             num_filters=int(num_filters2 * scale),
             stride=1,
             padding=0)
 
     def forward(self, inputs):
         y = self._depthwise_conv(inputs)
-        if self._se is not None:
+        if self.use_se:
             y = self._se(y)
         y = self._pointwise_conv(y)
         return y
 
 
 class MobileNetV1Enhance(nn.Module):
     def __init__(self,
@@ -85,14 +87,15 @@
         super().__init__()
         self.scale = scale
         self.block_list = []
 
         self.conv1 = ConvBNLayer(
             num_channels=in_channels,
             filter_size=3,
+            channels=3,
             num_filters=int(32 * scale),
             stride=2,
             padding=1)
 
         conv2_1 = DepthwiseSeparable(
             num_channels=int(32 * scale),
             num_filters1=32,
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_nrtr_mtb.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_nrtr_mtb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 import torch
 from torch import nn
 
 
 class MTB(nn.Module):
     def __init__(self, cnn_num, in_channels):
         super(MTB, self).__init__()
@@ -16,18 +17,20 @@
                         in_channels=in_channels
                         if i == 0 else 32 * (2**(i - 1)),
                         out_channels=32 * (2**i),
                         kernel_size=3,
                         stride=2,
                         padding=1))
                 self.block.add_module('relu_{}'.format(i), nn.ReLU())
-                self.block.add_module('bn_{}'.format(i), nn.BatchNorm2d(32 * (2**i)))
+                self.block.add_module('bn_{}'.format(i),
+                                        nn.BatchNorm2d(32 * (2**i)))
 
 
     def forward(self, images):
         x = self.block(images)
         if self.cnn_num == 2:
             # (b, w, h, c)
             x = x.permute(0, 3, 2, 1)
             x_shape = x.shape
-            x = torch.reshape(x, (x_shape[0], x_shape[1], x_shape[2] * x_shape[3]))
+            x = torch.reshape(
+                x, (x_shape[0], x_shape[1], x_shape[2] * x_shape[3]))
         return x
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_resnet_31.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_31.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,24 @@
+"""
+This code is refer from:
+https://github.com/open-mmlab/mmocr/blob/main/mmocr/models/textrecog/layers/conv_layer.py
+https://github.com/open-mmlab/mmocr/blob/main/mmocr/models/textrecog/backbones/resnet31_ocr.py
+"""
+
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
+import torch
 import torch.nn as nn
+import torch.nn.functional as F
+# import paddle
+# from paddle import ParamAttr
+# import paddle.nn as nn
+# import paddle.nn.functional as F
 
 
 __all__ = ["ResNet31"]
 
 
 def conv3x3(in_channel, out_channel, stride=1):
     return nn.Conv2d(
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_resnet_vd.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_vd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,41 @@
+import os, sys
+import torch
 import torch.nn as nn
 import torch.nn.functional as F
-
-from ..common import Activation
-
+from ...modeling.common import Activation
 
 class ConvBNLayer(nn.Module):
     def __init__(
             self,
             in_channels,
             out_channels,
             kernel_size,
             stride=1,
             groups=1,
             is_vd_mode=False,
-            act=None):
+            act=None,
+            name=None, ):
         super(ConvBNLayer, self).__init__()
         self.act = act
         self.is_vd_mode = is_vd_mode
         self._pool2d_avg = nn.AvgPool2d(
-            kernel_size=stride, stride=stride, padding=0, ceil_mode=False)
+            kernel_size=stride, stride=stride, padding=0, ceil_mode=True)
 
         self._conv = nn.Conv2d(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=kernel_size,
             stride=1 if is_vd_mode else stride,
             padding=(kernel_size - 1) // 2,
             groups=groups,
             bias=False)
 
         self._batch_norm = nn.BatchNorm2d(
-            out_channels, )
+            out_channels,)
         if self.act is not None:
             self._act = Activation(act_type=act, inplace=True)
 
     def forward(self, inputs):
         if self.is_vd_mode:
             inputs = self._pool2d_avg(inputs)
         y = self._conv(inputs)
@@ -49,42 +50,45 @@
                  in_channels,
                  out_channels,
                  stride,
                  shortcut=True,
                  if_first=False,
                  name=None):
         super(BottleneckBlock, self).__init__()
-        self.scale = 4
+
         self.conv0 = ConvBNLayer(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=1,
-            act='relu')
+            act='relu',
+            name=name + "_branch2a")
         self.conv1 = ConvBNLayer(
             in_channels=out_channels,
             out_channels=out_channels,
             kernel_size=3,
             stride=stride,
-            act='relu')
+            act='relu',
+            name=name + "_branch2b")
         self.conv2 = ConvBNLayer(
             in_channels=out_channels,
-            out_channels=out_channels * self.scale,
+            out_channels=out_channels * 4,
             kernel_size=1,
-            act=None)
+            act=None,
+            name=name + "_branch2c")
 
         if not shortcut:
             self.short = ConvBNLayer(
                 in_channels=in_channels,
-                out_channels=out_channels * self.scale,
+                out_channels=out_channels * 4,
                 kernel_size=1,
                 stride=stride,
-                is_vd_mode=not if_first and stride[0] != 1)
+                is_vd_mode=not if_first and stride[0] != 1,
+                name=name + "_branch1")
 
         self.shortcut = shortcut
-        self.out_channels = out_channels * self.scale
 
     def forward(self, inputs):
         y = self.conv0(inputs)
 
         conv1 = self.conv1(y)
         conv2 = self.conv2(conv1)
 
@@ -103,37 +107,38 @@
                  out_channels,
                  stride,
                  shortcut=True,
                  if_first=False,
                  name=None):
         super(BasicBlock, self).__init__()
         self.stride = stride
-        self.scale = 1
         self.conv0 = ConvBNLayer(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=3,
             stride=stride,
-            act='relu')
+            act='relu',
+            name=name + "_branch2a")
         self.conv1 = ConvBNLayer(
             in_channels=out_channels,
             out_channels=out_channels,
             kernel_size=3,
-            act=None)
+            act=None,
+            name=name + "_branch2b")
 
         if not shortcut:
             self.short = ConvBNLayer(
                 in_channels=in_channels,
                 out_channels=out_channels,
                 kernel_size=1,
                 stride=stride,
-                is_vd_mode=not if_first and stride[0] != 1)
+                is_vd_mode=not if_first and stride[0] != 1,
+                name=name + "_branch1")
 
         self.shortcut = shortcut
-        self.out_channels = out_channels * self.scale
 
     def forward(self, inputs):
         y = self.conv0(inputs)
         conv1 = self.conv1(y)
 
         if self.shortcut:
             short = inputs
@@ -160,76 +165,96 @@
             depth = [3, 4, 6, 3]
         elif layers == 101:
             depth = [3, 4, 23, 3]
         elif layers == 152:
             depth = [3, 8, 36, 3]
         elif layers == 200:
             depth = [3, 12, 48, 3]
-
-        if layers >= 50:
-            block_class = BottleneckBlock
-        else:
-            block_class = BasicBlock
+        num_channels = [64, 256, 512,
+                        1024] if layers >= 50 else [64, 64, 128, 256]
         num_filters = [64, 128, 256, 512]
 
         self.conv1_1 = ConvBNLayer(
             in_channels=in_channels,
             out_channels=32,
             kernel_size=3,
             stride=1,
-            act='relu')
+            act='relu',
+            name="conv1_1")
         self.conv1_2 = ConvBNLayer(
             in_channels=32,
             out_channels=32,
             kernel_size=3,
             stride=1,
-            act='relu')
+            act='relu',
+            name="conv1_2")
         self.conv1_3 = ConvBNLayer(
             in_channels=32,
             out_channels=64,
             kernel_size=3,
             stride=1,
-            act='relu')
+            act='relu',
+            name="conv1_3")
         self.pool2d_max = nn.MaxPool2d(kernel_size=3, stride=2, padding=1)
 
         # self.block_list = list()
         self.block_list = nn.Sequential()
-        in_channels = 64
-        for block in range(len(depth)):
-            shortcut = False
-            for i in range(depth[block]):
-                if layers in [101, 152, 200] and block == 2:
-                    if i == 0:
-                        conv_name = "res" + str(block + 2) + "a"
+        if layers >= 50:
+            for block in range(len(depth)):
+                shortcut = False
+                for i in range(depth[block]):
+                    if layers in [101, 152, 200] and block == 2:
+                        if i == 0:
+                            conv_name = "res" + str(block + 2) + "a"
+                        else:
+                            conv_name = "res" + str(block + 2) + "b" + str(i)
                     else:
-                        conv_name = "res" + str(block + 2) + "b" + str(i)
-                else:
-                    conv_name = "res" + str(block + 2) + chr(97 + i)
+                        conv_name = "res" + str(block + 2) + chr(97 + i)
 
-                if i == 0 and block != 0:
-                    stride = (2, 1)
-                else:
-                    stride = (1, 1)
+                    if i == 0 and block != 0:
+                        stride = (2, 1)
+                    else:
+                        stride = (1, 1)
 
-                block_instance = block_class(in_channels=in_channels,
+                    bottleneck_block = BottleneckBlock(in_channels=num_channels[block] if i == 0 else num_filters[block] * 4,
+                                                       out_channels=num_filters[block],
+                                                       stride=stride,
+                                                       shortcut=shortcut,
+                                                       if_first=block == i == 0,
+                                                       name=conv_name)
+                    shortcut = True
+                    # self.block_list.append(bottleneck_block)
+                    self.block_list.add_module('bb_%d_%d' % (block, i), bottleneck_block)
+                self.out_channels = num_filters[block]
+        else:
+            for block in range(len(depth)):
+                shortcut = False
+                for i in range(depth[block]):
+                    conv_name = "res" + str(block + 2) + chr(97 + i)
+                    if i == 0 and block != 0:
+                        stride = (2, 1)
+                    else:
+                        stride = (1, 1)
+
+                    basic_block = BasicBlock(in_channels=num_channels[block] if i == 0 else num_filters[block],
                                              out_channels=num_filters[block],
                                              stride=stride,
                                              shortcut=shortcut,
                                              if_first=block == i == 0,
                                              name=conv_name)
-                shortcut = True
-                in_channels = block_instance.out_channels
-                # self.block_list.append(bottleneck_block)
-                self.block_list.add_module('bb_%d_%d' % (block, i), block_instance)
-            self.out_channels = num_filters[block]
+
+                    shortcut = True
+                    # self.block_list.append(basic_block)
+                    self.block_list.add_module('bb_%d_%d' % (block, i), basic_block)
+                self.out_channels = num_filters[block]
         self.out_pool = nn.MaxPool2d(kernel_size=2, stride=2, padding=0)
 
     def forward(self, inputs):
         y = self.conv1_1(inputs)
         y = self.conv1_2(y)
         y = self.conv1_3(y)
         y = self.pool2d_max(y)
         for block in self.block_list:
             y = block(y)
         y = self.out_pool(y)
 
-        return y
+        return y
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/backbones/rec_svtrnet.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_svtrnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 import torch.nn as nn
-from ..common import Activation
+from ...modeling.common import Activation
 import numpy as np
 
 def drop_path(x, drop_prob=0., training=False):
     """Drop paths (Stochastic Depth) per sample (when applied in main path of residual blocks).
     the original name is misleading as 'Drop Connect' is a different form of dropout in a separate paper...
     See discussion: https://github.com/tensorflow/tpu/issues/494#issuecomment-532968956 ...
     """
@@ -139,26 +139,25 @@
         self.proj_drop = nn.Dropout(proj_drop)
         self.HW = HW
         if HW is not None:
             H = HW[0]
             W = HW[1]
             self.N = H * W
             self.C = dim
-        self.mask = None
         if mixer == 'Local' and HW is not None:
             hk = local_k[0]
             wk = local_k[1]
             mask = torch.ones(H * W, H + hk - 1, W + wk - 1, dtype=torch.float32)
             for h in range(0, H):
                 for w in range(0, W):
                     mask[h * W + w, h:h + hk, w:w + wk] = 0.
-            mask1 = mask[:, hk // 2:H + hk // 2, wk // 2:W + wk //
+            mask_paddle = mask[:, hk // 2:H + hk // 2, wk // 2:W + wk //
                                2].flatten(1)
             mask_inf = torch.full([H * W, H * W], fill_value=float("-Inf"), dtype=torch.float32)
-            mask = torch.where(mask1 < 1, mask1, mask_inf)
+            mask = torch.where(mask_paddle < 1, mask_paddle, mask_inf)
             self.mask = mask.unsqueeze(0).unsqueeze(1)
             # self.mask = mask[None, None, :]
         self.mixer = mixer
 
     def forward(self, x):
         if self.HW is not None:
             N = self.N
@@ -166,16 +165,16 @@
         else:
             _, N, C = x.shape
         qkv = self.qkv(x)
         qkv = qkv.reshape((-1, N, 3, self.num_heads, C // self.num_heads)).permute(2, 0, 3, 1, 4)
         q, k, v = qkv[0] * self.scale, qkv[1], qkv[2]
 
         attn = (q.matmul(k.permute(0, 1, 3, 2)))
-        if self.mask is not None:
-            attn += self.mask.to(attn)
+        if self.mixer == 'Local':
+            attn += self.mask
         attn = nn.functional.softmax(attn, dim=-1)
         attn = self.attn_drop(attn)
 
         x = (attn.matmul(v)).permute(0, 2, 1, 3).reshape((-1, N, C))
         x = self.proj(x)
         x = self.proj_drop(x)
         return x
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/common.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,42 @@
 
+
 import torch
 import torch.nn as nn
+import torch.nn.functional as F
+
+class Hswish(nn.Module):
+    def __init__(self, inplace=True):
+        super(Hswish, self).__init__()
+        self.inplace = inplace
+
+    def forward(self, x):
+        return x * F.relu6(x + 3., inplace=self.inplace) / 6.
+
+# out = max(0, min(1, slop*x+offset))
+# paddle.fluid.layers.hard_sigmoid(x, slope=0.2, offset=0.5, name=None)
+class Hsigmoid(nn.Module):
+    def __init__(self, inplace=True):
+        super(Hsigmoid, self).__init__()
+        self.inplace = inplace
+
+    def forward(self, x):
+        # torch: F.relu6(x + 3., inplace=self.inplace) / 6.
+        # paddle: F.relu6(1.2 * x + 3., inplace=self.inplace) / 6.
+        return F.relu6(1.2 * x + 3., inplace=self.inplace) / 6.
 
 class GELU(nn.Module):
     def __init__(self, inplace=True):
         super(GELU, self).__init__()
         self.inplace = inplace
 
     def forward(self, x):
         return torch.nn.functional.gelu(x)
 
+
 class Swish(nn.Module):
     def __init__(self, inplace=True):
         super(Swish, self).__init__()
         self.inplace = inplace
 
     def forward(self, x):
         if self.inplace:
@@ -28,19 +51,19 @@
         super(Activation, self).__init__()
         act_type = act_type.lower()
         if act_type == 'relu':
             self.act = nn.ReLU(inplace=inplace)
         elif act_type == 'relu6':
             self.act = nn.ReLU6(inplace=inplace)
         elif act_type == 'sigmoid':
-            self.act = nn.Sigmoid()
+            raise NotImplementedError
         elif act_type == 'hard_sigmoid':
-            self.act = nn.Hardsigmoid(inplace)
-        elif act_type == 'hard_swish':
-            self.act = nn.Hardswish(inplace=inplace)
+            self.act = Hsigmoid(inplace)#nn.Hardsigmoid(inplace=inplace)#Hsigmoid(inplace)#
+        elif act_type == 'hard_swish' or act_type == 'hswish':
+            self.act = Hswish(inplace=inplace)
         elif act_type == 'leakyrelu':
             self.act = nn.LeakyReLU(inplace=inplace)
         elif act_type == 'gelu':
             self.act = GELU(inplace=inplace)
         elif act_type == 'swish':
             self.act = Swish(inplace=inplace)
         else:
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/multiheadAttention.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/multiheadAttention.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,18 +69,30 @@
         """
         q_shape = query.shape
         src_shape = key.shape
         q = self._in_proj_q(query)
         k = self._in_proj_k(key)
         v = self._in_proj_v(value)
         q *= self.scaling
+        # q = paddle.transpose(
+        #     paddle.reshape(
+        #         q, [q_shape[0], q_shape[1], self.num_heads, self.head_dim]),
+        #     [1, 2, 0, 3])
         q = torch.reshape(q, (q_shape[0], q_shape[1], self.num_heads, self.head_dim))
         q = q.permute(1, 2, 0, 3)
+        # k = paddle.transpose(
+        #     paddle.reshape(
+        #         k, [src_shape[0], q_shape[1], self.num_heads, self.head_dim]),
+        #     [1, 2, 0, 3])
         k = torch.reshape(k, (src_shape[0], q_shape[1], self.num_heads, self.head_dim))
         k = k.permute(1, 2, 0, 3)
+        # v = paddle.transpose(
+        #     paddle.reshape(
+        #         v, [src_shape[0], q_shape[1], self.num_heads, self.head_dim]),
+        #     [1, 2, 0, 3])
         v = torch.reshape(v, (src_shape[0], q_shape[1], self.num_heads, self.head_dim))
         v = v.permute(1, 2, 0, 3)
         if key_padding_mask is not None:
             assert key_padding_mask.shape[0] == q_shape[1]
             assert key_padding_mask.shape[1] == src_shape[0]
         attn_output_weights = torch.matmul(q,
                                             k.permute(0, 1, 3, 2))
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/rec_att_head.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_att_head.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,110 +1,145 @@
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
+import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+from ...modeling.common import Activation
+
 
-    
 class AttentionHead(nn.Module):
     def __init__(self, in_channels, out_channels, hidden_size, **kwargs):
         super(AttentionHead, self).__init__()
         self.input_size = in_channels
         self.hidden_size = hidden_size
         self.num_classes = out_channels
 
-        self.attention_cell = AttentionGRUCell(in_channels, hidden_size, out_channels)
+        self.attention_cell = AttentionGRUCell(
+            in_channels, hidden_size, out_channels, use_gru=False)
         self.generator = nn.Linear(hidden_size, out_channels)
 
     def _char_to_onehot(self, input_char, onehot_dim):
-        input_ont_hot = F.one_hot(input_char.long(), onehot_dim)
+        input_ont_hot = F.one_hot(input_char.type(torch.int64), onehot_dim)
         return input_ont_hot
 
-    def forward(self, inputs, data=None, batch_max_length=25):
-        batch_size = inputs.size(0)
+    def forward(self, inputs, targets=None, batch_max_length=25):
+        batch_size = inputs.size()[0]
         num_steps = batch_max_length
 
-        hidden = (torch.zeros(batch_size, self.hidden_size, device=inputs.device),
-                  torch.zeros(batch_size, self.hidden_size, device=inputs.device))
+        hidden = torch.zeros((batch_size, self.hidden_size))
         output_hiddens = []
 
-        if self.training:
-            targets = data[0]
+        if targets is not None:
             for i in range(num_steps):
-                char_onehots = self._char_to_onehot(targets[:, i], onehot_dim=self.num_classes)
-                hidden, alpha = self.attention_cell(hidden, inputs, char_onehots)
-                output_hiddens.append(torch.unsqueeze(hidden[0], axis=1))
+                char_onehots = self._char_to_onehot(
+                    targets[:, i], onehot_dim=self.num_classes)
+                (outputs, hidden), alpha = self.attention_cell(hidden, inputs,
+                                                               char_onehots)
+                output_hiddens.append(torch.unsqueeze(outputs, dim=1))
             output = torch.cat(output_hiddens, dim=1)
             probs = self.generator(output)
+
         else:
-            targets = torch.zeros(batch_size, dtype=torch.int32, device=inputs.device)
-            probs = torch.zeros(batch_size, num_steps, self.num_classes, device=inputs.device)
-            # probs = None
+            targets = torch.zeros([batch_size], dtype=torch.int32)
+            probs = None
             char_onehots = None
             outputs = None
             alpha = None
 
             for i in range(num_steps):
-                char_onehots = self._char_to_onehot(targets, onehot_dim=self.num_classes)
-                hidden, alpha = self.attention_cell(hidden, inputs, char_onehots)
-                probs_step = self.generator(hidden[0])
-
-                probs[:, i, :] = probs_step
-                # if probs is None:
-                #     probs = torch.unsqueeze(probs_step, dim=1)
-                # else:
-                #     probs = torch.concat(
-                #         [probs, torch.unsqueeze(
-                #             probs_step, dim=1)], dim=1)
+                char_onehots = self._char_to_onehot(
+                    targets, onehot_dim=self.num_classes)
+                (outputs, hidden), alpha = self.attention_cell(hidden, inputs,
+                                                               char_onehots)
+                probs_step = self.generator(outputs)
+                if probs is None:
+                    probs = torch.unsqueeze(probs_step, dim=1)
+                else:
+                    probs = torch.cat(
+                        [probs, torch.unsqueeze(
+                            probs_step, dim=1)], dim=1)
                 next_input = probs_step.argmax(dim=1)
                 targets = next_input
-        if not self.training:
-            probs = F.softmax(probs, dim=2)
-        return {'res':probs}
+
+        return probs
+
+
+class AttentionGRUCell(nn.Module):
+    def __init__(self, input_size, hidden_size, num_embeddings, use_gru=False):
+        super(AttentionGRUCell, self).__init__()
+        self.i2h = nn.Linear(input_size, hidden_size, bias=False)
+        self.h2h = nn.Linear(hidden_size, hidden_size)
+        self.score = nn.Linear(hidden_size, 1, bias=False)
+
+        self.rnn = nn.GRUCell(
+            input_size=input_size + num_embeddings, hidden_size=hidden_size, bias=True)
+
+        self.hidden_size = hidden_size
+
+    def forward(self, prev_hidden, batch_H, char_onehots):
+
+        batch_H_proj = self.i2h(batch_H)
+        prev_hidden_proj = torch.unsqueeze(self.h2h(prev_hidden), dim=1)
+
+        res = torch.add(batch_H_proj, prev_hidden_proj)
+        res = torch.tanh(res)
+        e = self.score(res)
+
+        alpha = F.softmax(e, dim=1)
+        alpha = alpha.permute(0, 2, 1)
+        context = torch.squeeze(torch.matmul(alpha, batch_H), dim=1)
+        concat_context = torch.cat([context, char_onehots.float()], 1)
+
+        cur_hidden = self.rnn(concat_context, prev_hidden)
+
+        return (cur_hidden, cur_hidden), alpha
+
 
 class AttentionLSTM(nn.Module):
     def __init__(self, in_channels, out_channels, hidden_size, **kwargs):
         super(AttentionLSTM, self).__init__()
         self.input_size = in_channels
         self.hidden_size = hidden_size
         self.num_classes = out_channels
 
         self.attention_cell = AttentionLSTMCell(
             in_channels, hidden_size, out_channels, use_gru=False)
         self.generator = nn.Linear(hidden_size, out_channels)
 
     def _char_to_onehot(self, input_char, onehot_dim):
-        input_ont_hot = F.one_hot(input_char, onehot_dim)
+        input_ont_hot = F.one_hot(input_char.type(torch.int64), onehot_dim)
         return input_ont_hot
 
-    def forward(self, inputs, data=None, batch_max_length=25):
+    def forward(self, inputs, targets=None, batch_max_length=25):
         batch_size = inputs.shape[0]
         num_steps = batch_max_length
 
         hidden = (torch.zeros((batch_size, self.hidden_size)), torch.zeros(
             (batch_size, self.hidden_size)))
         output_hiddens = []
 
-        if self.training:
-            targets = data[0]
+        if targets is not None:
             for i in range(num_steps):
                 # one-hot vectors for a i-th char
                 char_onehots = self._char_to_onehot(
                     targets[:, i], onehot_dim=self.num_classes)
                 hidden, alpha = self.attention_cell(hidden, inputs,
                                                     char_onehots)
 
                 hidden = (hidden[1][0], hidden[1][1])
                 output_hiddens.append(torch.unsqueeze(hidden[0], dim=1))
             output = torch.cat(output_hiddens, dim=1)
             probs = self.generator(output)
 
         else:
-            targets = torch.zeros(batch_size, device=inputs.device, dtype=torch.int32)
+            targets = torch.zeros([batch_size], dtype=torch.int32)
             probs = None
-            char_onehots = None
-            alpha = None
 
             for i in range(num_steps):
                 char_onehots = self._char_to_onehot(
                     targets, onehot_dim=self.num_classes)
                 hidden, alpha = self.attention_cell(hidden, inputs,
                                                     char_onehots)
                 probs_step = self.generator(hidden[0])
@@ -115,64 +150,41 @@
                     probs = torch.cat(
                         [probs, torch.unsqueeze(
                             probs_step, dim=1)], dim=1)
 
                 next_input = probs_step.argmax(dim=1)
 
                 targets = next_input
-        if not self.training:
-            probs = F.softmax(probs, dim=2)
+
         return probs
 
 
 class AttentionLSTMCell(nn.Module):
-    def __init__(self, input_size, hidden_size, num_embeddings):
-        super(AttentionLSTMCell, self).__init__()
-        self.i2h = nn.Linear(input_size, hidden_size, bias=False)
-        self.h2h = nn.Linear(hidden_size, hidden_size)
-        self.score = nn.Linear(hidden_size, 1, bias=False)
-        self.rnn = nn.LSTMCell(input_size=input_size + num_embeddings, hidden_size=hidden_size)
-        self.hidden_size = hidden_size
-
-    def forward(self, prev_hidden, batch_H, char_onehots):
-        batch_H_proj = self.i2h(batch_H)
-        prev_hidden_proj = torch.unsqueeze(self.h2h(prev_hidden[1]), dim=1)
-
-        res = torch.tanh(batch_H_proj + prev_hidden_proj)
-        e = self.score(res)
-
-        alpha = F.softmax(e, dim=1)
-        alpha = torch.permute(alpha, [0, 2, 1])
-        context = torch.squeeze(torch.bmm(alpha, batch_H), dim=1)
-        concat_context = torch.cat([context, char_onehots], 1)
-        cur_hidden = self.rnn(concat_context, prev_hidden)
-        return cur_hidden, alpha
-
-
-class AttentionGRUCell(nn.Module):
     def __init__(self, input_size, hidden_size, num_embeddings, use_gru=False):
-        super(AttentionGRUCell, self).__init__()
+        super(AttentionLSTMCell, self).__init__()
         self.i2h = nn.Linear(input_size, hidden_size, bias=False)
         self.h2h = nn.Linear(hidden_size, hidden_size)
         self.score = nn.Linear(hidden_size, 1, bias=False)
-
-        self.rnn = nn.GRUCell(input_size=input_size + num_embeddings, hidden_size=hidden_size)
+        if not use_gru:
+            self.rnn = nn.LSTMCell(
+                input_size=input_size + num_embeddings, hidden_size=hidden_size)
+        else:
+            self.rnn = nn.GRUCell(
+                input_size=input_size + num_embeddings, hidden_size=hidden_size)
 
         self.hidden_size = hidden_size
 
     def forward(self, prev_hidden, batch_H, char_onehots):
-
         batch_H_proj = self.i2h(batch_H)
         prev_hidden_proj = torch.unsqueeze(self.h2h(prev_hidden[0]), dim=1)
-
         res = torch.add(batch_H_proj, prev_hidden_proj)
         res = torch.tanh(res)
         e = self.score(res)
 
         alpha = F.softmax(e, dim=1)
-        alpha = torch.permute(alpha, [0, 2, 1])
-        context = torch.squeeze(torch.bmm(alpha, batch_H), dim=1)
-        concat_context = torch.cat([context, char_onehots], 1)
+        alpha = alpha.permute(0, 2, 1)
+        context = torch.squeeze(torch.matmul(alpha, batch_H), dim=1)
+        concat_context = torch.cat([context, char_onehots.float()], 1)
 
-        cur_hidden = self.rnn(concat_context, prev_hidden[0])
+        cur_hidden = self.rnn(concat_context, prev_hidden)
 
-        return (cur_hidden, cur_hidden), alpha
+        return cur_hidden, alpha
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/rec_ctc_head.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_ctc_head.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import os, sys
+import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 class CTCHead(nn.Module):
     def __init__(self,
                  in_channels,
                  out_channels=6625,
+                 fc_decay=0.0004,
                  mid_channels=None,
                  return_feats=False,
                  **kwargs):
         super(CTCHead, self).__init__()
         if mid_channels is None:
             self.fc = nn.Linear(
                 in_channels,
@@ -27,15 +30,15 @@
             )
 
         self.out_channels = out_channels
         self.mid_channels = mid_channels
         self.return_feats = return_feats
 
 
-    def forward(self, x, data=None):
+    def forward(self, x, labels=None):
         if self.mid_channels is None:
             predicts = self.fc(x)
         else:
             x = self.fc1(x)
             predicts = self.fc2(x)
 
         if self.return_feats:
@@ -43,8 +46,8 @@
         else:
             result = predicts
 
         if not self.training:
             predicts = F.softmax(predicts, dim=2)
             result = predicts
 
-        return {'res': result}
+        return result
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/rec_multi_head.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_multi_head.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
 
-from ..necks.rnn import Im2Seq, SequenceEncoder
+from ...modeling.necks.rnn import Im2Seq, SequenceEncoder
 from .rec_nrtr_head import Transformer
 from .rec_ctc_head import CTCHead
 from .rec_sar_head import SARHead
 
 class FCTranspose(nn.Module):
     def __init__(self, in_channels, out_channels, only_transpose=False):
         super().__init__()
@@ -26,34 +26,36 @@
         self.head_list = kwargs.pop('head_list')
 
         self.gtc_head = 'sar'
         assert len(self.head_list) >= 2
         for idx, head_name in enumerate(self.head_list):
             name = list(head_name)[0]
             if name == 'SARHead':
-                # sar head
-                sar_args = self.head_list[idx][name]
-                self.sar_head = eval(name)(in_channels=in_channels, \
-                                           out_channels=out_channels_list['SARLabelDecode'], **sar_args)
+                pass
+                # # sar head
+                # sar_args = self.head_list[idx][name]
+                # self.sar_head = eval(name)(in_channels=in_channels, \
+                #                            out_channels=out_channels_list['SARLabelDecode'], **sar_args)
             elif name == 'NRTRHead':
-                gtc_args = self.head_list[idx][name]
-                max_text_length = gtc_args.get('max_text_length', 25)
-                nrtr_dim = gtc_args.get('nrtr_dim', 256)
-                num_decoder_layers = gtc_args.get('num_decoder_layers', 4)
-                self.before_gtc = nn.Sequential(
-                    nn.Flatten(2), FCTranspose(in_channels, nrtr_dim))
-                self.gtc_head = Transformer(
-                    d_model=nrtr_dim,
-                    nhead=nrtr_dim // 32,
-                    num_encoder_layers=-1,
-                    beam_size=-1,
-                    num_decoder_layers=num_decoder_layers,
-                    max_len=max_text_length,
-                    dim_feedforward=nrtr_dim * 4,
-                    out_channels=out_channels_list['NRTRLabelDecode'])
+                pass
+                # gtc_args = self.head_list[idx][name]
+                # max_text_length = gtc_args.get('max_text_length', 25)
+                # nrtr_dim = gtc_args.get('nrtr_dim', 256)
+                # num_decoder_layers = gtc_args.get('num_decoder_layers', 4)
+                # self.before_gtc = nn.Sequential(
+                #     nn.Flatten(2), FCTranspose(in_channels, nrtr_dim))
+                # self.gtc_head = Transformer(
+                #     d_model=nrtr_dim,
+                #     nhead=nrtr_dim // 32,
+                #     num_encoder_layers=-1,
+                #     beam_size=-1,
+                #     num_decoder_layers=num_decoder_layers,
+                #     max_len=max_text_length,
+                #     dim_feedforward=nrtr_dim * 4,
+                #     out_channels=out_channels_list['NRTRLabelDecode'])
             elif name == 'CTCHead':
                 # ctc neck
                 self.encoder_reshape = Im2Seq(in_channels)
                 neck_args = self.head_list[idx][name]['Neck']
                 encoder_type = neck_args.pop('name')
                 self.ctc_encoder = SequenceEncoder(in_channels=in_channels, \
                                                    encoder_type=encoder_type, **neck_args)
@@ -64,24 +66,23 @@
                 self.ctc_head = eval(name)(in_channels=self.ctc_encoder.out_channels, \
                                            out_channels=out_channels_list['CTCLabelDecode'], **head_args)
             else:
                 raise NotImplementedError(
                     '{} is not supported in MultiHead yet'.format(name))
 
     def forward(self, x, data=None):
-
         ctc_encoder = self.ctc_encoder(x)
-        ctc_out = self.ctc_head(ctc_encoder)['res']
+        ctc_out = self.ctc_head(ctc_encoder)
         head_out = dict()
         head_out['ctc'] = ctc_out
         head_out['res'] = ctc_out
         head_out['ctc_neck'] = ctc_encoder
         # eval mode
         if not self.training:
-            return {'res': ctc_out}
+            return ctc_out
         if self.gtc_head == 'sar':
             sar_out = self.sar_head(x, data[1:])['res']
             head_out['sar'] = sar_out
         else:
             gtc_out = self.gtc_head(self.before_gtc(x), data[1:])['res']
             head_out['nrtr'] = gtc_out
         return head_out
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/rec_nrtr_head.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_nrtr_head.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import math
 import torch
+import copy
 from torch import nn
 import torch.nn.functional as F
+from torch.nn import ModuleList as LayerList
+from torch.nn.init import xavier_uniform_
+from torch.nn import Dropout, LayerNorm, Conv2d
 import numpy as np
-from ..backbones.rec_svtrnet import Mlp
+from ...modeling.heads.multiheadAttention import MultiheadAttention
+from torch.nn.init import xavier_normal_
+
 
 class Transformer(nn.Module):
     """A transformer model. User is able to modify the attributes as needed. The architechture
     is based on the paper "Attention Is All You Need". Ashish Vaswani, Noam Shazeer,
     Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N Gomez, Lukasz Kaiser, and
     Illia Polosukhin. 2017. Attention is all you need. In Advances in Neural Information
     Processing Systems, pages 6000-6010.
@@ -17,166 +23,178 @@
         nhead: the number of heads in the multiheadattention models (default=8).
         num_encoder_layers: the number of sub-encoder-layers in the encoder (default=6).
         num_decoder_layers: the number of sub-decoder-layers in the decoder (default=6).
         dim_feedforward: the dimension of the feedforward network model (default=2048).
         dropout: the dropout value (default=0.1).
         custom_encoder: custom encoder (default=None).
         custom_decoder: custom decoder (default=None).
+
     """
 
     def __init__(self,
                  d_model=512,
                  nhead=8,
                  num_encoder_layers=6,
                  beam_size=0,
                  num_decoder_layers=6,
                  max_len=25,
                  dim_feedforward=1024,
                  attention_dropout_rate=0.0,
                  residual_dropout_rate=0.1,
+                 custom_encoder=None,
+                 custom_decoder=None,
                  in_channels=0,
                  out_channels=0,
                  scale_embedding=True):
         super(Transformer, self).__init__()
-        self.out_channels = out_channels + 1
+        self.out_channels = out_channels # out_channels + 1
         self.max_len = max_len
         self.embedding = Embeddings(
             d_model=d_model,
             vocab=self.out_channels,
             padding_idx=0,
             scale_embedding=scale_embedding)
         self.positional_encoding = PositionalEncoding(
-            dropout=residual_dropout_rate, dim=d_model)
-
-        if num_encoder_layers > 0:
-            self.encoder = nn.ModuleList([
-                TransformerBlock(
-                    d_model,
-                    nhead,
-                    dim_feedforward,
-                    attention_dropout_rate,
-                    residual_dropout_rate,
-                    with_self_attn=True,
-                    with_cross_attn=False) for i in range(num_encoder_layers)
-            ])
+            dropout=residual_dropout_rate,
+            dim=d_model, )
+        if custom_encoder is not None:
+            self.encoder = custom_encoder
         else:
-            self.encoder = None
+            if num_encoder_layers > 0:
+                encoder_layer = TransformerEncoderLayer(
+                    d_model, nhead, dim_feedforward, attention_dropout_rate,
+                    residual_dropout_rate)
+                self.encoder = TransformerEncoder(encoder_layer,
+                                                  num_encoder_layers)
+            else:
+                self.encoder = None
 
-        self.decoder = nn.ModuleList([
-            TransformerBlock(
-                d_model,
-                nhead,
-                dim_feedforward,
-                attention_dropout_rate,
-                residual_dropout_rate,
-                with_self_attn=True,
-                with_cross_attn=True) for i in range(num_decoder_layers)
-        ])
+        if custom_decoder is not None:
+            self.decoder = custom_decoder
+        else:
+            decoder_layer = TransformerDecoderLayer(
+                d_model, nhead, dim_feedforward, attention_dropout_rate,
+                residual_dropout_rate)
+            self.decoder = TransformerDecoder(decoder_layer, num_decoder_layers)
 
+        self._reset_parameters()
         self.beam_size = beam_size
         self.d_model = d_model
         self.nhead = nhead
-        self.tgt_word_prj = nn.Linear(d_model, self.out_channels, bias=False)
-        w0 = np.random.normal(0.0, d_model**-0.5,(d_model, self.out_channels)).astype(np.float32)
-        self.tgt_word_prj.weight.data = torch.from_numpy(w0.transpose())
+        self.tgt_word_prj = nn.Linear(
+            d_model, self.out_channels, bias=False)
+        w0 = np.random.normal(0.0, d_model ** -0.5,
+                              (self.out_channels, d_model)).astype(np.float32)
+        self.tgt_word_prj.weight.data = torch.from_numpy(w0)
         self.apply(self._init_weights)
 
     def _init_weights(self, m):
-        if isinstance(m, nn.Linear):
-            nn.init.xavier_normal_(m.weight)
+
+        if isinstance(m, nn.Conv2d):
+            xavier_normal_(m.weight)
             if m.bias is not None:
-                nn.init.zeros_(m.bias)
+                torch.nn.init.zeros_(m.bias)
 
     def forward_train(self, src, tgt):
         tgt = tgt[:, :-1]
 
-        tgt = self.embedding(tgt)
+        tgt_key_padding_mask = self.generate_padding_mask(tgt)
+        tgt = self.embedding(tgt).permute(1, 0, 2)
         tgt = self.positional_encoding(tgt)
-        tgt_mask = self.generate_square_subsequent_mask(tgt.shape[1], tgt.device)
+        tgt_mask = self.generate_square_subsequent_mask(tgt.shape[0], tgt.device)
 
         if self.encoder is not None:
-            src = self.positional_encoding(src)
-            for encoder_layer in self.encoder:
-                src = encoder_layer(src)
-            memory = src  # B N C
+            src = self.positional_encoding(src.permute(1, 0, 2))
+            memory = self.encoder(src)
         else:
-            memory = src  # B N C
-        for decoder_layer in self.decoder:
-            tgt = decoder_layer(tgt, memory, self_mask=tgt_mask)
-        output = tgt
+            memory = src.squeeze(2).permute(2, 0, 1)
+        output = self.decoder(
+            tgt,
+            memory,
+            tgt_mask=tgt_mask,
+            memory_mask=None,
+            tgt_key_padding_mask=tgt_key_padding_mask,
+            memory_key_padding_mask=None)
+        output = output.permute(1, 0, 2)
         logit = self.tgt_word_prj(output)
         return logit
 
-    def forward(self, src, data=None):
+    def forward(self, src, targets=None):
         """Take in and process masked source/target sequences.
         Args:
             src: the sequence to the encoder (required).
             tgt: the sequence to the decoder (required).
         Shape:
-            - src: :math:`(B, sN, C)`.
-            - tgt: :math:`(B, tN, C)`.
+            - src: :math:`(S, N, E)`.
+            - tgt: :math:`(T, N, E)`.
         Examples:
             >>> output = transformer_model(src, tgt)
         """
 
         if self.training:
-            max_len = data[1].max()
-            tgt = data[0][:, :2 + max_len]
-            res = self.forward_train(src, tgt)
+            max_len = targets[1].max()
+            tgt = targets[0][:, :2 + max_len]
+            return self.forward_train(src, tgt)
         else:
             if self.beam_size > 0:
-                res = self.forward_beam(src)
+                return self.forward_beam(src)
             else:
-                res = self.forward_test(src)
-        return {'res': res}
+                return self.forward_test(src)
 
     def forward_test(self, src):
-
-        bs = src.size(0)
+        bs = src.shape[0]
         if self.encoder is not None:
-            src = self.positional_encoding(src)
-            for encoder_layer in self.encoder:
-                src = encoder_layer(src)
-            memory = src  # B N C
+            src = self.positional_encoding(src.permute(1, 0, 2))
+            memory = self.encoder(src)
         else:
-            memory = src
-        dec_seq = torch.full((bs, 1), 2, dtype=torch.int64, device=src.device)
-        dec_prob = torch.full((bs, 1), 1., dtype=torch.float32, device=src.device)
-        for len_dec_seq in range(1, self.max_len):
-            dec_seq_embed = self.embedding(dec_seq)
+            memory = torch.squeeze(src, 2).permute(2, 0, 1)
+        dec_seq = torch.full((bs, 1), 2, dtype=torch.int64)
+        dec_prob = torch.full((bs, 1), 1., dtype=torch.float32)
+        for len_dec_seq in range(1, 25):
+            dec_seq_embed = self.embedding(dec_seq).permute(1, 0, 2)
             dec_seq_embed = self.positional_encoding(dec_seq_embed)
-            tgt_mask = self.generate_square_subsequent_mask(dec_seq_embed.size(1), dec_seq_embed.device)
-            tgt = dec_seq_embed
-            for decoder_layer in self.decoder:
-                tgt = decoder_layer(tgt, memory, self_mask=tgt_mask)
-            dec_output = tgt
+            tgt_mask = self.generate_square_subsequent_mask(
+                dec_seq_embed.shape[0])
+            output = self.decoder(
+                dec_seq_embed,
+                memory,
+                tgt_mask=tgt_mask,
+                memory_mask=None,
+                tgt_key_padding_mask=None,
+                memory_key_padding_mask=None)
+            dec_output = output.permute(1, 0, 2)
             dec_output = dec_output[:, -1, :]
-            word_prob = F.softmax(self.tgt_word_prj(dec_output), dim=-1)
-            preds_prob, preds_idx = torch.max(word_prob, dim=-1)
-            if torch.equal(preds_idx, torch.full_like(preds_idx, 3, dtype=torch.int64)):
+            tgt_word_prj = self.tgt_word_prj(dec_output)
+            word_prob = F.softmax(tgt_word_prj, dim=1)
+            preds_idx = word_prob.argmax(dim=1)
+            if torch.equal(
+                    preds_idx,
+                    torch.full(
+                        preds_idx.shape, 3, dtype=torch.int64)):
                 break
+            preds_prob = torch.max(word_prob, dim=1).values
             dec_seq = torch.cat(
-                [dec_seq, preds_idx.reshape([-1, 1])], dim=1)
-            dec_prob = torch.concat(
-                [dec_prob, preds_prob.reshape([-1, 1])], dim=1)
+                [dec_seq, torch.reshape(preds_idx, (-1, 1))], dim=1)
+            dec_prob = torch.cat(
+                [dec_prob, torch.reshape(preds_prob, (-1, 1))], dim=1)
         return [dec_seq, dec_prob]
 
     def forward_beam(self, images):
-        """ Translation work in one batch """
+        ''' Translation work in one batch '''
 
         def get_inst_idx_to_tensor_position_map(inst_idx_list):
-            """ Indicate the position of an instance in a tensor. """
+            ''' Indicate the position of an instance in a tensor. '''
             return {
                 inst_idx: tensor_position
                 for tensor_position, inst_idx in enumerate(inst_idx_list)
             }
 
         def collect_active_part(beamed_tensor, curr_active_inst_idx,
                                 n_prev_active_inst, n_bm):
-            """ Collect tensor parts associated to active instances. """
+            ''' Collect tensor parts associated to active instances. '''
 
             beamed_tensor_shape = beamed_tensor.shape
             n_curr_active_inst = len(curr_active_inst_idx)
             new_shape = (n_curr_active_inst * n_bm, beamed_tensor_shape[1],
                          beamed_tensor_shape[2])
 
             beamed_tensor = beamed_tensor.reshape([n_prev_active_inst, -1])
@@ -193,44 +211,50 @@
 
             n_prev_active_inst = len(inst_idx_to_position_map)
             active_inst_idx = [
                 inst_idx_to_position_map[k] for k in active_inst_idx_list
             ]
             active_inst_idx = torch.tensor(active_inst_idx, dtype=torch.int64)
             active_src_enc = collect_active_part(
-                src_enc.permute([1, 0, 2]), active_inst_idx,
-                n_prev_active_inst, n_bm).permute([1, 0, 2])
+                src_enc.permute(1, 0, 2), active_inst_idx,
+                n_prev_active_inst, n_bm).permute(1, 0, 2)
             active_inst_idx_to_position_map = get_inst_idx_to_tensor_position_map(
                 active_inst_idx_list)
             return active_src_enc, active_inst_idx_to_position_map
 
         def beam_decode_step(inst_dec_beams, len_dec_seq, enc_output,
-                             inst_idx_to_position_map, n_bm):
-            """ Decode and update beam status, and then return active beam idx """
+                             inst_idx_to_position_map, n_bm,
+                             memory_key_padding_mask):
+            ''' Decode and update beam status, and then return active beam idx '''
 
             def prepare_beam_dec_seq(inst_dec_beams, len_dec_seq):
                 dec_partial_seq = [
                     b.get_current_state() for b in inst_dec_beams if not b.done
                 ]
                 dec_partial_seq = torch.stack(dec_partial_seq)
                 dec_partial_seq = dec_partial_seq.reshape([-1, len_dec_seq])
                 return dec_partial_seq
 
-            def predict_word(dec_seq, enc_output, n_active_inst, n_bm):
-                dec_seq = self.embedding(dec_seq)
+            def predict_word(dec_seq, enc_output, n_active_inst, n_bm,
+                             memory_key_padding_mask):
+                dec_seq = self.embedding(dec_seq).permute(1, 0, 2)
                 dec_seq = self.positional_encoding(dec_seq)
-                tgt_mask = self.generate_square_subsequent_mask(dec_seq.size(1), dec_seq.device)
-                tgt = dec_seq
-                for decoder_layer in self.decoder:
-                    tgt = decoder_layer(tgt, enc_output, self_mask=tgt_mask)
-                dec_output = tgt
+                tgt_mask = self.generate_square_subsequent_mask(
+                    dec_seq.shape[0])
+                dec_output = self.decoder(
+                    dec_seq,
+                    enc_output,
+                    tgt_mask=tgt_mask,
+                    tgt_key_padding_mask=None,
+                    memory_key_padding_mask=memory_key_padding_mask, )
+                dec_output = dec_output.permute(1, 0, 2)
                 dec_output = dec_output[:,
                                         -1, :]  # Pick the last step: (bh * bm) * d_h
                 word_prob = F.softmax(self.tgt_word_prj(dec_output), dim=1)
-                word_prob = word_prob.reshape([n_active_inst, n_bm, -1])
+                word_prob = torch.reshape(word_prob, (n_active_inst, n_bm, -1))
                 return word_prob
 
             def collect_active_inst_idx_list(inst_beams, word_prob,
                                              inst_idx_to_position_map):
                 active_inst_idx_list = []
                 for inst_idx, inst_position in inst_idx_to_position_map.items():
                     is_inst_complete = inst_beams[inst_idx].advance(word_prob[
@@ -238,15 +262,16 @@
                     if not is_inst_complete:
                         active_inst_idx_list += [inst_idx]
 
                 return active_inst_idx_list
 
             n_active_inst = len(inst_idx_to_position_map)
             dec_seq = prepare_beam_dec_seq(inst_dec_beams, len_dec_seq)
-            word_prob = predict_word(dec_seq, enc_output, n_active_inst, n_bm)
+            word_prob = predict_word(dec_seq, enc_output, n_active_inst, n_bm,
+                                     None)
             # Update the beam with predicted word prob information and collect incomplete instances
             active_inst_idx_list = collect_active_inst_idx_list(
                 inst_dec_beams, word_prob, inst_idx_to_position_map)
             return active_inst_idx_list
 
         def collect_hypothesis_and_scores(inst_dec_beams, n_best):
             all_hyp, all_scores = [], []
@@ -259,32 +284,34 @@
                 ]
                 all_hyp += [hyps]
             return all_hyp, all_scores
 
         with torch.no_grad():
             #-- Encode
             if self.encoder is not None:
-                src = self.positional_encoding(images)
+                src = self.positional_encoding(images.permute(1, 0, 2))
                 src_enc = self.encoder(src)
             else:
-                src_enc = images
+                src_enc = images.squeeze(2).transpose([0, 2, 1])
 
             n_bm = self.beam_size
+            src_shape = src_enc.shape
             inst_dec_beams = [Beam(n_bm) for _ in range(1)]
             active_inst_idx_list = list(range(1))
             # Repeat data for beam search
-            src_enc = torch.tile(src_enc, [1, n_bm, 1])
+            # src_enc = paddle.tile(src_enc, [1, n_bm, 1])
+            src_enc = src_enc.repeat(1, n_bm, 1)
             inst_idx_to_position_map = get_inst_idx_to_tensor_position_map(
                 active_inst_idx_list)
             # Decode
-            for len_dec_seq in range(1, self.max_len):
+            for len_dec_seq in range(1, 25):
                 src_enc_copy = src_enc.clone()
                 active_inst_idx_list = beam_decode_step(
                     inst_dec_beams, len_dec_seq, src_enc_copy,
-                    inst_idx_to_position_map, n_bm)
+                    inst_idx_to_position_map, n_bm, None)
                 if not active_inst_idx_list:
                     break  # all instances have finished their path to <EOS>
                 src_enc, inst_idx_to_position_map = collate_active_info(
                     src_enc_copy, inst_idx_to_position_map,
                     active_inst_idx_list)
         batch_hyp, batch_scores = collect_hypothesis_and_scores(inst_dec_beams,
                                                                 1)
@@ -294,144 +321,285 @@
             l = len(bs_hyp[0])
             bs_hyp_pad = bs_hyp[0] + [3] * (25 - l)
             result_hyp.append(bs_hyp_pad)
             score = float(score) / l
             hyp_score = [score for _ in range(25)]
             hyp_scores.append(hyp_score)
         return [
-            torch.from_numpy(
+            torch.tensor(
                 np.array(result_hyp), dtype=torch.int64),
-            torch.from_numpy(hyp_scores)
+            torch.tensor(hyp_scores)
         ]
 
-    def generate_square_subsequent_mask(self, sz, device):
+    def generate_square_subsequent_mask(self, sz):
         """Generate a square mask for the sequence. The masked positions are filled with float('-inf').
             Unmasked positions are filled with float(0.0).
         """
         mask = torch.zeros([sz, sz], dtype=torch.float32)
         mask_inf = torch.triu(
-            torch.full(size=(sz, sz), dtype=torch.float32, fill_value=-torch.inf),
+            torch.full(
+                size=[sz, sz], fill_value=float('-Inf'),  dtype=torch.float32),
             diagonal=1)
         mask = mask + mask_inf
-        return mask.unsqueeze(0).unsqueeze(0).to(device)
+        return mask
 
+    def generate_padding_mask(self, x):
+        # padding_mask = paddle.equal(x, paddle.to_tensor(0, dtype=x.dtype))
+        padding_mask = (x == torch.tensor(0, dtype=x.dtype))
+        return padding_mask
 
-class MultiheadAttention(nn.Module):
-    """Allows the model to jointly attend to information
-    from different representation subspaces.
-    See reference: Attention Is All You Need
+    def _reset_parameters(self):
+        """Initiate parameters in the transformer model."""
 
-    .. math::
-        \text{MultiHead}(Q, K, V) = \text{Concat}(head_1,\dots,head_h)W^O
-        \text{where} head_i = \text{Attention}(QW_i^Q, KW_i^K, VW_i^V)
+        for p in self.parameters():
+            if p.dim() > 1:
+                xavier_uniform_(p)
+
+
+class TransformerEncoder(nn.Module):
+    """TransformerEncoder is a stack of N encoder layers
+    Args:
+        encoder_layer: an instance of the TransformerEncoderLayer() class (required).
+        num_layers: the number of sub-encoder-layers in the encoder (required).
+        norm: the layer normalization component (optional).
+    """
+
+    def __init__(self, encoder_layer, num_layers):
+        super(TransformerEncoder, self).__init__()
+        self.layers = _get_clones(encoder_layer, num_layers)
+        self.num_layers = num_layers
+
+    def forward(self, src):
+        """Pass the input through the endocder layers in turn.
+        Args:
+            src: the sequnce to the encoder (required).
+            mask: the mask for the src sequence (optional).
+            src_key_padding_mask: the mask for the src keys per batch (optional).
+        """
+        output = src
+
+        for i in range(self.num_layers):
+            output = self.layers[i](output,
+                                    src_mask=None,
+                                    src_key_padding_mask=None)
+
+        return output
+
+
+class TransformerDecoder(nn.Module):
+    """TransformerDecoder is a stack of N decoder layers
 
     Args:
-        embed_dim: total dimension of the model
-        num_heads: parallel attention layers, or heads
+        decoder_layer: an instance of the TransformerDecoderLayer() class (required).
+        num_layers: the number of sub-decoder-layers in the decoder (required).
+        norm: the layer normalization component (optional).
 
     """
 
-    def __init__(self, embed_dim, num_heads, dropout=0., self_attn=False):
-        super(MultiheadAttention, self).__init__()
-        self.embed_dim = embed_dim
-        self.num_heads = num_heads
-        # self.dropout = dropout
-        self.head_dim = embed_dim // num_heads
-        assert self.head_dim * num_heads == self.embed_dim, "embed_dim must be divisible by num_heads"
-        self.scale = self.head_dim**-0.5
-        self.self_attn = self_attn
-        if self_attn:
-            self.qkv = nn.Linear(embed_dim, embed_dim * 3)
-        else:
-            self.q = nn.Linear(embed_dim, embed_dim)
-            self.kv = nn.Linear(embed_dim, embed_dim * 2)
-        self.attn_drop = nn.Dropout(dropout)
-        self.out_proj = nn.Linear(embed_dim, embed_dim)
-
-    def forward(self, query, key=None, attn_mask=None):
-
-        qN = query.shape[1]
-
-        if self.self_attn:
-            qkv = self.qkv(query)
-            qkv = qkv.reshape((qkv.shape[0], qN, 3, self.num_heads, self.head_dim)).permute((2, 0, 3, 1, 4))
-            q, k, v = qkv[0], qkv[1], qkv[2]
-        else:
-            kN = key.shape[1]
-            q = self.q(query)
-            q = q.reshape([q.shape[0], qN, self.num_heads, self.head_dim]).permute([0, 2, 1, 3])
-            kv = self.kv(key)
-            kv = kv.reshape((kv.shape[0], kN, 2, self.num_heads, self.head_dim)).permute((2, 0, 3, 1, 4))
-            k, v = kv[0], kv[1]
+    def __init__(self, decoder_layer, num_layers):
+        super(TransformerDecoder, self).__init__()
+        self.layers = _get_clones(decoder_layer, num_layers)
+        self.num_layers = num_layers
+
+    def forward(self,
+                tgt,
+                memory,
+                tgt_mask=None,
+                memory_mask=None,
+                tgt_key_padding_mask=None,
+                memory_key_padding_mask=None):
+        """Pass the inputs (and mask) through the decoder layer in turn.
+
+        Args:
+            tgt: the sequence to the decoder (required).
+            memory: the sequnce from the last layer of the encoder (required).
+            tgt_mask: the mask for the tgt sequence (optional).
+            memory_mask: the mask for the memory sequence (optional).
+            tgt_key_padding_mask: the mask for the tgt keys per batch (optional).
+            memory_key_padding_mask: the mask for the memory keys per batch (optional).
+        """
+        output = tgt
+        for i in range(self.num_layers):
+            output = self.layers[i](
+                output,
+                memory,
+                tgt_mask=tgt_mask,
+                memory_mask=memory_mask,
+                tgt_key_padding_mask=tgt_key_padding_mask,
+                memory_key_padding_mask=memory_key_padding_mask)
+
+        return output
+
+
+class TransformerEncoderLayer(nn.Module):
+    """TransformerEncoderLayer is made up of self-attn and feedforward network.
+    This standard encoder layer is based on the paper "Attention Is All You Need".
+    Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N Gomez,
+    Lukasz Kaiser, and Illia Polosukhin. 2017. Attention is all you need. In Advances in
+    Neural Information Processing Systems, pages 6000-6010. Users may modify or implement
+    in a different way during application.
 
-        attn = (q.matmul(k.permute((0, 1, 3, 2)))) * self.scale
+    Args:
+        d_model: the number of expected features in the input (required).
+        nhead: the number of heads in the multiheadattention models (required).
+        dim_feedforward: the dimension of the feedforward network model (default=2048).
+        dropout: the dropout value (default=0.1).
 
-        if attn_mask is not None:
-            attn += attn_mask
+    """
 
-        attn = F.softmax(attn, dim=-1)
-        attn = self.attn_drop(attn)
+    def __init__(self,
+                 d_model,
+                 nhead,
+                 dim_feedforward=2048,
+                 attention_dropout_rate=0.0,
+                 residual_dropout_rate=0.1):
+        super(TransformerEncoderLayer, self).__init__()
+        self.self_attn = MultiheadAttention(
+            d_model, nhead, dropout=attention_dropout_rate)
+
+        self.conv1 = nn.Conv2d(
+            in_channels=d_model,
+            out_channels=dim_feedforward,
+            kernel_size=(1, 1))
+        self.conv2 = nn.Conv2d(
+            in_channels=dim_feedforward,
+            out_channels=d_model,
+            kernel_size=(1, 1))
+
+        self.norm1 = LayerNorm(d_model)
+        self.norm2 = LayerNorm(d_model)
+        self.dropout1 = Dropout(residual_dropout_rate)
+        self.dropout2 = Dropout(residual_dropout_rate)
 
-        x = (attn.matmul(v)).permute((0, 2, 1, 3))
-        x = x.reshape((x.shape[0], qN, self.embed_dim))
-        x = self.out_proj(x)
+    def forward(self, src, src_mask=None, src_key_padding_mask=None):
+        """Pass the input through the endocder layer.
+        Args:
+            src: the sequnce to the encoder layer (required).
+            src_mask: the mask for the src sequence (optional).
+            src_key_padding_mask: the mask for the src keys per batch (optional).
+        """
+        src2 = self.self_attn(
+            src,
+            src,
+            src,
+            attn_mask=src_mask,
+            key_padding_mask=src_key_padding_mask)
+        src = src + self.dropout1(src2)
+        src = self.norm1(src)
+
+        src = src.permute(1, 2, 0)
+        src = torch.unsqueeze(src, 2)
+        src2 = self.conv2(F.relu(self.conv1(src)))
+        src2 = torch.squeeze(src2, 2)
+        src2 = src2.permute(2, 0, 1)
+        src = torch.squeeze(src, 2)
+        src = src.permute(2, 0, 1)
+
+        src = src + self.dropout2(src2)
+        src = self.norm2(src)
+        return src
+
+
+class TransformerDecoderLayer(nn.Module):
+    """TransformerDecoderLayer is made up of self-attn, multi-head-attn and feedforward network.
+    This standard decoder layer is based on the paper "Attention Is All You Need".
+    Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N Gomez,
+    Lukasz Kaiser, and Illia Polosukhin. 2017. Attention is all you need. In Advances in
+    Neural Information Processing Systems, pages 6000-6010. Users may modify or implement
+    in a different way during application.
 
-        return x
+    Args:
+        d_model: the number of expected features in the input (required).
+        nhead: the number of heads in the multiheadattention models (required).
+        dim_feedforward: the dimension of the feedforward network model (default=2048).
+        dropout: the dropout value (default=0.1).
 
+    """
 
-class TransformerBlock(nn.Module):
     def __init__(self,
                  d_model,
                  nhead,
                  dim_feedforward=2048,
                  attention_dropout_rate=0.0,
-                 residual_dropout_rate=0.1,
-                 with_self_attn=True,
-                 with_cross_attn=False,
-                 epsilon=1e-5):
-        super(TransformerBlock, self).__init__()
-        self.with_self_attn = with_self_attn
-        if with_self_attn:
-            self.self_attn = MultiheadAttention(
-                d_model,
-                nhead,
-                dropout=attention_dropout_rate,
-                self_attn=with_self_attn)
-            self.norm1 = nn.LayerNorm(d_model, eps=epsilon)
-            self.dropout1 = nn.Dropout(residual_dropout_rate)
-        self.with_cross_attn = with_cross_attn
-        if with_cross_attn:
-            self.cross_attn = MultiheadAttention(  #for self_attn of encoder or cross_attn of decoder
-                d_model,
-                nhead,
-                dropout=attention_dropout_rate)
-            self.norm2 = nn.LayerNorm(d_model, eps=epsilon)
-            self.dropout2 = nn.Dropout(residual_dropout_rate)
-
-        self.mlp = Mlp(in_features=d_model,
-                       hidden_features=dim_feedforward,
-                       act_layer='relu',
-                       drop=residual_dropout_rate)
-
-        self.norm3 = nn.LayerNorm(d_model, eps=epsilon)
-
-        self.dropout3 = nn.Dropout(residual_dropout_rate)
-
-    def forward(self, tgt, memory=None, self_mask=None, cross_mask=None):
-        if self.with_self_attn:
-            tgt1 = self.self_attn(tgt, attn_mask=self_mask)
-            tgt = self.norm1(tgt + self.dropout1(tgt1))
-
-        if self.with_cross_attn:
-            tgt2 = self.cross_attn(tgt, key=memory, attn_mask=cross_mask)
-            tgt = self.norm2(tgt + self.dropout2(tgt2))
-        tgt = self.norm3(tgt + self.dropout3(self.mlp(tgt)))
+                 residual_dropout_rate=0.1):
+        super(TransformerDecoderLayer, self).__init__()
+        self.self_attn = MultiheadAttention(
+            d_model, nhead, dropout=attention_dropout_rate)
+        self.multihead_attn = MultiheadAttention(
+            d_model, nhead, dropout=attention_dropout_rate)
+
+        self.conv1 = nn.Conv2d(
+            in_channels=d_model,
+            out_channels=dim_feedforward,
+            kernel_size=(1, 1))
+        self.conv2 = nn.Conv2d(
+            in_channels=dim_feedforward,
+            out_channels=d_model,
+            kernel_size=(1, 1))
+
+        self.norm1 = LayerNorm(d_model)
+        self.norm2 = LayerNorm(d_model)
+        self.norm3 = LayerNorm(d_model)
+        self.dropout1 = Dropout(residual_dropout_rate)
+        self.dropout2 = Dropout(residual_dropout_rate)
+        self.dropout3 = Dropout(residual_dropout_rate)
+
+    def forward(self,
+                tgt,
+                memory,
+                tgt_mask=None,
+                memory_mask=None,
+                tgt_key_padding_mask=None,
+                memory_key_padding_mask=None):
+        """Pass the inputs (and mask) through the decoder layer.
+
+        Args:
+            tgt: the sequence to the decoder layer (required).
+            memory: the sequnce from the last layer of the encoder (required).
+            tgt_mask: the mask for the tgt sequence (optional).
+            memory_mask: the mask for the memory sequence (optional).
+            tgt_key_padding_mask: the mask for the tgt keys per batch (optional).
+            memory_key_padding_mask: the mask for the memory keys per batch (optional).
+
+        """
+        tgt2 = self.self_attn(
+            tgt,
+            tgt,
+            tgt,
+            attn_mask=tgt_mask,
+            key_padding_mask=tgt_key_padding_mask)
+        tgt = tgt + self.dropout1(tgt2)
+        tgt = self.norm1(tgt)
+        tgt2 = self.multihead_attn(
+            tgt,
+            memory,
+            memory,
+            attn_mask=memory_mask,
+            key_padding_mask=memory_key_padding_mask)
+        tgt = tgt + self.dropout2(tgt2)
+        tgt = self.norm2(tgt)
+
+        # default
+        tgt = tgt.permute(1, 2, 0)
+        tgt = torch.unsqueeze(tgt, 2)
+        tgt2 = self.conv2(F.relu(self.conv1(tgt)))
+        tgt2 = torch.squeeze(tgt2, 2)
+        tgt2 = tgt2.permute(2, 0, 1)
+        tgt = torch.squeeze(tgt, 2)
+        tgt = tgt.permute(2, 0, 1)
+
+        tgt = tgt + self.dropout3(tgt2)
+        tgt = self.norm3(tgt)
         return tgt
 
 
+def _get_clones(module, N):
+    return LayerList([copy.deepcopy(module) for i in range(N)])
+
+
 class PositionalEncoding(nn.Module):
     """Inject some information about the relative or absolute position of the tokens
         in the sequence. The positional encodings have the same dimension as
         the embeddings, so that the two can be summed. Here, we use sine and cosine
         functions of different frequencies.
     .. math::
         \text{PosEncoder}(pos, 2i) = sin(pos/10000^(2i/d_model))
@@ -448,35 +616,34 @@
     def __init__(self, dropout, dim, max_len=5000):
         super(PositionalEncoding, self).__init__()
         self.dropout = nn.Dropout(p=dropout)
 
         pe = torch.zeros([max_len, dim])
         position = torch.arange(0, max_len, dtype=torch.float32).unsqueeze(1)
         div_term = torch.exp(
-            torch.arange(0, dim, 2).float() *
+            torch.arange(0, dim, 2).type(torch.float32) *
             (-math.log(10000.0) / dim))
         pe[:, 0::2] = torch.sin(position * div_term)
         pe[:, 1::2] = torch.cos(position * div_term)
         pe = torch.unsqueeze(pe, 0)
-        pe = torch.permute(pe, [1, 0, 2])
+        pe = pe.permute(1, 0, 2)
         self.register_buffer('pe', pe)
 
     def forward(self, x):
         """Inputs of forward function
         Args:
             x: the sequence fed to the positional encoder model (required).
         Shape:
             x: [sequence length, batch size, embed dim]
             output: [sequence length, batch size, embed dim]
         Examples:
             >>> output = pos_encoder(x)
         """
-        x = x.permute([1, 0, 2])
-        x = x + self.pe[:x.size(0), :]
-        return self.dropout(x).permute([1, 0, 2])
+        x = x + self.pe[:x.shape[0], :]
+        return self.dropout(x)
 
 
 class PositionalEncoding_2d(nn.Module):
     """Inject some information about the relative or absolute position of the tokens
         in the sequence. The positional encodings have the same dimension as
         the embeddings, so that the two can be summed. Here, we use sine and cosine
         functions of different frequencies.
@@ -495,19 +662,19 @@
     def __init__(self, dropout, dim, max_len=5000):
         super(PositionalEncoding_2d, self).__init__()
         self.dropout = nn.Dropout(p=dropout)
 
         pe = torch.zeros([max_len, dim])
         position = torch.arange(0, max_len, dtype=torch.float32).unsqueeze(1)
         div_term = torch.exp(
-            torch.arange(0, dim, 2).float() *
+            torch.arange(0, dim, 2).type(torch.float32) *
             (-math.log(10000.0) / dim))
         pe[:, 0::2] = torch.sin(position * div_term)
         pe[:, 1::2] = torch.cos(position * div_term)
-        pe = torch.permute(torch.unsqueeze(pe, 0), [1, 0, 2])
+        pe = torch.unsqueeze(pe, 0).permute(1, 0, 2)
         self.register_buffer('pe', pe)
 
         self.avg_pool_1 = nn.AdaptiveAvgPool2d((1, 1))
         self.linear1 = nn.Linear(dim, dim)
         self.linear1.weight.data.fill_(1.)
         self.avg_pool_2 = nn.AdaptiveAvgPool2d((1, 1))
         self.linear2 = nn.Linear(dim, dim)
@@ -522,34 +689,33 @@
             output: [sequence length, batch size, embed dim]
         Examples:
             >>> output = pos_encoder(x)
         """
         w_pe = self.pe[:x.shape[-1], :]
         w1 = self.linear1(self.avg_pool_1(x).squeeze()).unsqueeze(0)
         w_pe = w_pe * w1
-        w_pe = torch.permute(w_pe, [1, 2, 0])
+        w_pe = w_pe.permute(1, 2, 0)
         w_pe = torch.unsqueeze(w_pe, 2)
 
         h_pe = self.pe[:x.shape[-2], :]
         w2 = self.linear2(self.avg_pool_2(x).squeeze()).unsqueeze(0)
         h_pe = h_pe * w2
-        h_pe = torch.permute(h_pe, [1, 2, 0])
+        h_pe = h_pe.permute(1, 2, 0)
         h_pe = torch.unsqueeze(h_pe, 3)
 
         x = x + w_pe + h_pe
-        x = torch.permute(
-            torch.reshape(x,
-                           [x.shape[0], x.shape[1], x.shape[2] * x.shape[3]]),
-            [2, 0, 1])
+        x = torch.reshape(
+            x, [x.shape[0], x.shape[1], x.shape[2] * x.shape[3]]
+        ).permute(2,0,1)
 
         return self.dropout(x)
 
 
 class Embeddings(nn.Module):
-    def __init__(self, d_model, vocab, padding_idx=None, scale_embedding=True):
+    def __init__(self, d_model, vocab, padding_idx, scale_embedding):
         super(Embeddings, self).__init__()
         self.embedding = nn.Embedding(vocab, d_model, padding_idx=padding_idx)
         w0 = np.random.normal(0.0, d_model**-0.5,
                               (vocab, d_model)).astype(np.float32)
         self.embedding.weight.data = torch.from_numpy(w0)
         self.d_model = d_model
         self.scale_embedding = scale_embedding
@@ -558,15 +724,15 @@
         if self.scale_embedding:
             x = self.embedding(x)
             return x * math.sqrt(self.d_model)
         return self.embedding(x)
 
 
 class Beam():
-    """ Beam search """
+    ''' Beam search '''
 
     def __init__(self, size, device=False):
 
         self.size = size
         self._done = False
         # The score for each translation on the beam.
         self.scores = torch.zeros((size, ), dtype=torch.float32)
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/heads/rec_sar_head.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_sar_head.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,25 @@
+"""
+This code is refer from:
+https://github.com/open-mmlab/mmocr/blob/main/mmocr/models/textrecog/encoders/sar_encoder.py
+https://github.com/open-mmlab/mmocr/blob/main/mmocr/models/textrecog/decoders/sar_decoder.py
+"""
+
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
+# import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+# import paddle
+# from paddle import ParamAttr
+# import paddle.nn as nn
+# import paddle.nn.functional as F
 
 
 class SAREncoder(nn.Module):
     """
     Args:
         enc_bi_rnn (bool): If True, use bidirectional RNN in encoder.
         enc_drop_rnn (float): Dropout probability of RNN layer in encoder.
@@ -60,26 +75,28 @@
         if img_metas is not None:
             assert len(img_metas[0]) == feat.size(0)
 
         valid_ratios = None
         if img_metas is not None and self.mask:
             valid_ratios = img_metas[-1]
 
-        h_feat = feat.size(2)  # bsz c h w
+        h_feat = feat.shape[2]  # bsz c h w
         feat_v = F.max_pool2d(
             feat, kernel_size=(h_feat, 1), stride=1, padding=0)
-
         feat_v = feat_v.squeeze(2)  # bsz * C * W
         feat_v = feat_v.permute(0, 2, 1).contiguous()  # bsz * W * C
         holistic_feat = self.rnn_encoder(feat_v)[0]  # bsz * T * C
+
         if valid_ratios is not None:
             valid_hf = []
             T = holistic_feat.size(1)
             for i in range(valid_ratios.size(0)):
-                valid_step = torch.minimum(torch.tensor(T), torch.ceil(T * valid_ratios[i]).int()) - 1
+                valid_step = torch.min(T, torch.ceil(T * valid_ratios[i])) - 1
+                # valid_step = paddle.minimum(
+                #     T, paddle.ceil(valid_ratios[i] * T).astype('int32')) - 1
                 valid_hf.append(holistic_feat[i, valid_step, :])
             valid_hf = torch.stack(valid_hf, dim=0)
         else:
             valid_hf = holistic_feat[:, -1, :]  # bsz * C
         holistic_feat = self.linear(valid_hf)  # bsz * C
 
         return holistic_feat
@@ -203,14 +220,15 @@
                       valid_ratios=None):
 
         y = self.rnn_decoder(decoder_input)[0]
         # y: bsz * (seq_len + 1) * hidden_size
 
         attn_query = self.conv1x1_1(y)  # bsz * (seq_len + 1) * attn_size
         bsz, seq_len, attn_size = attn_query.shape
+        # attn_query = paddle.unsqueeze(attn_query, axis=[3, 4])
         attn_query = attn_query.view(bsz, seq_len, attn_size, 1, 1)
         # attn_query = attn_query.unsqueeze(3).unsqueeze(4)
         # (bsz, seq_len + 1, attn_size, 1, 1)
 
         attn_key = self.conv3x3_1(feat)
         # bsz * attn_size * h * w
         attn_key = attn_key.unsqueeze(1)
@@ -225,18 +243,21 @@
         # bsz * (seq_len + 1) * h * w * 1
         bsz, T, h, w, c = attn_weight.size()
         assert c == 1
 
         if valid_ratios is not None:
             # cal mask of attention weight
             for i in range(valid_ratios.size(0)):
-                valid_width = torch.minimum(torch.tensor(w), torch.ceil(w * valid_ratios[i]).int())
+                valid_width = torch.min(w, torch.ceil(w * valid_ratios[i]))
+                # valid_width = paddle.minimum(
+                #     w, paddle.ceil(valid_ratios[i] * w).astype("int32"))
                 if valid_width < w:
                     attn_weight[i, :, :, valid_width:, :] = float('-inf')
 
+        # attn_weight = paddle.reshape(attn_weight, [bsz, T, -1])
         attn_weight = attn_weight.view(bsz, T, -1)
         attn_weight = F.softmax(attn_weight, dim=-1)
 
         attn_weight = attn_weight.view(bsz, T, h, w,
                                        c).permute(0, 1, 4, 2, 3).contiguous()
         # attn_weight: bsz * T * c * h * w
         # feat: bsz * c * h * w
@@ -356,26 +377,27 @@
             d_model=in_channels,
             d_enc=enc_dim,
             d_k=d_k,
             pred_dropout=pred_dropout,
             max_text_length=max_text_length,
             pred_concat=pred_concat)
 
-    def forward(self, feat, data=None):
+    def forward(self, feat, targets=None):
         '''
         img_metas: [label, valid_ratio]
         '''
-        holistic_feat = self.encoder(feat, data)  # bsz c
+        holistic_feat = self.encoder(feat, targets)  # bsz c
+
         if self.training:
-            label = data[0]  # label
+            label = targets[0]  # label
             final_out = self.decoder(
-                feat, holistic_feat, label, img_metas=data)
+                feat, holistic_feat, label, img_metas=targets)
         else:
             final_out = self.decoder(
                 feat,
                 holistic_feat,
                 label=None,
-                img_metas=data,
+                img_metas=targets,
                 train_mode=False)
             # (bsz, seq_len, num_classes)
 
-        return {'res': final_out}
+        return final_out
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/necks/db_fpn.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/db_fpn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+import os, sys
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ..common import Activation
 from ..backbones.det_mobilenet_v3 import SEModule
 from ..necks.intracl import IntraCLBlock
 
+def hard_swish(x, inplace=True):
+    return x * F.relu6(x + 3., inplace=inplace) / 6.
+
 class DSConv(nn.Module):
     def __init__(self,
                  in_channels,
                  out_channels,
                  kernel_size,
                  padding,
                  stride=1,
                  groups=None,
+                 if_act=True,
                  act="relu",
                  **kwargs):
         super(DSConv, self).__init__()
         if groups == None:
             groups = in_channels
+        self.if_act = if_act
         self.act = act
         self.conv1 = nn.Conv2d(
             in_channels=in_channels,
             out_channels=in_channels,
             kernel_size=kernel_size,
             stride=stride,
             padding=padding,
@@ -49,26 +54,31 @@
         if in_channels != out_channels:
             self.conv_end = nn.Conv2d(
                 in_channels=in_channels,
                 out_channels=out_channels,
                 kernel_size=1,
                 stride=1,
                 bias=False)
-        self.act = None
-        if act:
-            self.act = Activation(act)
+
     def forward(self, inputs):
 
         x = self.conv1(inputs)
         x = self.bn1(x)
 
         x = self.conv2(x)
         x = self.bn2(x)
-        if self.act:
-            x = self.act(x)
+        if self.if_act:
+            if self.act == "relu":
+                x = F.relu(x)
+            elif self.act == "hardswish":
+                x = hard_swish(x)
+            else:
+                print("The activation function({}) is selected incorrectly.".
+                      format(self.act))
+                exit()
 
         x = self.conv3(x)
         if self._c[0] != self._c[1]:
             x = x + self.conv_end(inputs)
         return x
 
 
@@ -181,14 +191,21 @@
 
 class RSEFPN(nn.Module):
     def __init__(self, in_channels, out_channels, shortcut=True, **kwargs):
         super(RSEFPN, self).__init__()
         self.out_channels = out_channels
         self.ins_conv = nn.ModuleList()
         self.inp_conv = nn.ModuleList()
+        self.intracl = False
+        if 'intracl' in kwargs.keys() and kwargs['intracl'] is True:
+            self.intracl = kwargs['intracl']
+            self.incl1 = IntraCLBlock(self.out_channels // 4, reduce_factor=2)
+            self.incl2 = IntraCLBlock(self.out_channels // 4, reduce_factor=2)
+            self.incl3 = IntraCLBlock(self.out_channels // 4, reduce_factor=2)
+            self.incl4 = IntraCLBlock(self.out_channels // 4, reduce_factor=2)
 
         for i in range(len(in_channels)):
             self.ins_conv.append(
                 RSELayer(
                     in_channels[i],
                     out_channels,
                     kernel_size=1,
@@ -204,29 +221,35 @@
         c2, c3, c4, c5 = x
 
         in5 = self.ins_conv[3](c5)
         in4 = self.ins_conv[2](c4)
         in3 = self.ins_conv[1](c3)
         in2 = self.ins_conv[0](c2)
 
-        out4 = in4 + F.upsample(
+        out4 = in4 + F.interpolate(
             in5, scale_factor=2, mode="nearest")  # 1/16
-        out3 = in3 + F.upsample(
+        out3 = in3 + F.interpolate(
             out4, scale_factor=2, mode="nearest")  # 1/8
-        out2 = in2 + F.upsample(
+        out2 = in2 + F.interpolate(
             out3, scale_factor=2, mode="nearest")  # 1/4
 
         p5 = self.inp_conv[3](in5)
         p4 = self.inp_conv[2](out4)
         p3 = self.inp_conv[1](out3)
         p2 = self.inp_conv[0](out2)
 
-        p5 = F.upsample(p5, scale_factor=8, mode="nearest")
-        p4 = F.upsample(p4, scale_factor=4, mode="nearest")
-        p3 = F.upsample(p3, scale_factor=2, mode="nearest")
+        if self.intracl is True:
+            p5 = self.incl4(p5)
+            p4 = self.incl3(p4)
+            p3 = self.incl2(p3)
+            p2 = self.incl1(p2)
+
+        p5 = F.interpolate(p5, scale_factor=8, mode="nearest")
+        p4 = F.interpolate(p4, scale_factor=4, mode="nearest")
+        p3 = F.interpolate(p3, scale_factor=2, mode="nearest")
 
         fuse = torch.cat([p5, p4, p3, p2], dim=1)
         return fuse
 
 
 class LKPAN(nn.Module):
     def __init__(self, in_channels, out_channels, mode='large', **kwargs):
@@ -276,34 +299,35 @@
             self.pan_lat_conv.append(
                 p_layer(
                     in_channels=self.out_channels // 4,
                     out_channels=self.out_channels // 4,
                     kernel_size=9,
                     padding=4,
                     bias=False))
-        self.intracl = False
-        if 'intracl' in kwargs.keys() and kwargs['intracl'] is True:
-            self.intracl = kwargs['intracl']
-            self.incl1 = IntraCLBlock(self.out_channels // 4, reduce_factor=2)
-            self.incl2 = IntraCLBlock(self.out_channels // 4, reduce_factor=2)
-            self.incl3 = IntraCLBlock(self.out_channels // 4, reduce_factor=2)
-            self.incl4 = IntraCLBlock(self.out_channels // 4, reduce_factor=2)
+            self.intracl = False
+            if 'intracl' in kwargs.keys() and kwargs['intracl'] is True:
+                self.intracl = kwargs['intracl']
+                self.incl1 = IntraCLBlock(self.out_channels // 4, reduce_factor=2)
+                self.incl2 = IntraCLBlock(self.out_channels // 4, reduce_factor=2)
+                self.incl3 = IntraCLBlock(self.out_channels // 4, reduce_factor=2)
+                self.incl4 = IntraCLBlock(self.out_channels // 4, reduce_factor=2)
+
     def forward(self, x):
         c2, c3, c4, c5 = x
 
         in5 = self.ins_conv[3](c5)
         in4 = self.ins_conv[2](c4)
         in3 = self.ins_conv[1](c3)
         in2 = self.ins_conv[0](c2)
 
-        out4 = in4 + F.upsample(
+        out4 = in4 + F.interpolate(
             in5, scale_factor=2, mode="nearest")  # 1/16
-        out3 = in3 + F.upsample(
+        out3 = in3 + F.interpolate(
             out4, scale_factor=2, mode="nearest")  # 1/8
-        out2 = in2 + F.upsample(
+        out2 = in2 + F.interpolate(
             out3, scale_factor=2, mode="nearest")  # 1/4
 
         f5 = self.inp_conv[3](in5)
         f4 = self.inp_conv[2](out4)
         f3 = self.inp_conv[1](out3)
         f2 = self.inp_conv[0](out2)
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/necks/intracl.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/intracl.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/necks/rnn.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/rnn.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 import os, sys
 import torch
 import torch.nn as nn
-from ..backbones.rec_svtrnet import Block, ConvBNLayer
+from ...modeling.backbones.rec_svtrnet import Block, ConvBNLayer
 
 class Im2Seq(nn.Module):
     def __init__(self, in_channels, **kwargs):
         super().__init__()
         self.out_channels = in_channels
 
     def forward(self, x):
         B, C, H, W = x.shape
-        assert H == 1
+        # assert H == 1
         x = x.squeeze(dim=2)
-        x = x.permute(0, 2, 1)
+        # x = x.transpose([0, 2, 1])  # paddle (NTC)(batch, width, channels)
+        x = x.permute(0,2,1)
         return x
 
 
+class EncoderWithRNN_(nn.Module):
+    def __init__(self, in_channels, hidden_size):
+        super(EncoderWithRNN_, self).__init__()
+        self.out_channels = hidden_size * 2
+        self.rnn1 = nn.LSTM(in_channels, hidden_size, bidirectional=False, batch_first=True, num_layers=2)
+        self.rnn2 = nn.LSTM(in_channels, hidden_size, bidirectional=False, batch_first=True, num_layers=2)
+
+    def forward(self, x):
+        self.rnn1.flatten_parameters()
+        self.rnn2.flatten_parameters()
+        out1, h1 = self.rnn1(x)
+        out2, h2 = self.rnn2(torch.flip(x, [1]))
+        return torch.cat([out1, torch.flip(out2, [1])], 2)
+
+
 class EncoderWithRNN(nn.Module):
     def __init__(self, in_channels, hidden_size):
         super(EncoderWithRNN, self).__init__()
         self.out_channels = hidden_size * 2
         self.lstm = nn.LSTM(
             in_channels, hidden_size, num_layers=2, batch_first=True, bidirectional=True) # batch_first:=True
 
@@ -51,17 +67,17 @@
             depth=2,
             hidden_dims=120,
             use_guide=False,
             num_heads=8,
             qkv_bias=True,
             mlp_ratio=2.0,
             drop_rate=0.1,
+            kernel_size=[3,3],
             attn_drop_rate=0.1,
             drop_path=0.,
-            kernel_size=[3, 3],
             qk_scale=None):
         super(EncoderWithSVTR, self).__init__()
         self.depth = depth
         self.use_guide = use_guide
         self.conv1 = ConvBNLayer(
             in_channels,
             in_channels // 8,
@@ -89,58 +105,68 @@
                 prenorm=False) for i in range(depth)
         ])
         self.norm = nn.LayerNorm(hidden_dims, eps=1e-6)
         self.conv3 = ConvBNLayer(
             hidden_dims, in_channels, kernel_size=1, act='swish')
         # last conv-nxn, the input is concat of input tensor and conv3 output tensor
         self.conv4 = ConvBNLayer(
-            2 * in_channels,
-            in_channels // 8,
-            kernel_size=kernel_size,
-            padding=[kernel_size[0] // 2, kernel_size[1] // 2],
-            act='swish')
+            2 * in_channels, in_channels // 8, padding=1, act='swish')
 
         self.conv1x1 = ConvBNLayer(
             in_channels // 8, dims, kernel_size=1, act='swish')
         self.out_channels = dims
         self.apply(self._init_weights)
 
     def _init_weights(self, m):
-        if isinstance(m, nn.Linear):
-            nn.init.trunc_normal_(m.weight)
-            if isinstance(m, nn.Linear) and m.bias is not None:
+        # weight initialization
+        if isinstance(m, nn.Conv2d):
+            nn.init.kaiming_normal_(m.weight, mode='fan_out')
+            if m.bias is not None:
+                nn.init.zeros_(m.bias)
+        elif isinstance(m, nn.BatchNorm2d):
+            nn.init.ones_(m.weight)
+            nn.init.zeros_(m.bias)
+        elif isinstance(m, nn.Linear):
+            nn.init.normal_(m.weight, 0, 0.01)
+            if m.bias is not None:
+                nn.init.zeros_(m.bias)
+        elif isinstance(m, nn.ConvTranspose2d):
+            nn.init.kaiming_normal_(m.weight, mode='fan_out')
+            if m.bias is not None:
                 nn.init.zeros_(m.bias)
         elif isinstance(m, nn.LayerNorm):
             nn.init.ones_(m.weight)
             nn.init.zeros_(m.bias)
 
-
     def forward(self, x):
         # for use guide
         if self.use_guide:
             z = x.clone()
             z.stop_gradient = True
         else:
             z = x
-        # for shortcut
+        # for short cut
         h = z
         # reduce dim
         z = self.conv1(z)
         z = self.conv2(z)
         # SVTR global block
         B, C, H, W = z.shape
-        z = z.flatten(2).permute([0, 2, 1])
+        z = z.flatten(2).permute(0, 2, 1)
+
         for blk in self.svtr_block:
             z = blk(z)
+
         z = self.norm(z)
         # last stage
-        z = z.reshape([-1, H, W, C]).permute([0, 3, 1, 2])
+        z = z.reshape([-1, H, W, C]).permute(0, 3, 1, 2)
         z = self.conv3(z)
         z = torch.cat((h, z), dim=1)
         z = self.conv1x1(self.conv4(z))
+
         return z
 
 
 class SequenceEncoder(nn.Module):
     def __init__(self, in_channels, encoder_type, hidden_size=48, **kwargs):
         super(SequenceEncoder, self).__init__()
         self.encoder_reshape = Im2Seq(in_channels)
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/modeling/transforms/tps.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/tps.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,54 @@
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
 import math
+import os, sys
 import torch
-from torch import nn
-from torch.nn import functional as F
-
-from ..common import Activation
+import torch.nn as nn
+import torch.nn.functional as F
+from ...modeling.common import Activation
+# import paddle
+# from paddle import nn, ParamAttr
+# from paddle.nn import functional as F
 import numpy as np
 
 
 class ConvBNLayer(nn.Module):
     def __init__(self,
                  in_channels,
                  out_channels,
                  kernel_size,
                  stride=1,
                  groups=1,
-                 act=None):
+                 act=None,
+                 name=None):
         super(ConvBNLayer, self).__init__()
         self.conv = nn.Conv2d(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=kernel_size,
             stride=stride,
             padding=(kernel_size - 1) // 2,
             groups=groups,
-            bias=False)
-        self.bn = nn.BatchNorm2d(out_channels)
-        self.act = Activation(act) if act else None
+            bias=False,
+        )
+        bn_name = "bn_" + name
+        self.bn = nn.BatchNorm2d(
+            out_channels, )
+        self.act = act
+        if act is not None:
+            self._act = Activation(act)
 
     def forward(self, x):
         x = self.conv(x)
         x = self.bn(x)
         if self.act is not None:
-            x = self.act(x)
+            x = self._act(x)
         return x
 
 
 class LocalizationNetwork(nn.Module):
     def __init__(self, in_channels, num_fiducial, loc_lr, model_name):
         super(LocalizationNetwork, self).__init__()
         self.F = num_fiducial
@@ -43,48 +56,73 @@
         if model_name == "large":
             num_filters_list = [64, 128, 256, 512]
             fc_dim = 256
         else:
             num_filters_list = [16, 32, 64, 128]
             fc_dim = 64
 
-        self.block_list = nn.ModuleList()
+        # self.block_list = []
+        self.block_list = nn.Sequential()
         for fno in range(0, len(num_filters_list)):
             num_filters = num_filters_list[fno]
+            name = "loc_conv%d" % fno
+            # conv = self.add_sublayer(
+            #     name,
+            #     ConvBNLayer(
+            #         in_channels=in_channels,
+            #         out_channels=num_filters,
+            #         kernel_size=3,
+            #         act='relu',
+            #         name=name))
             conv = ConvBNLayer(
                     in_channels=in_channels,
                     out_channels=num_filters,
                     kernel_size=3,
-                    act='relu')
-            self.block_list.append(conv)
+                    act='relu',
+                    name=name)
+            # self.block_list.append(conv)
+            self.block_list.add_module(name, conv)
             if fno == len(num_filters_list) - 1:
                 pool = nn.AdaptiveAvgPool2d(1)
             else:
+                # pool = nn.MaxPool2D(kernel_size=2, stride=2, padding=0)
                 pool = nn.MaxPool2d(kernel_size=2, stride=2, padding=0)
             in_channels = num_filters
-            self.block_list.append(pool)
-        self.fc1 = nn.Linear(in_channels, fc_dim)
+            # self.block_list.append(pool)
+            self.block_list.add_module('{}_pool'.format(name), pool)
+        name = "loc_fc1"
+        stdv = 1.0 / math.sqrt(num_filters_list[-1] * 1.0)
+        self.fc1 = nn.Linear(
+            in_channels,
+            fc_dim,
+            bias=True,
+        )
 
-        # Init fc2 in LocalizationNetwork
-        self.fc2 = nn.Linear(fc_dim,F * 2)
 
+        # Init fc2 in LocalizationNetwork
         initial_bias = self.get_initial_fiducials()
         initial_bias = initial_bias.reshape(-1)
-        self.fc2.bias.data = torch.tensor(initial_bias, dtype=torch.float32)
-        nn.init.zeros_(self.fc2.weight.data)
+        name = "loc_fc2"
+        self.fc2 = nn.Linear(
+            fc_dim,
+            F * 2,
+            bias=True
+        )
         self.out_channels = F * 2
 
     def forward(self, x):
         """
            Estimating parameters of geometric transformation
            Args:
                image: input
            Return:
                batch_C_prime: the matrix of the geometric transformation
         """
+        B = x.shape[0]
+        i = 0
         for block in self.block_list:
             x = block(x)
         x = x.squeeze(dim=2).squeeze(dim=2)
         x = self.fc1(x)
 
         x = F.relu(x)
         x = self.fc2(x)
@@ -105,41 +143,50 @@
 
 class GridGenerator(nn.Module):
     def __init__(self, in_channels, num_fiducial):
         super(GridGenerator, self).__init__()
         self.eps = 1e-6
         self.F = num_fiducial
 
-        self.fc = nn.Linear(in_channels,6)
-        nn.init.constant_(self.fc.weight, 0)
-        nn.init.constant_(self.fc.bias, 0)
-        self.fc.weight.requires_grad = False
-        self.fc.bias.requires_grad = False
+        name = "ex_fc"
+        self.fc = nn.Linear(
+            in_channels,
+            6,
+            bias=True
+        )
 
     def forward(self, batch_C_prime, I_r_size):
         """
         Generate the grid for the grid_sampler.
         Args:
             batch_C_prime: the matrix of the geometric transformation
             I_r_size: the shape of the input image
         Return:
             batch_P_prime: the grid for the grid_sampler
         """
         C = self.build_C_paddle()
         P = self.build_P_paddle(I_r_size)
 
-        inv_delta_C_tensor = self.build_inv_delta_C_paddle(C).float()
-        P_hat_tensor = self.build_P_hat_paddle(C, torch.tensor(P)).float()
+        inv_delta_C_tensor = self.build_inv_delta_C_paddle(C).type(torch.float32)
+        P_hat_tensor = self.build_P_hat_paddle(
+            C, torch.as_tensor(P)).type(torch.float32)
+
+        inv_delta_C_tensor.stop_gradient = True
+        P_hat_tensor.stop_gradient = True
 
         batch_C_ex_part_tensor = self.get_expand_tensor(batch_C_prime)
-        
+
+        batch_C_ex_part_tensor.stop_gradient = True
+
         batch_C_prime_with_zeros = torch.cat(
             [batch_C_prime, batch_C_ex_part_tensor], dim=1)
-        batch_T = torch.matmul(inv_delta_C_tensor.to(batch_C_prime_with_zeros.device), batch_C_prime_with_zeros)
-        batch_P_prime = torch.matmul(P_hat_tensor.to(batch_T.device), batch_T)
+        inv_delta_C_tensor = inv_delta_C_tensor.to(batch_C_prime_with_zeros.device)
+        batch_T = torch.matmul(inv_delta_C_tensor, batch_C_prime_with_zeros)
+        P_hat_tensor = P_hat_tensor.to(batch_T.device)
+        batch_P_prime = torch.matmul(P_hat_tensor, batch_T)
         return batch_P_prime
 
     def build_C_paddle(self):
         """ Return coordinates of fiducial points in I_r; C """
         F = self.F
         ctrl_pts_x = torch.linspace(-1.0, 1.0, int(F / 2), dtype=torch.float64)
         ctrl_pts_y_top = -1 * torch.ones([int(F / 2)], dtype=torch.float64)
@@ -148,74 +195,84 @@
         ctrl_pts_bottom = torch.stack([ctrl_pts_x, ctrl_pts_y_bottom], dim=1)
         C = torch.cat([ctrl_pts_top, ctrl_pts_bottom], dim=0)
         return C  # F x 2
 
     def build_P_paddle(self, I_r_size):
         I_r_height, I_r_width = I_r_size
         I_r_grid_x = (torch.arange(
-            -I_r_width, I_r_width, 2) + 1.0
-                      ) / torch.tensor(np.array([I_r_width]))
+            -I_r_width, I_r_width, 2, dtype=torch.float64) + 1.0
+                      ) / torch.as_tensor(np.array([I_r_width]).astype(np.float64))
 
         I_r_grid_y = (torch.arange(
-            -I_r_height, I_r_height, 2) + 1.0
-                      ) / torch.tensor(np.array([I_r_height]))
+            -I_r_height, I_r_height, 2, dtype=torch.float64) + 1.0
+                      ) / torch.as_tensor(np.array([I_r_height]).astype(np.float64))
 
         # P: self.I_r_width x self.I_r_height x 2
-        P = torch.stack(torch.meshgrid(I_r_grid_x, I_r_grid_y), dim=2)
-        P = torch.permute(P, [1, 0, 2])
+        P = torch.stack(torch.meshgrid([I_r_grid_x, I_r_grid_y]), dim=2)
+        # P = paddle.transpose(P, perm=[1, 0, 2])
+        P = P.permute(1, 0, 2)
         # n (= self.I_r_width x self.I_r_height) x 2
         return P.reshape([-1, 2])
 
     def build_inv_delta_C_paddle(self, C):
         """ Return inv_delta_C which is needed to calculate T """
         F = self.F
-        hat_eye = torch.eye(F)  # F x F
-        hat_C = torch.norm(
-            C.reshape([1, F, 2]) - C.reshape([F, 1, 2]), dim=2) + hat_eye
+        hat_C = torch.zeros((F, F), dtype=torch.float64)  # F x F
+        for i in range(0, F):
+            for j in range(i, F):
+                if i == j:
+                    hat_C[i, j] = 1
+                else:
+                    r = torch.norm(C[i] - C[j])
+                    hat_C[i, j] = r
+                    hat_C[j, i] = r
         hat_C = (hat_C**2) * torch.log(hat_C)
         delta_C = torch.cat(  # F+3 x F+3
             [
                 torch.cat(
                     [torch.ones(
-                        (F, 1)), C, hat_C], dim=1),  # F x F+3
-                torch.concat(
+                        (F, 1), dtype=torch.float64), C, hat_C], dim=1),  # F x F+3
+                torch.cat(
                     [
                         torch.zeros(
-                            (2, 3)), C.transpose(0,1)
+                            (2, 3), dtype=torch.float64), C.permute(1,0)
                     ],
                     dim=1),  # 2 x F+3
-                torch.concat(
+                torch.cat(
                     [
                         torch.zeros(
-                            (1, 3)), torch.ones(
-                                (1, F))
+                            (1, 3), dtype=torch.float64), torch.ones(
+                                (1, F), dtype=torch.float64)
                     ],
                     dim=1)  # 1 x F+3
             ],
-            axis=0)
+            dim=0)
         inv_delta_C = torch.inverse(delta_C)
         return inv_delta_C  # F+3 x F+3
 
     def build_P_hat_paddle(self, C, P):
         F = self.F
         eps = self.eps
         n = P.shape[0]  # n (= self.I_r_width x self.I_r_height)
         # P_tile: n x 2 -> n x 1 x 2 -> n x F x 2
-        P_tile = torch.tile(torch.unsqueeze(P, dim=1), (1, F, 1))
+        # P_tile = paddle.tile(paddle.unsqueeze(P, axis=1), (1, F, 1))
+        P_tile = torch.unsqueeze(P, dim=1).repeat(1, F, 1)
         C_tile = torch.unsqueeze(C, dim=0)  # 1 x F x 2
         P_diff = P_tile - C_tile  # n x F x 2
         # rbf_norm: n x F
         rbf_norm = torch.norm(P_diff, p=2, dim=2, keepdim=False)
 
         # rbf: n x F
-        rbf = torch.multiply(
-            torch.square(rbf_norm), torch.log(rbf_norm + eps))
+        # rbf = torch.mul(
+        #     torch.square(rbf_norm), torch.log(rbf_norm + eps))
+        rbf = torch.mul(
+            rbf_norm**2, torch.log(rbf_norm + eps))
         P_hat = torch.cat(
             [torch.ones(
-                (n, 1)), P, rbf], dim=1)
+                (n, 1), dtype=torch.float64), P, rbf], dim=1)
         return P_hat  # n x F+3
 
     def get_expand_tensor(self, batch_C_prime):
         B, H, C = batch_C_prime.shape
         batch_C_prime = batch_C_prime.reshape([B, H * C])
         batch_C_ex_part_tensor = self.fc(batch_C_prime)
         batch_C_ex_part_tensor = batch_C_ex_part_tensor.reshape([-1, 3, 2])
@@ -233,18 +290,12 @@
 
     def forward(self, image):
         image.stop_gradient = False
         batch_C_prime = self.loc_net(image)
         batch_P_prime = self.grid_generator(batch_C_prime, image.shape[2:])
         batch_P_prime = batch_P_prime.reshape(
             [-1, image.shape[2], image.shape[3], 2])
-        is_fp16 = False
-        if batch_P_prime.dtype != torch.float32:
-            data_type = batch_P_prime.dtype
-            image = image.float()
-            batch_P_prime = batch_P_prime.float()
-            is_fp16 = True
-        batch_I_r = F.grid_sample(image, grid=batch_P_prime)
-        if is_fp16:
-            batch_I_r = batch_I_r.astype(data_type)
-        
+        if torch.__version__ < '1.3.0':
+            batch_I_r = F.grid_sample(image, grid=batch_P_prime)
+        else:
+            batch_I_r = F.grid_sample(image, grid=batch_P_prime, align_corners=True)
         return batch_I_r
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/__init__.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,40 @@
-
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
 import copy
 
 __all__ = ['build_post_process']
 
-from .db_postprocess import DBPostProcess, DistillationDBPostProcess
-from .east_postprocess import EASTPostProcess
-from .sast_postprocess import SASTPostProcess
-from .fce_postprocess import FCEPostProcess
-from .rec_postprocess import CTCLabelDecode, AttnLabelDecode, SRNLabelDecode, \
-    DistillationCTCLabelDecode, NRTRLabelDecode, SARLabelDecode, \
-    SEEDLabelDecode, PRENLabelDecode, ViTSTRLabelDecode, ABINetLabelDecode, \
-    SPINLabelDecode, VLLabelDecode, RFLLabelDecode, SATRNLabelDecode
-from .cls_postprocess import ClsPostProcess
-from .pg_postprocess import PGPostProcess
-from .table_postprocess import TableMasterLabelDecode, TableLabelDecode
-from .picodet_postprocess import PicoDetPostProcess
-from .ct_postprocess import CTPostProcess
-from .drrg_postprocess import DRRGPostprocess
-from .rec_postprocess import CANLabelDecode
-
 
 def build_post_process(config, global_config=None):
+    from .db_postprocess import DBPostProcess
+    from .east_postprocess import EASTPostProcess
+    from .sast_postprocess import SASTPostProcess
+    from .fce_postprocess import FCEPostProcess
+    from .rec_postprocess import CTCLabelDecode, AttnLabelDecode, SRNLabelDecode, TableLabelDecode, \
+        NRTRLabelDecode, SARLabelDecode, ViTSTRLabelDecode, RFLLabelDecode
+    from .cls_postprocess import ClsPostProcess
+    from .pg_postprocess import PGPostProcess
+    from .rec_postprocess import CANLabelDecode
+
     support_dict = [
-        'DBPostProcess', 'EASTPostProcess', 'SASTPostProcess', 'FCEPostProcess',
-        'CTCLabelDecode', 'AttnLabelDecode', 'ClsPostProcess', 'SRNLabelDecode',
-        'PGPostProcess', 'DistillationCTCLabelDecode', 'TableLabelDecode',
-        'DistillationDBPostProcess', 'NRTRLabelDecode', 'SARLabelDecode',
-        'SEEDLabelDecode', 'VQASerTokenLayoutLMPostProcess',
-        'VQAReTokenLayoutLMPostProcess', 'PRENLabelDecode',
-        'DistillationSARLabelDecode', 'ViTSTRLabelDecode', 'ABINetLabelDecode',
-        'TableMasterLabelDecode', 'SPINLabelDecode',
-        'DistillationSerPostProcess', 'DistillationRePostProcess',
-        'VLLabelDecode', 'PicoDetPostProcess', 'CTPostProcess',
-        'RFLLabelDecode', 'DRRGPostprocess', 'CANLabelDecode',
-        'SATRNLabelDecode'
+        'DBPostProcess', 'EASTPostProcess', 'SASTPostProcess', 'CTCLabelDecode',
+        'AttnLabelDecode', 'ClsPostProcess', 'SRNLabelDecode', 'PGPostProcess',
+        'TableLabelDecode', 'NRTRLabelDecode', 'SARLabelDecode', 'FCEPostProcess',
+        'ViTSTRLabelDecode', 'CANLabelDecode', 'RFLLabelDecode'
     ]
 
     if config['name'] == 'PSEPostProcess':
         from .pse_postprocess import PSEPostProcess
         support_dict.append('PSEPostProcess')
 
     config = copy.deepcopy(config)
     module_name = config.pop('name')
-    if module_name == "None":
-        return
     if global_config is not None:
         config.update(global_config)
     assert module_name in support_dict, Exception(
-        'post process only support {}'.format(support_dict))
+        'post process only support {}, but got {}'.format(support_dict, module_name))
     module_class = eval(module_name)(**config)
     return module_class
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/cls_postprocess.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/cls_postprocess.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 import torch
 
 
 class ClsPostProcess(object):
     """ Convert between text-label and text-index """
 
-    def __init__(self, label_list=None, **kwargs):
+    def __init__(self, label_list, **kwargs):
         super(ClsPostProcess, self).__init__()
         self.label_list = label_list
 
-    def __call__(self, preds, batch=None, *args, **kwargs):
-        if 'res' in preds:
-            preds = preds['res']
+    def __call__(self, preds, label=None, *args, **kwargs):
         if isinstance(preds, torch.Tensor):
-            preds = preds.detach().cpu().numpy()
-
-        label_list = self.label_list
-        if label_list is None:
-            label_list = {idx: idx for idx in range(preds.shape[-1])}
-
+            preds = preds.cpu().numpy()
         pred_idxs = preds.argmax(axis=1)
-        decode_out = [(label_list[idx], preds[i, idx]) for i, idx in enumerate(pred_idxs)]
-        if batch is None:
+        decode_out = [(self.label_list[idx], preds[i, idx])
+                      for i, idx in enumerate(pred_idxs)]
+        if label is None:
             return decode_out
-        label = [(label_list[idx], 1.0) for idx in batch[1].cpu().numpy()]
-        return decode_out, label
+        label = [(self.label_list[idx], 1.0) for idx in label]
+        return decode_out, label
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/ct_postprocess.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/locality_aware_nms.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,129 +1,199 @@
+"""
+Locality aware nms.
+"""
+
 import numpy as np
-import cv2
-import torch
+from shapely.geometry import Polygon
+
+
+def intersection(g, p):
+    """
+    Intersection.
+    """
+    g = Polygon(g[:8].reshape((4, 2)))
+    p = Polygon(p[:8].reshape((4, 2)))
+    g = g.buffer(0)
+    p = p.buffer(0)
+    if not g.is_valid or not p.is_valid:
+        return 0
+    inter = Polygon(g).intersection(Polygon(p)).area
+    union = g.area + p.area - inter
+    if union == 0:
+        return 0
+    else:
+        return inter / union
+
+
+def intersection_iog(g, p):
+    """
+    Intersection_iog.
+    """
+    g = Polygon(g[:8].reshape((4, 2)))
+    p = Polygon(p[:8].reshape((4, 2)))
+    if not g.is_valid or not p.is_valid:
+        return 0
+    inter = Polygon(g).intersection(Polygon(p)).area
+    #union = g.area + p.area - inter
+    union = p.area
+    if union == 0:
+        print("p_area is very small")
+        return 0
+    else:
+        return inter / union
 
 
-class CTPostProcess(object):
+def weighted_merge(g, p):
     """
-    The post process for Centripetal Text (CT).
+    Weighted merge.
     """
+    g[:8] = (g[8] * g[:8] + p[8] * p[:8]) / (g[8] + p[8])
+    g[8] = (g[8] + p[8])
+    return g
 
-    def __init__(self, min_score=0.88, min_area=16, box_type='poly', **kwargs):
-        self.min_score = min_score
-        self.min_area = min_area
-        self.box_type = box_type
-
-        self.coord = np.zeros((2, 300, 300), dtype=np.int32)
-        for i in range(300):
-            for j in range(300):
-                self.coord[0, i, j] = j
-                self.coord[1, i, j] = i
-
-    def __call__(self, preds, batch):
-        outs = preds['maps']
-        out_scores = preds['score']
-
-        if isinstance(outs, torch.Tensor):
-            outs = outs.numpy()
-        if isinstance(out_scores, torch.Tensor):
-            out_scores = out_scores.numpy()
-
-        batch_size = outs.shape[0]
-        boxes_batch = []
-        for idx in range(batch_size):
-            bboxes = []
-            scores = []
-
-            img_shape = batch[idx]
-
-            org_img_size = img_shape[:3]
-            img_shape = img_shape[3:]
-            img_size = img_shape[:2]
-
-            out = np.expand_dims(outs[idx], axis=0)
-            outputs = dict()
-
-            score = np.expand_dims(out_scores[idx], axis=0)
-
-            kernel = out[:, 0, :, :] > 0.2
-            loc = out[:, 1:, :, :].astype("float32")
-
-            score = score[0].astype(np.float32)
-            kernel = kernel[0].astype(np.uint8)
-            loc = loc[0].astype(np.float32)
-
-            label_num, label_kernel = cv2.connectedComponents(
-                kernel, connectivity=4)
-
-            for i in range(1, label_num):
-                ind = (label_kernel == i)
-                if ind.sum(
-                ) < 10:  # pixel number less than 10, treated as background
-                    label_kernel[ind] = 0
-
-            label = np.zeros_like(label_kernel)
-            h, w = label_kernel.shape
-            pixels = self.coord[:, :h, :w].reshape(2, -1)
-            points = pixels.transpose([1, 0]).astype(np.float32)
-
-            off_points = (points + 10. / 4. * loc[:, pixels[1], pixels[0]].T
-                          ).astype(np.int32)
-            off_points[:, 0] = np.clip(off_points[:, 0], 0, label.shape[1] - 1)
-            off_points[:, 1] = np.clip(off_points[:, 1], 0, label.shape[0] - 1)
-
-            label[pixels[1], pixels[0]] = label_kernel[off_points[:, 1],
-                                                       off_points[:, 0]]
-            label[label_kernel > 0] = label_kernel[label_kernel > 0]
-
-            score_pocket = [0.0]
-            for i in range(1, label_num):
-                ind = (label_kernel == i)
-                if ind.sum() == 0:
-                    score_pocket.append(0.0)
-                    continue
-                score_i = np.mean(score[ind])
-                score_pocket.append(score_i)
-
-            label_num = np.max(label) + 1
-            label = cv2.resize(
-                label, (img_size[1], img_size[0]),
-                interpolation=cv2.INTER_NEAREST)
-
-            scale = (float(org_img_size[1]) / float(img_size[1]),
-                     float(org_img_size[0]) / float(img_size[0]))
-
-            for i in range(1, label_num):
-                ind = (label == i)
-                points = np.array(np.where(ind)).transpose((1, 0))
-
-                if points.shape[0] < self.min_area:
-                    continue
-
-                score_i = score_pocket[i]
-                if score_i < self.min_score:
-                    continue
-
-                if self.box_type == 'rect':
-                    rect = cv2.minAreaRect(points[:, ::-1])
-                    bbox = cv2.boxPoints(rect) * scale
-                    z = bbox.mean(0)
-                    bbox = z + (bbox - z) * 0.85
-                elif self.box_type == 'poly':
-                    binary = np.zeros(label.shape, dtype='uint8')
-                    binary[ind] = 1
-                    try:
-                        _, contours, _ = cv2.findContours(
-                            binary, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
-                    except BaseException:
-                        contours, _ = cv2.findContours(
-                            binary, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
-
-                    bbox = contours[0] * scale
-
-                bbox = bbox.astype('int32')
-                bboxes.append(bbox.reshape(-1, 2))
-                scores.append(score_i)
 
-            boxes_batch.append({'points': bboxes})
+def standard_nms(S, thres):
+    """
+    Standard nms.
+    """
+    order = np.argsort(S[:, 8])[::-1]
+    keep = []
+    while order.size > 0:
+        i = order[0]
+        keep.append(i)
+        ovr = np.array([intersection(S[i], S[t]) for t in order[1:]])
+
+        inds = np.where(ovr <= thres)[0]
+        order = order[inds + 1]
+
+    return S[keep]
+
+
+def standard_nms_inds(S, thres):
+    """
+    Standard nms, retun inds.
+    """
+    order = np.argsort(S[:, 8])[::-1]
+    keep = []
+    while order.size > 0:
+        i = order[0]
+        keep.append(i)
+        ovr = np.array([intersection(S[i], S[t]) for t in order[1:]])
 
-        return boxes_batch
+        inds = np.where(ovr <= thres)[0]
+        order = order[inds + 1]
+
+    return keep
+
+
+def nms(S, thres):
+    """
+    nms.
+    """
+    order = np.argsort(S[:, 8])[::-1]
+    keep = []
+    while order.size > 0:
+        i = order[0]
+        keep.append(i)
+        ovr = np.array([intersection(S[i], S[t]) for t in order[1:]])
+
+        inds = np.where(ovr <= thres)[0]
+        order = order[inds + 1]
+
+    return keep
+
+
+def soft_nms(boxes_in, Nt_thres=0.3, threshold=0.8, sigma=0.5, method=2):
+    """
+    soft_nms
+    :para boxes_in, N x 9 (coords + score)
+    :para threshould, eliminate cases min score(0.001)
+    :para Nt_thres, iou_threshi
+    :para sigma, gaussian weght
+    :method, linear or gaussian
+    """
+    boxes = boxes_in.copy()
+    N = boxes.shape[0]
+    if N is None or N < 1:
+        return np.array([])
+    pos, maxpos = 0, 0
+    weight = 0.0
+    inds = np.arange(N)
+    tbox, sbox = boxes[0].copy(), boxes[0].copy()
+    for i in range(N):
+        maxscore = boxes[i, 8]
+        maxpos = i
+        tbox = boxes[i].copy()
+        ti = inds[i]
+        pos = i + 1
+        #get max box
+        while pos < N:
+            if maxscore < boxes[pos, 8]:
+                maxscore = boxes[pos, 8]
+                maxpos = pos
+            pos = pos + 1
+        #add max box as a detection
+        boxes[i, :] = boxes[maxpos, :]
+        inds[i] = inds[maxpos]
+        #swap
+        boxes[maxpos, :] = tbox
+        inds[maxpos] = ti
+        tbox = boxes[i].copy()
+        pos = i + 1
+        #NMS iteration
+        while pos < N:
+            sbox = boxes[pos].copy()
+            ts_iou_val = intersection(tbox, sbox)
+            if ts_iou_val > 0:
+                if method == 1:
+                    if ts_iou_val > Nt_thres:
+                        weight = 1 - ts_iou_val
+                    else:
+                        weight = 1
+                elif method == 2:
+                    weight = np.exp(-1.0 * ts_iou_val**2 / sigma)
+                else:
+                    if ts_iou_val > Nt_thres:
+                        weight = 0
+                    else:
+                        weight = 1
+                boxes[pos, 8] = weight * boxes[pos, 8]
+                #if box score falls below thresold, discard the box by
+                #swaping last box update N
+                if boxes[pos, 8] < threshold:
+                    boxes[pos, :] = boxes[N - 1, :]
+                    inds[pos] = inds[N - 1]
+                    N = N - 1
+                    pos = pos - 1
+            pos = pos + 1
+
+    return boxes[:N]
+
+
+def nms_locality(polys, thres=0.3):
+    """
+    locality aware nms of EAST
+    :param polys: a N*9 numpy array. first 8 coordinates, then prob
+    :return: boxes after nms
+    """
+    S = []
+    p = None
+    for g in polys:
+        if p is not None and intersection(g, p) > thres:
+            p = weighted_merge(g, p)
+        else:
+            if p is not None:
+                S.append(p)
+            p = g
+    if p is not None:
+        S.append(p)
+
+    if len(S) == 0:
+        return np.array([])
+    return standard_nms(np.array(S), thres)
+
+
+if __name__ == '__main__':
+    # 343,350,448,135,474,143,369,359
+    print(
+        Polygon(np.array([[343, 350], [448, 135], [474, 143], [369, 359]]))
+        .area)
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/db_postprocess.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/db_postprocess.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""
+This code is refered from:
+https://github.com/WenmuZhou/DBNet.pytorch/blob/master/post_processing/seg_detector_representer.py
+"""
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
 import numpy as np
 import cv2
 import torch
 from shapely.geometry import Polygon
 import pyclipper
 
 
@@ -13,77 +21,28 @@
     def __init__(self,
                  thresh=0.3,
                  box_thresh=0.7,
                  max_candidates=1000,
                  unclip_ratio=2.0,
                  use_dilation=False,
                  score_mode="fast",
-                 box_type='quad',
                  **kwargs):
         self.thresh = thresh
         self.box_thresh = box_thresh
         self.max_candidates = max_candidates
         self.unclip_ratio = unclip_ratio
         self.min_size = 3
         self.score_mode = score_mode
-        self.box_type = box_type
         assert score_mode in [
             "slow", "fast"
         ], "Score mode must be in [slow, fast] but got: {}".format(score_mode)
 
         self.dilation_kernel = None if not use_dilation else np.array(
             [[1, 1], [1, 1]])
 
-    def polygons_from_bitmap(self, pred, _bitmap, dest_width, dest_height):
-        '''
-        _bitmap: single map with shape (1, H, W),
-            whose values are binarized as {0, 1}
-        '''
-
-        bitmap = _bitmap
-        height, width = bitmap.shape
-
-        boxes = []
-        scores = []
-
-        contours, _ = cv2.findContours((bitmap * 255).astype(np.uint8),
-                                       cv2.RETR_LIST, cv2.CHAIN_APPROX_SIMPLE)
-
-        for contour in contours[:self.max_candidates]:
-            epsilon = 0.002 * cv2.arcLength(contour, True)
-            approx = cv2.approxPolyDP(contour, epsilon, True)
-            points = approx.reshape((-1, 2))
-            if points.shape[0] < 4:
-                continue
-
-            score = self.box_score_fast(pred, points.reshape(-1, 2))
-            if self.box_thresh > score:
-                continue
-
-            if points.shape[0] > 2:
-                box = self.unclip(points, self.unclip_ratio)
-                if len(box) > 1:
-                    continue
-            else:
-                continue
-            box = box.reshape(-1, 2)
-
-            _, sside = self.get_mini_boxes(box.reshape((-1, 1, 2)))
-            if sside < self.min_size + 2:
-                continue
-
-            box = np.array(box)
-            box[:, 0] = np.clip(
-                np.round(box[:, 0] / width * dest_width), 0, dest_width)
-            box[:, 1] = np.clip(
-                np.round(box[:, 1] / height * dest_height), 0, dest_height)
-            boxes.append(box.tolist())
-            scores.append(score)
-        return boxes, scores
-
     def boxes_from_bitmap(self, pred, _bitmap, dest_width, dest_height):
         '''
         _bitmap: single map with shape (1, H, W),
                 whose values are binarized as {0, 1}
         '''
 
         bitmap = _bitmap
@@ -109,29 +68,30 @@
             if self.score_mode == "fast":
                 score = self.box_score_fast(pred, points.reshape(-1, 2))
             else:
                 score = self.box_score_slow(pred, contour)
             if self.box_thresh > score:
                 continue
 
-            box = self.unclip(points, self.unclip_ratio).reshape(-1, 1, 2)
+            box = self.unclip(points).reshape(-1, 1, 2)
             box, sside = self.get_mini_boxes(box)
             if sside < self.min_size + 2:
                 continue
             box = np.array(box)
-            # 将坐标映射到预处理前图像的相应坐标
+
             box[:, 0] = np.clip(
                 np.round(box[:, 0] / width * dest_width), 0, dest_width)
             box[:, 1] = np.clip(
                 np.round(box[:, 1] / height * dest_height), 0, dest_height)
-            boxes.append(box.astype("int32"))
+            boxes.append(box.astype(np.int16))
             scores.append(score)
-        return np.array(boxes, dtype="int32"), scores
+        return np.array(boxes, dtype=np.int16), scores
 
-    def unclip(self, box, unclip_ratio):
+    def unclip(self, box):
+        unclip_ratio = self.unclip_ratio
         poly = Polygon(box)
         distance = poly.area * unclip_ratio / poly.length
         offset = pyclipper.PyclipperOffset()
         offset.AddPath(box, pyclipper.JT_ROUND, pyclipper.ET_CLOSEDPOLYGON)
         expanded = np.array(offset.Execute(distance))
         return expanded
 
@@ -160,23 +120,23 @@
 
     def box_score_fast(self, bitmap, _box):
         '''
         box_score_fast: use bbox mean score as the mean score
         '''
         h, w = bitmap.shape[:2]
         box = _box.copy()
-        xmin = np.clip(np.floor(box[:, 0].min()).astype("int32"), 0, w - 1)
-        xmax = np.clip(np.ceil(box[:, 0].max()).astype("int32"), 0, w - 1)
-        ymin = np.clip(np.floor(box[:, 1].min()).astype("int32"), 0, h - 1)
-        ymax = np.clip(np.ceil(box[:, 1].max()).astype("int32"), 0, h - 1)
+        xmin = np.clip(np.floor(box[:, 0].min()).astype(int), 0, w - 1)
+        xmax = np.clip(np.ceil(box[:, 0].max()).astype(int), 0, w - 1)
+        ymin = np.clip(np.floor(box[:, 1].min()).astype(int), 0, h - 1)
+        ymax = np.clip(np.ceil(box[:, 1].max()).astype(int), 0, h - 1)
 
         mask = np.zeros((ymax - ymin + 1, xmax - xmin + 1), dtype=np.uint8)
         box[:, 0] = box[:, 0] - xmin
         box[:, 1] = box[:, 1] - ymin
-        cv2.fillPoly(mask, box.reshape(1, -1, 2).astype("int32"), 1)
+        cv2.fillPoly(mask, box.reshape(1, -1, 2).astype(np.int32), 1)
         return cv2.mean(bitmap[ymin:ymax + 1, xmin:xmax + 1], mask)[0]
 
     def box_score_slow(self, bitmap, contour):
         '''
         box_score_slow: use polyon mean score as the mean score
         '''
         h, w = bitmap.shape[:2]
@@ -189,70 +149,31 @@
         ymax = np.clip(np.max(contour[:, 1]), 0, h - 1)
 
         mask = np.zeros((ymax - ymin + 1, xmax - xmin + 1), dtype=np.uint8)
 
         contour[:, 0] = contour[:, 0] - xmin
         contour[:, 1] = contour[:, 1] - ymin
 
-        cv2.fillPoly(mask, contour.reshape(1, -1, 2).astype("int32"), 1)
+        cv2.fillPoly(mask, contour.reshape(1, -1, 2).astype(np.int32), 1)
         return cv2.mean(bitmap[ymin:ymax + 1, xmin:xmax + 1], mask)[0]
 
-    def __call__(self, preds, batch):
-        preds = preds['res']
-        shape_list = batch[1]
-        if isinstance(preds, torch.Tensor):
-            preds = preds.cpu().numpy()
-        if isinstance(shape_list, torch.Tensor):
-            shape_list = shape_list.cpu().numpy()
-        pred = preds[:, 0, :, :]
+    def __call__(self, outs_dict, shape_list):
+        pred = outs_dict['maps']
+        if isinstance(pred, torch.Tensor):
+            pred = pred.cpu().numpy()
+        pred = pred[:, 0, :, :]
         segmentation = pred > self.thresh
 
         boxes_batch = []
         for batch_index in range(pred.shape[0]):
             src_h, src_w, ratio_h, ratio_w = shape_list[batch_index]
             if self.dilation_kernel is not None:
                 mask = cv2.dilate(
                     np.array(segmentation[batch_index]).astype(np.uint8),
                     self.dilation_kernel)
             else:
                 mask = segmentation[batch_index]
-            if self.box_type == 'poly':
-                boxes, scores = self.polygons_from_bitmap(pred[batch_index],
-                                                          mask, src_w, src_h)
-            elif self.box_type == 'quad':
-                boxes, scores = self.boxes_from_bitmap(pred[batch_index], mask,
-                                                       src_w, src_h)
-            else:
-                raise ValueError("box_type can only be one of ['quad', 'poly']")
+            boxes, scores = self.boxes_from_bitmap(pred[batch_index], mask,
+                                                   src_w, src_h)
 
             boxes_batch.append({'points': boxes})
-        return boxes_batch
-
-
-class DistillationDBPostProcess(object):
-    def __init__(self,
-                 model_name=["student"],
-                 key=None,
-                 thresh=0.3,
-                 box_thresh=0.6,
-                 max_candidates=1000,
-                 unclip_ratio=1.5,
-                 use_dilation=False,
-                 score_mode="fast",
-                 box_type='quad',
-                 **kwargs):
-        self.model_name = model_name
-        self.key = key
-        self.post_process = DBPostProcess(
-            thresh=thresh,
-            box_thresh=box_thresh,
-            max_candidates=max_candidates,
-            unclip_ratio=unclip_ratio,
-            use_dilation=use_dilation,
-            score_mode=score_mode,
-            box_type=box_type)
-
-    def __call__(self, predicts, batch):
-        results = {}
-        for k in self.model_name:
-            results[k] = self.post_process(predicts[k], batch)
-        return results
+        return boxes_batch
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/east_postprocess.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/east_postprocess.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,32 @@
+# Copyright (c) 2020 PaddlePaddle Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
 import numpy as np
 from .locality_aware_nms import nms_locality
 import cv2
+# import paddle
 import torch
 
 import os
-from ..utils.utility import check_install
 import sys
 
 
 class EASTPostProcess(object):
     """
     The post process for EAST.
     """
@@ -19,14 +37,19 @@
                  nms_thresh=0.2,
                  **kwargs):
 
         self.score_thresh = score_thresh
         self.cover_thresh = cover_thresh
         self.nms_thresh = nms_thresh
 
+        # c++ la-nms is faster, but only support python 3.5
+        self.is_python35 = False
+        if sys.version_info.major == 3 and sys.version_info.minor == 5:
+            self.is_python35 = True
+
     def restore_rectangle_quad(self, origin, geometry):
         """
         Restore rectangle from quadrangle.
         """
         # quad
         origin_concat = np.concatenate(
             (origin, origin, origin, origin), axis=1)  # (n, 8)
@@ -39,70 +62,64 @@
                geo_map,
                score_thresh=0.8,
                cover_thresh=0.1,
                nms_thresh=0.2):
         """
         restore text boxes from score map and geo map
         """
-
         score_map = score_map[0]
         geo_map = np.swapaxes(geo_map, 1, 0)
         geo_map = np.swapaxes(geo_map, 1, 2)
         # filter the score map
         xy_text = np.argwhere(score_map > score_thresh)
         if len(xy_text) == 0:
             return []
         # sort the text boxes via the y axis
         xy_text = xy_text[np.argsort(xy_text[:, 0])]
-        #restore quad proposals
+        # restore quad proposals
         text_box_restored = self.restore_rectangle_quad(
             xy_text[:, ::-1] * 4, geo_map[xy_text[:, 0], xy_text[:, 1], :])
         boxes = np.zeros((text_box_restored.shape[0], 9), dtype=np.float32)
         boxes[:, :8] = text_box_restored.reshape((-1, 8))
         boxes[:, 8] = score_map[xy_text[:, 0], xy_text[:, 1]]
-
-        try:
-            check_install('lanms', 'lanms-nova')
+        if self.is_python35:
             import lanms
             boxes = lanms.merge_quadrangle_n9(boxes, nms_thresh)
-        except:
-            print(
-                'You should install lanms by pip3 install lanms-nova to speed up nms_locality'
-            )
+        else:
             boxes = nms_locality(boxes.astype(np.float64), nms_thresh)
         if boxes.shape[0] == 0:
             return []
-        # Here we filter some low score boxes by the average score map, 
+        # Here we filter some low score boxes by the average score map,
         #   this is different from the orginal paper.
         for i, box in enumerate(boxes):
             mask = np.zeros_like(score_map, dtype=np.uint8)
             cv2.fillPoly(mask, box[:8].reshape(
                 (-1, 4, 2)).astype(np.int32) // 4, 1)
             boxes[i, 8] = cv2.mean(score_map, mask)[0]
         boxes = boxes[boxes[:, 8] > cover_thresh]
         return boxes
 
     def sort_poly(self, p):
         """
         Sort polygons.
         """
         min_axis = np.argmin(np.sum(p, axis=1))
-        p = p[[min_axis, (min_axis + 1) % 4,\
-            (min_axis + 2) % 4, (min_axis + 3) % 4]]
+        p = p[[min_axis, (min_axis + 1) % 4, \
+               (min_axis + 2) % 4, (min_axis + 3) % 4]]
         if abs(p[0, 0] - p[1, 0]) > abs(p[0, 1] - p[1, 1]):
             return p
         else:
             return p[[0, 3, 2, 1]]
 
     def __call__(self, outs_dict, shape_list):
         score_list = outs_dict['f_score']
         geo_list = outs_dict['f_geo']
         if isinstance(score_list, torch.Tensor):
-            score_list = score_list.numpy()
-            geo_list = geo_list.numpy()
+            score_list = score_list.cpu().numpy()
+            geo_list = geo_list.cpu().numpy()
         img_num = len(shape_list)
         dt_boxes_list = []
         for ino in range(img_num):
             score = score_list[ino]
             geo = geo_list[ino]
             boxes = self.detect(
                 score_map=score,
@@ -116,12 +133,12 @@
                 src_h, src_w, ratio_h, ratio_w = shape_list[ino]
                 boxes = boxes[:, :8].reshape((-1, 4, 2))
                 boxes[:, :, 0] /= ratio_w
                 boxes[:, :, 1] /= ratio_h
                 for i_box, box in enumerate(boxes):
                     box = self.sort_poly(box.astype(np.int32))
                     if np.linalg.norm(box[0] - box[1]) < 5 \
-                        or np.linalg.norm(box[3] - box[0]) < 5:
+                            or np.linalg.norm(box[3] - box[0]) < 5:
                         continue
                     boxes_norm.append(box)
             dt_boxes_list.append({'points': np.array(boxes_norm)})
-        return dt_boxes_list
+        return dt_boxes_list
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/fce_postprocess.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/fce_postprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This code is refer from:
+https://github.com/open-mmlab/mmocr/blob/v0.3.0/mmocr/models/textdet/postprocess/wrapper.py
+"""
+
 import cv2
 import torch
 import numpy as np
 from numpy.fft import ifft
 from ..utils.poly_nms import poly_nms, valid_boundary
 
 
@@ -9,15 +14,15 @@
     h, w = input_mask.shape
     canvas = np.zeros((h + 2, w + 2), np.uint8)
     canvas[1:h + 1, 1:w + 1] = input_mask.copy()
 
     mask = np.zeros((h + 4, w + 4), np.uint8)
 
     cv2.floodFill(canvas, mask, (0, 0), 1)
-    canvas = canvas[1:h + 1, 1:w + 1].astype(np.bool_)
+    canvas = canvas[1:h + 1, 1:w + 1].astype(np.bool)
 
     return ~canvas | input_mask
 
 
 def fourier2poly(fourier_coeff, num_reconstr_points=50):
     """ Inverse Fourier transform
         Args:
@@ -212,12 +217,12 @@
 
         if box_type == 'quad':
             new_boundaries = []
             for boundary in boundaries:
                 poly = np.array(boundary[:-1]).reshape(-1, 2).astype(np.float32)
                 score = boundary[-1]
                 points = cv2.boxPoints(cv2.minAreaRect(poly))
-                points = np.int64(points)
+                points = np.int0(points)
                 new_boundaries.append(points.reshape(-1).tolist() + [score])
                 boundaries = new_boundaries
 
         return boundaries
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/pse_postprocess/pse_postprocess.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse_postprocess.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,54 @@
+"""
+This code is refer from:
+https://github.com/whai362/PSENet/blob/python3/models/head/psenet_head.py
+"""
+
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
 import numpy as np
 import cv2
 import torch
 from torch.nn import functional as F
 
-from ..pse_postprocess.pse import pse
+from ...postprocess.pse_postprocess.pse import pse
 
 
 class PSEPostProcess(object):
     """
     The post process for PSE.
     """
 
     def __init__(self,
                  thresh=0.5,
                  box_thresh=0.85,
                  min_area=16,
-                 box_type='quad',
+                 box_type='box',
                  scale=4,
                  **kwargs):
-        assert box_type in ['quad', 'poly'], 'Only quad and poly is supported'
+        assert box_type in ['box', 'poly'], 'Only box and poly is supported'
         self.thresh = thresh
         self.box_thresh = box_thresh
         self.min_area = min_area
         self.box_type = box_type
         self.scale = scale
 
     def __call__(self, outs_dict, shape_list):
         pred = outs_dict['maps']
         if not isinstance(pred, torch.Tensor):
-            pred = torch.tensor(pred)
+            pred = torch.as_tensor(pred)
         pred = F.interpolate(
             pred, scale_factor=4 // self.scale, mode='bilinear')
 
         score = F.sigmoid(pred[:, 0, :, :])
 
-        kernels = (pred > self.thresh).astype('float32')
+        kernels = (pred > self.thresh).type(torch.float32)
         text_mask = kernels[:, 0, :, :]
-        text_mask = torch.unsqueeze(text_mask, dim=1)
-
         kernels[:, 0:, :, :] = kernels[:, 0:, :, :] * text_mask
 
         score = score.numpy()
         kernels = kernels.numpy().astype(np.uint8)
 
         boxes_batch = []
         for batch_index in range(pred.shape[0]):
@@ -71,15 +78,15 @@
                 continue
 
             score_i = np.mean(score[ind])
             if score_i < self.box_thresh:
                 label[ind] = 0
                 continue
 
-            if self.box_type == 'quad':
+            if self.box_type == 'box':
                 rect = cv2.minAreaRect(points)
                 bbox = cv2.boxPoints(rect)
             elif self.box_type == 'poly':
                 box_height = np.max(points[:, 1]) + 10
                 box_width = np.max(points[:, 0]) + 10
 
                 mask = np.zeros((box_height, box_width), np.uint8)
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/postprocess/sast_postprocess.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/sast_postprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,35 @@
+# Copyright (c) 2020 PaddlePaddle Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
 import os
 import sys
 
 __dir__ = os.path.dirname(__file__)
 sys.path.append(__dir__)
 sys.path.append(os.path.join(__dir__, '..'))
 
 import numpy as np
 from .locality_aware_nms import nms_locality
+# import paddle
 import torch
 import cv2
 import time
 
 
 class SASTPostProcess(object):
     """
@@ -46,49 +65,38 @@
         point_num = len(point_pair_list) * 2
         point_list = [0] * point_num
         for idx, point_pair in enumerate(point_pair_list):
             point_list[idx] = point_pair[0]
             point_list[point_num - 1 - idx] = point_pair[1]
         return np.array(point_list).reshape(-1, 2)
 
-    def shrink_quad_along_width(self,
-                                quad,
-                                begin_width_ratio=0.,
-                                end_width_ratio=1.):
-        """ 
+    def shrink_quad_along_width(self, quad, begin_width_ratio=0., end_width_ratio=1.):
+        """
         Generate shrink_quad_along_width.
         """
-        ratio_pair = np.array(
-            [[begin_width_ratio], [end_width_ratio]], dtype=np.float32)
+        ratio_pair = np.array([[begin_width_ratio], [end_width_ratio]], dtype=np.float32)
         p0_1 = quad[0] + (quad[1] - quad[0]) * ratio_pair
         p3_2 = quad[3] + (quad[2] - quad[3]) * ratio_pair
         return np.array([p0_1[0], p0_1[1], p3_2[1], p3_2[0]])
 
     def expand_poly_along_width(self, poly, shrink_ratio_of_width=0.3):
         """
         expand poly along width.
         """
         point_num = poly.shape[0]
-        left_quad = np.array(
-            [poly[0], poly[1], poly[-2], poly[-1]], dtype=np.float32)
+        left_quad = np.array([poly[0], poly[1], poly[-2], poly[-1]], dtype=np.float32)
         left_ratio = -shrink_ratio_of_width * np.linalg.norm(left_quad[0] - left_quad[3]) / \
                      (np.linalg.norm(left_quad[0] - left_quad[1]) + 1e-6)
-        left_quad_expand = self.shrink_quad_along_width(left_quad, left_ratio,
-                                                        1.0)
-        right_quad = np.array(
-            [
-                poly[point_num // 2 - 2], poly[point_num // 2 - 1],
-                poly[point_num // 2], poly[point_num // 2 + 1]
-            ],
-            dtype=np.float32)
+        left_quad_expand = self.shrink_quad_along_width(left_quad, left_ratio, 1.0)
+        right_quad = np.array([poly[point_num // 2 - 2], poly[point_num // 2 - 1],
+                               poly[point_num // 2], poly[point_num // 2 + 1]], dtype=np.float32)
         right_ratio = 1.0 + \
                       shrink_ratio_of_width * np.linalg.norm(right_quad[0] - right_quad[3]) / \
                       (np.linalg.norm(right_quad[0] - right_quad[1]) + 1e-6)
-        right_quad_expand = self.shrink_quad_along_width(right_quad, 0.0,
-                                                         right_ratio)
+        right_quad_expand = self.shrink_quad_along_width(right_quad, 0.0, right_ratio)
         poly[0] = left_quad_expand[0]
         poly[-1] = left_quad_expand[-1]
         poly[point_num // 2 - 1] = right_quad_expand[1]
         poly[point_num // 2] = right_quad_expand[2]
         return poly
 
     def restore_quad(self, tcl_map, tcl_map_thresh, tvo_map):
@@ -111,24 +119,24 @@
 
         return scores, quads, xy_text
 
     def quad_area(self, quad):
         """
         compute area of a quad.
         """
-        edge = [(quad[1][0] - quad[0][0]) * (quad[1][1] + quad[0][1]),
-                (quad[2][0] - quad[1][0]) * (quad[2][1] + quad[1][1]),
-                (quad[3][0] - quad[2][0]) * (quad[3][1] + quad[2][1]),
-                (quad[0][0] - quad[3][0]) * (quad[0][1] + quad[3][1])]
+        edge = [
+            (quad[1][0] - quad[0][0]) * (quad[1][1] + quad[0][1]),
+            (quad[2][0] - quad[1][0]) * (quad[2][1] + quad[1][1]),
+            (quad[3][0] - quad[2][0]) * (quad[3][1] + quad[2][1]),
+            (quad[0][0] - quad[3][0]) * (quad[0][1] + quad[3][1])
+        ]
         return np.sum(edge) / 2.
 
     def nms(self, dets):
         if self.is_python35:
-            from torchocr.utils.utility import check_install
-            check_install('lanms', 'lanms-nova')
             import lanms
             dets = lanms.merge_quadrangle_n9(dets, self.nms_thresh)
         else:
             dets = nms_locality(dets, self.nms_thresh)
         return dets
 
     def cluster_by_quads_tco(self, tcl_map, tcl_map_thresh, quads, tco_map):
@@ -147,83 +155,60 @@
         tco = tco_map[xy_text[:, 1], xy_text[:, 0], :]  # (n, 2)
         pred_tc = xy_text - tco
 
         # get gt text center
         m = quads.shape[0]
         gt_tc = np.mean(quads, axis=1)  # (m, 2)
 
-        pred_tc_tile = np.tile(pred_tc[:, np.newaxis, :],
-                               (1, m, 1))  # (n, m, 2)
+        pred_tc_tile = np.tile(pred_tc[:, np.newaxis, :], (1, m, 1))  # (n, m, 2)
         gt_tc_tile = np.tile(gt_tc[np.newaxis, :, :], (n, 1, 1))  # (n, m, 2)
         dist_mat = np.linalg.norm(pred_tc_tile - gt_tc_tile, axis=2)  # (n, m)
         xy_text_assign = np.argmin(dist_mat, axis=1) + 1  # (n,)
 
         instance_label_map[xy_text[:, 1], xy_text[:, 0]] = xy_text_assign
         return instance_count, instance_label_map
 
     def estimate_sample_pts_num(self, quad, xy_text):
         """
         Estimate sample points number.
         """
-        eh = (np.linalg.norm(quad[0] - quad[3]) +
-              np.linalg.norm(quad[1] - quad[2])) / 2.0
-        ew = (np.linalg.norm(quad[0] - quad[1]) +
-              np.linalg.norm(quad[2] - quad[3])) / 2.0
+        eh = (np.linalg.norm(quad[0] - quad[3]) + np.linalg.norm(quad[1] - quad[2])) / 2.0
+        ew = (np.linalg.norm(quad[0] - quad[1]) + np.linalg.norm(quad[2] - quad[3])) / 2.0
 
         dense_sample_pts_num = max(2, int(ew))
-        dense_xy_center_line = xy_text[np.linspace(
-            0,
-            xy_text.shape[0] - 1,
-            dense_sample_pts_num,
-            endpoint=True,
-            dtype=np.float32).astype(np.int32)]
-
-        dense_xy_center_line_diff = dense_xy_center_line[
-            1:] - dense_xy_center_line[:-1]
-        estimate_arc_len = np.sum(
-            np.linalg.norm(
-                dense_xy_center_line_diff, axis=1))
+        dense_xy_center_line = xy_text[np.linspace(0, xy_text.shape[0] - 1, dense_sample_pts_num,
+                                                   endpoint=True, dtype=np.float32).astype(np.int32)]
+
+        dense_xy_center_line_diff = dense_xy_center_line[1:] - dense_xy_center_line[:-1]
+        estimate_arc_len = np.sum(np.linalg.norm(dense_xy_center_line_diff, axis=1))
 
         sample_pts_num = max(2, int(estimate_arc_len / eh))
         return sample_pts_num
 
-    def detect_sast(self,
-                    tcl_map,
-                    tvo_map,
-                    tbo_map,
-                    tco_map,
-                    ratio_w,
-                    ratio_h,
-                    src_w,
-                    src_h,
-                    shrink_ratio_of_width=0.3,
-                    tcl_map_thresh=0.5,
-                    offset_expand=1.0,
-                    out_strid=4.0):
+    def detect_sast(self, tcl_map, tvo_map, tbo_map, tco_map, ratio_w, ratio_h, src_w, src_h,
+                    shrink_ratio_of_width=0.3, tcl_map_thresh=0.5, offset_expand=1.0, out_strid=4.0):
         """
         first resize the tcl_map, tvo_map and tbo_map to the input_size, then restore the polys
         """
         # restore quad
-        scores, quads, xy_text = self.restore_quad(tcl_map, tcl_map_thresh,
-                                                   tvo_map)
+        scores, quads, xy_text = self.restore_quad(tcl_map, tcl_map_thresh, tvo_map)
         dets = np.hstack((quads, scores)).astype(np.float32, copy=False)
         dets = self.nms(dets)
         if dets.shape[0] == 0:
             return []
         quads = dets[:, :-1].reshape(-1, 4, 2)
 
         # Compute quad area
         quad_areas = []
         for quad in quads:
             quad_areas.append(-self.quad_area(quad))
 
         # instance segmentation
         # instance_count, instance_label_map = cv2.connectedComponents(tcl_map.astype(np.uint8), connectivity=8)
-        instance_count, instance_label_map = self.cluster_by_quads_tco(
-            tcl_map, tcl_map_thresh, quads, tco_map)
+        instance_count, instance_label_map = self.cluster_by_quads_tco(tcl_map, tcl_map_thresh, quads, tco_map)
 
         # restore single poly with tcl instance.
         poly_list = []
         for instance_idx in range(1, instance_count):
             xy_text = np.argwhere(instance_label_map == instance_idx)[:, ::-1]
             quad = quads[instance_idx - 1]
             q_area = quad_areas[instance_idx - 1]
@@ -244,96 +229,74 @@
             # filter low confidence instance
             xy_text_scores = tcl_map[xy_text[:, 1], xy_text[:, 0], 0]
             if np.sum(xy_text_scores) / quad_areas[instance_idx - 1] < 0.1:
                 # if np.sum(xy_text_scores) / quad_areas[instance_idx - 1] < 0.05:
                 continue
 
             # sort xy_text
-            left_center_pt = np.array(
-                [[(quad[0, 0] + quad[-1, 0]) / 2.0,
-                  (quad[0, 1] + quad[-1, 1]) / 2.0]])  # (1, 2)
-            right_center_pt = np.array(
-                [[(quad[1, 0] + quad[2, 0]) / 2.0,
-                  (quad[1, 1] + quad[2, 1]) / 2.0]])  # (1, 2)
+            left_center_pt = np.array([[(quad[0, 0] + quad[-1, 0]) / 2.0,
+                                        (quad[0, 1] + quad[-1, 1]) / 2.0]])  # (1, 2)
+            right_center_pt = np.array([[(quad[1, 0] + quad[2, 0]) / 2.0,
+                                         (quad[1, 1] + quad[2, 1]) / 2.0]])  # (1, 2)
             proj_unit_vec = (right_center_pt - left_center_pt) / \
                             (np.linalg.norm(right_center_pt - left_center_pt) + 1e-6)
             proj_value = np.sum(xy_text * proj_unit_vec, axis=1)
             xy_text = xy_text[np.argsort(proj_value)]
 
             # Sample pts in tcl map
             if self.sample_pts_num == 0:
                 sample_pts_num = self.estimate_sample_pts_num(quad, xy_text)
             else:
                 sample_pts_num = self.sample_pts_num
-            xy_center_line = xy_text[np.linspace(
-                0,
-                xy_text.shape[0] - 1,
-                sample_pts_num,
-                endpoint=True,
-                dtype=np.float32).astype(np.int32)]
+            xy_center_line = xy_text[np.linspace(0, xy_text.shape[0] - 1, sample_pts_num,
+                                                 endpoint=True, dtype=np.float32).astype(np.int32)]
 
             point_pair_list = []
             for x, y in xy_center_line:
                 # get corresponding offset
                 offset = tbo_map[y, x, :].reshape(2, 2)
                 if offset_expand != 1.0:
-                    offset_length = np.linalg.norm(
-                        offset, axis=1, keepdims=True)
-                    expand_length = np.clip(
-                        offset_length * (offset_expand - 1),
-                        a_min=0.5,
-                        a_max=3.0)
+                    offset_length = np.linalg.norm(offset, axis=1, keepdims=True)
+                    expand_length = np.clip(offset_length * (offset_expand - 1), a_min=0.5, a_max=3.0)
                     offset_detal = offset / offset_length * expand_length
                     offset = offset + offset_detal
                     # original point
                 ori_yx = np.array([y, x], dtype=np.float32)
-                point_pair = (ori_yx + offset)[:, ::-1] * out_strid / np.array(
-                    [ratio_w, ratio_h]).reshape(-1, 2)
+                point_pair = (ori_yx + offset)[:, ::-1] * out_strid / np.array([ratio_w, ratio_h]).reshape(-1, 2)
                 point_pair_list.append(point_pair)
 
             # ndarry: (x, 2), expand poly along width
             detected_poly = self.point_pair2poly(point_pair_list)
-            detected_poly = self.expand_poly_along_width(detected_poly,
-                                                         shrink_ratio_of_width)
-            detected_poly[:, 0] = np.clip(
-                detected_poly[:, 0], a_min=0, a_max=src_w)
-            detected_poly[:, 1] = np.clip(
-                detected_poly[:, 1], a_min=0, a_max=src_h)
+            detected_poly = self.expand_poly_along_width(detected_poly, shrink_ratio_of_width)
+            detected_poly[:, 0] = np.clip(detected_poly[:, 0], a_min=0, a_max=src_w)
+            detected_poly[:, 1] = np.clip(detected_poly[:, 1], a_min=0, a_max=src_h)
             poly_list.append(detected_poly)
 
         return poly_list
 
     def __call__(self, outs_dict, shape_list):
         score_list = outs_dict['f_score']
         border_list = outs_dict['f_border']
         tvo_list = outs_dict['f_tvo']
         tco_list = outs_dict['f_tco']
         if isinstance(score_list, torch.Tensor):
-            score_list = score_list.numpy()
-            border_list = border_list.numpy()
-            tvo_list = tvo_list.numpy()
-            tco_list = tco_list.numpy()
+            score_list = score_list.cpu().numpy()
+            border_list = border_list.cpu().numpy()
+            tvo_list = tvo_list.cpu().numpy()
+            tco_list = tco_list.cpu().numpy()
 
         img_num = len(shape_list)
         poly_lists = []
         for ino in range(img_num):
             p_score = score_list[ino].transpose((1, 2, 0))
             p_border = border_list[ino].transpose((1, 2, 0))
             p_tvo = tvo_list[ino].transpose((1, 2, 0))
             p_tco = tco_list[ino].transpose((1, 2, 0))
             src_h, src_w, ratio_h, ratio_w = shape_list[ino]
 
-            poly_list = self.detect_sast(
-                p_score,
-                p_tvo,
-                p_border,
-                p_tco,
-                ratio_w,
-                ratio_h,
-                src_w,
-                src_h,
-                shrink_ratio_of_width=self.shrink_ratio_of_width,
-                tcl_map_thresh=self.tcl_map_thresh,
-                offset_expand=self.expand_scale)
+            poly_list = self.detect_sast(p_score, p_tvo, p_border, p_tco, ratio_w, ratio_h, src_w, src_h,
+                                         shrink_ratio_of_width=self.shrink_ratio_of_width,
+                                         tcl_map_thresh=self.tcl_map_thresh, offset_expand=self.expand_scale)
             poly_lists.append({'points': np.array(poly_list)})
 
         return poly_lists
+
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/e2e_utils/extract_batchsize.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/extract_batchsize.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import torch
+raise ValueError('utils -> e2e_utils -> extract_batchsize')
+import paddle
 import numpy as np
 import copy
 
 
 def org_tcl_rois(batch_size, pos_lists, pos_masks, label_lists, tcl_bs):
     """
     """
@@ -74,14 +75,14 @@
         k = 0
         for j in range(max_text_length):
             if tt[i][j][0] != pad_num:
                 k += 1
             else:
                 break
         label.append(k)
-    label = torch.tensor(label)
-    label = label.long()
-    pos_list = torch.tensor(pos_list)
-    pos_mask = torch.tensor(pos_mask)
-    label_list = torch.squeeze(torch.tensor(label_list), dim=2)
-    label_list = label_list.int()
+    label = paddle.to_tensor(label)
+    label = paddle.cast(label, dtype='int64')
+    pos_list = paddle.to_tensor(pos_list)
+    pos_mask = paddle.to_tensor(pos_mask)
+    label_list = paddle.squeeze(paddle.to_tensor(label_list), axis=2)
+    label_list = paddle.cast(label_list, dtype='int32')
     return pos_list, pos_mask, label_list, label
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/e2e_utils/extract_textpoint_fast.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/extract_textpoint_fast.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+# Copyright (c) 2021 PaddlePaddle Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+"""Contains various CTC decoders."""
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
 import cv2
 import math
 
 import numpy as np
 from itertools import groupby
 from skimage.morphology._skeletonize import thin
 
@@ -66,72 +84,41 @@
     remove_blank_in_pos = None if keep_blank_in_idxs else blank
     dedup_str, keep_idx_list = get_keep_pos_idxs(
         raw_str, remove_blank=remove_blank_in_pos)
     dst_str = remove_blank(dedup_str, blank=blank)
     return dst_str, keep_idx_list
 
 
-def instance_ctc_greedy_decoder(gather_info,
-                                logits_map,
-                                pts_num=4,
-                                point_gather_mode=None):
+def instance_ctc_greedy_decoder(gather_info, logits_map, pts_num=4):
     _, _, C = logits_map.shape
-    if point_gather_mode == 'align':
-        insert_num = 0
-        gather_info = np.array(gather_info)
-        length = len(gather_info) - 1
-        for index in range(length):
-            stride_y = np.abs(gather_info[index + insert_num][0] - gather_info[
-                index + 1 + insert_num][0])
-            stride_x = np.abs(gather_info[index + insert_num][1] - gather_info[
-                index + 1 + insert_num][1])
-            max_points = int(max(stride_x, stride_y))
-            stride = (gather_info[index + insert_num] -
-                      gather_info[index + 1 + insert_num]) / (max_points)
-            insert_num_temp = max_points - 1
-
-            for i in range(int(insert_num_temp)):
-                insert_value = gather_info[index + insert_num] - (i + 1
-                                                                  ) * stride
-                insert_index = index + i + 1 + insert_num
-                gather_info = np.insert(
-                    gather_info, insert_index, insert_value, axis=0)
-            insert_num += insert_num_temp
-        gather_info = gather_info.tolist()
-    else:
-        pass
     ys, xs = zip(*gather_info)
     logits_seq = logits_map[list(ys), list(xs)]
     probs_seq = logits_seq
     labels = np.argmax(probs_seq, axis=1)
     dst_str = [k for k, v_ in groupby(labels) if k != C - 1]
     detal = len(gather_info) // (pts_num - 1)
     keep_idx_list = [0] + [detal * (i + 1) for i in range(pts_num - 2)] + [-1]
     keep_gather_list = [gather_info[idx] for idx in keep_idx_list]
     return dst_str, keep_gather_list
 
 
 def ctc_decoder_for_image(gather_info_list,
                           logits_map,
                           Lexicon_Table,
-                          pts_num=6,
-                          point_gather_mode=None):
+                          pts_num=6):
     """
     CTC decoder using multiple processes.
     """
     decoder_str = []
     decoder_xys = []
     for gather_info in gather_info_list:
         if len(gather_info) < pts_num:
             continue
         dst_str, xys_list = instance_ctc_greedy_decoder(
-            gather_info,
-            logits_map,
-            pts_num=pts_num,
-            point_gather_mode=point_gather_mode)
+            gather_info, logits_map, pts_num=pts_num)
         dst_str_readable = ''.join([Lexicon_Table[idx] for idx in dst_str])
         if len(dst_str_readable) < 2:
             continue
         decoder_str.append(dst_str_readable)
         decoder_xys.append(xys_list)
     return decoder_str, decoder_xys
 
@@ -365,16 +352,15 @@
     return poly_list, keep_str_list
 
 
 def generate_pivot_list_fast(p_score,
                              p_char_maps,
                              f_direction,
                              Lexicon_Table,
-                             score_thresh=0.5,
-                             point_gather_mode=None):
+                             score_thresh=0.5):
     """
     return center point and end point of TCL instance; filter with the char maps;
     """
     p_score = p_score[0]
     f_direction = f_direction.transpose(1, 2, 0)
     p_tcl_map = (p_score > score_thresh) * 1.0
     skeleton_map = thin(p_tcl_map.astype(np.uint8))
@@ -394,18 +380,15 @@
 
             pos_list_sorted = sort_and_expand_with_direction_v2(
                 pos_list, f_direction, p_tcl_map)
             all_pos_yxs.append(pos_list_sorted)
 
     p_char_maps = p_char_maps.transpose([1, 2, 0])
     decoded_str, keep_yxs_list = ctc_decoder_for_image(
-        all_pos_yxs,
-        logits_map=p_char_maps,
-        Lexicon_Table=Lexicon_Table,
-        point_gather_mode=point_gather_mode)
+        all_pos_yxs, logits_map=p_char_maps, Lexicon_Table=Lexicon_Table)
     return keep_yxs_list, decoded_str
 
 
 def extract_main_direction(pos_list, f_direction):
     """
     f_direction: h x w x 2
     pos_list: [[y, x], [y, x], [y, x] ...]
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/e2e_utils/extract_textpoint_slow.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/extract_textpoint_slow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+# Copyright (c) 2021 PaddlePaddle Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+"""Contains various CTC decoders."""
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
 import cv2
 import math
 
 import numpy as np
 from itertools import groupby
 from skimage.morphology._skeletonize import thin
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/e2e_utils/pgnet_pp_utils.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/pgnet_pp_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,32 @@
+
+
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
 import torch
 import os
 import sys
 
 __dir__ = os.path.dirname(__file__)
 sys.path.append(__dir__)
 sys.path.append(os.path.join(__dir__, '..'))
-from extract_textpoint_slow import *
-from extract_textpoint_fast import generate_pivot_list_fast, restore_poly
+from .extract_textpoint_slow import *
+from .extract_textpoint_fast import generate_pivot_list_fast, restore_poly
 
 
 class PGNet_PostProcess(object):
     # two different post-process
-    def __init__(self,
-                 character_dict_path,
-                 valid_set,
-                 score_thresh,
-                 outs_dict,
-                 shape_list,
-                 point_gather_mode=None):
+    def __init__(self, character_dict_path, valid_set, score_thresh, outs_dict,
+                 shape_list):
         self.Lexicon_Table = get_dict(character_dict_path)
         self.valid_set = valid_set
         self.score_thresh = score_thresh
         self.outs_dict = outs_dict
         self.shape_list = shape_list
-        self.point_gather_mode = point_gather_mode
 
     def pg_postprocess_fast(self):
         p_score = self.outs_dict['f_score']
         p_border = self.outs_dict['f_border']
         p_char = self.outs_dict['f_char']
         p_direction = self.outs_dict['f_direction']
         if isinstance(p_score, torch.Tensor):
@@ -43,16 +42,15 @@
 
         src_h, src_w, ratio_h, ratio_w = self.shape_list[0]
         instance_yxs_list, seq_strs = generate_pivot_list_fast(
             p_score,
             p_char,
             p_direction,
             self.Lexicon_Table,
-            score_thresh=self.score_thresh,
-            point_gather_mode=self.point_gather_mode)
+            score_thresh=self.score_thresh)
         poly_list, keep_str_list = restore_poly(instance_yxs_list, seq_strs,
                                                 p_border, ratio_w, ratio_h,
                                                 src_w, src_h, self.valid_set)
         data = {
             'points': poly_list,
             'texts': keep_str_list,
         }
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/e2e_utils/visual.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/visual.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+# Copyright (c) 2021 PaddlePaddle Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 import numpy as np
 import cv2
 import time
 
 
 def resize_image(im, max_side_len=512):
     """
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr/torchocr/utils/logging.py` & `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 import sys
 import logging
 import functools
-import torch
 import torch.distributed as dist
 
 logger_initialized = {}
 
 
 @functools.lru_cache()
-def get_logger(name='torchocr', log_file=None, log_level=logging.DEBUG):
+def get_logger(name='root', log_file=None, log_level=logging.DEBUG):
     """Initialize and get a logger by name.
     If the logger has not been initialized, this method will initialize the
     logger by adding one or two handlers, otherwise the initialized logger will
     be directly returned. During initialization, a StreamHandler will always be
     added. If `log_file` is specified a FileHandler will also be added.
     Args:
         name (str): Logger name.
@@ -35,22 +34,19 @@
     formatter = logging.Formatter(
         '[%(asctime)s] %(name)s %(levelname)s: %(message)s',
         datefmt="%Y/%m/%d %H:%M:%S")
 
     stream_handler = logging.StreamHandler(stream=sys.stdout)
     stream_handler.setFormatter(formatter)
     logger.addHandler(stream_handler)
-
-    rank = int(os.environ['LOCAL_RANK']) if 'LOCAL_RANK' in os.environ else 0
-    if log_file is not None and rank==0:
+    if log_file is not None and dist.get_rank() == 0:
         log_file_folder = os.path.split(log_file)[0]
         os.makedirs(log_file_folder, exist_ok=True)
         file_handler = logging.FileHandler(log_file, 'a')
         file_handler.setFormatter(formatter)
         logger.addHandler(file_handler)
-    if rank==0:
-        logger.setLevel(log_level)
-    else:
-        logger.setLevel(logging.ERROR)
+    # if dist.get_rank() == 0:
+    #     logger.setLevel(log_level)
+    # else:
+    #     logger.setLevel(logging.ERROR)
     logger_initialized[name] = True
-    logger.propagate = False
-    return logger
+    return logger
```

### Comparing `easypaddleocr-0.1.5/easypaddleocr.egg-info/PKG-INFO` & `easypaddleocr-0.2.0/easypaddleocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypaddleocr
-Version: 0.1.5
+Version: 0.2.0
 Summary: A simple, optional tool for PaddleOCR Detection, direction classification and recognition on CPU and GPU using torch.
 Author: pk5ls20, hv0905
 Project-URL: Code, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Documentation, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Download, https://pypi.org/project/easypaddleocr
 Project-URL: Homepage, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Issues, https://github.com/pk5ls20/EasyPaddleOCR/issues
```

### Comparing `easypaddleocr-0.1.5/pyproject.toml` & `easypaddleocr-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "easypaddleocr"
-version = "0.1.5"
+version = "0.2.0"
 authors = [
     { name = "pk5ls20" },
     { name = "hv0905" }
 ]
 description = "A simple, optional tool for PaddleOCR Detection, direction classification and recognition on CPU and GPU using torch."
 readme = "readme.md"
 license = { file="LICENSE" }
```

### Comparing `easypaddleocr-0.1.5/readme.md` & `easypaddleocr-0.2.0/readme.md`

 * *Files identical despite different names*

