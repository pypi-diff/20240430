# Comparing `tmp/keras-cv-0.8.2.tar.gz` & `tmp/keras_cv-0.9.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-cv-0.8.2.tar", last modified: Thu Feb  1 00:08:44 2024, max compression
+gzip compressed data, was "keras_cv-0.9.0.dev0.tar", last modified: Tue Apr 30 00:13:52 2024, max compression
```

## Comparing `keras-cv-0.8.2.tar` & `keras_cv-0.9.0.dev0.tar`

### file list

```diff
@@ -1,412 +1,438 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.909271 keras-cv-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-02-01 00:08:44.909271 keras-cv-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-02-01 00:08:33.000000 keras-cv-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.849270 keras-cv-0.8.2/keras_cv/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.849270 keras-cv-0.8.2/keras_cv/bounding_box/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/bounding_box/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/core/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/datasets/imagenet/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/datasets/imagenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/datasets/pascal_voc/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/datasets/pascal_voc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/datasets/pascal_voc/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/datasets/pascal_voc/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/datasets/waymo/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/datasets/waymo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/keypoint/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/keypoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/retinanet/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/retinanet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/stable_diffusion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/yolov8/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/yolov8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.857270 keras-cv-0.8.2/keras_cv/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.857270 keras-cv-0.8.2/keras_cv/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/tf_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.857270 keras-cv-0.8.2/keras_cv/src/bounding_box/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/ensure_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/mask_invalid_detections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/to_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/to_ragged.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/validate_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.857270 keras-cv-0.8.2/keras_cv/src/bounding_box_3d/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box_3d/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/callbacks/pycoco_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/callbacks/waymo_evaluation_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/core/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/core/factor_sampler/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/core/factor_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/core/factor_sampler/constant_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/core/factor_sampler/factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/core/factor_sampler/normal_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/core/factor_sampler/uniform_factor_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/custom_ops/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/custom_ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/datasets/imagenet/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/imagenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/imagenet/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    18975 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/datasets/waymo/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/waymo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/waymo/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/waymo/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    27677 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/waymo/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/keypoint/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/keypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/keypoint/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/keypoint/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/keypoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.865270 keras-cv-0.8.2/keras_cv/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/feature_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/fusedmbconv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/hierarchical_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/mbconv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.869270 keras-cv-0.8.2/keras_cv/src/layers/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/anchor_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/multi_class_non_max_suppression.py
--rw-r--r--   0 runner    (1001) docker     (127)    21214 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/non_max_suppression.py
--rw-r--r--   0 runner    (1001) docker     (127)    16294 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/rpn_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.869270 keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16712 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/centernet_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/heatmap_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/voxelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/overlapping_patching_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.877270 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/aug_mix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/auto_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)    22948 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/base_image_augmentation_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/channel_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/cut_mix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/fourier_mix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/grayscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/grid_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/jittered_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/mix_up.py
--rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/posterization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/rand_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_aspect_ratio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_augmentation_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_channel_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_color_degeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_crop_and_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_cutout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_gaussian_blur.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_hue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_jpeg_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)    12287 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_saturation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_sharpness.py
--rw-r--r--   0 runner    (1001) docker     (127)    14063 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_shear.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/repeated_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    15385 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/solarization.py
--rw-r--r--   0 runner    (1001) docker     (127)    22644 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/vectorized_base_image_augmentation_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.877270 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/base_augmentation_layer_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.877270 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_dropping_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_point_feature_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_dropping_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11154 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/group_points_by_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12343 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/random_copy_paste.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/random_drop_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/swap_background.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/regularization/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/regularization/dropblock_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/regularization/squeeze_excite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/regularization/stochastic_depth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/segformer_multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/spatial_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    20736 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/vit_det_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/vit_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/centernet_box_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/ciou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/focal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/iou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/penalty_reduced_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/simclr_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/smooth_l1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/metrics/coco/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/metrics/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/metrics/coco/pycoco_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/metrics/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/metrics/object_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/metrics/object_detection/box_coco_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.885270 keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.885270 keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/densenet_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/densenet_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/densenet_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.885270 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.885270 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.885270 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.889271 keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/mix_transformer_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.889271 keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.889271 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/resnet_v1_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.889271 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/resnet_v2_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/test_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.889271 keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/vit_det_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/vit_det_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/vit_det_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.889271 keras-cv-0.8.2/keras_cv/src/models/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/classification/image_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/classification/image_classifier_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.893271 keras-cv-0.8.2/keras_cv/src/models/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14449 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/convmixer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20273 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    11070 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/darknet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/mlp_mixer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.893271 keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.893271 keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23894 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/faster_rcnn/faster_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    45780 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/regnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    26176 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.893271 keras-cv-0.8.2/keras_cv/src/models/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/__internal__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.893271 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/feature_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/prediction_head.py
--rw-r--r--   0 runner    (1001) docker     (127)    23044 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/retinanet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10678 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/retinanet_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/retinanet_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.897271 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    24653 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.897271 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/binary_crossentropy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.897271 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_pafpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.897271 keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/center_pillar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/center_pillar_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/center_pillar_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.897271 keras-cv-0.8.2/keras_cv/src/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.897271 keras-cv-0.8.2/keras_cv/src/models/segmentation/basnet/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/basnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/basnet/basnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/basnet/basnet_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.901271 keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.901271 keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/segformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/segformer_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/segformer_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.901271 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.905271 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/attention_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/clip_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/diffusion_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/noise_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/padded_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/resnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/text_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.905271 keras-cv-0.8.2/keras_cv/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/ops/iou_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.905271 keras-cv-0.8.2/keras_cv/src/point_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/point_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18300 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/point_cloud/point_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.905271 keras-cv-0.8.2/keras_cv/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/tests/test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.905271 keras-cv-0.8.2/keras_cv/src/training/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.905271 keras-cv-0.8.2/keras_cv/src/training/contrastive/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/training/contrastive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/training/contrastive/contrastive_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/training/contrastive/simclr_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.909271 keras-cv-0.8.2/keras_cv/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/conditional_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/conv_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/fill_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14437 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/preset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/resource_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/target_gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/version_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/src/version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.909271 keras-cv-0.8.2/keras_cv/src/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/visualization/draw_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/visualization/plot_bounding_box_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/visualization/plot_image_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/visualization/plot_segmentation_mask_gallery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.909271 keras-cv-0.8.2/keras_cv/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.909271 keras-cv-0.8.2/keras_cv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-02-01 00:08:44.000000 keras-cv-0.8.2/keras_cv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16381 2024-02-01 00:08:44.000000 keras-cv-0.8.2/keras_cv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 00:08:44.000000 keras-cv-0.8.2/keras_cv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-01 00:08:44.000000 keras-cv-0.8.2/keras_cv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-01 00:08:44.000000 keras-cv-0.8.2/keras_cv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-02-01 00:08:44.909271 keras-cv-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-02-01 00:08:33.000000 keras-cv-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.778687 keras_cv-0.9.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-30 00:13:52.778687 keras_cv-0.9.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-04-30 00:13:42.000000 keras_cv-0.9.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.710687 keras_cv-0.9.0.dev0/keras_cv/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/bounding_box/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/bounding_box/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/datasets/imagenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/datasets/imagenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/datasets/pascal_voc/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/datasets/pascal_voc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/datasets/pascal_voc/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/datasets/pascal_voc/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/datasets/waymo/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/datasets/waymo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/keypoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/keypoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     9426 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/models/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/models/feature_extractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/models/feature_extractor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/models/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/models/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/models/retinanet/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/models/retinanet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/models/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.714687 keras_cv-0.9.0.dev0/keras_cv/api/models/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/models/stable_diffusion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.718687 keras_cv-0.9.0.dev0/keras_cv/api/models/yolov8/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/models/yolov8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.718687 keras_cv-0.9.0.dev0/keras_cv/api/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/api/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.718687 keras_cv-0.9.0.dev0/keras_cv/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.718687 keras_cv-0.9.0.dev0/keras_cv/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/backend/keras2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/backend/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/backend/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/backend/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/backend/tf_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.722687 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18498 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/ensure_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/mask_invalid_detections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/to_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/to_ragged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/validate_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.722687 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/bounding_box_3d/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.722687 keras_cv-0.9.0.dev0/keras_cv/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/callbacks/pycoco_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/callbacks/waymo_evaluation_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.722687 keras_cv-0.9.0.dev0/keras_cv/src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.722687 keras_cv-0.9.0.dev0/keras_cv/src/core/factor_sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/core/factor_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/core/factor_sampler/constant_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/core/factor_sampler/factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/core/factor_sampler/normal_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/core/factor_sampler/uniform_factor_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.722687 keras_cv-0.9.0.dev0/keras_cv/src/custom_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/custom_ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.722687 keras_cv-0.9.0.dev0/keras_cv/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.722687 keras_cv-0.9.0.dev0/keras_cv/src/datasets/imagenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/datasets/imagenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/datasets/imagenet/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.722687 keras_cv-0.9.0.dev0/keras_cv/src/datasets/pascal_voc/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/datasets/pascal_voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/datasets/pascal_voc/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18974 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/datasets/pascal_voc/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.726687 keras_cv-0.9.0.dev0/keras_cv/src/datasets/waymo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/datasets/waymo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/datasets/waymo/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/datasets/waymo/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27676 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/datasets/waymo/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.726687 keras_cv-0.9.0.dev0/keras_cv/src/keypoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/keypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/keypoint/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/keypoint/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/keypoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.726687 keras_cv-0.9.0.dev0/keras_cv/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/feature_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/fusedmbconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/hierarchical_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/mbconv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.730687 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/anchor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/multi_class_non_max_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/non_max_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15399 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/roi_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/roi_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/rpn_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.730687 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16711 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection_3d/centernet_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection_3d/heatmap_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-30 00:11:46.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection_3d/voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection_3d/voxelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/overlapping_patching_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.738687 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/aug_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/auto_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22947 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/base_image_augmentation_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/channel_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/cut_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/fourier_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/grid_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11774 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/jittered_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/mix_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14083 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/posterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/rand_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_aspect_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_augmentation_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_channel_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_color_degeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_crop_and_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_gaussian_blur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_hue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_jpeg_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12286 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_sharpness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_shear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11327 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/repeated_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15384 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/solarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22643 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/vectorized_base_image_augmentation_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.738687 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/base_augmentation_layer_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.742687 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_dropping_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_point_feature_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_dropping_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/group_points_by_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12342 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/random_copy_paste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/random_drop_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/swap_background.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.742687 keras_cv-0.9.0.dev0/keras_cv/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/regularization/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/regularization/dropblock_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/regularization/squeeze_excite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/regularization/stochastic_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/segformer_multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/spatial_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20735 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/vit_det_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/layers/vit_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.742687 keras_cv-0.9.0.dev0/keras_cv/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/losses/centernet_box_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/losses/ciou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/losses/focal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/losses/iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/losses/penalty_reduced_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/losses/simclr_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/losses/smooth_l1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.742687 keras_cv-0.9.0.dev0/keras_cv/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.746687 keras_cv-0.9.0.dev0/keras_cv/src/metrics/coco/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/metrics/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/metrics/coco/pycoco_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.746687 keras_cv-0.9.0.dev0/keras_cv/src/metrics/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/metrics/object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/metrics/object_detection/box_coco_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.746687 keras_cv-0.9.0.dev0/keras_cv/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.746687 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.746687 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/csp_darknet/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/csp_darknet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.746687 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/densenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/densenet/densenet_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/densenet/densenet_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/densenet/densenet_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.750687 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.750687 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16395 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.750687 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13129 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.750687 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mix_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mix_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mix_transformer/mix_transformer_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.750687 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mobilenet_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.750687 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v1/resnet_v1_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.754687 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v2/resnet_v2_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/test_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.754687 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/vgg16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/vgg16/vgg16_backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.754687 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/video_swin/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/video_swin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/video_swin/video_swin_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/video_swin/video_swin_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/video_swin/video_swin_backbone_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/video_swin/video_swin_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.754687 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/vit_det/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/vit_det/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/vit_det/vit_det_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/vit_det/vit_det_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/vit_det/vit_det_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.754687 keras_cv-0.9.0.dev0/keras_cv/src/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/classification/image_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/classification/image_classifier_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/classification/video_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/classification/video_classifier_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.754687 keras_cv-0.9.0.dev0/keras_cv/src/models/feature_extractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/feature_extractor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.758687 keras_cv-0.9.0.dev0/keras_cv/src/models/feature_extractor/clip/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/feature_extractor/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/feature_extractor/clip/clip_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/feature_extractor/clip/clip_image_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/feature_extractor/clip/clip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/feature_extractor/clip/clip_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/feature_extractor/clip/clip_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/feature_extractor/clip/clip_processor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/feature_extractor/clip/clip_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/feature_extractor/clip/clip_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.758687 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14448 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/convmixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/darknet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/mlp_mixer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.758687 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.762687 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/object_detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/object_detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23913 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/object_detection/faster_rcnn/faster_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45779 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/regnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26175 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.762687 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/__internal__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.762687 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/retinanet/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/retinanet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/retinanet/feature_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/retinanet/prediction_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23042 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/retinanet/retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/retinanet/retinanet_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/retinanet/retinanet_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.762687 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.762687 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/binary_crossentropy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.766687 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_pafpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.766687 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13123 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection_3d/center_pillar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection_3d/center_pillar_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection_3d/center_pillar_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.766687 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.766687 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/basnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/basnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/basnet/basnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/basnet/basnet_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.766687 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.766687 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segformer/segformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segformer/segformer_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segformer/segformer_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.770687 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/sam_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/sam_mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/sam_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/sam_prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/sam_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.770687 keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/clip_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17410 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/diffusion_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/noise_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/padded_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/resnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20238 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.770687 keras_cv-0.9.0.dev0/keras_cv/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/ops/iou_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.770687 keras_cv-0.9.0.dev0/keras_cv/src/point_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/point_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/point_cloud/point_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.770687 keras_cv-0.9.0.dev0/keras_cv/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/tests/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.774687 keras_cv-0.9.0.dev0/keras_cv/src/training/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.774687 keras_cv-0.9.0.dev0/keras_cv/src/training/contrastive/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/training/contrastive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/training/contrastive/contrastive_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/training/contrastive/simclr_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.774687 keras_cv-0.9.0.dev0/keras_cv/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/utils/conditional_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/utils/conv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/utils/fill_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14438 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/utils/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/utils/preset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/utils/resource_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/utils/target_gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/utils/to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/utils/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/version_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-30 00:13:50.000000 keras_cv-0.9.0.dev0/keras_cv/src/version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.774687 keras_cv-0.9.0.dev0/keras_cv/src/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/visualization/draw_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/visualization/plot_bounding_box_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/visualization/plot_image_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-30 00:11:47.000000 keras_cv-0.9.0.dev0/keras_cv/src/visualization/plot_segmentation_mask_gallery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:52.778687 keras_cv-0.9.0.dev0/keras_cv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-30 00:13:52.000000 keras_cv-0.9.0.dev0/keras_cv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17640 2024-04-30 00:13:52.000000 keras_cv-0.9.0.dev0/keras_cv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:13:52.000000 keras_cv-0.9.0.dev0/keras_cv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-30 00:13:52.000000 keras_cv-0.9.0.dev0/keras_cv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 00:13:52.000000 keras_cv-0.9.0.dev0/keras_cv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-30 00:13:52.778687 keras_cv-0.9.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-30 00:13:42.000000 keras_cv-0.9.0.dev0/setup.py
```

### Comparing `keras-cv-0.8.2/PKG-INFO` & `keras_cv-0.9.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-cv
-Version: 0.8.2
+Version: 0.9.0.dev0
 Summary: Industry-strength computer Vision extensions for Keras.
 Home-page: https://github.com/keras-team/keras-cv
 Author: Keras team
 Author-email: keras-cv@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-cv-0.8.2/README.md` & `keras_cv-0.9.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.2/keras_cv/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/api/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
-from keras_cv import bounding_box
-from keras_cv import callbacks
-from keras_cv import core
-from keras_cv import datasets
-from keras_cv import keypoint
-from keras_cv import layers
-from keras_cv import losses
-from keras_cv import metrics
-from keras_cv import models
-from keras_cv import visualization
-from keras_cv.src.version_utils import version
+from keras_cv.api import bounding_box
+from keras_cv.api import callbacks
+from keras_cv.api import core
+from keras_cv.api import datasets
+from keras_cv.api import keypoint
+from keras_cv.api import layers
+from keras_cv.api import losses
+from keras_cv.api import metrics
+from keras_cv.api import models
+from keras_cv.api import visualization
 from keras_cv.src.version_utils import __version__
+from keras_cv.src.version_utils import version
```

### Comparing `keras-cv-0.8.2/keras_cv/bounding_box/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/api/bounding_box/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras_cv.src.bounding_box.converters import convert_format
 from keras_cv.src.bounding_box.ensure_tensor import ensure_tensor
 from keras_cv.src.bounding_box.formats import CENTER_XYWH
 from keras_cv.src.bounding_box.formats import REL_XYWH
 from keras_cv.src.bounding_box.formats import REL_XYXY
 from keras_cv.src.bounding_box.formats import REL_YXYX
 from keras_cv.src.bounding_box.formats import XYWH
 from keras_cv.src.bounding_box.formats import XYXY
 from keras_cv.src.bounding_box.formats import YXYX
 from keras_cv.src.bounding_box.iou import compute_ciou
 from keras_cv.src.bounding_box.iou import compute_iou
-from keras_cv.src.bounding_box.mask_invalid_detections import mask_invalid_detections
+from keras_cv.src.bounding_box.mask_invalid_detections import (
+    mask_invalid_detections,
+)
 from keras_cv.src.bounding_box.to_dense import to_dense
 from keras_cv.src.bounding_box.to_ragged import to_ragged
 from keras_cv.src.bounding_box.utils import as_relative
 from keras_cv.src.bounding_box.utils import clip_to_image
 from keras_cv.src.bounding_box.utils import is_relative
 from keras_cv.src.bounding_box.validate_format import validate_format
```

### Comparing `keras-cv-0.8.2/keras_cv/datasets/waymo/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/api/datasets/waymo/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras_cv.src.datasets.waymo.load import load
-from keras_cv.src.datasets.waymo.transformer import build_tensors_for_augmentation
+from keras_cv.src.datasets.waymo.transformer import (
+    build_tensors_for_augmentation,
+)
 from keras_cv.src.datasets.waymo.transformer import build_tensors_from_wod_frame
-from keras_cv.src.datasets.waymo.transformer import convert_to_center_pillar_inputs
+from keras_cv.src.datasets.waymo.transformer import (
+    convert_to_center_pillar_inputs,
+)
 from keras_cv.src.datasets.waymo.transformer import pad_or_trim_tensors
 from keras_cv.src.datasets.waymo.transformer import transform_to_vehicle_frame
```

### Comparing `keras-cv-0.8.2/keras_cv/layers/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/api/layers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,163 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras_cv.src.layers.augmenter import Augmenter
 from keras_cv.src.layers.feature_pyramid import FeaturePyramid
 from keras_cv.src.layers.fusedmbconv import FusedMBConvBlock
-from keras_cv.src.layers.hierarchical_transformer_encoder import HierarchicalTransformerEncoder
+from keras_cv.src.layers.hierarchical_transformer_encoder import (
+    HierarchicalTransformerEncoder,
+)
 from keras_cv.src.layers.mbconv import MBConvBlock
-from keras_cv.src.layers.object_detection.anchor_generator import AnchorGenerator
+from keras_cv.src.layers.object_detection.anchor_generator import (
+    AnchorGenerator,
+)
 from keras_cv.src.layers.object_detection.box_matcher import BoxMatcher
-from keras_cv.src.layers.object_detection.multi_class_non_max_suppression import MultiClassNonMaxSuppression
-from keras_cv.src.layers.object_detection.non_max_suppression import NonMaxSuppression
+from keras_cv.src.layers.object_detection.multi_class_non_max_suppression import (
+    MultiClassNonMaxSuppression,
+)
+from keras_cv.src.layers.object_detection.non_max_suppression import (
+    NonMaxSuppression,
+)
 from keras_cv.src.layers.object_detection.roi_generator import ROIGenerator
 from keras_cv.src.layers.object_detection.roi_pool import ROIPooler
-from keras_cv.src.layers.object_detection_3d.centernet_label_encoder import CenterNetLabelEncoder
-from keras_cv.src.layers.object_detection_3d.heatmap_decoder import HeatmapDecoder
-from keras_cv.src.layers.object_detection_3d.voxelization import DynamicVoxelization
-from keras_cv.src.layers.overlapping_patching_embedding import OverlappingPatchingAndEmbedding
+from keras_cv.src.layers.object_detection_3d.centernet_label_encoder import (
+    CenterNetLabelEncoder,
+)
+from keras_cv.src.layers.object_detection_3d.heatmap_decoder import (
+    HeatmapDecoder,
+)
+from keras_cv.src.layers.object_detection_3d.voxelization import (
+    DynamicVoxelization,
+)
+from keras_cv.src.layers.overlapping_patching_embedding import (
+    OverlappingPatchingAndEmbedding,
+)
 from keras_cv.src.layers.preprocessing.aug_mix import AugMix
 from keras_cv.src.layers.preprocessing.auto_contrast import AutoContrast
-from keras_cv.src.layers.preprocessing.base_image_augmentation_layer import BaseImageAugmentationLayer
+from keras_cv.src.layers.preprocessing.base_image_augmentation_layer import (
+    BaseImageAugmentationLayer,
+)
 from keras_cv.src.layers.preprocessing.channel_shuffle import ChannelShuffle
 from keras_cv.src.layers.preprocessing.cut_mix import CutMix
 from keras_cv.src.layers.preprocessing.equalization import Equalization
 from keras_cv.src.layers.preprocessing.fourier_mix import FourierMix
 from keras_cv.src.layers.preprocessing.grayscale import Grayscale
 from keras_cv.src.layers.preprocessing.grid_mask import GridMask
 from keras_cv.src.layers.preprocessing.jittered_resize import JitteredResize
 from keras_cv.src.layers.preprocessing.mix_up import MixUp
 from keras_cv.src.layers.preprocessing.mosaic import Mosaic
 from keras_cv.src.layers.preprocessing.posterization import Posterization
 from keras_cv.src.layers.preprocessing.rand_augment import RandAugment
 from keras_cv.src.layers.preprocessing.random_apply import RandomApply
-from keras_cv.src.layers.preprocessing.random_aspect_ratio import RandomAspectRatio
-from keras_cv.src.layers.preprocessing.random_augmentation_pipeline import RandomAugmentationPipeline
+from keras_cv.src.layers.preprocessing.random_aspect_ratio import (
+    RandomAspectRatio,
+)
+from keras_cv.src.layers.preprocessing.random_augmentation_pipeline import (
+    RandomAugmentationPipeline,
+)
 from keras_cv.src.layers.preprocessing.random_brightness import RandomBrightness
-from keras_cv.src.layers.preprocessing.random_channel_shift import RandomChannelShift
+from keras_cv.src.layers.preprocessing.random_channel_shift import (
+    RandomChannelShift,
+)
 from keras_cv.src.layers.preprocessing.random_choice import RandomChoice
-from keras_cv.src.layers.preprocessing.random_color_degeneration import RandomColorDegeneration
-from keras_cv.src.layers.preprocessing.random_color_jitter import RandomColorJitter
+from keras_cv.src.layers.preprocessing.random_color_degeneration import (
+    RandomColorDegeneration,
+)
+from keras_cv.src.layers.preprocessing.random_color_jitter import (
+    RandomColorJitter,
+)
 from keras_cv.src.layers.preprocessing.random_contrast import RandomContrast
 from keras_cv.src.layers.preprocessing.random_crop import RandomCrop
-from keras_cv.src.layers.preprocessing.random_crop_and_resize import RandomCropAndResize
+from keras_cv.src.layers.preprocessing.random_crop_and_resize import (
+    RandomCropAndResize,
+)
 from keras_cv.src.layers.preprocessing.random_cutout import RandomCutout
 from keras_cv.src.layers.preprocessing.random_flip import RandomFlip
-from keras_cv.src.layers.preprocessing.random_gaussian_blur import RandomGaussianBlur
+from keras_cv.src.layers.preprocessing.random_gaussian_blur import (
+    RandomGaussianBlur,
+)
 from keras_cv.src.layers.preprocessing.random_hue import RandomHue
-from keras_cv.src.layers.preprocessing.random_jpeg_quality import RandomJpegQuality
+from keras_cv.src.layers.preprocessing.random_jpeg_quality import (
+    RandomJpegQuality,
+)
 from keras_cv.src.layers.preprocessing.random_rotation import RandomRotation
 from keras_cv.src.layers.preprocessing.random_saturation import RandomSaturation
 from keras_cv.src.layers.preprocessing.random_sharpness import RandomSharpness
 from keras_cv.src.layers.preprocessing.random_shear import RandomShear
-from keras_cv.src.layers.preprocessing.random_translation import RandomTranslation
+from keras_cv.src.layers.preprocessing.random_translation import (
+    RandomTranslation,
+)
 from keras_cv.src.layers.preprocessing.random_zoom import RandomZoom
-from keras_cv.src.layers.preprocessing.repeated_augmentation import RepeatedAugmentation
+from keras_cv.src.layers.preprocessing.repeated_augmentation import (
+    RepeatedAugmentation,
+)
 from keras_cv.src.layers.preprocessing.rescaling import Rescaling
 from keras_cv.src.layers.preprocessing.resizing import Resizing
 from keras_cv.src.layers.preprocessing.solarization import Solarization
-from keras_cv.src.layers.preprocessing.vectorized_base_image_augmentation_layer import VectorizedBaseImageAugmentationLayer
-from keras_cv.src.layers.preprocessing_3d.base_augmentation_layer_3d import BaseAugmentationLayer3D
-from keras_cv.src.layers.preprocessing_3d.waymo.frustum_random_dropping_points import FrustumRandomDroppingPoints
-from keras_cv.src.layers.preprocessing_3d.waymo.frustum_random_point_feature_noise import FrustumRandomPointFeatureNoise
-from keras_cv.src.layers.preprocessing_3d.waymo.global_random_dropping_points import GlobalRandomDroppingPoints
-from keras_cv.src.layers.preprocessing_3d.waymo.global_random_flip import GlobalRandomFlip
-from keras_cv.src.layers.preprocessing_3d.waymo.global_random_rotation import GlobalRandomRotation
-from keras_cv.src.layers.preprocessing_3d.waymo.global_random_scaling import GlobalRandomScaling
-from keras_cv.src.layers.preprocessing_3d.waymo.global_random_translation import GlobalRandomTranslation
-from keras_cv.src.layers.preprocessing_3d.waymo.group_points_by_bounding_boxes import GroupPointsByBoundingBoxes
-from keras_cv.src.layers.preprocessing_3d.waymo.random_copy_paste import RandomCopyPaste
-from keras_cv.src.layers.preprocessing_3d.waymo.random_drop_box import RandomDropBox
-from keras_cv.src.layers.preprocessing_3d.waymo.swap_background import SwapBackground
+from keras_cv.src.layers.preprocessing.vectorized_base_image_augmentation_layer import (
+    VectorizedBaseImageAugmentationLayer,
+)
+from keras_cv.src.layers.preprocessing_3d.base_augmentation_layer_3d import (
+    BaseAugmentationLayer3D,
+)
+from keras_cv.src.layers.preprocessing_3d.waymo.frustum_random_dropping_points import (
+    FrustumRandomDroppingPoints,
+)
+from keras_cv.src.layers.preprocessing_3d.waymo.frustum_random_point_feature_noise import (
+    FrustumRandomPointFeatureNoise,
+)
+from keras_cv.src.layers.preprocessing_3d.waymo.global_random_dropping_points import (
+    GlobalRandomDroppingPoints,
+)
+from keras_cv.src.layers.preprocessing_3d.waymo.global_random_flip import (
+    GlobalRandomFlip,
+)
+from keras_cv.src.layers.preprocessing_3d.waymo.global_random_rotation import (
+    GlobalRandomRotation,
+)
+from keras_cv.src.layers.preprocessing_3d.waymo.global_random_scaling import (
+    GlobalRandomScaling,
+)
+from keras_cv.src.layers.preprocessing_3d.waymo.global_random_translation import (
+    GlobalRandomTranslation,
+)
+from keras_cv.src.layers.preprocessing_3d.waymo.group_points_by_bounding_boxes import (
+    GroupPointsByBoundingBoxes,
+)
+from keras_cv.src.layers.preprocessing_3d.waymo.random_copy_paste import (
+    RandomCopyPaste,
+)
+from keras_cv.src.layers.preprocessing_3d.waymo.random_drop_box import (
+    RandomDropBox,
+)
+from keras_cv.src.layers.preprocessing_3d.waymo.swap_background import (
+    SwapBackground,
+)
 from keras_cv.src.layers.regularization.drop_path import DropPath
 from keras_cv.src.layers.regularization.dropblock_2d import DropBlock2D
 from keras_cv.src.layers.regularization.squeeze_excite import SqueezeAndExcite2D
 from keras_cv.src.layers.regularization.stochastic_depth import StochasticDepth
-from keras_cv.src.layers.segformer_multihead_attention import SegFormerMultiheadAttention
+from keras_cv.src.layers.segformer_multihead_attention import (
+    SegFormerMultiheadAttention,
+)
 from keras_cv.src.layers.spatial_pyramid import SpatialPyramidPooling
 from keras_cv.src.layers.transformer_encoder import TransformerEncoder
 from keras_cv.src.layers.vit_det_layers import AddPositionalEmbedding
 from keras_cv.src.layers.vit_det_layers import AddRelativePositionalEmbedding
 from keras_cv.src.layers.vit_det_layers import MultiHeadAttentionWithRelativePE
 from keras_cv.src.layers.vit_det_layers import ViTDetPatchingAndEmbedding
-from keras_cv.src.layers.vit_det_layers import WindowPartitioning
 from keras_cv.src.layers.vit_det_layers import WindowedTransformerEncoder
+from keras_cv.src.layers.vit_det_layers import WindowPartitioning
 from keras_cv.src.layers.vit_layers import PatchingAndEmbedding
-from keras_cv.src.models.segmentation.segment_anything.sam_layers import MultiHeadAttentionWithDownsampling
-from keras_cv.src.models.segmentation.segment_anything.sam_layers import RandomFrequencyPositionalEmbeddings
-from keras_cv.src.models.segmentation.segment_anything.sam_layers import TwoWayMultiHeadAttention
+from keras_cv.src.models.segmentation.segment_anything.sam_layers import (
+    MultiHeadAttentionWithDownsampling,
+)
+from keras_cv.src.models.segmentation.segment_anything.sam_layers import (
+    RandomFrequencyPositionalEmbeddings,
+)
+from keras_cv.src.models.segmentation.segment_anything.sam_layers import (
+    TwoWayMultiHeadAttention,
+)
```

### Comparing `keras-cv-0.8.2/keras_cv/models/stable_diffusion/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/api/models/stable_diffusion/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras_cv.src.models.stable_diffusion.clip_tokenizer import SimpleTokenizer
 from keras_cv.src.models.stable_diffusion.decoder import Decoder
 from keras_cv.src.models.stable_diffusion.diffusion_model import DiffusionModel
 from keras_cv.src.models.stable_diffusion.image_encoder import ImageEncoder
 from keras_cv.src.models.stable_diffusion.noise_scheduler import NoiseScheduler
 from keras_cv.src.models.stable_diffusion.text_encoder import TextEncoder
 from keras_cv.src.models.stable_diffusion.text_encoder import TextEncoderV2
```

### Comparing `keras-cv-0.8.2/keras_cv/src/api_export.py` & `keras_cv-0.9.0.dev0/keras_cv/src/api_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,7 @@
     class keras_cv_export:
         def __init__(self, path, package="keras_cv"):
             self.package = package
 
         def __call__(self, symbol):
             maybe_register_serializable(symbol, self.package)
             return symbol
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/backend/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/backend/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,22 @@
 
 - `config`: check which version of Keras is being run.
 - `keras`: The full `keras` API with compat shims for older Keras versions.
 - `ops`: `keras.ops` for Keras 3 or `keras_core.ops` for Keras 2.
 - `random`: `keras.random` for Keras 3 or `keras_core.ops` for Keras 2.
 """
 from keras_cv.src.backend import config  # noqa: E402
-from keras_cv.src.backend import keras  # noqa: E402
+
+if not config.keras_3():
+    import keras_cv.src.backend.keras2 as keras  # noqa: E402
+else:
+    import keras  # noqa: E402
+
+    keras.backend.name_scope = keras.name_scope
+
 from keras_cv.src.backend import ops  # noqa: E402
 from keras_cv.src.backend import random  # noqa: E402
 from keras_cv.src.backend import tf_ops  # noqa: E402
 
 
 def assert_tf_keras(src):
     if config.keras_3():
@@ -38,8 +45,7 @@
             f"KerasCV component {src} does not yet support Keras 3, and can "
             "only be used in `tf.keras`."
         )
 
 
 def supports_ragged():
     return not config.keras_3()
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/backend/config.py` & `keras_cv-0.9.0.dev0/keras_cv/src/backend/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,7 @@
     """Check the backend framework."""
     if not keras_3():
         return "tensorflow"
 
     import keras
 
     return keras.config.backend()
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/backend/keras.py` & `keras_cv-0.9.0.dev0/keras_cv/src/backend/keras2.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,57 +10,50 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import types
 
-from keras_cv.src.backend import config
+from tensorflow import keras  # noqa: F403, F401
+from tensorflow.keras import *  # noqa: F403, F401
+
+from keras_cv.src.backend import config  # noqa: F403, F401
 
 _KERAS_CORE_ALIASES = {
     "utils->saving": [
         "register_keras_serializable",
         "deserialize_keras_object",
         "serialize_keras_object",
         "get_registered_object",
     ],
     "models->saving": ["load_model"],
 }
 
-if config.keras_3():
-    import keras  # noqa: F403, F401
-    from keras import *  # noqa: F403, F401
-
-    keras.backend.name_scope = keras.name_scope
-else:
-    from tensorflow import keras  # noqa: F403, F401
-    from tensorflow.keras import *  # noqa: F403, F401
-
-    if not hasattr(keras, "saving"):
-        keras.saving = types.SimpleNamespace()
-
-    # add aliases
-    for key, value in _KERAS_CORE_ALIASES.items():
-        src, _, dst = key.partition("->")
-        src = src.split(".")
-        dst = dst.split(".")
-
-        src_mod, dst_mod = keras, keras
-
-        # navigate to where we want to alias the attributes
-        for mod in src:
-            src_mod = getattr(src_mod, mod)
-        for mod in dst:
-            dst_mod = getattr(dst_mod, mod)
-
-        # add an alias for each attribute
-        for attr in value:
-            if isinstance(attr, tuple):
-                src_attr, dst_attr = attr
-            else:
-                src_attr, dst_attr = attr, attr
-            attr_val = getattr(src_mod, src_attr)
-            setattr(dst_mod, dst_attr, attr_val)
+if not hasattr(keras, "saving"):
+    keras.saving = types.SimpleNamespace()
 
-    # TF Keras doesn't have this rename.
-    keras.activations.silu = keras.activations.swish
+# add aliases
+for key, value in _KERAS_CORE_ALIASES.items():
+    src, _, dst = key.partition("->")
+    src = src.split(".")
+    dst = dst.split(".")
+
+    src_mod, dst_mod = keras, keras
+
+    # navigate to where we want to alias the attributes
+    for mod in src:
+        src_mod = getattr(src_mod, mod)
+    for mod in dst:
+        dst_mod = getattr(dst_mod, mod)
+
+    # add an alias for each attribute
+    for attr in value:
+        if isinstance(attr, tuple):
+            src_attr, dst_attr = attr
+        else:
+            src_attr, dst_attr = attr, attr
+        attr_val = getattr(src_mod, src_attr)
+        setattr(dst_mod, dst_attr, attr_val)
 
+# TF Keras doesn't have this rename.
+keras.activations.silu = keras.activations.swish
```

### Comparing `keras-cv-0.8.2/keras_cv/src/backend/ops.py` & `keras_cv-0.9.0.dev0/keras_cv/src/backend/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,7 @@
         from keras_core.src.backend import vectorized_map  # noqa: F403, F401
         from keras_core.src.ops import *  # noqa: F403, F401
         from keras_core.src.utils.image_utils import (  # noqa: F403, F401
             smart_resize,
         )
     if config.backend() == "tensorflow":
         from keras_cv.src.backend.tf_ops import *  # noqa: F403, F401
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/backend/random.py` & `keras_cv-0.9.0.dev0/keras_cv/src/backend/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,8 +140,7 @@
 
         return tf.random.stateless_categorical(
             logits=logits,
             num_samples=num_samples,
             seed=init_seed,
             **kwargs,
         )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/backend/scope.py` & `keras_cv-0.9.0.dev0/keras_cv/src/backend/scope.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,8 +53,7 @@
         global _IN_TF_DATA_SCOPE
         _IN_TF_DATA_SCOPE -= 1
         if _IN_TF_DATA_SCOPE == 0:
             for k, v in ops.__dict__.items():
                 setattr(ops, k, _ORIGINAL_OPS[k])
             backend.supports_ragged = _ORIGINAL_SUPPORTS_RAGGED
             _IN_TF_DATA_SCOPE = False
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/backend/tf_ops.py` & `keras_cv-0.9.0.dev0/keras_cv/src/backend/tf_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,8 +107,7 @@
         if img.shape.rank == 4:
             img.set_shape((None, None, None, static_num_channels))
         if img.shape.rank == 3:
             img.set_shape((None, None, static_num_channels))
     if isinstance(x, np.ndarray):
         return img.numpy()
     return img
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/bounding_box/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,7 @@
 )
 from keras_cv.src.bounding_box.to_dense import to_dense
 from keras_cv.src.bounding_box.to_ragged import to_ragged
 from keras_cv.src.bounding_box.utils import as_relative
 from keras_cv.src.bounding_box.utils import clip_to_image
 from keras_cv.src.bounding_box.utils import is_relative
 from keras_cv.src.bounding_box.validate_format import validate_format
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/bounding_box/converters.py` & `keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
     Relative formats, abbreviated `rel`, make use of the shapes of the `images`
     passed. In these formats, the coordinates, widths, and heights are all
     specified as percentages of the host image. `images` may be a ragged
     Tensor. Note that using a ragged Tensor for images may cause a substantial
     performance loss, as each image will need to be processed separately due to
     the mismatching image shapes.
 
-    Usage:
+    Example:
 
     ```python
     boxes = load_coco_dataset()
     boxes_in_xywh = keras_cv.bounding_box.convert_format(
         boxes,
         source='xyxy',
         target='xyWH'
@@ -522,8 +522,7 @@
             height = ops.reshape(images.row_lengths(), (-1, 1))
             width = ops.reshape(ops.max(images.row_lengths(axis=2), 1), (-1, 1))
             height = ops.expand_dims(height, axis=-1)
             width = ops.expand_dims(width, axis=-1)
     else:
         height, width = image_shape[0], image_shape[1]
     return ops.cast(height, boxes.dtype), ops.cast(width, boxes.dtype)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/bounding_box/ensure_tensor.py` & `keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/ensure_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,7 @@
     for key in ["boxes", "classes", "confidence"]:
         if key in boxes:
             boxes[key] = preprocessing.ensure_tensor(
                 boxes[key],
                 dtype=dtype,
             )
     return boxes
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/bounding_box/formats.py` & `keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,8 +156,7 @@
     - RIGHT: right of the bounding box
     """
 
     TOP = 0
     LEFT = 1
     BOTTOM = 2
     RIGHT = 3
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/bounding_box/iou.py` & `keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/iou.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,8 +254,7 @@
         axis=-1,
     )
     alpha = v / (v - iou + (1 + keras.backend.epsilon()))
 
     return iou - (
         centers_distance_squared / convex_diagonal_squared + v * alpha
     )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/bounding_box/mask_invalid_detections.py` & `keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/mask_invalid_detections.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,8 +89,7 @@
     if confidence is not None:
         result["confidence"] = confidence
 
     if output_ragged and backend.supports_ragged():
         return to_ragged(result)
 
     return result
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/bounding_box/to_dense.py` & `keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/to_dense.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,8 +87,7 @@
                     info["is_batched"],
                     bounding_boxes["confidence"].shape,
                     max_boxes,
                 ),
             )
 
     return bounding_boxes
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/bounding_box/to_ragged.py` & `keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/to_ragged.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     Bounding boxes are ragged tensors in most use cases. Converting them to a
     dense tensor makes it easier to work with Tensorflow ecosystem.
     This function can be used to filter out the masked out bounding boxes by
     checking for padded sentinel value of the class_id axis of the
     bounding_boxes.
 
-    Usage:
+    Example:
     ```python
     bounding_boxes = {
         "boxes": tf.constant([[2, 3, 4, 5], [0, 1, 2, 3]]),
         "classes": tf.constant([[-1, 1]]),
     }
     bounding_boxes = bounding_box.to_ragged(bounding_boxes)
     print(bounding_boxes)
@@ -90,8 +90,7 @@
     result["boxes"] = tf.cast(boxes, dtype)
     result["classes"] = tf.cast(classes, dtype)
 
     if confidence is not None:
         result["confidence"] = tf.cast(confidence, dtype)
 
     return result
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/bounding_box/utils.py` & `keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,8 +191,7 @@
     return boxes, classes, images, False
 
 
 def _format_outputs(boxes, classes, squeeze):
     if squeeze:
         return ops.squeeze(boxes, axis=0), ops.squeeze(classes, axis=0)
     return boxes, classes
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/bounding_box/validate_format.py` & `keras_cv-0.9.0.dev0/keras_cv/src/bounding_box/validate_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,8 +89,7 @@
         raise ValueError(
             "Expected `boxes` and `classes` to have matching dimensions "
             "on the first two axes when operating in batched mode. "
             f"Got `boxes.shape={boxes.shape}`, `classes.shape={classes.shape}`."
         )
 
     return info
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/bounding_box_3d/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/bounding_box_3d/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from keras_cv.src.bounding_box_3d.formats import CENTER_XYZ_DXDYDZ_PHI
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/bounding_box_3d/formats.py` & `keras_cv-0.9.0.dev0/keras_cv/src/bounding_box_3d/formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,8 +42,7 @@
     Y = 1
     Z = 2
     DX = 3
     DY = 4
     DZ = 5
     PHI = 6
     CLASS = 7
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/callbacks/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/callbacks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from keras_cv.src.callbacks.pycoco_callback import PyCOCOCallback
-from keras_cv.src.callbacks.waymo_evaluation_callback import WaymoEvaluationCallback
-
+from keras_cv.src.callbacks.waymo_evaluation_callback import (
+    WaymoEvaluationCallback,
+)
```

### Comparing `keras-cv-0.8.2/keras_cv/src/callbacks/pycoco_callback.py` & `keras_cv-0.9.0.dev0/keras_cv/src/callbacks/pycoco_callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,8 +131,7 @@
         }
 
         metrics = compute_pycoco_metrics(ground_truth, predictions)
         # Mark these as validation metrics by prepending a val_ prefix
         metrics = {"val_" + name: val for name, val in metrics.items()}
 
         logs.update(metrics)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/callbacks/waymo_evaluation_callback.py` & `keras_cv-0.9.0.dev0/keras_cv/src/callbacks/waymo_evaluation_callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,8 +179,7 @@
             "prediction_score": tf.squeeze(prediction_scores),
             "prediction_overlap_nlz": tf.cast(
                 tf.zeros(predicted_boxes.shape[0]), tf.bool
             ),
         }
 
         return ground_truth, predictions
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/core/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,7 @@
 from keras_cv.src.core.factor_sampler.factor_sampler import FactorSampler
 from keras_cv.src.core.factor_sampler.normal_factor_sampler import (
     NormalFactorSampler,
 )
 from keras_cv.src.core.factor_sampler.uniform_factor_sampler import (
     UniformFactorSampler,
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/core/factor_sampler/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/core/factor_sampler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/core/factor_sampler/constant_factor_sampler.py` & `keras_cv-0.9.0.dev0/keras_cv/src/core/factor_sampler/constant_factor_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
     This is useful in cases where a user wants to always ensure that an
     augmentation layer performs augmentations of the same strength.
 
     Args:
         value: the value to return from `__call__()`.
 
-    Usage:
+    Example:
     ```python
-    constant_factor = keras_cv.ConstantFactorSampler(0.5)
+    constant_factor = keras_cv.src.ConstantFactorSampler(0.5)
     random_sharpness = keras_cv.layers.RandomSharpness(factor=constant_factor)
     # random_sharpness will now always use a factor of 0.5
     ```
     """
 
     def __init__(self, value):
         self.value = value
@@ -45,8 +45,7 @@
 
     def get_config(self):
         return {"value": self.value}
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/core/factor_sampler/factor_sampler.py` & `keras_cv-0.9.0.dev0/keras_cv/src/core/factor_sampler/factor_sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,7 @@
     def __call__(self, shape=None, dtype="float32"):
         raise NotImplementedError(
             "FactorSampler subclasses must implement a `__call__()` method."
         )
 
     def get_config(self):
         return {}
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/core/factor_sampler/normal_factor_sampler.py` & `keras_cv-0.9.0.dev0/keras_cv/src/core/factor_sampler/normal_factor_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     Args:
         mean: mean value for the distribution.
         stddev: standard deviation of the distribution.
         min_value: values below min_value are clipped to min_value.
         max_value: values above max_value are clipped to max_value.
 
-    Usage:
+    Example:
     ```python
     factor = keras_cv.core.NormalFactor(
         mean=0.5,
         stddev=0.1,
         lower=0,
         upper=1
     )
@@ -73,8 +73,7 @@
             "max_value": self.max_value,
             "seed": self.seed,
         }
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/core/factor_sampler/uniform_factor_sampler.py` & `keras_cv-0.9.0.dev0/keras_cv/src/core/factor_sampler/uniform_factor_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 
     Args:
         lower: the lower bound of values returned from `__call__()`.
         upper: the upper bound of values returned from `__call__()`.
         seed: A shape int or Tensor, the seed to the random number generator.
             Must have dtype int32 or int64. (When using XLA, only int32 is
             allowed.)
-    Usage:
+    Example:
     ```python
-    uniform_factor = keras_cv.UniformFactorSampler(0, 0.5)
+    uniform_factor = keras_cv.src.UniformFactorSampler(0, 0.5)
     random_sharpness = keras_cv.layers.RandomSharpness(factor=uniform_factor)
     # random_sharpness will now sample factors between 0, and 0.5
     ```
     """
 
     def __init__(self, lower, upper, seed=None):
         self.lower = lower
@@ -59,8 +59,7 @@
             "upper": self.upper,
             "seed": self.seed,
         }
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/custom_ops/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/custom_ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/datasets/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/datasets/imagenet/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,9 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from keras_cv.src.datasets import pascal_voc
-
+from keras_cv.src.datasets.imagenet.load import load
```

### Comparing `keras-cv-0.8.2/keras_cv/src/datasets/imagenet/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/datasets/pascal_voc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,9 +7,8 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from keras_cv.src.datasets.imagenet.load import load
-
+from keras_cv.src.datasets.pascal_voc.load import load
```

### Comparing `keras-cv-0.8.2/keras_cv/src/datasets/imagenet/load.py` & `keras_cv-0.9.0.dev0/keras_cv/src/datasets/imagenet/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     shuffle_buffer=None,
     reshuffle_each_iteration=False,
     img_size=None,
     crop_to_aspect_ratio=True,
 ):
     """Loads the ImageNet dataset from TFRecords
 
-    Usage:
+    Example:
     ```python
     dataset, ds_info = keras_cv.datasets.imagenet.load(
         split="train", tfrecord_path="gs://my-bucket/imagenet-tfrecords"
     )
     ```
 
     Args:
@@ -130,8 +130,7 @@
             shuffle_buffer, reshuffle_each_iteration=reshuffle_each_iteration
         )
 
     if batch_size is not None:
         dataset = dataset.batch(batch_size)
 
     return dataset.prefetch(tf.data.AUTOTUNE)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/basnet/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Copyright 2022 The KerasCV Authors
+# Copyright 2023 The KerasCV Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from keras_cv.src.datasets.pascal_voc.load import load
 
+from keras_cv.src.models.segmentation.basnet.basnet import BASNet
```

### Comparing `keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/load.py` & `keras_cv-0.9.0.dev0/keras_cv/src/datasets/pascal_voc/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     batch_size=None,
     shuffle_files=True,
     shuffle_buffer=None,
     dataset="voc/2007",
 ):
     """Loads the PascalVOC 2007 dataset.
 
-    Usage:
+    Example:
     ```python
     dataset, ds_info = keras_cv.datasets.pascal_voc.load(
         split="train", bounding_box_format="xywh", batch_size=9
     )
     ```
 
     Args:
@@ -97,8 +97,7 @@
         dataset = dataset.shuffle(shuffle_buffer, reshuffle_each_iteration=True)
 
     if batch_size is not None:
         dataset = dataset.apply(
             tf.data.experimental.dense_to_ragged_batch(batch_size=batch_size)
         )
     return dataset, dataset_info
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/segmentation.py` & `keras_cv-0.9.0.dev0/keras_cv/src/datasets/pascal_voc/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,8 +541,7 @@
         SBD_URL, extracted_dir=extracted_dir, local_dir_path=data_dir
     )
     image_ids = _get_sbd_image_ids(data_dir, split)
     # len(metadata) = #samples, metadata[i] is a dict.
     metadata = _build_sbd_metadata(data_dir, image_ids)
     dataset = _build_sbd_dataset_from_metadata(metadata)
     return dataset
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/datasets/waymo/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/datasets/waymo/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,13 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Following symbols are only available when Waymo Open Dataset dependencies are
 # installed.
 from keras_cv.src.datasets.waymo.load import load
-from keras_cv.src.datasets.waymo.transformer import build_tensors_for_augmentation
+from keras_cv.src.datasets.waymo.transformer import (
+    build_tensors_for_augmentation,
+)
 from keras_cv.src.datasets.waymo.transformer import build_tensors_from_wod_frame
-from keras_cv.src.datasets.waymo.transformer import convert_to_center_pillar_inputs
+from keras_cv.src.datasets.waymo.transformer import (
+    convert_to_center_pillar_inputs,
+)
 from keras_cv.src.datasets.waymo.transformer import pad_or_trim_tensors
 from keras_cv.src.datasets.waymo.transformer import transform_to_vehicle_frame
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/datasets/waymo/load.py` & `keras_cv-0.9.0.dev0/keras_cv/src/datasets/waymo/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     Returns:
         tf.data.Dataset containing the features extracted from Frames using the
         provided transformer.
 
     Example:
 
     ```python
-    from keras_cv.datasets.waymo import load
+    from keras_cv.src.datasets.waymo import load
 
     def simple_transformer(frame):
         return {"timestamp_micros": frame.timestamp_micros}
 
     output_signature = {"timestamp_micros": tf.TensorSpec((), tf.int64)}
     load("/path/to/tfrecords", simple_transformer, output_signature)
     ```
@@ -89,8 +89,7 @@
             os.path.join(tfrecord_path, "*.tfrecord")
         )
     segments = tf.data.TFRecordDataset(filenames)
     return tf.data.Dataset.from_generator(
         _generate_frames(segments, transformer),
         output_signature=output_signature,
     )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/datasets/waymo/struct.py` & `keras_cv-0.9.0.dev0/keras_cv/src/datasets/waymo/struct.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,8 +49,7 @@
     label_box_density: Optional[tf.Tensor] = None
     # [M] detection difficulty level.
     label_box_detection_difficulty: Optional[tf.Tensor] = None
     # [M] valid box mask.
     label_box_mask: Optional[tf.Tensor] = None
     # [M] object class of each point.
     label_point_class: Optional[tf.Tensor] = None
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/datasets/waymo/transformer.py` & `keras_cv-0.9.0.dev0/keras_cv/src/datasets/waymo/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -850,8 +850,7 @@
         ],
         axis=-1,
     )
     return {
         "point_clouds": tf.squeeze(point_cloud, axis=0),
         "bounding_boxes": tf.squeeze(boxes, axis=0),
     }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/keypoint/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/keypoint/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,7 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from keras_cv.src.keypoint.converters import convert_format
 from keras_cv.src.keypoint.formats import REL_XY
 from keras_cv.src.keypoint.formats import XY
 from keras_cv.src.keypoint.utils import filter_out_of_image
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/keypoint/converters.py` & `keras_cv-0.9.0.dev0/keras_cv/src/keypoint/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     `images` passed. In these formats, the coordinates, widths, and
     heights are all specified as percentages of the host image.
     `images` may be a ragged Tensor. Note that using a ragged Tensor
     for images may cause a substantial performance loss, as each image
     will need to be processed separately due to the mismatching image
     shapes.
 
-    Usage:
+    Example:
 
     ```python
     images, keypoints = load_my_dataset()
     keypoints_in_rel = keras_cv.keypoint.convert_format(
         keypoint,
         source='xy',
         target='rel_xy',
@@ -195,8 +195,7 @@
     return keypoints, images, squeeze_axis
 
 
 def _format_outputs(result, squeeze_axis):
     if len(squeeze_axis) == 0:
         return result
     return tf.squeeze(result, axis=squeeze_axis)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/keypoint/formats.py` & `keras_cv-0.9.0.dev0/keras_cv/src/keypoint/formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,8 +61,7 @@
     - CONFIDENCE: confidence of the keypoints
     """
 
     X = 0
     Y = 1
     CLASS = 2
     CONFIDENCE = 3
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/keypoint/utils.py` & `keras_cv-0.9.0.dev0/keras_cv/src/keypoint/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,7 @@
             keypoints[..., 1] >= 0, keypoints[..., 1] < image_shape[H_AXIS]
         ),
     )
     masked = tf.ragged.boolean_mask(keypoints, mask)
     if isinstance(masked, tf.RaggedTensor):
         return masked
     return tf.RaggedTensor.from_tensor(masked)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,26 +19,30 @@
 from keras_cv.src.layers.augmenter import Augmenter
 from keras_cv.src.layers.feature_pyramid import FeaturePyramid
 from keras_cv.src.layers.fusedmbconv import FusedMBConvBlock
 from keras_cv.src.layers.hierarchical_transformer_encoder import (
     HierarchicalTransformerEncoder,
 )
 from keras_cv.src.layers.mbconv import MBConvBlock
-from keras_cv.src.layers.object_detection.anchor_generator import AnchorGenerator
+from keras_cv.src.layers.object_detection.anchor_generator import (
+    AnchorGenerator,
+)
 from keras_cv.src.layers.object_detection.box_matcher import BoxMatcher
-from keras_cv.src.layers.object_detection.multi_class_non_max_suppression import (
+from keras_cv.src.layers.object_detection.multi_class_non_max_suppression import (  # noqa: E501
     MultiClassNonMaxSuppression,
 )
 from keras_cv.src.layers.object_detection.non_max_suppression import (
     NonMaxSuppression,
 )
 from keras_cv.src.layers.object_detection_3d.centernet_label_encoder import (
     CenterNetLabelEncoder,
 )
-from keras_cv.src.layers.object_detection_3d.voxelization import DynamicVoxelization
+from keras_cv.src.layers.object_detection_3d.voxelization import (
+    DynamicVoxelization,
+)
 from keras_cv.src.layers.overlapping_patching_embedding import (
     OverlappingPatchingAndEmbedding,
 )
 from keras_cv.src.layers.preprocessing.aug_mix import AugMix
 from keras_cv.src.layers.preprocessing.auto_contrast import AutoContrast
 from keras_cv.src.layers.preprocessing.base_image_augmentation_layer import (
     BaseImageAugmentationLayer,
@@ -51,44 +55,52 @@
 from keras_cv.src.layers.preprocessing.grid_mask import GridMask
 from keras_cv.src.layers.preprocessing.jittered_resize import JitteredResize
 from keras_cv.src.layers.preprocessing.mix_up import MixUp
 from keras_cv.src.layers.preprocessing.mosaic import Mosaic
 from keras_cv.src.layers.preprocessing.posterization import Posterization
 from keras_cv.src.layers.preprocessing.rand_augment import RandAugment
 from keras_cv.src.layers.preprocessing.random_apply import RandomApply
-from keras_cv.src.layers.preprocessing.random_aspect_ratio import RandomAspectRatio
+from keras_cv.src.layers.preprocessing.random_aspect_ratio import (
+    RandomAspectRatio,
+)
 from keras_cv.src.layers.preprocessing.random_augmentation_pipeline import (
     RandomAugmentationPipeline,
 )
 from keras_cv.src.layers.preprocessing.random_brightness import RandomBrightness
 from keras_cv.src.layers.preprocessing.random_channel_shift import (
     RandomChannelShift,
 )
 from keras_cv.src.layers.preprocessing.random_choice import RandomChoice
 from keras_cv.src.layers.preprocessing.random_color_degeneration import (
     RandomColorDegeneration,
 )
-from keras_cv.src.layers.preprocessing.random_color_jitter import RandomColorJitter
+from keras_cv.src.layers.preprocessing.random_color_jitter import (
+    RandomColorJitter,
+)
 from keras_cv.src.layers.preprocessing.random_contrast import RandomContrast
 from keras_cv.src.layers.preprocessing.random_crop import RandomCrop
 from keras_cv.src.layers.preprocessing.random_crop_and_resize import (
     RandomCropAndResize,
 )
 from keras_cv.src.layers.preprocessing.random_cutout import RandomCutout
 from keras_cv.src.layers.preprocessing.random_flip import RandomFlip
 from keras_cv.src.layers.preprocessing.random_gaussian_blur import (
     RandomGaussianBlur,
 )
 from keras_cv.src.layers.preprocessing.random_hue import RandomHue
-from keras_cv.src.layers.preprocessing.random_jpeg_quality import RandomJpegQuality
+from keras_cv.src.layers.preprocessing.random_jpeg_quality import (
+    RandomJpegQuality,
+)
 from keras_cv.src.layers.preprocessing.random_rotation import RandomRotation
 from keras_cv.src.layers.preprocessing.random_saturation import RandomSaturation
 from keras_cv.src.layers.preprocessing.random_sharpness import RandomSharpness
 from keras_cv.src.layers.preprocessing.random_shear import RandomShear
-from keras_cv.src.layers.preprocessing.random_translation import RandomTranslation
+from keras_cv.src.layers.preprocessing.random_translation import (
+    RandomTranslation,
+)
 from keras_cv.src.layers.preprocessing.random_zoom import RandomZoom
 from keras_cv.src.layers.preprocessing.repeated_augmentation import (
     RepeatedAugmentation,
 )
 from keras_cv.src.layers.preprocessing.rescaling import Rescaling
 from keras_cv.src.layers.preprocessing.resizing import Resizing
 from keras_cv.src.layers.preprocessing.solarization import Solarization
@@ -109,24 +121,26 @@
 )
 from keras_cv.src.layers.preprocessing_3d.waymo.global_random_rotation import (
     GlobalRandomRotation,
 )
 from keras_cv.src.layers.preprocessing_3d.waymo.global_random_scaling import (
     GlobalRandomScaling,
 )
-from keras_cv.src.layers.preprocessing_3d.waymo.global_random_translation import (
+from keras_cv.src.layers.preprocessing_3d.waymo.global_random_translation import (  # noqa: E501
     GlobalRandomTranslation,
 )
 from keras_cv.src.layers.preprocessing_3d.waymo.group_points_by_bounding_boxes import (  # noqa: E501
     GroupPointsByBoundingBoxes,
 )
 from keras_cv.src.layers.preprocessing_3d.waymo.random_copy_paste import (
     RandomCopyPaste,
 )
-from keras_cv.src.layers.preprocessing_3d.waymo.random_drop_box import RandomDropBox
+from keras_cv.src.layers.preprocessing_3d.waymo.random_drop_box import (
+    RandomDropBox,
+)
 from keras_cv.src.layers.preprocessing_3d.waymo.swap_background import (
     SwapBackground,
 )
 from keras_cv.src.layers.regularization.drop_path import DropPath
 from keras_cv.src.layers.regularization.dropblock_2d import DropBlock2D
 from keras_cv.src.layers.regularization.squeeze_excite import SqueezeAndExcite2D
 from keras_cv.src.layers.regularization.stochastic_depth import StochasticDepth
@@ -137,8 +151,7 @@
 from keras_cv.src.layers.transformer_encoder import TransformerEncoder
 from keras_cv.src.layers.vit_det_layers import AddRelativePositionalEmbedding
 from keras_cv.src.layers.vit_det_layers import MultiHeadAttentionWithRelativePE
 from keras_cv.src.layers.vit_det_layers import ViTDetPatchingAndEmbedding
 from keras_cv.src.layers.vit_det_layers import WindowedTransformerEncoder
 from keras_cv.src.layers.vit_det_layers import WindowPartitioning
 from keras_cv.src.layers.vit_layers import PatchingAndEmbedding
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/augmenter.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/augmenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 @keras_cv_export("keras_cv.layers.Augmenter")
 class Augmenter(keras.layers.Layer):
     """Light-weight class to apply augmentations to data.
 
     Args:
         layers: A list of `keras.layers.Layers` to apply to the example
 
-    Examples:
-    from keras_cv import layers
+    Example:
+    from keras_cv.src import layers
     images = np.ones((16, 256, 256, 3))
     augmenter = layers.Augmenter(
         [
             layers.RandomFlip(),
             layers.RandAugment(value_range=(0, 255)),
             layers.CutMix(),
         ]
@@ -39,8 +39,7 @@
     def __init__(self, layers):
         self.layers = layers
 
     def __call__(self, inputs):
         for layer in self.layers:
             inputs = layer(inputs)
         return inputs
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/feature_pyramid.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/feature_pyramid.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             will be created for each pyramid level.
         output_layers: a python dict with int keys that matches to each of the
             pyramid level. The values of the dict should be `keras.Layer`, which
             will be called with feature inputs and merged result from upstream
             levels. Defaults to None, and a `keras.Conv2D` layer with kernel 3x3
             will be created for each pyramid level.
 
-    Sample Usage:
+    Example:
     ```python
 
     inp = keras.layers.Input((384, 384, 3))
     backbone = keras.applications.EfficientNetB0(
         input_tensor=inp,
         include_top=False
     )
@@ -214,8 +214,7 @@
             "max_level": self.max_level,
             "num_channels": self.num_channels,
             "lateral_layers": self.lateral_layers_passed,
             "output_layers": self.output_layers_passed,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/fusedmbconv.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/fusedmbconv.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             the output convolution, defaults to 0.8
 
     Returns:
         A `tf.Tensor` representing a feature map, passed through the FusedMBConv
         block
 
 
-    Example usage:
+    Example:
 
     ```
     inputs = tf.random.normal(shape=(1, 64, 64, 32), dtype=tf.float32)
     layer = keras_cv.layers.FusedMBConvBlock(
         input_filters=32,
         output_filters=32
     )
@@ -232,8 +232,7 @@
             "bn_momentum": self.bn_momentum,
             "activation": self.activation,
             "survival_probability": self.survival_probability,
         }
 
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/hierarchical_transformer_encoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/hierarchical_transformer_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             sample using the `DropPath` layer. Defaults to `0.0`.
         layer_norm_epsilon: float, the epsilon for
             `LayerNormalization` layers. Defaults to `1e-06`
         sr_ratio: integer, the ratio to use within
             `SegFormerMultiheadAttention`. If set to > 1, a `Conv2D`
              layer is used to reduce the length of the sequence. Defaults to `1`.
 
-    Basic usage:
+    Example:
 
     ```
     project_dim = 1024
     num_heads = 4
     patch_size = 16
 
     encoded_patches = keras_cv.layers.OverlappingPatchingAndEmbedding(
@@ -134,8 +134,7 @@
             B, C = shape[0], shape[2]
             x = ops.reshape(x, (B, H, W, C))
             x = self.dwconv(x)
             x = ops.reshape(x, (B, -1, C))
             x = ops.nn.gelu(x)
             x = self.fc2(x)
             return x
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/mbconv.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/mbconv.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                 before the output convolution, defaults to 0.8
 
         Returns:
             A `tf.Tensor` representing a feature map, passed through the MBConv
             block
 
 
-        Example usage:
+        Example:
 
         ```
         inputs = tf.random.normal(shape=(1, 64, 64, 32), dtype=tf.float32)
         layer = keras_cv.layers.MBConvBlock(input_filters=32, output_filters=32)
 
         output = layer(inputs)
         output.shape # TensorShape([1, 64, 64, 32])
@@ -239,8 +239,7 @@
             "se_ratio": self.se_ratio,
             "bn_momentum": self.bn_momentum,
             "activation": self.activation,
             "survival_probability": self.survival_probability,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection/anchor_generator.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/anchor_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
       aspect_ratios: A list of floats representing the ratio of anchor width to
         height.
       strides: iterable of ints that represent the anchor stride size between
         center of anchors at each scale.
       clip_boxes: whether to clip generated anchor boxes to the image
         size, defaults to `False`.
 
-    Usage:
+    Example:
     ```python
     strides = [8, 16, 32]
     scales = [1, 1.2599210498948732, 1.5874010519681994]
     sizes = [32.0, 64.0, 128.0]
     aspect_ratios = [0.5, 1.0, 2.0]
 
     image = np.random.uniform(size=(512, 512, 3))
@@ -298,8 +298,7 @@
             x_min = ops.maximum(ops.minimum(x_min, image_width), 0.0)
             x_max = ops.maximum(ops.minimum(x_max, image_width), 0.0)
 
         # [H * W * K, 4]
         return ops.cast(
             ops.concatenate([y_min, x_min, y_max, x_max], axis=-1), self.dtype
         )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection/box_matcher.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/box_matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
           result. Setting this to True guarantees that each column will be
           matched to positive result to at least one row.
 
     Raises:
         ValueError: if `thresholds` not sorted or
         len(`match_values`) != len(`thresholds`) + 1
 
-    Usage:
+    Example:
 
     ```python
     box_matcher = keras_cv.layers.BoxMatcher([0.3, 0.7], [-1, 0, 1])
     iou_metric = keras_cv.bounding_box.compute_iou(anchors, boxes)
     matched_columns, matched_match_values = box_matcher(iou_metric)
     cls_mask = ops.less_equal(matched_match_values, 0)
     ```
@@ -264,8 +264,7 @@
     def get_config(self):
         config = {
             "thresholds": self.thresholds[1:-1],
             "match_values": self.match_values,
             "force_match_for_each_col": self.force_match_for_each_col,
         }
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection/multi_class_non_max_suppression.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/multi_class_non_max_suppression.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,8 +133,7 @@
             "iou_threshold": self.iou_threshold,
             "confidence_threshold": self.confidence_threshold,
             "max_detections_per_class": self.max_detections_per_class,
             "max_detections": self.max_detections,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection/non_max_suppression.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/non_max_suppression.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,8 +546,7 @@
         boxes = ops.reshape(boxes, [batch_size, -1, 4])
 
         # Updates output_size.
         output_size += ops.cast(
             ops.sum(ops.any(box_slice > 0, [2]), [1]), "int32"
         )
     return boxes, iou_threshold, output_size, idx + 1
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_align.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/roi_align.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,29 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Dict
-from typing import Mapping
 from typing import Optional
-from typing import Tuple
-
-import tensorflow as tf
-from tensorflow import keras
 
 from keras_cv.src import bounding_box
-from keras_cv.src.backend import assert_tf_keras
+from keras_cv.src.backend import keras
+from keras_cv.src.backend import ops
 
 
-def _feature_bilinear_interpolation(
-    features: tf.Tensor, kernel_y: tf.Tensor, kernel_x: tf.Tensor
-) -> tf.Tensor:
+def _feature_bilinear_interpolation(features, kernel_y, kernel_x):
     """
     Feature bilinear interpolation.
 
     The RoIAlign feature f can be computed by bilinear interpolation
     of four neighboring feature points f0, f1, f2, and f3.
     f(y, x) = [hy, ly] * [[f00, f01], * [hx, lx]^T
                           [f10, f11]]
@@ -45,50 +38,56 @@
       kernel_y: Tensor of size [batch_size, boxes, output_size, 2, 1].
       kernel_x: Tensor of size [batch_size, boxes, output_size, 2, 1].
 
     Returns:
       A 5-D tensor representing feature crop of shape
       [batch_size, num_boxes, output_size, output_size, num_filters].
     """
-    features_shape = tf.shape(features)
+    features_shape = ops.shape(features)
     batch_size, num_boxes, output_size, num_filters = (
         features_shape[0],
         features_shape[1],
         features_shape[2],
         features_shape[4],
     )
 
     output_size = output_size // 2
-    kernel_y = tf.reshape(kernel_y, [batch_size, num_boxes, output_size * 2, 1])
-    kernel_x = tf.reshape(kernel_x, [batch_size, num_boxes, 1, output_size * 2])
+    kernel_y = ops.reshape(
+        kernel_y, [batch_size, num_boxes, output_size * 2, 1]
+    )
+    kernel_x = ops.reshape(
+        kernel_x, [batch_size, num_boxes, 1, output_size * 2]
+    )
     # Use implicit broadcast to generate the interpolation kernel. The
     # multiplier `4` is for avg pooling.
     interpolation_kernel = kernel_y * kernel_x * 4
 
     # Interpolate the gathered features with computed interpolation kernels.
-    features *= tf.cast(
-        tf.expand_dims(interpolation_kernel, axis=-1), dtype=features.dtype
+    features *= ops.cast(
+        ops.expand_dims(interpolation_kernel, axis=-1), dtype=features.dtype
     )
-    features = tf.reshape(
+    features = ops.reshape(
         features,
         [batch_size * num_boxes, output_size * 2, output_size * 2, num_filters],
     )
-    features = tf.nn.avg_pool(features, [1, 2, 2, 1], [1, 2, 2, 1], "VALID")
-    features = tf.reshape(
+    features = ops.nn.average_pool(
+        features, [1, 2, 2, 1], [1, 2, 2, 1], "VALID"
+    )
+    features = ops.reshape(
         features, [batch_size, num_boxes, output_size, output_size, num_filters]
     )
     return features
 
 
 def _compute_grid_positions(
-    boxes: tf.Tensor,
-    boundaries: tf.Tensor,
-    output_size: int,
-    sample_offset: float,
-) -> Tuple[tf.Tensor, tf.Tensor, tf.Tensor, tf.Tensor]:
+    boxes,
+    boundaries,
+    output_size,
+    sample_offset,
+):
     """
     Computes the grid position w.r.t. the corresponding feature map.
 
     Args:
       boxes: a 3-D tensor of shape [batch_size, num_boxes, 4] encoding the
         information of each box w.r.t. the corresponding feature map.
         boxes[:, :, 0:2] are the grid position in (y, x) (float) of the top-left
@@ -104,76 +103,80 @@
 
     Returns:
       kernel_y: Tensor of size [batch_size, boxes, output_size, 2, 1].
       kernel_x: Tensor of size [batch_size, boxes, output_size, 2, 1].
       box_grid_y0y1: Tensor of size [batch_size, boxes, output_size, 2]
       box_grid_x0x1: Tensor of size [batch_size, boxes, output_size, 2]
     """
-    boxes_shape = tf.shape(boxes)
+    boxes_shape = ops.shape(boxes)
     batch_size, num_boxes = boxes_shape[0], boxes_shape[1]
     if batch_size is None:
-        batch_size = tf.shape(boxes)[0]
+        batch_size = ops.shape(boxes)[0]
     box_grid_x = []
     box_grid_y = []
     for i in range(output_size):
         box_grid_x.append(
             boxes[:, :, 1] + (i + sample_offset) * boxes[:, :, 3] / output_size
         )
         box_grid_y.append(
             boxes[:, :, 0] + (i + sample_offset) * boxes[:, :, 2] / output_size
         )
-    box_grid_x = tf.stack(box_grid_x, axis=2)
-    box_grid_y = tf.stack(box_grid_y, axis=2)
+    box_grid_x = ops.stack(box_grid_x, axis=2)
+    box_grid_y = ops.stack(box_grid_y, axis=2)
 
-    box_grid_y0 = tf.floor(box_grid_y)
-    box_grid_x0 = tf.floor(box_grid_x)
-    box_grid_x0 = tf.maximum(tf.cast(0.0, dtype=box_grid_x0.dtype), box_grid_x0)
-    box_grid_y0 = tf.maximum(tf.cast(0.0, dtype=box_grid_y0.dtype), box_grid_y0)
+    box_grid_y0 = ops.floor(box_grid_y)
+    box_grid_x0 = ops.floor(box_grid_x)
+    box_grid_x0 = ops.maximum(
+        ops.cast(0.0, dtype=box_grid_x0.dtype), box_grid_x0
+    )
+    box_grid_y0 = ops.maximum(
+        ops.cast(0.0, dtype=box_grid_y0.dtype), box_grid_y0
+    )
 
-    box_grid_x0 = tf.minimum(
-        box_grid_x0, tf.expand_dims(boundaries[:, :, 1], -1)
+    box_grid_x0 = ops.minimum(
+        box_grid_x0, ops.expand_dims(boundaries[:, :, 1], -1)
     )
-    box_grid_x1 = tf.minimum(
-        box_grid_x0 + 1, tf.expand_dims(boundaries[:, :, 1], -1)
+    box_grid_x1 = ops.minimum(
+        box_grid_x0 + 1, ops.expand_dims(boundaries[:, :, 1], -1)
     )
-    box_grid_y0 = tf.minimum(
-        box_grid_y0, tf.expand_dims(boundaries[:, :, 0], -1)
+    box_grid_y0 = ops.minimum(
+        box_grid_y0, ops.expand_dims(boundaries[:, :, 0], -1)
     )
-    box_grid_y1 = tf.minimum(
-        box_grid_y0 + 1, tf.expand_dims(boundaries[:, :, 0], -1)
+    box_grid_y1 = ops.minimum(
+        box_grid_y0 + 1, ops.expand_dims(boundaries[:, :, 0], -1)
     )
 
-    box_gridx0x1 = tf.stack([box_grid_x0, box_grid_x1], axis=-1)
-    box_gridy0y1 = tf.stack([box_grid_y0, box_grid_y1], axis=-1)
+    box_gridx0x1 = ops.stack([box_grid_x0, box_grid_x1], axis=-1)
+    box_gridy0y1 = ops.stack([box_grid_y0, box_grid_y1], axis=-1)
 
     # The RoIAlign feature f can be computed by bilinear interpolation of four
     # neighboring feature points f0, f1, f2, and f3.
     # f(y, x) = [hy, ly] * [[f00, f01], * [hx, lx]^T
     #                       [f10, f11]]
     # f(y, x) = (hy*hx)f00 + (hy*lx)f01 + (ly*hx)f10 + (lx*ly)f11
     # f(y, x) = w00*f00 + w01*f01 + w10*f10 + w11*f11
     ly = box_grid_y - box_grid_y0
     lx = box_grid_x - box_grid_x0
     hy = 1.0 - ly
     hx = 1.0 - lx
-    kernel_y = tf.reshape(
-        tf.stack([hy, ly], axis=3), [batch_size, num_boxes, output_size, 2, 1]
+    kernel_y = ops.reshape(
+        ops.stack([hy, ly], axis=3), [batch_size, num_boxes, output_size, 2, 1]
     )
-    kernel_x = tf.reshape(
-        tf.stack([hx, lx], axis=3), [batch_size, num_boxes, output_size, 2, 1]
+    kernel_x = ops.reshape(
+        ops.stack([hx, lx], axis=3), [batch_size, num_boxes, output_size, 2, 1]
     )
     return kernel_y, kernel_x, box_gridy0y1, box_gridx0x1
 
 
 def multilevel_crop_and_resize(
-    features: Dict[str, tf.Tensor],
-    boxes: tf.Tensor,
+    features,
+    boxes,
     output_size: int = 7,
     sample_offset: float = 0.5,
-) -> tf.Tensor:
+):
     """
     Crop and resize on multilevel feature pyramid.
 
     Generate the (output_size, output_size) set of pixels for each input box
     by first locating the box into the correct feature level, and then cropping
     and resizing it using the corresponding feature map of that level.
 
@@ -190,190 +193,189 @@
         offset from grid point.
 
     Returns:
       A 5-D tensor representing feature crop of shape
       [batch_size, num_boxes, output_size, output_size, num_filters].
     """
 
-    with tf.name_scope("multilevel_crop_and_resize"):
-        levels_str = list(features.keys())
-        # Levels are represented by strings with a prefix "P" to represent
-        # pyramid levels. The integer level can be obtained by looking at
-        # the value that follows the "P".
-        levels = [int(level_str[1:]) for level_str in levels_str]
-        min_level = min(levels)
-        max_level = max(levels)
-        features_shape = tf.shape(features[f"P{min_level}"])
-        batch_size, max_feature_height, max_feature_width, num_filters = (
-            features_shape[0],
-            features_shape[1],
-            features_shape[2],
-            features_shape[3],
-        )
+    levels_str = list(features.keys())
+    # Levels are represented by strings with a prefix "P" to represent
+    # pyramid levels. The integer level can be obtained by looking at
+    # the value that follows the "P".
+    levels = [int(level_str[1:]) for level_str in levels_str]
+    min_level = min(levels)
+    max_level = max(levels)
+    features_shape = ops.shape(features[f"P{min_level}"])
+    batch_size, max_feature_height, max_feature_width, num_filters = (
+        features_shape[0],
+        features_shape[1],
+        features_shape[2],
+        features_shape[3],
+    )
 
-        num_boxes = tf.shape(boxes)[1]
+    num_boxes = ops.shape(boxes)[1]
 
-        # Stack feature pyramid into a features_all of shape
-        # [batch_size, levels, height, width, num_filters].
-        features_all = []
-        feature_heights = []
-        feature_widths = []
-        for level in range(min_level, max_level + 1):
-            shape = features[f"P{level}"].get_shape().as_list()
-            feature_heights.append(shape[1])
-            feature_widths.append(shape[2])
-            # Concat tensor of [batch_size, height_l * width_l, num_filters] for
-            # each level.
-            features_all.append(
-                tf.reshape(features[f"P{level}"], [batch_size, -1, num_filters])
-            )
-        features_r2 = tf.reshape(tf.concat(features_all, 1), [-1, num_filters])
-
-        # Calculate height_l * width_l for each level.
-        level_dim_sizes = [
-            feature_widths[i] * feature_heights[i]
-            for i in range(len(feature_widths))
-        ]
-        # level_dim_offsets is accumulated sum of level_dim_size.
-        level_dim_offsets = [0]
-        for i in range(len(feature_widths) - 1):
-            level_dim_offsets.append(level_dim_offsets[i] + level_dim_sizes[i])
-        batch_dim_size = level_dim_offsets[-1] + level_dim_sizes[-1]
-        level_dim_offsets = tf.constant(level_dim_offsets, tf.int32)
-        height_dim_sizes = tf.constant(feature_widths, tf.int32)
-
-        # Assigns boxes to the right level.
-        box_width = boxes[:, :, 3] - boxes[:, :, 1]
-        box_height = boxes[:, :, 2] - boxes[:, :, 0]
-        areas_sqrt = tf.sqrt(
-            tf.cast(box_height, tf.float32) * tf.cast(box_width, tf.float32)
+    # Stack feature pyramid into a features_all of shape
+    # [batch_size, levels, height, width, num_filters].
+    features_all = []
+    feature_heights = []
+    feature_widths = []
+    for level in range(min_level, max_level + 1):
+        shape = ops.shape(features[f"P{level}"])
+        feature_heights.append(shape[1])
+        feature_widths.append(shape[2])
+        # Concat tensor of [batch_size, height_l * width_l, num_filters] for
+        # each level.
+        features_all.append(
+            ops.reshape(features[f"P{level}"], [batch_size, -1, num_filters])
         )
+    features_r2 = ops.reshape(
+        ops.concatenate(features_all, 1), [-1, num_filters]
+    )
 
-        # following the FPN paper to divide by 224.
-        levels = tf.cast(
-            tf.math.floordiv(
-                tf.math.log(tf.math.divide_no_nan(areas_sqrt, 224.0)),
-                tf.math.log(2.0),
-            )
-            + 4.0,
-            dtype=tf.int32,
-        )
-        # Maps levels between [min_level, max_level].
-        levels = tf.minimum(max_level, tf.maximum(levels, min_level))
+    # Calculate height_l * width_l for each level.
+    level_dim_sizes = [
+        feature_widths[i] * feature_heights[i]
+        for i in range(len(feature_widths))
+    ]
+    # level_dim_offsets is accumulated sum of level_dim_size.
+    level_dim_offsets = [0]
+    for i in range(len(feature_widths) - 1):
+        level_dim_offsets.append(level_dim_offsets[i] + level_dim_sizes[i])
+    batch_dim_size = level_dim_offsets[-1] + level_dim_sizes[-1]
+    level_dim_offsets = (
+        ops.ones_like(level_dim_offsets, dtype="int32") * level_dim_offsets
+    )
+    height_dim_sizes = (
+        ops.ones_like(feature_widths, dtype="int32") * feature_widths
+    )
 
-        # Projects box location and sizes to corresponding feature levels.
-        scale_to_level = tf.cast(
-            tf.pow(tf.constant(2.0), tf.cast(levels, tf.float32)),
-            dtype=boxes.dtype,
+    # Assigns boxes to the right level.
+    box_width = boxes[:, :, 3] - boxes[:, :, 1]
+    box_height = boxes[:, :, 2] - boxes[:, :, 0]
+    areas_sqrt = ops.sqrt(
+        ops.cast(box_height, "float32") * ops.cast(box_width, "float32")
+    )
+
+    # following the FPN paper to divide by 224.
+    levels = ops.cast(
+        ops.floor_divide(
+            ops.log(ops.divide(areas_sqrt, 224.0)),
+            ops.log(2.0),
         )
-        boxes /= tf.expand_dims(scale_to_level, axis=2)
-        box_width /= scale_to_level
-        box_height /= scale_to_level
-        boxes = tf.concat(
+        + 4.0,
+        dtype="int32",
+    )
+    # Maps levels between [min_level, max_level].
+    levels = ops.minimum(max_level, ops.maximum(levels, min_level))
+
+    # Projects box location and sizes to corresponding feature levels.
+    scale_to_level = ops.cast(
+        ops.power(2.0, ops.cast(levels, "float32")),
+        dtype=boxes.dtype,
+    )
+    boxes /= ops.expand_dims(scale_to_level, axis=2)
+    box_width /= scale_to_level
+    box_height /= scale_to_level
+    boxes = ops.concatenate(
+        [
+            boxes[:, :, 0:2],
+            ops.expand_dims(box_height, -1),
+            ops.expand_dims(box_width, -1),
+        ],
+        axis=-1,
+    )
+
+    # Maps levels to [0, max_level-min_level].
+    levels -= min_level
+    level_strides = ops.power([[2.0]], ops.cast(levels, "float32"))
+    boundary = ops.cast(
+        ops.concatenate(
             [
-                boxes[:, :, 0:2],
-                tf.expand_dims(box_height, -1),
-                tf.expand_dims(box_width, -1),
+                ops.expand_dims(
+                    [[ops.cast(max_feature_height, "float32")]] / level_strides
+                    - 1,
+                    axis=-1,
+                ),
+                ops.expand_dims(
+                    [[ops.cast(max_feature_width, "float32")]] / level_strides
+                    - 1,
+                    axis=-1,
+                ),
             ],
             axis=-1,
-        )
-
-        # Maps levels to [0, max_level-min_level].
-        levels -= min_level
-        level_strides = tf.pow([[2.0]], tf.cast(levels, tf.float32))
-        boundary = tf.cast(
-            tf.concat(
-                [
-                    tf.expand_dims(
-                        [[tf.cast(max_feature_height, tf.float32)]]
-                        / level_strides
-                        - 1,
-                        axis=-1,
-                    ),
-                    tf.expand_dims(
-                        [[tf.cast(max_feature_width, tf.float32)]]
-                        / level_strides
-                        - 1,
-                        axis=-1,
-                    ),
-                ],
-                axis=-1,
-            ),
-            boxes.dtype,
-        )
+        ),
+        boxes.dtype,
+    )
 
-        # Compute grid positions.
-        (
-            kernel_y,
-            kernel_x,
-            box_gridy0y1,
-            box_gridx0x1,
-        ) = _compute_grid_positions(boxes, boundary, output_size, sample_offset)
-
-        x_indices = tf.cast(
-            tf.reshape(box_gridx0x1, [batch_size, num_boxes, output_size * 2]),
-            dtype=tf.int32,
-        )
-        y_indices = tf.cast(
-            tf.reshape(box_gridy0y1, [batch_size, num_boxes, output_size * 2]),
-            dtype=tf.int32,
-        )
+    # Compute grid positions.
+    (
+        kernel_y,
+        kernel_x,
+        box_gridy0y1,
+        box_gridx0x1,
+    ) = _compute_grid_positions(boxes, boundary, output_size, sample_offset)
+
+    x_indices = ops.cast(
+        ops.reshape(box_gridx0x1, [batch_size, num_boxes, output_size * 2]),
+        dtype="int32",
+    )
+    y_indices = ops.cast(
+        ops.reshape(box_gridy0y1, [batch_size, num_boxes, output_size * 2]),
+        dtype="int32",
+    )
 
-        batch_size_offset = tf.tile(
-            tf.reshape(
-                tf.range(batch_size) * batch_dim_size, [batch_size, 1, 1, 1]
-            ),
-            [1, num_boxes, output_size * 2, output_size * 2],
-        )
-        # Get level offset for each box. Each box belongs to one level.
-        levels_offset = tf.tile(
-            tf.reshape(
-                tf.gather(level_dim_offsets, levels),
-                [batch_size, num_boxes, 1, 1],
-            ),
-            [1, 1, output_size * 2, output_size * 2],
-        )
-        y_indices_offset = tf.tile(
-            tf.reshape(
-                y_indices
-                * tf.expand_dims(tf.gather(height_dim_sizes, levels), -1),
-                [batch_size, num_boxes, output_size * 2, 1],
-            ),
-            [1, 1, 1, output_size * 2],
-        )
-        x_indices_offset = tf.tile(
-            tf.reshape(x_indices, [batch_size, num_boxes, 1, output_size * 2]),
-            [1, 1, output_size * 2, 1],
-        )
-        indices = tf.reshape(
-            batch_size_offset
-            + levels_offset
-            + y_indices_offset
-            + x_indices_offset,
-            [-1],
-        )
+    batch_size_offset = ops.tile(
+        ops.reshape(
+            ops.arange(batch_size) * batch_dim_size, [batch_size, 1, 1, 1]
+        ),
+        [1, num_boxes, output_size * 2, output_size * 2],
+    )
+    # Get level offset for each box. Each box belongs to one level.
+    levels_offset = ops.tile(
+        ops.reshape(
+            ops.take(level_dim_offsets, levels),
+            [batch_size, num_boxes, 1, 1],
+        ),
+        [1, 1, output_size * 2, output_size * 2],
+    )
+    y_indices_offset = ops.tile(
+        ops.reshape(
+            y_indices * ops.expand_dims(ops.take(height_dim_sizes, levels), -1),
+            [batch_size, num_boxes, output_size * 2, 1],
+        ),
+        [1, 1, 1, output_size * 2],
+    )
+    x_indices_offset = ops.tile(
+        ops.reshape(x_indices, [batch_size, num_boxes, 1, output_size * 2]),
+        [1, 1, output_size * 2, 1],
+    )
+    indices = ops.reshape(
+        batch_size_offset + levels_offset + y_indices_offset + x_indices_offset,
+        [-1],
+    )
 
-        # TODO(tanzhenyu): replace tf.gather with tf.gather_nd and try to get
-        #  similar performance.
-        features_per_box = tf.reshape(
-            tf.gather(features_r2, indices),
-            [
-                batch_size,
-                num_boxes,
-                output_size * 2,
-                output_size * 2,
-                num_filters,
-            ],
-        )
+    # TODO(tanzhenyu): replace tf.gather with tf.gather_nd and try to get
+    #  similar performance.
+    features_per_box = ops.reshape(
+        ops.take(features_r2, indices),
+        [
+            batch_size,
+            num_boxes,
+            output_size * 2,
+            output_size * 2,
+            num_filters,
+        ],
+    )
 
-        # Bilinear interpolation.
-        features_per_box = _feature_bilinear_interpolation(
-            features_per_box, kernel_y, kernel_x
-        )
-        return features_per_box
+    # Bilinear interpolation.
+    features_per_box = _feature_bilinear_interpolation(
+        features_per_box, kernel_y, kernel_x
+    )
+    return features_per_box
 
 
 # TODO(tanzhenyu): Remove this implementation once roi_pool has better
 #  performance as this is mostly a duplicate of
 #  https://github.com/tensorflow/models/blob/master/official/legacy/detection/ops/spatial_transform_ops.py#L324
 @keras.utils.register_keras_serializable(package="keras_cv")
 class _ROIAligner(keras.layers.Layer):
@@ -391,26 +393,26 @@
 
         Args:
           bounding_box_format: the input format for boxes.
           crop_size: An `int` of the output size of the cropped features.
           sample_offset: A `float` in [0, 1] of the subpixel sample offset.
           **kwargs: Additional keyword arguments passed to Layer.
         """
-        assert_tf_keras("keras_cv.layers._ROIAligner")
+        # assert_tf_keras("keras_cv.layers._ROIAligner")
         self._config_dict = {
             "bounding_box_format": bounding_box_format,
             "crop_size": target_size,
             "sample_offset": sample_offset,
         }
         super().__init__(**kwargs)
 
     def call(
         self,
-        features: Mapping[str, tf.Tensor],
-        boxes: tf.Tensor,
+        features,
+        boxes,
         training: Optional[bool] = None,
     ):
         """
 
         Args:
           features: A dictionary with key as pyramid level and value as
             features. The features are in shape of
@@ -434,8 +436,7 @@
             output_size=self._config_dict["crop_size"],
             sample_offset=self._config_dict["sample_offset"],
         )
         return roi_features
 
     def get_config(self):
         return self._config_dict
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_generator.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/roi_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,25 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Mapping
 from typing import Optional
-from typing import Tuple
-from typing import Union
 
-import tensorflow as tf
-from tensorflow import keras
-
-from keras_cv.src import bounding_box
 from keras_cv.src.api_export import keras_cv_export
-from keras_cv.src.backend import assert_tf_keras
+from keras_cv.src.backend import keras
+from keras_cv.src.backend import ops
+from keras_cv.src.layers import NonMaxSuppression
 
 
 @keras_cv_export("keras_cv.layers.ROIGenerator")
 class ROIGenerator(keras.layers.Layer):
     """
     Generates region of interests (ROI, or proposal) from scores.
 
@@ -70,15 +65,15 @@
         nms_iou_threshold_test: float. IOU threshold to use for NMS in inference
             mode.
         post_nms_topk_test: int. number of top k scoring proposals to keep after
             applying NMS in inference mode. When RPN is run on multiple
             feature maps / levels (as in FPN) this number is per
             feature map / level.
 
-    Usage:
+    Example:
     ```python
     roi_generator = ROIGenerator("xyxy")
     boxes = {2: tf.random.normal([32, 5, 4])}
     scores = {2: tf.random.normal([32, 5])}
     rois, roi_scores = roi_generator(boxes, scores, training=True)
     ```
 
@@ -93,33 +88,32 @@
         post_nms_topk_train: int = 1000,
         pre_nms_topk_test: int = 1000,
         nms_score_threshold_test: float = 0.0,
         nms_iou_threshold_test: float = 0.7,
         post_nms_topk_test: int = 1000,
         **kwargs,
     ):
-        assert_tf_keras("keras_cv.layers.ROIGenerator")
         super().__init__(**kwargs)
         self.bounding_box_format = bounding_box_format
         self.pre_nms_topk_train = pre_nms_topk_train
         self.nms_score_threshold_train = nms_score_threshold_train
         self.nms_iou_threshold_train = nms_iou_threshold_train
         self.post_nms_topk_train = post_nms_topk_train
         self.pre_nms_topk_test = pre_nms_topk_test
         self.nms_score_threshold_test = nms_score_threshold_test
         self.nms_iou_threshold_test = nms_iou_threshold_test
         self.post_nms_topk_test = post_nms_topk_test
         self.built = True
 
     def call(
         self,
-        multi_level_boxes: Union[tf.Tensor, Mapping[int, tf.Tensor]],
-        multi_level_scores: Union[tf.Tensor, Mapping[int, tf.Tensor]],
+        multi_level_boxes,
+        multi_level_scores,
         training: Optional[bool] = None,
-    ) -> Tuple[tf.Tensor, tf.Tensor]:
+    ):
         """
         Args:
           multi_level_boxes: float Tensor. A dictionary or single Tensor of
             boxes, one per level. Shape is [batch_size, num_boxes, 4] each
             level, in `bounding_box_format`. The boxes from RPNs are usually
             encoded as deltas w.r.t to anchors, they need to be decoded before
             passing in here.
@@ -127,95 +121,77 @@
             scores, typically confidence scores, one per level. Shape is
             [batch_size, num_boxes] each level.
 
         Returns:
           rois: float Tensor of [batch_size, post_nms_topk, 4]
           roi_scores: float Tensor of [batch_size, post_nms_topk]
         """
-
         if training:
             pre_nms_topk = self.pre_nms_topk_train
             post_nms_topk = self.post_nms_topk_train
             nms_score_threshold = self.nms_score_threshold_train
             nms_iou_threshold = self.nms_iou_threshold_train
         else:
             pre_nms_topk = self.pre_nms_topk_test
             post_nms_topk = self.post_nms_topk_test
             nms_score_threshold = self.nms_score_threshold_test
             nms_iou_threshold = self.nms_iou_threshold_test
 
         def per_level_gen(boxes, scores):
-            scores_shape = scores.get_shape().as_list()
-            # scores can also be [batch_size, num_boxes, 1]
+            boxes = ops.convert_to_tensor(boxes, dtype="float32")
+            scores = ops.convert_to_tensor(scores, dtype="float32")
+            scores_shape = ops.shape(scores)
+            # Check if scores is a 3-dimensional tensor
+            # ([batch_size, num_boxes, 1])
+            # If so, remove the last dimension to make it 2D
             if len(scores_shape) == 3:
-                scores = tf.squeeze(scores, axis=-1)
-            _, num_boxes = scores.get_shape().as_list()
+                scores = ops.squeeze(scores, axis=-1)
+                scores_shape = ops.shape(scores)
+            _, num_boxes = scores_shape
             level_pre_nms_topk = min(num_boxes, pre_nms_topk)
             level_post_nms_topk = min(num_boxes, post_nms_topk)
-            scores, sorted_indices = tf.nn.top_k(
+            scores, sorted_indices = ops.top_k(
                 scores, k=level_pre_nms_topk, sorted=True
             )
-            boxes = tf.gather(boxes, sorted_indices, batch_dims=1)
-            # convert from input format to yxyx for the TF NMS operation
-            boxes = bounding_box.convert_format(
-                boxes,
-                source=self.bounding_box_format,
-                target="yxyx",
+            boxes = ops.take_along_axis(
+                boxes, sorted_indices[..., None], axis=1
             )
             # TODO(tanzhenyu): consider supporting soft / batched nms for accl
-            selected_indices, num_valid = tf.image.non_max_suppression_padded(
-                boxes,
-                scores,
-                max_output_size=level_post_nms_topk,
+            boxes = NonMaxSuppression(
+                bounding_box_format=self.bounding_box_format,
+                from_logits=False,
                 iou_threshold=nms_iou_threshold,
-                score_threshold=nms_score_threshold,
-                pad_to_max_output_size=True,
-                sorted_input=True,
-                canonicalized_coordinates=True,
-            )
-            # convert back to input format
-            boxes = bounding_box.convert_format(
-                boxes,
-                source="yxyx",
-                target=self.bounding_box_format,
+                confidence_threshold=nms_score_threshold,
+                max_detections=level_post_nms_topk,
+            )(
+                box_prediction=boxes,
+                class_prediction=scores[..., None],
             )
-            level_rois = tf.gather(boxes, selected_indices, batch_dims=1)
-            level_roi_scores = tf.gather(scores, selected_indices, batch_dims=1)
-            level_rois = level_rois * tf.cast(
-                tf.reshape(tf.range(level_post_nms_topk), [1, -1, 1])
-                < tf.reshape(num_valid, [-1, 1, 1]),
-                level_rois.dtype,
-            )
-            level_roi_scores = level_roi_scores * tf.cast(
-                tf.reshape(tf.range(level_post_nms_topk), [1, -1])
-                < tf.reshape(num_valid, [-1, 1]),
-                level_roi_scores.dtype,
-            )
-            return level_rois, level_roi_scores
+            return boxes["boxes"], boxes["confidence"]
 
         if not isinstance(multi_level_boxes, dict):
             return per_level_gen(multi_level_boxes, multi_level_scores)
 
         rois = []
         roi_scores = []
         for level in sorted(multi_level_scores.keys()):
             boxes = multi_level_boxes[level]
             scores = multi_level_scores[level]
             level_rois, level_roi_scores = per_level_gen(boxes, scores)
             rois.append(level_rois)
             roi_scores.append(level_roi_scores)
 
-        rois = tf.concat(rois, axis=1)
-        roi_scores = tf.concat(roi_scores, axis=1)
-        _, num_valid_rois = roi_scores.get_shape().as_list()
+        rois = ops.concatenate(rois, axis=1)
+        roi_scores = ops.concatenate(roi_scores, axis=1)
+        _, num_valid_rois = ops.shape(roi_scores)
         overall_top_k = min(num_valid_rois, post_nms_topk)
-        roi_scores, sorted_indices = tf.nn.top_k(
+        roi_scores, sorted_indices = ops.top_k(
             roi_scores, k=overall_top_k, sorted=True
         )
-        rois = tf.gather(rois, sorted_indices, batch_dims=1)
+        rois = ops.take_along_axis(rois, sorted_indices[..., None], axis=1)
 
         return rois, roi_scores
 
     def get_config(self):
         config = {
             "bounding_box_format": self.bounding_box_format,
             "pre_nms_topk_train": self.pre_nms_topk_train,
@@ -225,8 +201,7 @@
             "pre_nms_topk_test": self.pre_nms_topk_test,
             "nms_score_threshold_test": self.nms_score_threshold_test,
             "nms_iou_threshold_test": self.nms_iou_threshold_test,
             "post_nms_topk_test": self.post_nms_topk_test,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_pool.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/roi_pool.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import tensorflow as tf
-from tensorflow import keras
 
 from keras_cv.src import bounding_box
 from keras_cv.src.api_export import keras_cv_export
-from keras_cv.src.backend import assert_tf_keras
+from keras_cv.src.backend import keras
+from keras_cv.src.backend import ops
 
 
 @keras_cv_export("keras_cv.layers.ROIPooler")
 class ROIPooler(keras.layers.Layer):
     """
     Pooling feature map of dynamic shape into region of interest (ROI) of fixed
     shape.
@@ -37,15 +36,15 @@
         bounding_box_format: a case-insensitive string.
             For detailed information on the supported format, see the
             [KerasCV bounding box documentation](https://keras.io/api/keras_cv/bounding_box/formats/).
         target_size: List or Tuple of 2 integers of the pooled shape
         image_shape: List of Tuple of 3 integers, or `TensorShape` of the input
             image shape.
 
-    Usage:
+    Example:
     ```python
     feature_map = tf.random.normal([2, 16, 16, 512])
     roi_pooler = ROIPooler(bounding_box_format="yxyx", target_size=[7, 7],
       image_shape=[224, 224, 3])
     rois = tf.constant([[[15., 30., 25., 45.]], [[22., 1., 30., 32.]]])
     pooled_feature_map = roi_pooler(feature_map, rois)
     ```
@@ -55,15 +54,14 @@
         self,
         bounding_box_format,
         # TODO(consolidate size vs shape for KPL and here)
         target_size,
         image_shape,
         **kwargs,
     ):
-        assert_tf_keras("keras_cv.layers.ROIPooler")
         if not isinstance(target_size, (tuple, list)):
             raise ValueError(
                 "Expected `target_size` to be tuple or list, got "
                 f"{type(target_size)}"
             )
         if len(target_size) != 2:
             raise ValueError(
@@ -97,73 +95,88 @@
         # convert to relative format given feature map shape != image shape
         rois = bounding_box.convert_format(
             rois,
             source=self.bounding_box_format,
             target="rel_yxyx",
             image_shape=self.image_shape,
         )
-        pooled_feature_map = tf.vectorized_map(
-            self._pool_single_sample, (feature_map, rois)
-        )
-        return pooled_feature_map
+        pooled_feature_map = list()
+        for batch_idx in range(ops.shape(feature_map)[0]):
+            pooled_feature_map.append(
+                self._pool_single_sample(
+                    args=[feature_map[batch_idx], rois[batch_idx]]
+                )
+            )
+        return ops.stack(pooled_feature_map, axis=0)
 
     def _pool_single_sample(self, args):
         """
         Args: tuple of
           feature_map: [H, W, C] float Tensor
           rois: [N, 4] float Tensor
         Returns:
-          pooled_feature_map: [target_size, C] float Tensor
+          pooled_feature_map: [N, target_height, target_width, C] float Tensor
         """
         feature_map, rois = args
-        num_rois = rois.get_shape().as_list()[0]
-        height, width, channel = feature_map.get_shape().as_list()
+        num_rois = ops.shape(rois)[0]
+        height, width, channel = ops.shape(feature_map)
+        regions = []
         # TODO (consider vectorize it for better performance)
         for n in range(num_rois):
             # [4]
             roi = rois[n, :]
             y_start = height * roi[0]
             x_start = width * roi[1]
             region_height = height * (roi[2] - roi[0])
             region_width = width * (roi[3] - roi[1])
             h_step = region_height / self.target_height
             w_step = region_width / self.target_width
-            regions = []
+            region_steps = []
             for i in range(self.target_height):
                 for j in range(self.target_width):
                     height_start = y_start + i * h_step
                     height_end = height_start + h_step
-                    height_start = tf.cast(height_start, tf.int32)
-                    height_end = tf.cast(height_end, tf.int32)
+                    height_start = ops.cast(height_start, "int32")
+                    height_end = ops.cast(height_end, "int32")
                     # if feature_map shape smaller than roi, h_step would be 0
                     # in this case the result will be feature_map[0, 0, ...]
-                    height_end = height_start + tf.maximum(
+                    height_end = height_start + ops.maximum(
                         1, height_end - height_start
                     )
                     width_start = x_start + j * w_step
                     width_end = width_start + w_step
-                    width_start = tf.cast(width_start, tf.int32)
-                    width_end = tf.cast(width_end, tf.int32)
-                    width_end = width_start + tf.maximum(
+                    width_start = ops.cast(width_start, "int32")
+                    width_end = ops.cast(width_end, "int32")
+                    width_end = width_start + ops.maximum(
                         1, width_end - width_start
                     )
                     # [h_step, w_step, C]
-                    region = feature_map[
-                        height_start:height_end, width_start:width_end, :
-                    ]
-                    # target_height * target_width * [C]
-                    regions.append(tf.reduce_max(region, axis=[0, 1]))
-            regions = tf.reshape(
-                tf.stack(regions),
-                [self.target_height, self.target_width, channel],
+                    region_step = ops.slice(
+                        inputs=feature_map,
+                        start_indices=[
+                            height_start,
+                            width_start,
+                            ops.convert_to_tensor(0, dtype="int32"),
+                        ],
+                        shape=[
+                            height_end - height_start,
+                            width_end - width_start,
+                            ops.shape(feature_map)[-1],
+                        ],
+                    )
+                    region_steps.append(ops.max(region_step, axis=[0, 1]))
+            regions.append(
+                ops.reshape(
+                    ops.stack(region_steps),
+                    [self.target_height, self.target_width, channel],
+                )
             )
-            return regions
+        return ops.stack(regions)
 
     def get_config(self):
         config = {
             "bounding_box_format": self.bounding_box_format,
             "target_size": [self.target_height, self.target_width],
             "image_shape": self.image_shape,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_sampler.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/roi_sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import tensorflow as tf
-from tensorflow import keras
-
 from keras_cv.src import bounding_box
-from keras_cv.src.backend import assert_tf_keras
+from keras_cv.src.backend import keras
+from keras_cv.src.backend import ops
 from keras_cv.src.bounding_box import iou
 from keras_cv.src.layers.object_detection import box_matcher
 from keras_cv.src.layers.object_detection import sampling
 from keras_cv.src.utils import target_gather
 
 
 @keras.utils.register_keras_serializable(package="keras_cv")
@@ -65,32 +63,31 @@
         roi_matcher: box_matcher.BoxMatcher,
         positive_fraction: float = 0.25,
         background_class: int = 0,
         num_sampled_rois: int = 256,
         append_gt_boxes: bool = True,
         **kwargs,
     ):
-        assert_tf_keras("keras_cv.layers._ROISampler")
         super().__init__(**kwargs)
         self.bounding_box_format = bounding_box_format
         self.roi_matcher = roi_matcher
         self.positive_fraction = positive_fraction
         self.background_class = background_class
         self.num_sampled_rois = num_sampled_rois
         self.append_gt_boxes = append_gt_boxes
         self.built = True
         # for debugging.
         self._positives = keras.metrics.Mean()
         self._negatives = keras.metrics.Mean()
 
     def call(
         self,
-        rois: tf.Tensor,
-        gt_boxes: tf.Tensor,
-        gt_classes: tf.Tensor,
+        rois,
+        gt_boxes,
+        gt_classes,
     ):
         """
         Args:
           rois: [batch_size, num_rois, 4]
           gt_boxes: [batch_size, num_gt, 4]
           gt_classes: [batch_size, num_gt, 1]
         Returns:
@@ -98,19 +95,19 @@
           sampled_gt_boxes: [batch_size, num_sampled_rois, 4]
           sampled_box_weights: [batch_size, num_sampled_rois, 1]
           sampled_gt_classes: [batch_size, num_sampled_rois, 1]
           sampled_class_weights: [batch_size, num_sampled_rois, 1]
         """
         if self.append_gt_boxes:
             # num_rois += num_gt
-            rois = tf.concat([rois, gt_boxes], axis=1)
-        num_rois = rois.get_shape().as_list()[1]
+            rois = ops.concatenate([rois, gt_boxes], axis=1)
+        num_rois = ops.shape(rois)[1]
         if num_rois is None:
             raise ValueError(
-                f"`rois` must have static shape, got {rois.get_shape()}"
+                f"`rois` must have static shape, got {ops.shape(rois)}"
             )
         if num_rois < self.num_sampled_rois:
             raise ValueError(
                 "num_rois must be less than `num_sampled_rois` "
                 f"({self.num_sampled_rois}), got {num_rois}"
             )
         rois = bounding_box.convert_format(
@@ -122,35 +119,35 @@
         # [batch_size, num_rois, num_gt]
         similarity_mat = iou.compute_iou(
             rois, gt_boxes, bounding_box_format="yxyx", use_masking=True
         )
         # [batch_size, num_rois] | [batch_size, num_rois]
         matched_gt_cols, matched_vals = self.roi_matcher(similarity_mat)
         # [batch_size, num_rois]
-        positive_matches = tf.math.equal(matched_vals, 1)
-        negative_matches = tf.math.equal(matched_vals, -1)
+        positive_matches = ops.equal(matched_vals, 1)
+        negative_matches = ops.equal(matched_vals, -1)
         self._positives.update_state(
-            tf.reduce_sum(tf.cast(positive_matches, tf.float32), axis=-1)
+            ops.sum(ops.cast(positive_matches, "float32"), axis=-1)
         )
         self._negatives.update_state(
-            tf.reduce_sum(tf.cast(negative_matches, tf.float32), axis=-1)
+            ops.sum(ops.cast(negative_matches, "float32"), axis=-1)
         )
         # [batch_size, num_rois, 1]
-        background_mask = tf.expand_dims(
-            tf.logical_not(positive_matches), axis=-1
+        background_mask = ops.expand_dims(
+            ops.logical_not(positive_matches), axis=-1
         )
         # [batch_size, num_rois, 1]
         matched_gt_classes = target_gather._target_gather(
             gt_classes, matched_gt_cols
         )
         # also set all background matches to `background_class`
-        matched_gt_classes = tf.where(
+        matched_gt_classes = ops.where(
             background_mask,
-            tf.cast(
-                self.background_class * tf.ones_like(matched_gt_classes),
+            ops.cast(
+                self.background_class * ops.ones_like(matched_gt_classes),
                 gt_classes.dtype,
             ),
             matched_gt_classes,
         )
         # [batch_size, num_rois, 4]
         matched_gt_boxes = target_gather._target_gather(
             gt_boxes, matched_gt_cols
@@ -159,28 +156,28 @@
             anchors=rois,
             boxes=matched_gt_boxes,
             anchor_format="yxyx",
             box_format="yxyx",
             variance=[0.1, 0.1, 0.2, 0.2],
         )
         # also set all background matches to 0 coordinates
-        encoded_matched_gt_boxes = tf.where(
+        encoded_matched_gt_boxes = ops.where(
             background_mask,
-            tf.zeros_like(matched_gt_boxes),
+            ops.zeros_like(matched_gt_boxes),
             encoded_matched_gt_boxes,
         )
         # [batch_size, num_rois]
         sampled_indicators = sampling.balanced_sample(
             positive_matches,
             negative_matches,
             self.num_sampled_rois,
             self.positive_fraction,
         )
         # [batch_size, num_sampled_rois] in the range of [0, num_rois)
-        sampled_indicators, sampled_indices = tf.math.top_k(
+        sampled_indicators, sampled_indices = ops.top_k(
             sampled_indicators, k=self.num_sampled_rois, sorted=True
         )
         # [batch_size, num_sampled_rois, 4]
         sampled_rois = target_gather._target_gather(rois, sampled_indices)
         # [batch_size, num_sampled_rois, 4]
         sampled_gt_boxes = target_gather._target_gather(
             encoded_matched_gt_boxes, sampled_indices
@@ -188,20 +185,20 @@
         # [batch_size, num_sampled_rois, 1]
         sampled_gt_classes = target_gather._target_gather(
             matched_gt_classes, sampled_indices
         )
         # [batch_size, num_sampled_rois, 1]
         # all negative samples will be ignored in regression
         sampled_box_weights = target_gather._target_gather(
-            tf.cast(positive_matches[..., tf.newaxis], gt_boxes.dtype),
+            ops.cast(positive_matches[..., None], gt_boxes.dtype),
             sampled_indices,
         )
         # [batch_size, num_sampled_rois, 1]
-        sampled_indicators = sampled_indicators[..., tf.newaxis]
-        sampled_class_weights = tf.cast(sampled_indicators, gt_classes.dtype)
+        sampled_indicators = sampled_indicators[..., None]
+        sampled_class_weights = ops.cast(sampled_indicators, gt_classes.dtype)
         return (
             sampled_rois,
             sampled_gt_boxes,
             sampled_box_weights,
             sampled_gt_classes,
             sampled_class_weights,
         )
@@ -219,8 +216,7 @@
         return dict(list(base_config.items()) + list(config.items()))
 
     @classmethod
     def from_config(cls, config, custom_objects=None):
         roi_matcher_config = config.pop("roi_matcher")
         roi_matcher = box_matcher.BoxMatcher(**roi_matcher_config)
         return cls(roi_matcher=roi_matcher, **config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection/rpn_label_encoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/rpn_label_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Mapping
-
-import tensorflow as tf
-from tensorflow import keras
+import tree
 
 from keras_cv.src import bounding_box
-from keras_cv.src.backend import assert_tf_keras
+from keras_cv.src.backend import keras
+from keras_cv.src.backend import ops
 from keras_cv.src.bounding_box import iou
 from keras_cv.src.layers.object_detection import box_matcher
 from keras_cv.src.layers.object_detection import sampling
 from keras_cv.src.utils import target_gather
 
 
 @keras.utils.register_keras_serializable(package="keras_cv")
@@ -69,15 +67,14 @@
         positive_threshold,
         negative_threshold,
         samples_per_image,
         positive_fraction,
         box_variance=[0.1, 0.1, 0.2, 0.2],
         **kwargs,
     ):
-        assert_tf_keras("keras_cv.layers._RpnLabelEncoder")
         super().__init__(**kwargs)
         self.anchor_format = anchor_format
         self.ground_truth_box_format = ground_truth_box_format
         self.positive_threshold = positive_threshold
         self.negative_threshold = negative_threshold
         self.samples_per_image = samples_per_image
         self.positive_fraction = positive_fraction
@@ -88,17 +85,17 @@
         )
         self.box_variance = box_variance
         self.built = True
         self._positives = keras.metrics.Mean(name="percent_boxes_matched")
 
     def call(
         self,
-        anchors_dict: Mapping[str, tf.Tensor],
-        gt_boxes: tf.Tensor,
-        gt_classes: tf.Tensor,
+        anchors_dict,
+        gt_boxes,
+        gt_classes,
     ):
         """
         Args:
           anchors_dict: dict of [num_anchors, 4] or [batch_size, num_anchors, 4]
             float Tensor for each level.
           gt_boxes: [num_gt, 4] or [batch_size, num_anchors] float Tensor.
           gt_classes: [num_gt, 1] float or integer Tensor.
@@ -108,74 +105,74 @@
           class_targets: dict of [num_anchors, 1] for each level.
           class_weights: dict of [num_anchors, 1] for each level.
         """
         pack = False
         anchors = anchors_dict
         if isinstance(anchors, dict):
             pack = True
-            anchors = tf.concat(tf.nest.flatten(anchors), axis=0)
+            anchors = ops.concatenate(tree.flatten(anchors), axis=0)
         anchors = bounding_box.convert_format(
             anchors, source=self.anchor_format, target="yxyx"
         )
         gt_boxes = bounding_box.convert_format(
             gt_boxes, source=self.ground_truth_box_format, target="yxyx"
         )
         # [num_anchors, num_gt] or [batch_size, num_anchors, num_gt]
         similarity_mat = iou.compute_iou(
             anchors, gt_boxes, bounding_box_format="yxyx"
         )
         # [num_anchors] or [batch_size, num_anchors]
         matched_gt_indices, matched_vals = self.box_matcher(similarity_mat)
         # [num_anchors] or [batch_size, num_anchors]
-        positive_matches = tf.math.equal(matched_vals, 1)
+        positive_matches = ops.equal(matched_vals, 1)
         # currently SyncOnReadVariable does not support `assign_add` in
         # cross-replica.
         #    self._positives.update_state(
         #        tf.reduce_sum(tf.cast(positive_matches, tf.float32), axis=-1)
         #    )
 
-        negative_matches = tf.math.equal(matched_vals, -1)
+        negative_matches = ops.equal(matched_vals, -1)
         # [num_anchors, 4] or [batch_size, num_anchors, 4]
         matched_gt_boxes = target_gather._target_gather(
             gt_boxes, matched_gt_indices
         )
         # [num_anchors, 4] or [batch_size, num_anchors, 4], used as `y_true` for
         # regression loss
         encoded_box_targets = bounding_box._encode_box_to_deltas(
             anchors,
             matched_gt_boxes,
             anchor_format="yxyx",
             box_format="yxyx",
             variance=self.box_variance,
         )
         # [num_anchors, 1] or [batch_size, num_anchors, 1]
-        box_sample_weights = tf.cast(
-            positive_matches[..., tf.newaxis], gt_boxes.dtype
+        box_sample_weights = ops.cast(
+            positive_matches[..., None], gt_boxes.dtype
         )
 
         # [num_anchors, 1] or [batch_size, num_anchors, 1]
-        positive_mask = tf.expand_dims(positive_matches, axis=-1)
+        positive_mask = ops.expand_dims(positive_matches, axis=-1)
         # set all negative and ignored matches to 0, and all positive matches to
         # 1 [num_anchors, 1] or [batch_size, num_anchors, 1]
-        positive_classes = tf.ones_like(positive_mask, dtype=gt_classes.dtype)
-        negative_classes = tf.zeros_like(positive_mask, dtype=gt_classes.dtype)
+        positive_classes = ops.ones_like(positive_mask, dtype=gt_classes.dtype)
+        negative_classes = ops.zeros_like(positive_mask, dtype=gt_classes.dtype)
         # [num_anchors, 1] or [batch_size, num_anchors, 1]
-        class_targets = tf.where(
+        class_targets = ops.where(
             positive_mask, positive_classes, negative_classes
         )
         # [num_anchors] or [batch_size, num_anchors]
         sampled_indicators = sampling.balanced_sample(
             positive_matches,
             negative_matches,
             self.samples_per_image,
             self.positive_fraction,
         )
         # [num_anchors, 1] or [batch_size, num_anchors, 1]
-        class_sample_weights = tf.cast(
-            sampled_indicators[..., tf.newaxis], gt_classes.dtype
+        class_sample_weights = ops.cast(
+            sampled_indicators[..., None], gt_classes.dtype
         )
         if pack:
             encoded_box_targets = self.unpack_targets(
                 encoded_box_targets, anchors_dict
             )
             box_sample_weights = self.unpack_targets(
                 box_sample_weights, anchors_dict
@@ -188,24 +185,24 @@
             encoded_box_targets,
             box_sample_weights,
             class_targets,
             class_sample_weights,
         )
 
     def unpack_targets(self, targets, anchors_dict):
-        target_shape = len(targets.get_shape().as_list())
+        target_shape = len(ops.shape(targets))
         if target_shape != 2 and target_shape != 3:
             raise ValueError(
                 "unpacking targets must be rank 2 or rank 3, got "
                 f"{target_shape}"
             )
         unpacked_targets = {}
         count = 0
         for level, anchors in anchors_dict.items():
-            num_anchors_lvl = anchors.get_shape().as_list()[0]
+            num_anchors_lvl = ops.shape(anchors)[0]
             if target_shape == 2:
                 unpacked_targets[level] = targets[
                     count : count + num_anchors_lvl, ...
                 ]
             else:
                 unpacked_targets[level] = targets[
                     :, count : count + num_anchors_lvl, ...
@@ -220,8 +217,7 @@
             "positive_threshold": self.positive_threshold,
             "negative_threshold": self.negative_threshold,
             "samples_per_image": self.samples_per_image,
             "positive_fraction": self.positive_fraction,
             "box_variance": self.box_variance,
         }
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection/sampling.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection/sampling.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import tensorflow as tf
+from keras_cv.src.backend import ops
+from keras_cv.src.backend import random
 
 
 def balanced_sample(
-    positive_matches: tf.Tensor,
-    negative_matches: tf.Tensor,
+    positive_matches,
+    negative_matches,
     num_samples: int,
     positive_fraction: float,
 ):
     """
     Sampling ops to balance positive and negative samples, deals with both
     batched and unbatched inputs.
 
@@ -36,48 +37,49 @@
 
     Returns:
       selected_indicators: [N] or [batch_size, N]
         integer Tensor, 1 for indicating the index is sampled, 0 for
         indicating the index is not sampled.
     """
 
-    N = positive_matches.get_shape().as_list()[-1]
+    N = ops.shape(positive_matches)[-1]
     if N < num_samples:
         raise ValueError(
             "passed in {positive_matches.shape} has less element than "
             f"{num_samples}"
         )
     # random_val = tf.random.uniform(tf.shape(positive_matches), minval=0.,
     # maxval=1.)
-    zeros = tf.zeros_like(positive_matches, dtype=tf.float32)
-    ones = tf.ones_like(positive_matches, dtype=tf.float32)
-    ones_rand = ones + tf.random.uniform(ones.shape, minval=-0.2, maxval=0.2)
-    halfs = 0.5 * tf.ones_like(positive_matches, dtype=tf.float32)
-    halfs_rand = halfs + tf.random.uniform(halfs.shape, minval=-0.2, maxval=0.2)
+    zeros = ops.zeros_like(positive_matches, dtype="float32")
+    ones = ops.ones_like(positive_matches, dtype="float32")
+    ones_rand = ones + random.uniform(ops.shape(ones), minval=-0.2, maxval=0.2)
+    halfs = 0.5 * ops.ones_like(positive_matches, dtype="float32")
+    halfs_rand = halfs + random.uniform(
+        ops.shape(halfs), minval=-0.2, maxval=0.2
+    )
     values = zeros
-    values = tf.where(positive_matches, ones_rand, values)
-    values = tf.where(negative_matches, halfs_rand, values)
+    values = ops.where(positive_matches, ones_rand, values)
+    values = ops.where(negative_matches, halfs_rand, values)
     num_pos_samples = int(num_samples * positive_fraction)
-    valid_matches = tf.logical_or(positive_matches, negative_matches)
+    valid_matches = ops.logical_or(positive_matches, negative_matches)
     # this might contain negative samples as well
-    _, positive_indices = tf.math.top_k(values, k=num_pos_samples)
-    selected_indicators = tf.cast(
-        tf.reduce_sum(tf.one_hot(positive_indices, depth=N), axis=-2), tf.bool
+    _, positive_indices = ops.top_k(values, k=num_pos_samples)
+    selected_indicators = ops.cast(
+        ops.sum(ops.one_hot(positive_indices, N), axis=-2), dtype="bool"
     )
     # setting all selected samples to zeros
-    values = tf.where(selected_indicators, zeros, values)
+    values = ops.where(selected_indicators, zeros, values)
     # setting all excessive positive matches to zeros as well
-    values = tf.where(positive_matches, zeros, values)
+    values = ops.where(positive_matches, zeros, values)
     num_neg_samples = num_samples - num_pos_samples
-    _, negative_indices = tf.math.top_k(values, k=num_neg_samples)
-    selected_indices = tf.concat([positive_indices, negative_indices], axis=-1)
-    selected_indicators = tf.reduce_sum(
-        tf.one_hot(selected_indices, depth=N), axis=-2
+    _, negative_indices = ops.top_k(values, k=num_neg_samples)
+    selected_indices = ops.concatenate(
+        [positive_indices, negative_indices], axis=-1
     )
-    selected_indicators = tf.minimum(
-        selected_indicators, tf.ones_like(selected_indicators)
+    selected_indicators = ops.sum(ops.one_hot(selected_indices, N), axis=-2)
+    selected_indicators = ops.minimum(
+        selected_indicators, ops.ones_like(selected_indicators)
     )
-    selected_indicators = tf.where(
-        valid_matches, selected_indicators, tf.zeros_like(selected_indicators)
+    selected_indicators = ops.where(
+        valid_matches, selected_indicators, ops.zeros_like(selected_indicators)
     )
     return selected_indicators
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection_3d/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/centernet_label_encoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection_3d/centernet_label_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,8 +462,7 @@
                     "heatmap": dense_heatmap_i,
                     "boxes": dense_box_3d_i,
                     "top_k_index": top_k_heatmap_feature_idx_i,
                 }
 
             inputs.update(centernet_targets)
             return inputs
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/heatmap_decoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection_3d/heatmap_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,8 +215,7 @@
             "max_num_box": self.max_num_box,
             "heatmap_threshold": self.heatmap_threshold,
             "voxel_size": self.voxel_size,
             "spatial_size": self.spatial_size,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/voxel_utils.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection_3d/voxel_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,8 +259,7 @@
         # for dim_i.
         slice_begin = tf.shape(x) + pad - shape
 
     x = tf.pad(x, paddings, constant_values=pad_val)
     x = tf.slice(x, slice_begin, shape)
 
     return tf.reshape(x, shape)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/voxelization.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/object_detection_3d/voxelization.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,8 +251,7 @@
         if out_shape[-2] == 1:
             out_shape = out_shape[:-2] + [out_shape[-1]]
         voxel_feature = ops.reshape(voxel_feature, out_shape)
         return voxel_feature
 
     def compute_output_shape(self, input_shape):
         return tuple([input_shape[0]] + self._voxel_spatial_size[:-1] + [128])
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/overlapping_patching_embedding.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/overlapping_patching_embedding.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             project_dim: integer, the dimensionality of the projection.
                 Defaults to `32`.
             patch_size: integer, the size of the patches to encode.
                 Defaults to `7`.
             stride: integer, the stride to use for the patching before
                 projection. Defaults to `5`.
 
-        Basic usage:
+        Example:
 
         ```
         project_dim = 1024
         patch_size = 16
 
         encoded_patches = keras_cv.layers.OverlappingPatchingAndEmbedding(
         project_dim=project_dim, patch_size=patch_size)(img_batch)
@@ -79,8 +79,7 @@
             {
                 "project_dim": self.project_dim,
                 "patch_size": self.patch_size,
                 "stride": self.stride,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,48 +32,55 @@
 from keras_cv.src.layers.preprocessing.grid_mask import GridMask
 from keras_cv.src.layers.preprocessing.jittered_resize import JitteredResize
 from keras_cv.src.layers.preprocessing.mix_up import MixUp
 from keras_cv.src.layers.preprocessing.mosaic import Mosaic
 from keras_cv.src.layers.preprocessing.posterization import Posterization
 from keras_cv.src.layers.preprocessing.rand_augment import RandAugment
 from keras_cv.src.layers.preprocessing.random_apply import RandomApply
-from keras_cv.src.layers.preprocessing.random_aspect_ratio import RandomAspectRatio
+from keras_cv.src.layers.preprocessing.random_aspect_ratio import (
+    RandomAspectRatio,
+)
 from keras_cv.src.layers.preprocessing.random_augmentation_pipeline import (
     RandomAugmentationPipeline,
 )
 from keras_cv.src.layers.preprocessing.random_brightness import RandomBrightness
 from keras_cv.src.layers.preprocessing.random_channel_shift import (
     RandomChannelShift,
 )
 from keras_cv.src.layers.preprocessing.random_choice import RandomChoice
 from keras_cv.src.layers.preprocessing.random_color_degeneration import (
     RandomColorDegeneration,
 )
-from keras_cv.src.layers.preprocessing.random_color_jitter import RandomColorJitter
+from keras_cv.src.layers.preprocessing.random_color_jitter import (
+    RandomColorJitter,
+)
 from keras_cv.src.layers.preprocessing.random_contrast import RandomContrast
 from keras_cv.src.layers.preprocessing.random_crop import RandomCrop
 from keras_cv.src.layers.preprocessing.random_crop_and_resize import (
     RandomCropAndResize,
 )
 from keras_cv.src.layers.preprocessing.random_cutout import RandomCutout
 from keras_cv.src.layers.preprocessing.random_flip import RandomFlip
 from keras_cv.src.layers.preprocessing.random_gaussian_blur import (
     RandomGaussianBlur,
 )
 from keras_cv.src.layers.preprocessing.random_hue import RandomHue
-from keras_cv.src.layers.preprocessing.random_jpeg_quality import RandomJpegQuality
+from keras_cv.src.layers.preprocessing.random_jpeg_quality import (
+    RandomJpegQuality,
+)
 from keras_cv.src.layers.preprocessing.random_rotation import RandomRotation
 from keras_cv.src.layers.preprocessing.random_saturation import RandomSaturation
 from keras_cv.src.layers.preprocessing.random_sharpness import RandomSharpness
 from keras_cv.src.layers.preprocessing.random_shear import RandomShear
-from keras_cv.src.layers.preprocessing.random_translation import RandomTranslation
+from keras_cv.src.layers.preprocessing.random_translation import (
+    RandomTranslation,
+)
 from keras_cv.src.layers.preprocessing.random_zoom import RandomZoom
 from keras_cv.src.layers.preprocessing.repeated_augmentation import (
     RepeatedAugmentation,
 )
 from keras_cv.src.layers.preprocessing.rescaling import Rescaling
 from keras_cv.src.layers.preprocessing.resizing import Resizing
 from keras_cv.src.layers.preprocessing.solarization import Solarization
 from keras_cv.src.layers.preprocessing.vectorized_base_image_augmentation_layer import (  # noqa: E501
     VectorizedBaseImageAugmentationLayer,
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/aug_mix.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/aug_mix.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         seed: Integer. Used to create a random seed.
 
     References:
         - [AugMix paper](https://arxiv.org/pdf/1912.02781)
         - [Official Code](https://github.com/google-research/augmix)
         - [Unofficial TF Code](https://github.com/szacho/augmix-tf)
 
-    Sample Usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     augmix = keras_cv.layers.AugMix([0, 255])
     augmented_images = augmix(images[:100])
     ```
     """
 
@@ -386,8 +386,7 @@
             "num_chains": self.num_chains,
             "chain_depth": self.chain_depth,
             "alpha": self.alpha,
             "seed": self.seed,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/auto_contrast.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/auto_contrast.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,8 +93,7 @@
             image, transformations=transformation, **kwargs
         )
 
     def get_config(self):
         config = super().get_config()
         config.update({"value_range": self.value_range})
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/base_image_augmentation_layer.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/base_image_augmentation_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -603,8 +603,7 @@
             self.compute_dtype,
         )
         if BOUNDING_BOXES in inputs:
             inputs[BOUNDING_BOXES] = bounding_box.ensure_tensor(
                 inputs[BOUNDING_BOXES], dtype=self.compute_dtype
             )
         return inputs
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/channel_shuffle.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/channel_shuffle.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         3D (unbatched) or 4D (batched) tensor with shape:
         `(..., height, width, channels)`, in `"channels_last"` format
 
     Args:
         groups: Number of groups to divide the input channels, defaults to 3.
         seed: Integer. Used to create a random seed.
 
-    Usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     channel_shuffle = ChannelShuffle(groups=3)
     augmented_images = channel_shuffle(images)
     ```
     """
 
@@ -120,8 +120,7 @@
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/cut_mix.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/cut_mix.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,8 +211,7 @@
     def get_config(self):
         config = {
             "alpha": self.alpha,
             "seed": self.seed,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/equalization.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/equalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         value_range: a tuple or a list of two elements. The first value
             represents the lower bound for values in passed images, the second
             represents the upper bound. Images passed to the layer should have
             values within `value_range`.
         bins: Integer indicating the number of bins to use in histogram
             equalization. Should be in the range [0, 256].
 
-    Usage:
+    Example:
     ```python
     equalize = Equalization()
 
     (images, labels), _ = keras.datasets.cifar10.load_data()
     # Note that images are an int8 Tensor with values in the range [0, 255]
     images = equalize(images)
     ```
@@ -184,8 +184,7 @@
         )
         return tf.squeeze(image, axis=0)
 
     def get_config(self):
         config = super().get_config()
         config.update({"bins": self.bins, "value_range": self.value_range})
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/fourier_mix.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/fourier_mix.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             is a recommended value in the paper.
         decay_power: A float value representing the decay power, defaults to 3,
             as recommended in the paper.
         seed: Integer. Used to create a random seed.
     References:
         - [FMix paper](https://arxiv.org/abs/2002.12047).
 
-    Sample usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     fourier_mix = keras_cv.layers.preprocessing.FourierMix(0.5)
     augmented_images, updated_labels = fourier_mix(
         {'images': images, 'labels': labels}
     )
     # output == {'images': updated_images, 'labels': updated_labels}
@@ -243,8 +243,7 @@
         config = {
             "alpha": self.alpha,
             "decay_power": self.decay_power,
             "seed": self.seed,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/grayscale.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/grayscale.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             Number color channels present in the output image.
             The output_channels can be 1 or 3. RGB image with shape
             (..., height, width, 3) will have the following shapes
             after the `Grayscale` operation:
                  a. (..., height, width, 1) if output_channels = 1
                  b. (..., height, width, 3) if output_channels = 3.
 
-    Usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     to_grayscale = keras_cv.layers.preprocessing.Grayscale()
     augmented_images = to_grayscale(images)
     ```
     """
 
@@ -97,8 +97,7 @@
 
     def get_config(self):
         config = {
             "output_channels": self.output_channels,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/grid_mask.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/grid_mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     Args:
         ratio_factor: A float, tuple of two floats, or `keras_cv.FactorSampler`.
             Ratio determines the ratio from spacings to grid masks.
             Lower values make the grid
             size smaller, and higher values make the grid mask large.
             Floats should be in the range [0, 1]. 0.5 indicates that grid and
             spacing will be of equal size. To always use the same value, pass a
-            `keras_cv.ConstantFactorSampler()`.
+            `keras_cv.src.ConstantFactorSampler()`.
 
             Defaults to `(0, 0.5)`.
         rotation_factor:
             The rotation_factor will be used to randomly rotate the grid_mask
             during training. Default to 0.1, which results in an output rotating
             by a random amount in the range [-10% * 2pi, 10% * 2pi].
 
@@ -78,15 +78,15 @@
             - *constant*: Pixels are filled with the same constant value.
             - *gaussian_noise*: Pixels are filled with random gaussian noise.
         fill_value: an integer represents of value to be filled inside the
             gridblock when `fill_mode="constant"`. Valid integer range
             [0 to 255]
         seed: Integer. Used to create a random seed.
 
-    Usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     random_gridmask = keras_cv.layers.preprocessing.GridMask()
     augmented_images = random_gridmask(images)
     ```
 
     References:
@@ -257,8 +257,7 @@
             "rotation_factor": self.rotation_factor,
             "fill_mode": self.fill_mode,
             "fill_value": self.fill_value,
             "seed": self.seed,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/jittered_resize.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/jittered_resize.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             for more details on supported bounding box formats.
         interpolation: String, the interpolation method, defaults to
             `"bilinear"`. Supports `"bilinear"`, `"nearest"`, `"bicubic"`,
             `"area"`, `"lanczos3"`, `"lanczos5"`, `"gaussian"`,
             `"mitchellcubic"`.
         seed: (Optional) integer to use as the random seed.
 
-    Usage:
+    Example:
     ```python
     train_ds = load_object_detection_dataset()
     jittered_resize = layers.JitteredResize(
         target_size=(640, 640),
         scale_factor=(0.8, 1.25),
         bounding_box_format="xywh",
     )
@@ -306,8 +306,7 @@
             }
         )
         return config
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/mix_up.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/mix_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             recommended value when training an imagenet1k classification model.
         seed: Integer. Used to create a random seed.
 
     References:
         - [MixUp paper](https://arxiv.org/abs/1710.09412).
         - [MixUp for Object Detection paper](https://arxiv.org/pdf/1902.04103).
 
-    Sample usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     images, labels = images[:10], labels[:10]
     # Labels must be floating-point and one-hot encoded
     labels = tf.cast(tf.one_hot(labels, 10), tf.float32)
     mixup = keras_cv.layers.preprocessing.MixUp(10)
     augmented_images, updated_labels = mixup(
@@ -195,8 +195,7 @@
     def get_config(self):
         config = {
             "alpha": self.alpha,
             "seed": self.seed,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/mosaic.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/mosaic.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         seed: integer, used to create a random seed.
 
     References:
         - [Yolov4 paper](https://arxiv.org/pdf/2004.10934).
         - [Yolov5 implementation](https://github.com/ultralytics/yolov5).
         - [YoloX implementation](https://github.com/Megvii-BaseDetection/YOLOX)
 
-    Sample usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     labels = tf.one_hot(labels,10)
     labels = tf.cast(tf.squeeze(labels), tf.float32)
     mosaic = keras_cv.layers.preprocessing.Mosaic()
     output = mosaic({'images': images, 'labels': labels})
     # output == {'images': updated_images, 'labels': updated_labels}
@@ -329,8 +329,7 @@
         base_config = super().get_config()
 
         return dict(list(base_config.items()) + list(config.items()))
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/posterization.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/posterization.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,30 +33,30 @@
         value_range: a tuple or a list of two elements. The first value
             represents the lower bound for values in passed images, the second
             represents the upper bound. Images passed to the layer should have
             values within `value_range`. Defaults to `(0, 255)`.
         bits: integer, the number of bits to keep for each channel. Must be a
             value between 1-8.
 
-     Usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     print(images[0, 0, 0])
     # [59 62 63]
     # Note that images are Tensors with values in the range [0, 255] and uint8
     dtype
     posterization = Posterization(bits=4, value_range=[0, 255])
     images = posterization(images)
     print(images[0, 0, 0])
     # [48., 48., 48.]
     # NOTE: the layer will output values in tf.float32, regardless of input
         dtype.
     ```
 
-     Call arguments:
+    Call arguments:
         inputs: input tensor in two possible formats:
             1. single 3D (HWC) image or 4D (NHWC) batch of images.
             2. A dict of tensors where the images are under `"images"` key.
     """  # noqa: E501
 
     def __init__(self, value_range, bits, **kwargs):
         super().__init__(**kwargs)
@@ -114,8 +114,7 @@
     def augment_label(self, label, transformation=None, **kwargs):
         return label
 
     def get_config(self):
         config = {"bits": 8 - self._shift, "value_range": self._value_range}
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/rand_augment.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/rand_augment.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             this to `10/11`. The original `RandAugment` paper includes an
             Identity transform. By setting the rate to 10/11 in our
             implementation, the behavior is identical to sampling an Identity
             augmentation 10/11th of the time. Defaults to `1.0`.
         geometric: whether to include geometric augmentations. This
             should be set to False when performing object detection. Defaults to
             True.
-    Usage:
+    Example:
     ```python
     (x_test, y_test), _ = keras.datasets.cifar10.load_data()
     rand_augment = keras_cv.layers.RandAugment(
         value_range=(0, 255), augmentations_per_image=3, magnitude=0.5
     )
     x_test = rand_augment(x_test)
     ```
@@ -299,8 +299,7 @@
 
 
 def create_rand_augment_policy(magnitude, magnitude_stddev):
     result = {}
     for name, policy_fn in POLICY_PAIRS.items():
         result[name] = policy_fn(magnitude, magnitude_stddev)
     return result
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_apply.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_apply.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             layer. This is useful when using `MixUp()`, `CutMix()`, `Mosaic()`,
             etc.
         auto_vectorize: bool, whether to use tf.vectorized_map or tf.map_fn for
             batched input. Setting this to True might give better performance
             but currently doesn't work with XLA. Defaults to False.
         seed: integer, controls random behaviour.
 
-    Example usage:
+    Example:
     ```
     # Let's declare an example layer that will set all image pixels to zero.
     zero_out = keras.layers.Lambda(lambda x: {"images": 0 * x["images"]})
 
     # Create a small batch of random, single-channel, 2x2 images:
     images = tf.random.stateless_uniform(shape=(5, 2, 2, 1), seed=[0, 1])
     print(images[..., 0])
@@ -138,8 +138,7 @@
                 "layer": self._layer,
                 "seed": self.seed,
                 "batchwise": self.batchwise,
                 "auto_vectorize": self.auto_vectorize,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_aspect_ratio.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_aspect_ratio.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,8 +128,7 @@
             "factor": self.factor,
             "interpolation": self.interpolation,
             "bounding_box_format": self.bounding_box_format,
             "seed": self.seed,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_augmentation_pipeline.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_augmentation_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     the policy then selects a random layer from the provided list of `layers`.
     It then calls the `layer()` on the inputs. This is done
     `augmentations_per_image` times.
 
     This layer can be used to create custom policies resembling `RandAugment` or
     `AutoAugment`.
 
-    Usage:
+    Example:
     ```python
     # construct a list of layers
     layers = keras_cv.layers.RandAugment.get_standard_policy(
         value_range=(0, 255), magnitude=0.75, magnitude_stddev=0.3
     )
     layers = layers[:4]  # slice out some layers you don't want for whatever
                            reason
@@ -126,8 +126,7 @@
     def from_config(cls, config):
         layers = config.pop("layers", None)
         if layers:
             if isinstance(layers[0], dict):
                 layers = keras.utils.deserialize_keras_object(layers)
             config["layers"] = layers
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_brightness.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_brightness.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     Inputs: 3D (HWC) or 4D (NHWC) tensor, with float or int dtype. Input pixel
       values can be of any range (e.g. `[0., 1.)` or `[0, 255]`)
     Output: 3D (HWC) or 4D (NHWC) tensor with brightness adjusted based on the
       `factor`. By default, the layer will output floats. The output value will
       be clipped to the range `[0, 255]`, the valid range of RGB colors, and
       rescaled based on the `value_range` if needed.
 
-    Usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     random_brightness = keras_cv.layers.preprocessing.RandomBrightness()
     augmented_images = random_brightness(images)
     ```
     """
 
@@ -123,8 +123,7 @@
     @classmethod
     def from_config(cls, config):
         if isinstance(config["factor"], dict):
             config["factor"] = keras.utils.deserialize_keras_object(
                 config["factor"]
             )
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_channel_shift.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_channel_shift.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             interpret as equivalent to the tuple `(0.0, factor)`. The `factor`
             will sample between its range for every image to augment.
         channels: integer, the number of channels to shift, defaults to 3 which
             corresponds to an RGB shift. In some cases, there may ber more or
             less channels.
         seed: Integer. Used to create a random seed.
 
-    Usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     rgb_shift = keras_cv.layers.RandomChannelShift(value_range=(0, 255),
         factor=0.5)
     augmented_images = rgb_shift(images)
     ```
     """
@@ -115,8 +115,7 @@
                 "factor": self.factor,
                 "channels": self.channels,
                 "value_range": self.value_range,
                 "seed": self.seed,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_choice.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_choice.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class RandomChoice(BaseImageAugmentationLayer):
     """RandomChoice constructs a pipeline based on provided arguments.
 
     The implemented policy does the following: for each input provided in
     `call`(), the policy selects a random layer from the provided list of
     `layers`. It then calls the `layer()` on the inputs.
 
-    Usage:
+    Example:
     ```python
     # construct a list of layers
     layers = keras_cv.layers.RandAugment.get_standard_policy(
         value_range=(0, 255), magnitude=0.75, magnitude_stddev=0.3
     )
     layers = layers[:4]  # slice out some layers you don't want for whatever
                            reason
@@ -117,8 +117,7 @@
                 "layers": self.layers,
                 "auto_vectorize": self.auto_vectorize,
                 "seed": self.seed,
                 "batchwise": self.batchwise,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_color_degeneration.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_color_degeneration.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,8 +99,7 @@
     @classmethod
     def from_config(cls, config):
         if isinstance(config["factor"], dict):
             config["factor"] = keras.utils.deserialize_keras_object(
                 config["factor"]
             )
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_color_jitter.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_color_jitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             contrast adjustment available. If a tuple is used, a `factor` is
             sampled between the two values for every image augmented. If a
             single float is used, a value between `0.0` and the passed float is
             sampled. In order to ensure the value is always the same, please
             pass a tuple with two identical floats: `(0.5, 0.5)`.
         seed: Integer. Used to create a random seed.
 
-    Usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     color_jitter = keras_cv.layers.RandomColorJitter(
             value_range=(0, 255),
             brightness_factor=(-0.2, 0.5),
             contrast_factor=(0.5, 0.9),
             saturation_factor=(0.5, 0.9),
@@ -160,8 +160,7 @@
             }
         )
         return config
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_contrast.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_contrast.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             size 2 representing lower and upper bound. When represented as a
             single float, lower = upper. The contrast factor will be randomly
             picked between `[1.0 - lower, 1.0 + upper]`. For any pixel x in the
             channel, the output will be `(x - mean) * factor + mean` where
             `mean` is the mean value of the channel.
         seed: Integer. Used to create a random seed.
 
-    Usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     random_contrast = keras_cv.layers.preprocessing.RandomContrast()
     augmented_images = random_contrast(images)
     ```
     """
 
@@ -118,8 +118,7 @@
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_crop.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,8 +307,7 @@
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_crop_and_resize.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_crop_and_resize.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,8 +291,7 @@
             [0],  # box_indices: maps boxes to images along batch axis
             # [0] since there is only one image
             self.target_size,  # output size
             method=method or self.interpolation,
         )
 
         return tf.squeeze(augmented_image, axis=0)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_cutout.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_cutout.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             mode (one of `{"constant", "gaussian_noise"}`).
             - *constant*: Pixels are filled with the same constant value.
             - *gaussian_noise*: Pixels are filled with random gaussian noise.
         fill_value: a float represents the value to be filled inside the patches
             when `fill_mode="constant"`.
         seed: Integer. Used to create a random seed.
 
-    Sample usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     random_cutout = keras_cv.layers.preprocessing.RandomCutout(0.5, 0.5)
     augmented_images = random_cutout(images)
     ```
     """
 
@@ -246,8 +246,7 @@
                 "width_factor": self.width_factor,
                 "fill_mode": self.fill_mode,
                 "fill_value": self.fill_value,
                 "seed": self.seed,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_flip.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_flip.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,8 +245,7 @@
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_gaussian_blur.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_gaussian_blur.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,8 +118,7 @@
         blur_filter /= tf.reduce_sum(blur_filter)
         return blur_filter
 
     def get_config(self):
         config = super().get_config()
         config.update({"factor": self.factor, "kernel_size": self.kernel_size})
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_hue.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_hue.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             pass a tuple with two identical floats: `(0.5, 0.5)`.
         value_range: the range of values the incoming images will have.
             Represented as a two number tuple written [low, high]. This is
             typically either `[0, 1]` or `[0, 255]` depending on how your
             preprocessing pipeline is set up.
         seed: Integer. Used to create a random seed.
 
-    Usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     random_hue = keras_cv.layers.preprocessing.RandomHue()
     augmented_images = random_hue(images)
     ```
     """
 
@@ -125,8 +125,7 @@
     @classmethod
     def from_config(cls, config):
         if isinstance(config["factor"], dict):
             config["factor"] = keras.utils.deserialize_keras_object(
                 config["factor"]
             )
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_jpeg_quality.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_jpeg_quality.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,84 @@
-# Copyright 2022 The KerasCV Authors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import tensorflow as tf
-
-from keras_cv.src.api_export import keras_cv_export
-from keras_cv.src.layers.preprocessing.base_image_augmentation_layer import (
-    BaseImageAugmentationLayer,
-)
-from keras_cv.src.utils import preprocessing
-
-
-@keras_cv_export("keras_cv.layers.RandomJpegQuality")
-class RandomJpegQuality(BaseImageAugmentationLayer):
-    """Applies Random Jpeg compression artifacts to an image.
-
-    Performs the jpeg compression algorithm on the image. This layer can be used
-    in order to ensure your model is robust to artifacts introduced by JPEG
-    compression.
-
-    Args:
-        factor: 2 element tuple or 2 element list. During augmentation, a random
-        number is drawn from the factor distribution. This value is passed to
-        `tf.image.adjust_jpeg_quality()`.
-        seed: Integer. Used to create a random seed.
-
-    Usage:
-    ```python
-    layer = keras_cv.RandomJpegQuality(factor=(75, 100)))
-    (images, labels), _ = keras.datasets.cifar10.load_data()
-    augmented_images = layer(images)
-    ```
-    """
-
-    def __init__(self, factor, seed=None, **kwargs):
-        super().__init__(**kwargs)
-        if isinstance(factor, (float, int)):
-            raise ValueError(
-                "RandomJpegQuality() expects factor to be a 2 element "
-                "tuple, list or a `keras_cv.FactorSampler`. "
-                "RandomJpegQuality() received `factor={factor}`."
-            )
-        self.seed = seed
-        self.factor = preprocessing.parse_factor(
-            factor,
-            min_value=0,
-            max_value=100,
-            param_name="factor",
-            seed=self.seed,
-        )
-
-    def get_random_transformation(self, **kwargs):
-        return self.factor(dtype=tf.int32)
-
-    def augment_image(self, image, transformation=None, **kwargs):
-        jpeg_quality = transformation
-        return tf.image.adjust_jpeg_quality(image, jpeg_quality)
-
-    def augment_bounding_boxes(self, bounding_boxes, **kwargs):
-        return bounding_boxes
-
-    def augment_label(self, label, transformation=None, **kwargs):
-        return label
-
-    def augment_segmentation_mask(
-        self, segmentation_mask, transformation, **kwargs
-    ):
-        return segmentation_mask
-
-    def get_config(self):
-        config = super().get_config()
-        config.update({"factor": self.factor, "seed": self.seed})
-        return config
-
+# Copyright 2022 The KerasCV Authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import tensorflow as tf
+
+from keras_cv.src.api_export import keras_cv_export
+from keras_cv.src.layers.preprocessing.base_image_augmentation_layer import (
+    BaseImageAugmentationLayer,
+)
+from keras_cv.src.utils import preprocessing
+
+
+@keras_cv_export("keras_cv.layers.RandomJpegQuality")
+class RandomJpegQuality(BaseImageAugmentationLayer):
+    """Applies Random Jpeg compression artifacts to an image.
+
+    Performs the jpeg compression algorithm on the image. This layer can be used
+    in order to ensure your model is robust to artifacts introduced by JPEG
+    compression.
+
+    Args:
+        factor: 2 element tuple or 2 element list. During augmentation, a random
+        number is drawn from the factor distribution. This value is passed to
+        `tf.image.adjust_jpeg_quality()`.
+        seed: Integer. Used to create a random seed.
+
+    Example:
+    ```python
+    layer = keras_cv.RandomJpegQuality(factor=(75, 100)))
+    (images, labels), _ = keras.datasets.cifar10.load_data()
+    augmented_images = layer(images)
+    ```
+    """
+
+    def __init__(self, factor, seed=None, **kwargs):
+        super().__init__(**kwargs)
+        if isinstance(factor, (float, int)):
+            raise ValueError(
+                "RandomJpegQuality() expects factor to be a 2 element "
+                "tuple, list or a `keras_cv.FactorSampler`. "
+                "RandomJpegQuality() received `factor={factor}`."
+            )
+        self.seed = seed
+        self.factor = preprocessing.parse_factor(
+            factor,
+            min_value=0,
+            max_value=100,
+            param_name="factor",
+            seed=self.seed,
+        )
+
+    def get_random_transformation(self, **kwargs):
+        return self.factor(dtype=tf.int32)
+
+    def augment_image(self, image, transformation=None, **kwargs):
+        jpeg_quality = transformation
+        return tf.image.adjust_jpeg_quality(image, jpeg_quality)
+
+    def augment_bounding_boxes(self, bounding_boxes, **kwargs):
+        return bounding_boxes
+
+    def augment_label(self, label, transformation=None, **kwargs):
+        return label
+
+    def augment_segmentation_mask(
+        self, segmentation_mask, transformation, **kwargs
+    ):
+        return segmentation_mask
+
+    def get_config(self):
+        config = super().get_config()
+        config.update({"factor": self.factor, "seed": self.seed})
+        return config
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_rotation.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_rotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,8 +284,7 @@
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_saturation.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_saturation.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             Values should be between `0.0` and `1.0`. If a tuple is used, a
             `factor` is sampled between the two values for every image
             augmented. If a single float is used, a value between `0.0` and the
             passed float is sampled. In order to ensure the value is always the
             same, please pass a tuple with two identical floats: `(0.5, 0.5)`.
         seed: Integer. Used to create a random seed.
 
-    Usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     random_saturation = keras_cv.layers.preprocessing.RandomSaturation()
     augmented_images = random_saturation(images)
     ```
     """
 
@@ -120,8 +120,7 @@
     @classmethod
     def from_config(cls, config):
         if isinstance(config["factor"], dict):
             config["factor"] = keras.utils.deserialize_keras_object(
                 config["factor"]
             )
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_sharpness.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_sharpness.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,8 +148,7 @@
             {
                 "factor": self.factor,
                 "value_range": self.value_range,
                 "seed": self.seed,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_shear.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_shear.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,8 +360,7 @@
                 "fill_mode": self.fill_mode,
                 "fill_value": self.fill_value,
                 "bounding_box_format": self.bounding_box_format,
                 "seed": self.seed,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_translation.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_translation.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,8 +288,7 @@
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_zoom.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/random_zoom.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,8 +271,7 @@
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/repeated_augmentation.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/repeated_augmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     This layer increases your batch size by a factor of `len(augmenters)`.
 
     Args:
         augmenters: the augmenters to use to augment the image
         shuffle: whether to shuffle the result. Essential when using an
             asynchronous distribution strategy such as ParameterServerStrategy.
 
-    Usage:
+    Example:
 
     List of identical augmenters:
     ```python
     repeated_augment = cv_layers.RepeatedAugmentation(
         augmenters=[cv_layers.RandAugment(value_range=(0, 255))] * 8
     )
     inputs = {
@@ -124,8 +124,7 @@
     @classmethod
     def from_config(cls, config):
         if config["augmenters"] and isinstance(config["augmenters"][0], dict):
             config["augmenters"] = keras.utils.deserialize_keras_object(
                 config["augmenters"]
             )
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/rescaling.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/rescaling.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,8 +82,7 @@
     def get_config(self):
         config = {
             "scale": self.scale,
             "offset": self.offset,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/resizing.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/resizing.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,8 +389,7 @@
             "interpolation": self.interpolation,
             "crop_to_aspect_ratio": self.crop_to_aspect_ratio,
             "pad_to_aspect_ratio": self.pad_to_aspect_ratio,
             "bounding_box_format": self.bounding_box_format,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/solarization.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/solarization.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         threshold_factor: (Optional)  A tuple of two floats, a single float or
             a `keras_cv.FactorSampler`. For each augmented image a value is
             sampled from the provided range. If a float is passed, the range is
             interpreted as `(0, threshold_factor)`. If specified, only pixel
             values above this threshold will be solarized.
         seed: Integer. Used to create a random seed.
 
-    Usage:
+    Example:
     ```python
     (images, labels), _ = keras.datasets.cifar10.load_data()
     print(images[0, 0, 0])
     # [59 62 63]
     # Note that images are Tensor with values in the range [0, 255]
     solarization = Solarization(value_range=(0, 255))
     images = solarization(images)
@@ -161,8 +161,7 @@
                 config["threshold_factor"]
             )
         if isinstance(config["addition_factor"], dict):
             config["addition_factor"] = keras.utils.deserialize_keras_object(
                 config["addition_factor"]
             )
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/vectorized_base_image_augmentation_layer.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing/vectorized_base_image_augmentation_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -564,8 +564,7 @@
             raise ValueError(
                 "Bounding boxes are missing class_id. If you would like to pad "
                 "the bounding boxes with class_id, use: "
                 "`bounding_boxes['classes'] = "
                 "tf.ones_like(bounding_boxes['boxes'])`."
             )
         return bounding_boxes
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,21 +29,22 @@
 )
 from keras_cv.src.layers.preprocessing_3d.waymo.global_random_rotation import (
     GlobalRandomRotation,
 )
 from keras_cv.src.layers.preprocessing_3d.waymo.global_random_scaling import (
     GlobalRandomScaling,
 )
-from keras_cv.src.layers.preprocessing_3d.waymo.global_random_translation import (
+from keras_cv.src.layers.preprocessing_3d.waymo.global_random_translation import (  # noqa: E501
     GlobalRandomTranslation,
 )
 from keras_cv.src.layers.preprocessing_3d.waymo.group_points_by_bounding_boxes import (  # noqa: E501
     GroupPointsByBoundingBoxes,
 )
 from keras_cv.src.layers.preprocessing_3d.waymo.random_copy_paste import (
     RandomCopyPaste,
 )
-from keras_cv.src.layers.preprocessing_3d.waymo.random_drop_box import RandomDropBox
+from keras_cv.src.layers.preprocessing_3d.waymo.random_drop_box import (
+    RandomDropBox,
+)
 from keras_cv.src.layers.preprocessing_3d.waymo.swap_background import (
     SwapBackground,
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/base_augmentation_layer_3d.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/base_augmentation_layer_3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,8 +285,7 @@
                 axis=-1,
             )
         )
 
     boxes = tf.concat(box_tensors, axis=-1)
 
     return point_clouds, boxes
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_dropping_points.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_dropping_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,8 +146,7 @@
         for excluded_class in self._exclude_classes:
             protected_points |= point_clouds[0, :, -1] == excluded_class
         point_mask = tf.where(
             protected_points[tf.newaxis, :, tf.newaxis], True, point_mask
         )
         point_clouds = tf.where(point_mask, point_clouds, 0.0)
         return (point_clouds, bounding_boxes)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_point_feature_noise.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_point_feature_noise.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,8 +154,7 @@
 
         no_noise = tf.ones_like(point_noise, point_noise.dtype)
         point_noise = tf.where(
             protected_points[:, :, tf.newaxis], no_noise, point_noise
         )
         point_clouds *= point_noise
         return (point_clouds, bounding_boxes)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_dropping_points.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_dropping_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,8 +82,7 @@
             protected_points |= point_clouds[0, :, -1] == excluded_class
 
         point_mask = tf.where(
             protected_points[tf.newaxis, :, tf.newaxis], True, point_mask
         )
         point_clouds = tf.where(point_mask, point_clouds, 0.0)
         return (point_clouds, bounding_boxes)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_flip.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_flip.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,8 +103,7 @@
 
     def get_config(self):
         return {
             "flip_x": self.flip_x,
             "flip_y": self.flip_y,
             "flip_z": self.flip_z,
         }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_rotation.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_rotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,8 +147,7 @@
                 bounding_boxes_heading,
                 bounding_boxes[..., CENTER_XYZ_DXDYDZ_PHI.CLASS :],
             ],
             axis=-1,
         )
 
         return (point_clouds, bounding_boxes)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_scaling.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_scaling.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,8 +185,7 @@
                 bounding_boxes_xyzdxdydz,
                 bounding_boxes[..., CENTER_XYZ_DXDYDZ_PHI.PHI :],
             ],
             axis=-1,
         )
 
         return (point_clouds, bounding_boxes)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_translation.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_translation.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,8 +120,7 @@
                 bounding_boxes_xyz,
                 bounding_boxes[..., CENTER_XYZ_DXDYDZ_PHI.DX :],
             ],
             axis=-1,
         )
 
         return (point_clouds, bounding_boxes)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/group_points_by_bounding_boxes.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/group_points_by_bounding_boxes.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,8 +267,7 @@
                 "Point clouds augmentation layers are expecting inputs "
                 "point clouds and bounding boxes to be rank 3D (Frame, "
                 "Point, Feature) or 4D (Batch, Frame, Point, Feature) "
                 "tensors. Got shape: {} and {}".format(
                     point_clouds.shape, bounding_boxes.shape
                 )
             )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/random_copy_paste.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/random_copy_paste.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,8 +286,7 @@
                 "Point clouds augmentation layers are expecting inputs "
                 "point clouds and bounding boxes to be rank 3D (Frame, "
                 "Point, Feature) or 4D (Batch, Frame, Point, Feature) "
                 "tensors. Got shape: {} and {}".format(
                     point_clouds.shape, bounding_boxes.shape
                 )
             )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/random_drop_box.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/random_drop_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,8 +119,7 @@
             tf.where(~drop_points_mask, point_clouds, 0.0),
             tf.where(
                 ~drop_bounding_boxes_mask[tf.newaxis, :, tf.newaxis],
                 bounding_boxes,
                 0.0,
             ),
         )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/swap_background.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/preprocessing_3d/waymo/swap_background.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,8 +168,7 @@
             bounding_boxes=bounding_boxes,
             transformation=transformation,
         )
         result.update(
             {POINT_CLOUDS: point_clouds, BOUNDING_BOXES: bounding_boxes}
         )
         return result
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/regularization/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/regularization/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,7 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from keras_cv.src.layers.regularization.drop_path import DropPath
 from keras_cv.src.layers.regularization.dropblock_2d import DropBlock2D
 from keras_cv.src.layers.regularization.squeeze_excite import SqueezeAndExcite2D
 from keras_cv.src.layers.regularization.stochastic_depth import StochasticDepth
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/regularization/drop_path.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/regularization/drop_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         - [FractalNet](https://arxiv.org/abs/1605.07648v4).
         - [rwightman/pytorch-image-models](https://github.com/rwightman/pytorch-image-models/blob/7c67d6aca992f039eece0af5f7c29a43d48c00e4/timm/models/layers/drop.py#L135)
 
     Args:
         rate: float, the probability of the residual branch being dropped.
         seed: (Optional) integer. Used to create a random seed.
 
-    Usage:
+    Example:
     `DropPath` can be used in any network as follows:
     ```python
 
     # (...)
     input = tf.ones((1, 3, 3, 1), dtype=tf.float32)
     residual = keras.layers.Conv2D(1, 1)(input)
     output = keras_cv.layers.DropPath()(input)
@@ -67,8 +67,7 @@
             x = x * drop_map
             return x
 
     def get_config(self):
         config = super().get_config()
         config.update({"rate": self.rate, "seed": self._seed_val})
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/regularization/dropblock_2d.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/regularization/dropblock_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             bigger than 0, and should not be bigger than the input feature map
             size. The paper authors use `block_size=7` for input feature's of
             size `14x14xchannels`. If this value is greater or equal to the
             input feature map size you will encounter `nan` values.
         seed: integer. To use as random seed.
         name: string. The name of the layer.
 
-    Usage:
+    Examples:
     DropBlock2D can be used inside a `keras.Model`:
     ```python
     # (...)
     x = Conv2D(32, (1, 1))(x)
     x = BatchNormalization()(x)
     x = ReLU()(x)
     x = DropBlock2D(0.1, block_size=7)(x)
@@ -234,8 +234,7 @@
             {
                 "rate": self._rate,
                 "block_size": (self._dropblock_height, self._dropblock_width),
                 "seed": self.seed,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/regularization/squeeze_excite.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/regularization/squeeze_excite.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             keras.layers.Layer) or keras.activations.Activation instance
             denoting activation to be applied after squeeze convolution.
             Defaults to `relu`.
         excite_activation: (Optional) String, callable (or
             keras.layers.Layer) or keras.activations.Activation instance
             denoting activation to be applied after excite convolution.
             Defaults to `sigmoid`.
-    Usage:
+    Example:
 
     ```python
     # (...)
     input = tf.ones((1, 5, 5, 16), dtype=tf.float32)
     x = keras.layers.Conv2D(16, (3, 3))(input)
     output = keras_cv.layers.SqueezeAndExciteBlock(16)(x)
     # (...)
@@ -124,8 +124,7 @@
                 )
             )
         if isinstance(config["excite_activation"], dict):
             config["excite_activation"] = keras.saving.deserialize_keras_object(
                 config["excite_activation"]
             )
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/regularization/stochastic_depth.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/regularization/stochastic_depth.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     Reference:
         - [Deep Networks with Stochastic Depth](https://arxiv.org/abs/1603.09382)
         - [Docstring taken from [stochastic_depth.py](https://tinyurl.com/mr3y2af6)
 
     Args:
         rate: float, the probability of the residual branch being dropped.
 
-    Usage:
+    Example:
 
     `StochasticDepth` can be used in a residual network as follows:
     ```python
     # (...)
     input = tf.ones((1, 3, 3, 1), dtype=tf.float32)
     residual = keras.layers.Conv2D(1, 1)(input)
     output = keras_cv.layers.StochasticDepth()([input, residual])
@@ -76,8 +76,7 @@
         else:
             return shortcut + self.survival_probability * residual
 
     def get_config(self):
         config = {"rate": self.rate}
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/segformer_multihead_attention.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/segformer_multihead_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             project_dim: integer, the dimensionality of the projection
                 of the `SegFormerMultiheadAttention` layer.
             num_heads: integer, the number of heads to use in the
                 attention computation.
             sr_ratio: integer, the sequence reduction ratio to perform
                 on the sequence before key and value projections.
 
-        Basic usage:
+        Example:
 
         ```
         tensor = tf.random.uniform([1, 196, 32])
         output = keras_cv.layers.SegFormerMultiheadAttention(project_dim=768,
                                                             num_heads=2,
                                                             sr_ratio=4)(tensor)
         print(output.shape) # (1, 196, 32)
@@ -126,8 +126,7 @@
         attn = ops.reshape(
             ops.transpose(attn, [0, 2, 1, 3]),
             [input_shape[0], input_shape[1], input_shape[2]],
         )
 
         x = self.proj(attn)
         return x
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/spatial_pyramid.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/spatial_pyramid.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,8 +184,7 @@
             "dilation_rates": self.dilation_rates,
             "num_channels": self.num_channels,
             "activation": self.activation,
             "dropout": self.dropout,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/transformer_encoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/transformer_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         attention_dropout: default 0.1, the dropout rate to apply in the
             MultiHeadAttention layer
         activation: default 'tf.activations.gelu', the activation function to
             apply in the MLP head - should be a function
         layer_norm_epsilon: default 1e-06, the epsilon for `LayerNormalization`
             layers
 
-    Basic usage:
+    Example:
 
     ```
     project_dim = 1024
     mlp_dim = 3072
     num_heads = 4
 
     encoded_patches = keras_cv.layers.PatchingAndEmbedding(
@@ -147,8 +147,7 @@
 
     @classmethod
     def from_config(cls, config, custom_objects=None):
         activation = config.pop("activation")
         if isinstance(activation, (str, dict)):
             activation = keras.activations.deserialize(activation)
         return cls(activation=activation, **config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/vit_det_layers.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/vit_det_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,8 +582,7 @@
             {
                 "img_size": self.img_size,
                 "patch_size": self.patch_size,
                 "embed_dim": self.embed_dim,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/layers/vit_layers.py` & `keras_cv-0.9.0.dev0/keras_cv/src/layers/vit_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         patch_size: the patch size
         padding: default 'VALID', the padding to apply for patchifying images
 
     Returns:
         Patchified and linearly projected input images, including a prepended
         learnable class token with shape (batch, num_patches+1, project_dim)
 
-    Basic usage:
+    Example:
 
     ```
     images = #... batch of images
     encoded_patches = keras_cv.layers.PatchingAndEmbedding(
         project_dim=project_dim,
         patch_size=patch_size)(patches)
     print(encoded_patches.shape) # (1, 197, 1024)
@@ -217,8 +217,7 @@
         config = {
             "project_dim": self.project_dim,
             "patch_size": self.patch_size,
             "padding": self.padding,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/losses/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/losses/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,8 +18,7 @@
 from keras_cv.src.losses.giou_loss import GIoULoss
 from keras_cv.src.losses.iou_loss import IoULoss
 from keras_cv.src.losses.penalty_reduced_focal_loss import (
     BinaryPenaltyReducedFocalCrossEntropy,
 )
 from keras_cv.src.losses.simclr_loss import SimCLRLoss
 from keras_cv.src.losses.smooth_l1 import SmoothL1Loss
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/losses/centernet_box_loss.py` & `keras_cv-0.9.0.dev0/keras_cv/src/losses/centernet_box_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,8 +132,7 @@
     def get_config(self):
         config = {
             "num_heading_bins": self.num_heading_bins,
             "anchor_size": self.anchor_size,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/losses/ciou_loss.py` & `keras_cv-0.9.0.dev0/keras_cv/src/losses/ciou_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             documentation](https://keras.io/api/keras_cv/bounding_box/formats/).
         eps: A small value added to avoid division by zero and stabilize
             calculations.
 
     References:
         - [CIoU paper](https://arxiv.org/pdf/2005.03572.pdf)
 
-    Sample Usage:
+    Example:
     ```python
     y_true = np.random.uniform(
         size=(5, 10, 5),
         low=0,
         high=10)
     y_pred = np.random.uniform(
         (5, 10, 4),
@@ -96,8 +96,7 @@
         config = super().get_config()
         config.update(
             {
                 "eps": self.eps,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/losses/focal.py` & `keras_cv-0.9.0.dev0/keras_cv/src/losses/focal.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             labels by squeezing them towards `0.5`, i.e., using
             `1. - 0.5 * label_smoothing` for the target class and
             `0.5 * label_smoothing` for the non-target class.
 
     References:
         - [Focal Loss paper](https://arxiv.org/abs/1708.02002)
 
-    Standalone usage:
+    Example:
     ```python
     y_true = np.random.uniform(size=[10], low=0, high=4)
     y_pred = np.random.uniform(size=[10], low=0, high=4)
     loss = FocalLoss()
     loss(y_true, y_pred)
     ```
     Usage with the `compile()` API:
@@ -112,8 +112,7 @@
                 "alpha": self.alpha,
                 "gamma": self.gamma,
                 "from_logits": self.from_logits,
                 "label_smoothing": self.label_smoothing,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/losses/giou_loss.py` & `keras_cv-0.9.0.dev0/keras_cv/src/losses/giou_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             documentation](https://keras.io/api/keras_cv/bounding_box/formats/).
         axis: the axis along which to mean the ious, defaults to -1.
 
     References:
         - [GIoU paper](https://arxiv.org/pdf/1902.09630)
         - [TFAddons Implementation](https://www.tensorflow.org/addons/api_docs/python/tfa/losses/GIoULoss)
 
-    Sample Usage:
+    Example:
     ```python
     y_true = np.random.uniform(size=(5, 10, 5), low=0, high=10)
     y_pred = np.random.uniform(size=(5, 10, 4), low=0, high=10)
     loss = GIoULoss(bounding_box_format = "xyWH")
     loss(y_true, y_pred).numpy()
     ```
 
@@ -177,8 +177,7 @@
         config.update(
             {
                 "bounding_box_format": self.bounding_box_format,
                 "axis": self.axis,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/losses/iou_loss.py` & `keras_cv-0.9.0.dev0/keras_cv/src/losses/iou_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             - `"log"`. The loss will be calculated as -ln(iou)
             Defaults to "log".
         axis: the axis along which to mean the ious, defaults to -1.
 
     References:
         - [UnitBox paper](https://arxiv.org/pdf/1608.01471)
 
-    Sample Usage:
+    Example:
     ```python
     y_true = np.random.uniform(size=(5, 10, 5), low=10, high=10)
     y_pred = np.random.uniform(size=(5, 10, 5), low=10, high=10)
     loss = IoULoss(bounding_box_format = "xyWH")
     loss(y_true, y_pred)
     ```
 
@@ -124,8 +124,7 @@
             {
                 "bounding_box_format": self.bounding_box_format,
                 "mode": self.mode,
                 "axis": self.axis,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/losses/penalty_reduced_focal_loss.py` & `keras_cv-0.9.0.dev0/keras_cv/src/losses/penalty_reduced_focal_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,8 +110,7 @@
                 "from_logits": self.from_logits,
                 "positive_threshold": self.positive_threshold,
                 "positive_weight": self.positive_weight,
                 "negative_weight": self.negative_weight,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/losses/simclr_loss.py` & `keras_cv-0.9.0.dev0/keras_cv/src/losses/simclr_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,8 +99,7 @@
 
         return loss_a + loss_b
 
     def get_config(self):
         config = super().get_config()
         config.update({"temperature": self.temperature})
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/losses/smooth_l1.py` & `keras_cv-0.9.0.dev0/keras_cv/src/losses/smooth_l1.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,8 +48,7 @@
 
     def get_config(self):
         config = {
             "l1_cutoff": self.l1_cutoff,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/metrics/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Copyright 2022 The KerasCV Authors
+# Copyright 2023 The KerasCV Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from keras_cv.src.metrics.object_detection.box_coco_metrics import BoxCOCOMetrics
-
+from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_label_encoder import (
+    YOLOV8LabelEncoder,
+)
```

### Comparing `keras-cv-0.8.2/keras_cv/src/metrics/coco/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/metrics/coco/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from keras_cv.src.metrics.coco.pycoco_wrapper import PyCOCOWrapper
 from keras_cv.src.metrics.coco.pycoco_wrapper import compute_pycoco_metrics
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/metrics/coco/pycoco_wrapper.py` & `keras_cv-0.9.0.dev0/keras_cv/src/metrics/coco/pycoco_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,8 +233,7 @@
     metrics = coco_metrics
 
     metrics_dict = {}
     for i, name in enumerate(METRIC_NAMES):
         metrics_dict[name] = metrics[i].astype(np.float32)
 
     return metrics_dict
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/metrics/object_detection/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/metrics/object_detection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/metrics/object_detection/box_coco_metrics.py` & `keras_cv-0.9.0.dev0/keras_cv/src/metrics/object_detection/box_coco_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         bounding_box_format: the bounding box format for inputs.
         evaluate_freq: the number of steps to run before each evaluation.
             Due to the high computational cost of metric evaluation the final
             results are only updated once every `evaluate_freq` steps. Higher
             values will allow for faster training times, while lower numbers
             allow for higher numerical precision in metric reporting.
 
-    Usage:
+    Example:
     `BoxCOCOMetrics()` can be used like any standard metric with any
     KerasCV object detection model. Inputs to `y_true` must be KerasCV bounding
     box dictionaries, `{"classes": classes, "boxes": boxes}`, and `y_pred` must
     follow the same format with an additional `confidence` key.
 
     Unfortunately, at the moment `BoxCOCOMetrics()` are not TPU compatible with
     the `fit()` API. If you wish to evaluate `BoxCOCOMetrics()` for a model
@@ -309,8 +309,7 @@
     predictions["detection_classes"] = [ops.convert_to_numpy(cls_pred)]
     predictions["detection_scores"] = [ops.convert_to_numpy(confidence_pred)]
     predictions["num_detections"] = [
         ops.sum(ops.cast(confidence_pred > 0, "int32"), axis=-1)
     ]
 
     return coco.compute_pycoco_metrics(ground_truth, predictions)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,84 +57,84 @@
 )
 from keras_cv.src.models.backbones.efficientnet_lite.efficientnet_lite_aliases import (  # noqa: E501
     EfficientNetLiteB4Backbone,
 )
 from keras_cv.src.models.backbones.efficientnet_lite.efficientnet_lite_backbone import (  # noqa: E501
     EfficientNetLiteBackbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (  # noqa: E501
     EfficientNetV1B0Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (  # noqa: E501
     EfficientNetV1B1Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (  # noqa: E501
     EfficientNetV1B2Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (  # noqa: E501
     EfficientNetV1B3Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (  # noqa: E501
     EfficientNetV1B4Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (  # noqa: E501
     EfficientNetV1B5Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (  # noqa: E501
     EfficientNetV1B6Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (  # noqa: E501
     EfficientNetV1B7Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_aliases import (  # noqa: E501
     EfficientNetV1Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (  # noqa: E501
     EfficientNetV2B0Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (  # noqa: E501
     EfficientNetV2B1Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (  # noqa: E501
     EfficientNetV2B2Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (  # noqa: E501
     EfficientNetV2B3Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (  # noqa: E501
     EfficientNetV2Backbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (  # noqa: E501
     EfficientNetV2LBackbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (  # noqa: E501
     EfficientNetV2MBackbone,
 )
-from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (
+from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_aliases import (  # noqa: E501
     EfficientNetV2SBackbone,
 )
-from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (
+from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (  # noqa: E501
     MiTB0Backbone,
 )
-from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (
+from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (  # noqa: E501
     MiTB1Backbone,
 )
-from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (
+from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (  # noqa: E501
     MiTB2Backbone,
 )
-from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (
+from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (  # noqa: E501
     MiTB3Backbone,
 )
-from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (
+from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (  # noqa: E501
     MiTB4Backbone,
 )
-from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (
+from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (  # noqa: E501
     MiTB5Backbone,
 )
-from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (
+from keras_cv.src.models.backbones.mix_transformer.mix_transformer_aliases import (  # noqa: E501
     MiTBackbone,
 )
 from keras_cv.src.models.backbones.mobilenet_v3.mobilenet_v3_aliases import (
     MobileNetV3LargeBackbone,
 )
 from keras_cv.src.models.backbones.mobilenet_v3.mobilenet_v3_aliases import (
     MobileNetV3SmallBackbone,
@@ -174,35 +174,71 @@
 )
 from keras_cv.src.models.backbones.resnet_v2.resnet_v2_aliases import (
     ResNet152V2Backbone,
 )
 from keras_cv.src.models.backbones.resnet_v2.resnet_v2_backbone import (
     ResNetV2Backbone,
 )
-from keras_cv.src.models.backbones.vit_det.vit_det_aliases import ViTDetBBackbone
-from keras_cv.src.models.backbones.vit_det.vit_det_aliases import ViTDetHBackbone
-from keras_cv.src.models.backbones.vit_det.vit_det_aliases import ViTDetLBackbone
-from keras_cv.src.models.backbones.vit_det.vit_det_backbone import ViTDetBackbone
+from keras_cv.src.models.backbones.vgg16.vgg16_backbone import VGG16Backbone
+from keras_cv.src.models.backbones.video_swin.video_swin_aliases import (
+    VideoSwinBBackbone,
+)
+from keras_cv.src.models.backbones.video_swin.video_swin_aliases import (
+    VideoSwinSBackbone,
+)
+from keras_cv.src.models.backbones.video_swin.video_swin_aliases import (
+    VideoSwinTBackbone,
+)
+from keras_cv.src.models.backbones.video_swin.video_swin_backbone import (
+    VideoSwinBackbone,
+)
+from keras_cv.src.models.backbones.vit_det.vit_det_aliases import (
+    ViTDetBBackbone,
+)
+from keras_cv.src.models.backbones.vit_det.vit_det_aliases import (
+    ViTDetHBackbone,
+)
+from keras_cv.src.models.backbones.vit_det.vit_det_aliases import (
+    ViTDetLBackbone,
+)
+from keras_cv.src.models.backbones.vit_det.vit_det_backbone import (
+    ViTDetBackbone,
+)
 from keras_cv.src.models.classification.image_classifier import ImageClassifier
+from keras_cv.src.models.classification.video_classifier import VideoClassifier
+from keras_cv.src.models.feature_extractor.clip import CLIP
 from keras_cv.src.models.object_detection.retinanet.retinanet import RetinaNet
 from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_backbone import (
     YOLOV8Backbone,
 )
 from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_detector import (
     YOLOV8Detector,
 )
 from keras_cv.src.models.segmentation import BASNet
 from keras_cv.src.models.segmentation import DeepLabV3Plus
 from keras_cv.src.models.segmentation import SAMMaskDecoder
 from keras_cv.src.models.segmentation import SAMPromptEncoder
 from keras_cv.src.models.segmentation import SegmentAnythingModel
 from keras_cv.src.models.segmentation import TwoWayTransformer
-from keras_cv.src.models.segmentation.segformer.segformer_aliases import SegFormer
-from keras_cv.src.models.segmentation.segformer.segformer_aliases import SegFormerB0
-from keras_cv.src.models.segmentation.segformer.segformer_aliases import SegFormerB1
-from keras_cv.src.models.segmentation.segformer.segformer_aliases import SegFormerB2
-from keras_cv.src.models.segmentation.segformer.segformer_aliases import SegFormerB3
-from keras_cv.src.models.segmentation.segformer.segformer_aliases import SegFormerB4
-from keras_cv.src.models.segmentation.segformer.segformer_aliases import SegFormerB5
+from keras_cv.src.models.segmentation.segformer.segformer_aliases import (
+    SegFormer,
+)
+from keras_cv.src.models.segmentation.segformer.segformer_aliases import (
+    SegFormerB0,
+)
+from keras_cv.src.models.segmentation.segformer.segformer_aliases import (
+    SegFormerB1,
+)
+from keras_cv.src.models.segmentation.segformer.segformer_aliases import (
+    SegFormerB2,
+)
+from keras_cv.src.models.segmentation.segformer.segformer_aliases import (
+    SegFormerB3,
+)
+from keras_cv.src.models.segmentation.segformer.segformer_aliases import (
+    SegFormerB4,
+)
+from keras_cv.src.models.segmentation.segformer.segformer_aliases import (
+    SegFormerB5,
+)
 from keras_cv.src.models.stable_diffusion import StableDiffusion
 from keras_cv.src.models.stable_diffusion import StableDiffusionV2
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/backbone.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,8 +170,7 @@
         ```
         """
         return self._pyramid_level_inputs
 
     @pyramid_level_inputs.setter
     def pyramid_level_inputs(self, value):
         self._pyramid_level_inputs = value
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/backbone_presets.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,55 +10,63 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """All Backbone presets"""
 
-from keras_cv.src.models.backbones.csp_darknet import csp_darknet_backbone_presets
+from keras_cv.src.models.backbones.csp_darknet import (
+    csp_darknet_backbone_presets,
+)
 from keras_cv.src.models.backbones.densenet import densenet_backbone_presets
 from keras_cv.src.models.backbones.efficientnet_lite import (
     efficientnet_lite_backbone_presets,
 )
 from keras_cv.src.models.backbones.efficientnet_v1 import (
     efficientnet_v1_backbone_presets,
 )
 from keras_cv.src.models.backbones.efficientnet_v2 import (
     efficientnet_v2_backbone_presets,
 )
-from keras_cv.src.models.backbones.mobilenet_v3 import mobilenet_v3_backbone_presets
+from keras_cv.src.models.backbones.mobilenet_v3 import (
+    mobilenet_v3_backbone_presets,
+)
 from keras_cv.src.models.backbones.resnet_v1 import resnet_v1_backbone_presets
 from keras_cv.src.models.backbones.resnet_v2 import resnet_v2_backbone_presets
+from keras_cv.src.models.backbones.video_swin import video_swin_backbone_presets
 from keras_cv.src.models.backbones.vit_det import vit_det_backbone_presets
-from keras_cv.src.models.object_detection.yolo_v8 import yolo_v8_backbone_presets
+from keras_cv.src.models.object_detection.yolo_v8 import (
+    yolo_v8_backbone_presets,
+)
 
 backbone_presets_no_weights = {
     **resnet_v1_backbone_presets.backbone_presets_no_weights,
     **resnet_v2_backbone_presets.backbone_presets_no_weights,
     **mobilenet_v3_backbone_presets.backbone_presets_no_weights,
     **csp_darknet_backbone_presets.backbone_presets_no_weights,
     **efficientnet_v1_backbone_presets.backbone_presets_no_weights,
     **efficientnet_v2_backbone_presets.backbone_presets_no_weights,
     **densenet_backbone_presets.backbone_presets_no_weights,
     **efficientnet_lite_backbone_presets.backbone_presets_no_weights,
     **yolo_v8_backbone_presets.backbone_presets_no_weights,
     **vit_det_backbone_presets.backbone_presets_no_weights,
+    **video_swin_backbone_presets.backbone_presets_no_weights,
 }
 
 backbone_presets_with_weights = {
     **resnet_v1_backbone_presets.backbone_presets_with_weights,
     **resnet_v2_backbone_presets.backbone_presets_with_weights,
     **mobilenet_v3_backbone_presets.backbone_presets_with_weights,
     **csp_darknet_backbone_presets.backbone_presets_with_weights,
     **efficientnet_v1_backbone_presets.backbone_presets_with_weights,
     **efficientnet_v2_backbone_presets.backbone_presets_with_weights,
     **densenet_backbone_presets.backbone_presets_with_weights,
     **efficientnet_lite_backbone_presets.backbone_presets_with_weights,
     **yolo_v8_backbone_presets.backbone_presets_with_weights,
     **vit_det_backbone_presets.backbone_presets_with_weights,
+    **video_swin_backbone_presets.backbone_presets_with_weights,
 }
 
 backbone_presets = {
     **backbone_presets_no_weights,
     **backbone_presets_with_weights,
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/csp_darknet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_aliases.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_aliases.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import copy
 
 from keras_cv.src.api_export import keras_cv_export
 from keras_cv.src.models.backbones.csp_darknet.csp_darknet_backbone import (
     CSPDarkNetBackbone,
 )
-from keras_cv.src.models.backbones.csp_darknet.csp_darknet_backbone_presets import (
+from keras_cv.src.models.backbones.csp_darknet.csp_darknet_backbone_presets import (  # noqa: E501
     backbone_presets,
 )
 from keras_cv.src.utils.python_utils import classproperty
 
 ALIAS_DOCSTRING = """CSPDarkNetBackbone model with {stackwise_channels} channels
     and {stackwise_depth} depths.
 
@@ -37,26 +37,26 @@
     Args:
         include_rescaling: bool, whether or not to rescale the inputs. If set to
             True, inputs will be passed through a `Rescaling(1/255.0)` layer.
         input_tensor: optional Keras tensor (i.e. output of `layers.Input()`)
             to use as image input for the model.
         input_shape: optional shape tuple, defaults to (None, None, 3).
 
-    Examples:
+    Example:
     ```python
     input_data = tf.ones(shape=(8, 224, 224, 3))
 
     # Randomly initialized backbone
     model = CSPDarkNet{name}Backbone()
     output = model(input_data)
     ```
 """  # noqa: E501
 
 
-@keras_cv_export("keras_cv.losses.CSPDarkNetTinyBackbone")
+@keras_cv_export("keras_cv.models.CSPDarkNetTinyBackbone")
 class CSPDarkNetTinyBackbone(CSPDarkNetBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -83,15 +83,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return cls.presets
 
 
-@keras_cv_export("keras_cv.losses.CSPDarkNetSBackbone")
+@keras_cv_export("keras_cv.models.CSPDarkNetSBackbone")
 class CSPDarkNetSBackbone(CSPDarkNetBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -114,15 +114,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return {}
 
 
-@keras_cv_export("keras_cv.losses.CSPDarkNetMBackbone")
+@keras_cv_export("keras_cv.models.CSPDarkNetMBackbone")
 class CSPDarkNetMBackbone(CSPDarkNetBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -145,15 +145,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return {}
 
 
-@keras_cv_export("keras_cv.losses.CSPDarkNetLBackbone")
+@keras_cv_export("keras_cv.models.CSPDarkNetLBackbone")
 class CSPDarkNetLBackbone(CSPDarkNetBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -180,15 +180,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return cls.presets
 
 
-@keras_cv_export("keras_cv.losses.CSPDarkNetXLBackbone")
+@keras_cv_export("keras_cv.models.CSPDarkNetXLBackbone")
 class CSPDarkNetXLBackbone(CSPDarkNetBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -256,8 +256,7 @@
     "__doc__",
     ALIAS_DOCSTRING.format(
         name="XL",
         stackwise_channels="[170, 340, 680, 1360]",
         stackwise_depth="[4, 12, 12, 4]",
     ),
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 """CSPDarkNet backbone model. """
 import copy
 
 from keras_cv.src.api_export import keras_cv_export
 from keras_cv.src.backend import keras
 from keras_cv.src.models import utils
 from keras_cv.src.models.backbones.backbone import Backbone
-from keras_cv.src.models.backbones.csp_darknet.csp_darknet_backbone_presets import (
+from keras_cv.src.models.backbones.csp_darknet.csp_darknet_backbone_presets import (  # noqa: E501
     backbone_presets,
 )
-from keras_cv.src.models.backbones.csp_darknet.csp_darknet_backbone_presets import (
+from keras_cv.src.models.backbones.csp_darknet.csp_darknet_backbone_presets import (  # noqa: E501
     backbone_presets_with_weights,
 )
 from keras_cv.src.models.backbones.csp_darknet.csp_darknet_utils import (
     CrossStagePartial,
 )
 from keras_cv.src.models.backbones.csp_darknet.csp_darknet_utils import (
     DarknetConvBlock,
@@ -176,8 +176,7 @@
         return copy.deepcopy(backbone_presets)
 
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return copy.deepcopy(backbone_presets_with_weights)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,8 +113,7 @@
     },
 }
 
 backbone_presets = {
     **backbone_presets_no_weights,
     **backbone_presets_with_weights,
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_utils.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,8 +368,7 @@
                 x[..., 1::2, ::2, :],
                 x[..., ::2, 1::2, :],
                 x[..., 1::2, 1::2, :],
             ],
         )
 
     return apply
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/densenet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/densenet_aliases.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/densenet/densenet_aliases.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         include_rescaling: bool, whether to rescale the inputs. If set
             to `True`, inputs will be passed through a `Rescaling(1/255.0)`
             layer.
         input_shape: optional shape tuple, defaults to (None, None, 3).
         input_tensor: optional Keras tensor (i.e. output of `layers.Input()`)
             to use as image input for the model.
 
-    Examples:
+    Example:
     ```python
     input_data = tf.ones(shape=(8, 224, 224, 3))
 
     # Randomly initialized backbone
     model = DenseNet{num_layers}Backbone()
     output = model(input_data)
     ```
@@ -151,8 +151,7 @@
         """Dictionary of preset names and configurations that include weights."""  # noqa: E501
         return cls.presets
 
 
 setattr(DenseNet121Backbone, "__doc__", ALIAS_DOCSTRING.format(num_layers=121))
 setattr(DenseNet169Backbone, "__doc__", ALIAS_DOCSTRING.format(num_layers=169))
 setattr(DenseNet201Backbone, "__doc__", ALIAS_DOCSTRING.format(num_layers=201))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/densenet_backbone.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/densenet/densenet_backbone.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,8 +236,7 @@
         use_bias=False,
         name=f"{name}_2_conv",
     )(x)
     x = keras.layers.Concatenate(axis=BN_AXIS, name=f"{name}_concat")(
         [shortcut, x]
     )
     return x
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/densenet_backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/densenet/densenet_backbone_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,7 @@
     },
 }
 
 backbone_presets = {
     **backbone_presets_no_weights,
     **backbone_presets_with_weights,
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_lite/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_aliases.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_aliases.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from keras_cv.src.api_export import keras_cv_export
 from keras_cv.src.models.backbones.efficientnet_lite.efficientnet_lite_backbone import (  # noqa: E501
     EfficientNetLiteBackbone,
 )
 from keras_cv.src.utils.python_utils import classproperty
 
 ALIAS_DOCSTRING = """Instantiates the {name} architecture.
 
@@ -26,25 +27,26 @@
     Args:
         include_rescaling: bool, whether to rescale the inputs. If set
             to `True`, inputs will be passed through a `Rescaling(1/255.0)`
             layer.
         input_shape: optional shape tuple, defaults to (None, None, 3).
         input_tensor: optional Keras tensor (i.e. output of `layers.Input()`)
             to use as image input for the model.
-    Usage:
+    Example:
     ```python
     input_data = np.ones(shape=(8, 224, 224, 3))
 
     # Randomly initialized backbone
     model = {name}Backbone()
     output = model(input_data)
     ```
 """  # noqa: E501
 
 
+@keras_cv_export("keras_cv.models.EfficientNetLiteB0Backbone")
 class EfficientNetLiteB0Backbone(EfficientNetLiteBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -69,14 +71,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.EfficientNetLiteB1Backbone")
 class EfficientNetLiteB1Backbone(EfficientNetLiteBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -101,14 +104,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.EfficientNetLiteB2Backbone")
 class EfficientNetLiteB2Backbone(EfficientNetLiteBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -133,14 +137,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.EfficientNetLiteB3Backbone")
 class EfficientNetLiteB3Backbone(EfficientNetLiteBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -165,14 +170,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.EfficientNetLiteB4Backbone")
 class EfficientNetLiteB4Backbone(EfficientNetLiteBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -222,8 +228,7 @@
     ALIAS_DOCSTRING.format(name="EfficientNetLiteB3"),
 )
 setattr(
     EfficientNetLiteB4Backbone,
     "__doc__",
     ALIAS_DOCSTRING.format(name="EfficientNetLiteB4"),
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,27 @@
         (ICML 2019)
     - [Based on the original EfficientNet Lite's](https://github.com/tensorflow/tpu/tree/master/models/official/efficientnet/lite)
 """  # noqa: E501
 
 import copy
 import math
 
+from keras_cv.src.api_export import keras_cv_export
 from keras_cv.src.backend import keras
 from keras_cv.src.models import utils
 from keras_cv.src.models.backbones.backbone import Backbone
 from keras_cv.src.models.backbones.efficientnet_lite.efficientnet_lite_backbone_presets import (  # noqa: E501
     backbone_presets,
 )
 from keras_cv.src.utils.python_utils import classproperty
 
 BN_AXIS = 3
 
 
+@keras_cv_export("keras_cv.models.EfficientNetLiteBackbone")
 @keras.saving.register_keras_serializable(package="keras_cv.models")
 class EfficientNetLiteBackbone(Backbone):
     """Instantiates the EfficientNetLite architecture using given scaling
     coefficients.
 
     Reference:
     - [EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks](https://arxiv.org/abs/1905.11946)
@@ -57,15 +59,15 @@
             is set to 8.
         activation: activation function.
         input_shape: optional shape tuple,
             It should have exactly 3 inputs channels.
         input_tensor: optional Keras tensor (i.e. output of `keras.layers.Input()`)
             to use as image input for the model.
 
-    Usage:
+    Example:
     ```python
     # Construct an EfficientNetLite from a preset:
     efficientnet = models.EfficientNetLiteBackbone.from_preset(
         "efficientnetlite_b0"
     )
     images = np.ones((1, 256, 256, 3))
     outputs = efficientnet.predict(images)
@@ -360,8 +362,7 @@
     if strides == 1 and filters_in == filters_out:
         if dropout_rate > 0:
             x = keras.layers.Dropout(
                 dropout_rate, noise_shape=(None, 1, 1, 1), name=name + "drop"
             )(x)
         x = keras.layers.Add(name=name + "add")([x, inputs])
     return x
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,8 +84,7 @@
 
 backbone_presets_with_weights = {}
 
 backbone_presets = {
     **backbone_presets_no_weights,
     **backbone_presets_with_weights,
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_aliases.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_aliases.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_backbone import (
+from keras_cv.src.api_export import keras_cv_export
+from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_backbone import (  # noqa: E501
     EfficientNetV1Backbone,
 )
 from keras_cv.src.utils.python_utils import classproperty
 
 ALIAS_DOCSTRING = """Instantiates the {name} architecture.
 
     Reference:
@@ -29,14 +30,15 @@
             layer.
         input_shape: optional shape tuple, defaults to (None, None, 3).
         input_tensor: optional Keras tensor (i.e. output of `layers.Input()`)
             to use as image input for the model.
 """  # noqa: E501
 
 
+@keras_cv_export("keras_cv.models.EfficientNetV1B0Backbone")
 class EfficientNetV1B0Backbone(EfficientNetV1Backbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -59,14 +61,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.EfficientNetV1B1Backbone")
 class EfficientNetV1B1Backbone(EfficientNetV1Backbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -89,14 +92,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.EfficientNetV1B2Backbone")
 class EfficientNetV1B2Backbone(EfficientNetV1Backbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -119,14 +123,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.EfficientNetV1B3Backbone")
 class EfficientNetV1B3Backbone(EfficientNetV1Backbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -149,14 +154,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.EfficientNetV1B4Backbone")
 class EfficientNetV1B4Backbone(EfficientNetV1Backbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -179,14 +185,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.EfficientNetV1B5Backbone")
 class EfficientNetV1B5Backbone(EfficientNetV1Backbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -209,14 +216,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.EfficientNetV1B6Backbone")
 class EfficientNetV1B6Backbone(EfficientNetV1Backbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -239,14 +247,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.EfficientNetV1B7Backbone")
 class EfficientNetV1B7Backbone(EfficientNetV1Backbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(None, None, 3),
         input_tensor=None,
         **kwargs,
@@ -309,8 +318,7 @@
     ALIAS_DOCSTRING.format(name="EfficientNetV1B6"),
 )
 setattr(
     EfficientNetV1B7Backbone,
     "__doc__",
     ALIAS_DOCSTRING.format(name="EfficientNetV1B7"),
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 import math
 
+from keras_cv.src.api_export import keras_cv_export
 from keras_cv.src.backend import keras
 from keras_cv.src.models import utils
 from keras_cv.src.models.backbones.backbone import Backbone
 from keras_cv.src.models.backbones.efficientnet_v1.efficientnet_v1_backbone_presets import (  # noqa: E501
     backbone_presets,
 )
 from keras_cv.src.utils.python_utils import classproperty
 
 
+@keras_cv_export("keras_cv.models.EfficientNetV1Backbone")
 @keras.saving.register_keras_serializable(package="keras_cv.models")
 class EfficientNetV1Backbone(Backbone):
     """Instantiates the EfficientNetV1 architecture.
 
     Reference:
     - [EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks](https://arxiv.org/abs/1905.11946)
         (ICML 2019)
@@ -57,15 +59,15 @@
             each stack in the conv blocks model.
         stackwise_expansion_ratios: list of floats, expand ratio passed to the
             squeeze and excitation blocks.
         stackwise_strides: list of ints, stackwise_strides for each conv block.
         stackwise_squeeze_and_excite_ratios: list of ints, the squeeze and
             excite ratios passed to the squeeze and excitation blocks.
 
-    Usage:
+    Example:
     ```python
     # Construct an EfficientNetV1 from a preset:
     efficientnet = keras_cv.models.EfficientNetV1Backbone.from_preset(
         "efficientnetv1_b0"
     )
     images = np.ones((1, 256, 256, 3))
     outputs = efficientnet.predict(images)
@@ -448,8 +450,7 @@
                 dropout_rate,
                 noise_shape=(None, 1, 1, 1),
                 name=name + "drop",
             )(x)
         x = keras.layers.Add(name=name + "add")([x, inputs])
 
     return x
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,8 +123,7 @@
 
 backbone_presets_with_weights = {}
 
 backbone_presets = {
     **backbone_presets_no_weights,
     **backbone_presets_with_weights,
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_aliases.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_aliases.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 
 from keras_cv.src.api_export import keras_cv_export
-from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_backbone import (
+from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_backbone import (  # noqa: E501
     EfficientNetV2Backbone,
 )
 from keras_cv.src.models.backbones.efficientnet_v2.efficientnet_v2_backbone_presets import (  # noqa: E501
     backbone_presets,
 )
 from keras_cv.src.utils.python_utils import classproperty
 
@@ -302,8 +302,7 @@
     ALIAS_DOCSTRING.format(name="EfficientNetV2B2"),
 )
 setattr(
     EfficientNetV2B3Backbone,
     "__doc__",
     ALIAS_DOCSTRING.format(name="EfficientNetV2B3"),
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,8 +337,7 @@
         return FusedMBConvBlock
     else:
         raise ValueError(
             "Expected `conv_type` to be "
             "one of 'unfused', 'fused', but got "
             f"`conv_type={conv_type}`"
         )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,8 +172,7 @@
     },
 }
 
 backbone_presets = {
     **backbone_presets_no_weights,
     **backbone_presets_with_weights,
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mix_transformer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/mix_transformer_aliases.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mix_transformer/mix_transformer_aliases.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 
-from keras_cv.src.models.backbones.mix_transformer.mix_transformer_backbone import (
+from keras_cv.src.api_export import keras_cv_export
+from keras_cv.src.models.backbones.mix_transformer.mix_transformer_backbone import (  # noqa: E501
     MiTBackbone,
 )
 from keras_cv.src.models.backbones.mix_transformer.mix_transformer_backbone_presets import (  # noqa: E501
     backbone_presets,
 )
 from keras_cv.src.utils.python_utils import classproperty
 
@@ -31,25 +32,26 @@
         include_rescaling: bool, whether to rescale the inputs. If set to
             True, inputs will be passed through a `Rescaling(scale=1 / 255)`
             layer. Defaults to True.
         input_shape: optional shape tuple, defaults to (None, None, 3).
         input_tensor: optional Keras tensor (i.e., output of `layers.Input()`)
             to use as image input for the model.
 
-    Examples:
+    Example:
     ```python
     input_data = tf.ones(shape=(8, 224, 224, 3))
 
     # Randomly initialized backbone
     model = {name}Backbone()
     output = model(input_data)
     ```
 """  # noqa: E501
 
 
+@keras_cv_export("keras_cv.models.MiTB0Backbone")
 class MiTB0Backbone(MiTBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(224, 224, 3),
         input_tensor=None,
         **kwargs,
@@ -76,14 +78,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return cls.presets
 
 
+@keras_cv_export("keras_cv.models.MiTB1Backbone")
 class MiTB1Backbone(MiTBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(224, 224, 3),
         input_tensor=None,
         **kwargs,
@@ -105,14 +108,15 @@
 
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.MiTB2Backbone")
 class MiTB2Backbone(MiTBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(224, 224, 3),
         input_tensor=None,
         **kwargs,
@@ -134,14 +138,15 @@
 
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.MiTB3Backbone")
 class MiTB3Backbone(MiTBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(224, 224, 3),
         input_tensor=None,
         **kwargs,
@@ -163,14 +168,15 @@
 
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.MiTB4Backbone")
 class MiTB4Backbone(MiTBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(224, 224, 3),
         input_tensor=None,
         **kwargs,
@@ -192,14 +198,15 @@
 
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations."""
         return {}
 
 
+@keras_cv_export("keras_cv.models.MiTB5Backbone")
 class MiTB5Backbone(MiTBackbone):
     def __new__(
         cls,
         include_rescaling=True,
         input_shape=(224, 224, 3),
         input_tensor=None,
         **kwargs,
@@ -256,8 +263,7 @@
 )
 
 setattr(
     MiTB5Backbone,
     "__doc__",
     ALIAS_DOCSTRING.format(name="MiTB5"),
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                 network
             embedding_dims: the embedding dims per hierarchical stage, used as
                 the levels of the feature pyramid
             input_shape: optional shape tuple, defaults to (None, None, 3).
             input_tensor: optional Keras tensor (i.e. output of `keras.layers.Input()`)
                 to use as image input for the model.
 
-        Examples:
+        Example:
 
         Using the class with a `backbone`:
 
         ```python
         import tensorflow as tf
         import keras_cv
 
@@ -182,8 +182,7 @@
         return copy.deepcopy(backbone_presets)
 
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return copy.deepcopy(backbone_presets_with_weights)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone_presets.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,8 +96,7 @@
     },
 }
 
 backbone_presets = {
     **backbone_presets_no_weights,
     **backbone_presets_with_weights,
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mobilenet_v3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_aliases.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_aliases.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         include_rescaling: bool, whether to rescale the inputs. If set to
             True, inputs will be passed through a `Rescaling(scale=1 / 255)`
             layer. Defaults to True.
         input_shape: optional shape tuple, defaults to (None, None, 3).
         input_tensor: optional Keras tensor (i.e., output of `layers.Input()`)
             to use as image input for the model.
 
-    Examples:
+    Example:
     ```python
     input_data = tf.ones(shape=(8, 224, 224, 3))
 
     # Randomly initialized backbone
     model = {name}Backbone()
     output = model(input_data)
     ```
@@ -126,8 +126,7 @@
     ALIAS_DOCSTRING.format(name="MobileNetV3Large", num_layers="28"),
 )
 setattr(
     MobileNetV3SmallBackbone,
     "__doc__",
     ALIAS_DOCSTRING.format(name="MobileNetV3Small", num_layers="14"),
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             - If `alpha` < 1.0, proportionally decreases the number
                 of filters in each layer.
             - If `alpha` > 1.0, proportionally increases the number
                 of filters in each layer.
             - If `alpha` = 1, default number of filters from the paper
                 are used at each layer.
 
-    Examples:
+    Example:
     ```python
     input_data = tf.ones(shape=(8, 224, 224, 3))
 
     # Randomly initialized backbone with a custom config
     model = MobileNetV3Backbone(
         stackwise_expansion=[1, 72.0 / 16, 88.0 / 24, 4, 6, 6, 3, 3, 6, 6, 6],
         stackwise_filters=[16, 24, 24, 40, 40, 40, 48, 48, 96, 96, 96],
@@ -356,8 +356,7 @@
         name=prefix + "project_BatchNorm",
     )(x)
 
     if stride == 1 and infilters == filters:
         x = keras.layers.Add(name=prefix + "Add")([shortcut, x])
 
     return x
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,8 +73,7 @@
     },
 }
 
 backbone_presets = {
     **backbone_presets_no_weights,
     **backbone_presets_with_weights,
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/resnet_v1_aliases.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v1/resnet_v1_aliases.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         include_rescaling: bool, whether to rescale the inputs. If set
             to `True`, inputs will be passed through a `Rescaling(1/255.0)`
             layer.
         input_shape: optional shape tuple, defaults to (None, None, 3).
         input_tensor: optional Keras tensor (i.e. output of `layers.Input()`)
             to use as image input for the model.
 
-    Examples:
+    Example:
     ```python
     input_data = tf.ones(shape=(8, 224, 224, 3))
 
     # Randomly initialized backbone
     model = ResNet{num_layers}Backbone()
     output = model(input_data)
     ```
@@ -216,8 +216,7 @@
 
 
 setattr(ResNet18Backbone, "__doc__", ALIAS_DOCSTRING.format(num_layers=18))
 setattr(ResNet34Backbone, "__doc__", ALIAS_DOCSTRING.format(num_layers=34))
 setattr(ResNet50Backbone, "__doc__", ALIAS_DOCSTRING.format(num_layers=50))
 setattr(ResNet101Backbone, "__doc__", ALIAS_DOCSTRING.format(num_layers=101))
 setattr(ResNet152Backbone, "__doc__", ALIAS_DOCSTRING.format(num_layers=152))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,8 +353,7 @@
         conv_shortcut=first_shortcut,
     )
     for i in range(2, blocks + 1):
         x = block_fn(
             x, filters, conv_shortcut=False, name=name + "_block" + str(i)
         )
     return x
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,8 +98,7 @@
     },
 }
 
 backbone_presets = {
     **backbone_presets_no_weights,
     **backbone_presets_with_weights,
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/resnet_v2_aliases.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v2/resnet_v2_aliases.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         include_rescaling: bool, whether to rescale the inputs. If set
             to `True`, inputs will be passed through a `Rescaling(1/255.0)`
             layer.
         input_shape: optional shape tuple, defaults to (None, None, 3).
         input_tensor: optional Keras tensor (i.e. output of `layers.Input()`)
             to use as image input for the model.
 
-    Examples:
+    Example:
     ```python
     input_data = tf.ones(shape=(8, 224, 224, 3))
 
     # Randomly initialized backbone
     model = ResNet{num_layers}V2Backbone()
     output = model(input_data)
     ```
@@ -236,8 +236,7 @@
     ALIAS_DOCSTRING.format(num_layers=101),
 )
 setattr(
     ResNet152V2Backbone,
     "__doc__",
     ALIAS_DOCSTRING.format(num_layers=152),
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,8 +399,7 @@
         x,
         filters,
         stride=stride,
         dilation=dilations,
         name=name + "_block" + str(blocks),
     )
     return x
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,8 +92,7 @@
     },
 }
 
 backbone_presets = {
     **backbone_presets_no_weights,
     **backbone_presets_with_weights,
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/test_backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/test_backbone_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,7 @@
     "csp_darknet_tiny",
     "densenet121",
     "efficientnetv2_b0",
     "mobilenet_v3_small",
     "resnet18",
     "resnet18_v2",
 ]
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/vgg16/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/vit_det_aliases.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/vit_det/vit_det_aliases.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 
-from keras_cv.src.models.backbones.vit_det.vit_det_backbone import ViTDetBackbone
+from keras_cv.src.api_export import keras_cv_export
+from keras_cv.src.models.backbones.vit_det.vit_det_backbone import (
+    ViTDetBackbone,
+)
 from keras_cv.src.models.backbones.vit_det.vit_det_backbone_presets import (
     backbone_presets,
 )
 from keras_cv.src.utils.python_utils import classproperty
 
 ALIAS_DOCSTRING = """VitDet{size}Backbone model.
 
@@ -26,25 +29,26 @@
         - [Detectron2](https://github.com/facebookresearch/detectron2)
         - [Segment Anything paper](https://arxiv.org/abs/2304.02643)
         - [Segment Anything GitHub](https://github.com/facebookresearch/segment-anything)
 
     For transfer learning use cases, make sure to read the
     [guide to transfer learning & fine-tuning](https://keras.io/guides/transfer_learning/).
 
-    Examples:
+    Example:
     ```python
     input_data = np.ones(shape=(1, 1024, 1024, 3))
 
     # Randomly initialized backbone
     model = VitDet{size}Backbone()
     output = model(input_data)
     ```
 """  # noqa: E501
 
 
+@keras_cv_export("keras_cv.models.ViTDetBBackbone")
 class ViTDetBBackbone(ViTDetBackbone):
     def __new__(
         cls,
         **kwargs,
     ):
         return ViTDetBackbone.from_preset("vitdet_base", **kwargs)
 
@@ -60,14 +64,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return cls.presets
 
 
+@keras_cv_export("keras_cv.models.ViTDetLBackbone")
 class ViTDetLBackbone(ViTDetBackbone):
     def __new__(
         cls,
         **kwargs,
     ):
         return ViTDetBackbone.from_preset("vitdet_large", **kwargs)
 
@@ -83,14 +88,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return cls.presets
 
 
+@keras_cv_export("keras_cv.models.ViTDetHBackbone")
 class ViTDetHBackbone(ViTDetBackbone):
     def __new__(
         cls,
         **kwargs,
     ):
         return ViTDetBackbone.from_preset("vitdet_huge", **kwargs)
 
@@ -109,8 +115,7 @@
         weights."""
         return cls.presets
 
 
 setattr(ViTDetBBackbone, "__doc__", ALIAS_DOCSTRING.format(size="B"))
 setattr(ViTDetLBackbone, "__doc__", ALIAS_DOCSTRING.format(size="L"))
 setattr(ViTDetHBackbone, "__doc__", ALIAS_DOCSTRING.format(size="H"))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/vit_det_backbone.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/vit_det/vit_det_backbone.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,8 +218,7 @@
         return copy.deepcopy(backbone_presets)
 
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return copy.deepcopy(backbone_presets_with_weights)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/vit_det_backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/vit_det/vit_det_backbone_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,8 +96,7 @@
 }
 
 
 backbone_presets = {
     **backbone_presets_no_weights,
     **backbone_presets_with_weights,
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/classification/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/backbones/vit_det/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/classification/image_classifier.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/classification/image_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,8 +140,7 @@
         )
 
     @classproperty
     def backbone_presets(cls):
         """Dictionary of preset names and configurations of compatible
         backbones."""
         return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/classification/image_classifier_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/classification/image_classifier_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,8 +120,7 @@
             "params": 3_957_352,  # TODO this is wrong
             "official_name": "ImageClassifier",
             "path": "image_classifier",
         },
         "kaggle_handle": "kaggle://keras/mobilenetv3/keras/mobilenet_v3_large_imagenet_classifier/2",  # noqa: E501
     },
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from keras_cv.src.models.legacy.convnext import ConvNeXtTiny
 from keras_cv.src.models.legacy.convnext import ConvNeXtXLarge
 from keras_cv.src.models.legacy.darknet import DarkNet21
 from keras_cv.src.models.legacy.darknet import DarkNet53
 from keras_cv.src.models.legacy.mlp_mixer import MLPMixerB16
 from keras_cv.src.models.legacy.mlp_mixer import MLPMixerB32
 from keras_cv.src.models.legacy.mlp_mixer import MLPMixerL16
-from keras_cv.src.models.legacy.object_detection.faster_rcnn.faster_rcnn import (
+from keras_cv.src.models.legacy.object_detection.faster_rcnn.faster_rcnn import (  # noqa: E501
     FasterRCNN,
 )
 from keras_cv.src.models.legacy.regnet import RegNetX002
 from keras_cv.src.models.legacy.regnet import RegNetX004
 from keras_cv.src.models.legacy.regnet import RegNetX006
 from keras_cv.src.models.legacy.regnet import RegNetX008
 from keras_cv.src.models.legacy.regnet import RegNetX016
@@ -62,8 +62,7 @@
 from keras_cv.src.models.legacy.vit import ViTH32
 from keras_cv.src.models.legacy.vit import ViTL16
 from keras_cv.src.models.legacy.vit import ViTL32
 from keras_cv.src.models.legacy.vit import ViTS16
 from keras_cv.src.models.legacy.vit import ViTS32
 from keras_cv.src.models.legacy.vit import ViTTiny16
 from keras_cv.src.models.legacy.vit import ViTTiny32
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/convmixer.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/convmixer.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,8 +438,7 @@
     ConvMixer_1024_16,
     "__doc__",
     BASE_DOCSTRING.format(name="ConvMixer_1024_16"),
 )
 setattr(
     ConvMixer_512_16, "__doc__", BASE_DOCSTRING.format(name="ConvMixer_512_16")
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/convnext.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/convnext.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,8 +579,7 @@
 
 
 ConvNeXtTiny.__doc__ = BASE_DOCSTRING.format(name="ConvNeXtTiny")
 ConvNeXtSmall.__doc__ = BASE_DOCSTRING.format(name="ConvNeXtSmall")
 ConvNeXtBase.__doc__ = BASE_DOCSTRING.format(name="ConvNeXtBase")
 ConvNeXtLarge.__doc__ = BASE_DOCSTRING.format(name="ConvNeXtLarge")
 ConvNeXtXLarge.__doc__ = BASE_DOCSTRING.format(name="ConvNeXtXLarge")
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/darknet.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/darknet.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,8 +307,7 @@
         name=name,
         **kwargs,
     )
 
 
 setattr(DarkNet21, "__doc__", BASE_DOCSTRING.format(name="DarkNet21"))
 setattr(DarkNet53, "__doc__", BASE_DOCSTRING.format(name="DarkNet53"))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/mlp_mixer.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/mlp_mixer.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,8 +406,7 @@
         **kwargs,
     )
 
 
 setattr(MLPMixerB16, "__doc__", BASE_DOCSTRING.format(name="MLPMixerB16"))
 setattr(MLPMixerB32, "__doc__", BASE_DOCSTRING.format(name="MLPMixerB32"))
 setattr(MLPMixerL16, "__doc__", BASE_DOCSTRING.format(name="MLPMixerL16"))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/object_detection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/faster_rcnn/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/classification/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/faster_rcnn/faster_rcnn.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/object_detection/faster_rcnn/faster_rcnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,24 @@
 from tensorflow import keras
 
 from keras_cv.src import bounding_box
 from keras_cv.src import layers as cv_layers
 from keras_cv.src import models
 from keras_cv.src.bounding_box.converters import _decode_deltas_to_boxes
 from keras_cv.src.bounding_box.utils import _clip_boxes
-from keras_cv.src.layers.object_detection.anchor_generator import AnchorGenerator
+from keras_cv.src.layers.object_detection.anchor_generator import (
+    AnchorGenerator,
+)
 from keras_cv.src.layers.object_detection.box_matcher import BoxMatcher
 from keras_cv.src.layers.object_detection.roi_align import _ROIAligner
 from keras_cv.src.layers.object_detection.roi_generator import ROIGenerator
 from keras_cv.src.layers.object_detection.roi_sampler import _ROISampler
-from keras_cv.src.layers.object_detection.rpn_label_encoder import _RpnLabelEncoder
+from keras_cv.src.layers.object_detection.rpn_label_encoder import (
+    _RpnLabelEncoder,
+)
 from keras_cv.src.models.object_detection import predict_utils
 from keras_cv.src.models.object_detection.__internal__ import unpack_input
 from keras_cv.src.utils.train import get_feature_extractor
 
 BOX_VARIANCE = [0.1, 0.1, 0.2, 0.2]
 
 
@@ -227,15 +231,15 @@
 
     Implements the FasterRCNN architecture for object detection. The constructor
     requires `num_classes`, `bounding_box_format` and a `backbone`.
 
     References:
         - [FasterRCNN](https://arxiv.org/pdf/1506.01497.pdf)
 
-    Usage:
+    Example:
     ```python
     retinanet = keras_cv.models.FasterRCNN(
         num_classes=20,
         bounding_box_format="xywh",
         backbone=None,
     )
     ```
@@ -612,8 +616,7 @@
     if loss.reduction != keras.losses.Reduction.SUM:
         logging.info(
             f"FasterRCNN only accepts `SUM` reduction, got {loss.reduction}, "
             "automatically converted."
         )
         loss.reduction = keras.losses.Reduction.SUM
     return loss
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/regnet.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/regnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1593,8 +1593,7 @@
 RegNetY032.__doc__ = BASE_DOCSTRING.format(name="RegNetY032")
 RegNetY040.__doc__ = BASE_DOCSTRING.format(name="RegNetY040")
 RegNetY064.__doc__ = BASE_DOCSTRING.format(name="RegNetY064")
 RegNetY080.__doc__ = BASE_DOCSTRING.format(name="RegNetY080")
 RegNetY120.__doc__ = BASE_DOCSTRING.format(name="RegNetY120")
 RegNetY160.__doc__ = BASE_DOCSTRING.format(name="RegNetY160")
 RegNetY320.__doc__ = BASE_DOCSTRING.format(name="RegNetY320")
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/utils.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,8 +80,7 @@
         return keras.Model(inputs=self.inputs, outputs=outputs)
 
     else:
         raise ValueError(
             "The current model doesn't have any feature level "
             "information and can't be convert to backbone model."
         )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/vgg16.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/vgg16.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,8 +237,7 @@
             "classifier_activation": self.classifier_activation,
             "trainable": self.trainable,
         }
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/vgg19.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/vgg19.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,8 +198,7 @@
             "classifier_activation": self.classifier_activation,
             "trainable": self.trainable,
         }
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/vit.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/vit.py`

 * *Files 0% similar despite different names*

```diff
@@ -750,8 +750,7 @@
 setattr(ViTL16, "__doc__", BASE_DOCSTRING.format(name="ViTL16"))
 setattr(ViTH16, "__doc__", BASE_DOCSTRING.format(name="ViTH16"))
 setattr(ViTTiny32, "__doc__", BASE_DOCSTRING.format(name="ViTTiny32"))
 setattr(ViTS32, "__doc__", BASE_DOCSTRING.format(name="ViTS32"))
 setattr(ViTB32, "__doc__", BASE_DOCSTRING.format(name="ViTB32"))
 setattr(ViTL32, "__doc__", BASE_DOCSTRING.format(name="ViTL32"))
 setattr(ViTH32, "__doc__", BASE_DOCSTRING.format(name="ViTH32"))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/legacy/weights.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/weights.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,8 +177,7 @@
         "imagenet/classification-v0-notop": "f3907845eff780a4d29c1c56e0ae053411f02fff6fdce1147c4c3bb2124698cd",  # noqa: E501
     },
     "vitb32": {
         "imagenet/classification-v0": "73025caa78459dc8f9b1de7b58f1d64e24a823f170d17e25fcc8eb6179bea179",  # noqa: E501
         "imagenet/classification-v0-notop": "f07b80c03336d731a2a3a02af5cac1e9fc9aa62659cd29e2e7e5c7474150cc71",  # noqa: E501
     },
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/__internal__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/__internal__.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,8 +130,7 @@
         functools.partial(_split, start=0, end=split_at), arrays
     )
     val_arrays = tf.nest.map_structure(
         functools.partial(_split, start=split_at, end=batch_dim), arrays
     )
 
     return train_arrays, val_arrays
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/predict_utils.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/predict_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,8 +97,7 @@
             return outputs
 
     if not model.run_eagerly:
         predict_function = tf.function(predict_function, reduce_retracing=True)
     model.predict_function = predict_function
 
     return predict_function
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/retinanet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,7 @@
 )
 from keras_cv.src.models.object_detection.retinanet.prediction_head import (
     PredictionHead,
 )
 from keras_cv.src.models.object_detection.retinanet.retinanet_label_encoder import (  # noqa: E501
     RetinaNetLabelEncoder,
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/feature_pyramid.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/retinanet/feature_pyramid.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,8 +76,7 @@
         return (
             (tuple(p3_shape) + (256,)),
             (tuple(p4_shape) + (256,)),
             (tuple(p5_shape) + (256,)),
             (tuple(p5_shape) + (256,)),
             (tuple(p5_shape) + (256,)),
         )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/prediction_head.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/retinanet/prediction_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,8 +92,7 @@
 
         intermediate_shape = tuple(input_shape[:-1]) + (256,)
         for conv_layer in self.conv_layers[1:]:
             conv_layer.build(intermediate_shape)
 
         self.prediction_layer.build(intermediate_shape)
         self.built = True
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/retinanet.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/retinanet/retinanet.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 class RetinaNet(Task):
     """A Keras model implementing the RetinaNet meta-architecture.
 
     Implements the RetinaNet architecture for object detection. The constructor
     requires `num_classes`, `bounding_box_format`, and a backbone. Optionally,
     a custom label encoder, and prediction decoder may be provided.
 
-    Examples:
+    Example:
     ```python
     images = np.ones((1, 512, 512, 3))
     labels = {
         "boxes": tf.cast([
             [
                 [0, 0, 100, 100],
                 [100, 100, 200, 200],
@@ -578,8 +578,7 @@
     if loss.lower() == "focal":
         return losses.FocalLoss(from_logits=True, reduction="sum")
 
     raise ValueError(
         "Expected `classification_loss` to be either a Keras Loss, "
         f"callable, or the string 'Focal'. Got loss={loss}."
     )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/retinanet_label_encoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/retinanet/retinanet_label_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,8 +246,7 @@
         return super().from_config(config)
 
 
 class MatchedBoxesMetric(keras.metrics.BinaryAccuracy):
     # Prevent `load_weights` from accessing metric
     def load_own_variables(self, store):
         return
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/retinanet_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/retinanet/retinanet_presets.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,7 @@
             "params": 35596952,
             "official_name": "RetinaNet",
             "path": "retinanet",
         },
         "kaggle_handle": "kaggle://keras/retinanet/keras/retinanet_resnet50_pascalvoc/2",  # noqa: E501
     },
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segformer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,11 +7,9 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_label_encoder import (
-    YOLOV8LabelEncoder,
-)
 
+from keras_cv.src.models.segmentation.segformer.segformer import SegFormer
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 import copy
 
 from keras_cv.src.api_export import keras_cv_export
 from keras_cv.src.backend import keras
 from keras_cv.src.backend import ops
 from keras_cv.src.models import utils
 from keras_cv.src.models.backbones.backbone import Backbone
-from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_backbone_presets import (
+from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_backbone_presets import (  # noqa: E501
     backbone_presets,
 )
-from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_backbone_presets import (
+from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_backbone_presets import (  # noqa: E501
     backbone_presets_with_weights,
 )
 from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_layers import (
     apply_conv_bn,
 )
 from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_layers import (
     apply_csp_block,
@@ -209,8 +209,7 @@
         return copy.deepcopy(backbone_presets)
 
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return copy.deepcopy(backbone_presets_with_weights)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,8 +114,7 @@
     },
 }
 
 backbone_presets = {
     **backbone_presets_no_weights,
     **backbone_presets_with_weights,
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from keras_cv.src.backend import ops
 from keras_cv.src.losses.ciou_loss import CIoULoss
 from keras_cv.src.models.backbones.backbone_presets import backbone_presets
 from keras_cv.src.models.backbones.backbone_presets import (
     backbone_presets_with_weights,
 )
 from keras_cv.src.models.object_detection.__internal__ import unpack_input
-from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_detector_presets import (
+from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_detector_presets import (  # noqa: E501
     yolo_v8_detector_presets,
 )
 from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_label_encoder import (
     YOLOV8LabelEncoder,
 )
 from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_layers import (
     apply_conv_bn,
@@ -327,15 +327,15 @@
     ]
 )
 class YOLOV8Detector(Task):
     """Implements the YOLOV8 architecture for object detection.
 
     Args:
         backbone: `keras.Model`, must implement the `pyramid_level_inputs`
-            property with keys "P2", "P3", and "P4" and layer names as values.
+            property with keys "P3", "P4", and "P5" and layer names as values.
             A sensible backbone to use is the `keras_cv.models.YOLOV8Backbone`.
         num_classes: integer, the number of classes in your dataset excluding the
             background class. Classes should be represented by integers in the
             range [0, num_classes).
         bounding_box_format: string, the format of bounding boxes of input dataset.
             Refer
             [to the keras.io docs](https://keras.io/api/keras_cv/bounding_box/formats/)
@@ -350,15 +350,15 @@
         prediction_decoder: (Optional)  A `keras.layers.Layer` that is
             responsible for transforming YOLOV8 predictions into usable
             bounding boxes. If not provided, a default is provided. The
             default `prediction_decoder` layer is a
             `keras_cv.layers.MultiClassNonMaxSuppression` layer, which uses
             a Non-Max Suppression for box pruning.
 
-    Examples:
+    Example:
     ```python
     images = tf.ones(shape=(1, 512, 512, 3))
     labels = {
         "boxes": tf.constant([
             [
                 [0, 0, 100, 100],
                 [100, 100, 200, 200],
@@ -682,8 +682,7 @@
         )
 
     @classproperty
     def backbone_presets(cls):
         """Dictionary of preset names and configurations of compatible
         backbones."""
         return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,7 @@
             "params": 25901004,
             "official_name": "YOLOV8Detector",
             "path": "yolo_v8_detector",
         },
         "kaggle_handle": "kaggle://keras/yolov8/keras/yolo_v8_m_pascalvoc/2",
     },
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_label_encoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_label_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,8 +268,7 @@
             "num_classes": self.num_classes,
             "alpha": self.alpha,
             "beta": self.beta,
             "epsilon": self.epsilon,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_layers.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,8 +97,7 @@
         out,
         channels,
         kernel_size=1,
         activation=activation,
         name=f"{name}_output",
     )
     return out
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/feature_extractor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/binary_crossentropy.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/binary_crossentropy.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             0, we compute the loss between the predicted labels and a smoothed
             version of the true labels, where the smoothing squeezes the labels
             towards 0.5.  Larger values of `label_smoothing` correspond to
             heavier smoothing.
         axis: the axis along which to mean the ious. Defaults to `no_reduction`
             which implies mean across no axes.
 
-    Usage:
+    Example:
     ```python
     model.compile(
       loss=BinaryCrossentropy(from_logits=True)
       ....
     )
     ```
     """
@@ -92,8 +92,7 @@
             {
                 "from_logits": self.from_logits,
                 "label_smoothing": self.label_smoothing,
                 "axis": self.axis,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/layers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,13 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from keras_cv.src.models.object_detection.yolox.layers.yolox_decoder import (
     YoloXPredictionDecoder,
 )
-from keras_cv.src.models.object_detection.yolox.layers.yolox_head import YoloXHead
-from keras_cv.src.models.object_detection.yolox.layers.yolox_label_encoder import (
+from keras_cv.src.models.object_detection.yolox.layers.yolox_head import (
+    YoloXHead,
+)
+from keras_cv.src.models.object_detection.yolox.layers.yolox_label_encoder import (  # noqa: E501
     YoloXLabelEncoder,
 )
-from keras_cv.src.models.object_detection.yolox.layers.yolox_pafpn import YoloXPAFPN
-
+from keras_cv.src.models.object_detection.yolox.layers.yolox_pafpn import (
+    YoloXPAFPN,
+)
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_decoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,8 +165,7 @@
         class_predictions = tf.one_hot(class_predictions, self.num_classes)
 
         scores = (
             tf.expand_dims(outputs["confidence"], axis=-1) * class_predictions
         )
 
         return self.suppression_layer(outputs["boxes"], scores)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_head.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_head.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,8 +155,7 @@
             objectness = self.objectness_preds[i](boxes_feat)
 
             output = keras.layers.Concatenate(axis=-1)(
                 [boxes, objectness, classes]
             )
             outputs.append(output)
         return outputs
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_label_encoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_label_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,8 +45,7 @@
 
         box_labels = bounding_box.to_dense(box_labels)
         box_labels["classes"] = box_labels["classes"][..., tf.newaxis]
 
         encoded_box_targets = box_labels["boxes"]
         class_targets = box_labels["classes"]
         return encoded_box_targets, class_targets
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_pafpn.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_pafpn.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,8 +142,7 @@
         pan_out1 = self.C3_n3(p_out1)
 
         p_out0 = self.bu_conv1(pan_out1)
         p_out0 = self.concat([p_out0, fpn_out0])
         pan_out0 = self.C3_n4(p_out0)
 
         return pan_out2, pan_out1, pan_out0
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection_3d/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,7 @@
 # limitations under the License.
 from keras_cv.src.models.object_detection_3d.center_pillar import (
     MultiHeadCenterPillar,
 )
 from keras_cv.src.models.object_detection_3d.center_pillar_backbone import (
     CenterPillarBackbone,
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/center_pillar.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection_3d/center_pillar.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 # limitations under the License.
 
 import copy
 
 from keras_cv.src.api_export import keras_cv_export
 from keras_cv.src.backend import keras
 from keras_cv.src.backend import ops
-from keras_cv.src.layers.object_detection_3d.heatmap_decoder import HeatmapDecoder
-from keras_cv.src.models.object_detection_3d.center_pillar_backbone_presets import (
+from keras_cv.src.layers.object_detection_3d.heatmap_decoder import (
+    HeatmapDecoder,
+)
+from keras_cv.src.models.object_detection_3d.center_pillar_backbone_presets import (  # noqa: E501
     backbone_presets,
 )
 from keras_cv.src.models.task import Task
 from keras_cv.src.utils.python_utils import classproperty
 
 
 @keras_cv_export("keras_cv.models.MultiHeadCenterPillar")
@@ -336,8 +338,7 @@
         return {
             "3d_boxes": {
                 "boxes": ops.concatenate(box_predictions, axis=1),
                 "classes": ops.concatenate(class_predictions, axis=1),
                 "confidence": ops.concatenate(box_confidence, axis=1),
             }
         }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/center_pillar_backbone.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection_3d/center_pillar_backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 
 from keras_cv.src.api_export import keras_cv_export
 from keras_cv.src.backend import keras
 from keras_cv.src.models.backbones.backbone import Backbone
-from keras_cv.src.models.object_detection_3d.center_pillar_backbone_presets import (
+from keras_cv.src.models.object_detection_3d.center_pillar_backbone_presets import (  # noqa: E501
     backbone_presets,
 )
 from keras_cv.src.utils.python_utils import classproperty
 
 
 @keras_cv_export("keras_cv.models.CenterPillarBackbone")
 class CenterPillarBackbone(Backbone):
@@ -218,8 +218,7 @@
 
         x = keras.layers.Add()([x, lateral_input])
         x = Block(filters, downsample=False)(x)
 
         return x
 
     return apply
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/center_pillar_backbone_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/object_detection_3d/center_pillar_backbone_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,7 @@
             "description": "An example CenterPillar backbone for WOD.",
             "params": 1277680,
             "official_name": "CenterPillar",
         },
         "kaggle_handle": "gs://keras-cv-kaggle/center_pillar_waymo_open_dataset",  # noqa: E501
     },
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 # limitations under the License.
 
 from keras_cv.src.models.segmentation.basnet import BASNet
 from keras_cv.src.models.segmentation.deeplab_v3_plus import DeepLabV3Plus
 from keras_cv.src.models.segmentation.segformer import SegFormer
 from keras_cv.src.models.segmentation.segment_anything import SAMMaskDecoder
 from keras_cv.src.models.segmentation.segment_anything import SAMPromptEncoder
-from keras_cv.src.models.segmentation.segment_anything import SegmentAnythingModel
+from keras_cv.src.models.segmentation.segment_anything import (
+    SegmentAnythingModel,
+)
 from keras_cv.src.models.segmentation.segment_anything import TwoWayTransformer
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/basnet/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# Copyright 2023 The KerasCV Authors
+# Copyright 2022 The KerasCV Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from keras_cv.src.models.segmentation.basnet.basnet import BASNet
-
+from keras_cv.src.models.segmentation.deeplab_v3_plus.deeplab_v3_plus import (
+    DeepLabV3Plus,
+)
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/basnet/basnet.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/basnet/basnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 from keras_cv.src.api_export import keras_cv_export
 from keras_cv.src.backend import keras
 from keras_cv.src.models import utils
 from keras_cv.src.models.backbones.backbone_presets import backbone_presets
 from keras_cv.src.models.backbones.resnet_v1.resnet_v1_backbone import (
     apply_basic_block as resnet_basic_block,
 )
-from keras_cv.src.models.segmentation.basnet.basnet_presets import basnet_presets
+from keras_cv.src.models.segmentation.basnet.basnet_presets import (
+    basnet_presets,
+)
 from keras_cv.src.models.segmentation.basnet.basnet_presets import (
     presets_no_weights,
 )
 from keras_cv.src.models.segmentation.basnet.basnet_presets import (
     presets_with_weights,
 )
 from keras_cv.src.models.task import Task
@@ -66,15 +68,15 @@
         prediction_heads: (Optional) List of `keras.layers.Layer` defining
             the prediction module head for the model. If not provided, a
             default head is created with a Conv2D layer followed by resizing.
         refinement_head: (Optional) a `keras.layers.Layer` defining the
             refinement module head for the model. If not provided, a default
             head is created with a Conv2D layer.
 
-    Examples:
+    Example:
     ```python
 
     import keras_cv
 
     images = np.ones(shape=(1, 288, 288, 3))
     labels = np.zeros(shape=(1, 288, 288, 1))
 
@@ -448,8 +450,7 @@
 
     x = segmentation_head(x)  # Refinement segmentation head.
 
     # ------------- refined = coarse + residual
     x = keras.layers.Add()([x_input, x])  # Add prediction + refinement output
 
     return keras.models.Model(inputs=base_model.input, outputs=[x])
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/basnet/basnet_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/basnet/basnet_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,7 @@
 }
 
 presets_with_weights = {
     # TODO: Add BASNet preset with weights
 }
 
 basnet_presets = {**presets_no_weights, **presets_with_weights}
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/visualization/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-# Copyright 2022 The KerasCV Authors
+# Copyright 2023 The KerasCV Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from keras_cv.src.models.segmentation.deeplab_v3_plus.deeplab_v3_plus import (
-    DeepLabV3Plus,
+from keras_cv.src.visualization.plot_bounding_box_gallery import (
+    plot_bounding_box_gallery,
+)
+from keras_cv.src.visualization.plot_image_gallery import plot_image_gallery
+from keras_cv.src.visualization.plot_segmentation_mask_gallery import (
+    plot_segmentation_mask_gallery,
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             `keras_cv.layers.spatial_pyramid.SpatialPyramidPooling` is used.
         segmentation_head: (Optional) a `keras.layers.Layer`. If provided, the
             outputs of the DeepLabV3 encoder is passed to this layer and it
             should predict the segmentation mask based on feature from backbone
             and feature from decoder, otherwise a default DeepLabV3
             convolutional head is used.
 
-    Examples:
+    Example:
     ```python
     import keras_cv
 
     images = np.ones(shape=(1, 96, 96, 3))
     labels = np.zeros(shape=(1, 96, 96, 1))
     backbone = keras_cv.models.ResNet50V2Backbone(input_shape=[96, 96, 3])
     model = keras_cv.models.segmentation.DeepLabV3Plus(
@@ -255,8 +255,7 @@
         )
 
     @classproperty
     def backbone_presets(cls):
         """Dictionary of preset names and configurations of compatible
         backbones."""
         return copy.deepcopy(backbone_presets)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,7 @@
             "params": 39191488,
             "official_name": "DeepLabV3Plus",
             "path": "deeplab_v3_plus",
         },
         "kaggle_handle": "kaggle://keras/deeplabv3plus/keras/deeplab_v3_plus_resnet50_pascalvoc/2",  # noqa: E501
     },
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/datasets/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# Copyright 2023 The KerasCV Authors
+# Copyright 2022 The KerasCV Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from keras_cv.src.models.segmentation.segformer.segformer import SegFormer
-
+from keras_cv.src.datasets import pascal_voc
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/segformer.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segformer/segformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             values.
         num_classes: int, the number of classes for the detection model,
             including the background class.
         projection_filters: int, number of filters in the
             convolution layer projecting the concatenated features into
             a segmentation map. Defaults to 256`.
 
-    Examples:
+    Example:
 
     Using the class with a `backbone`:
 
     ```python
     import tensorflow as tf
     import keras_cv
 
@@ -203,8 +203,7 @@
         """Dictionary of preset names and configurations that include
         weights."""
         return copy.deepcopy(presets_with_weights)
 
     @classproperty
     def backbone_presets(cls):
         return copy.deepcopy(MiTBackbone.presets)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/segformer_aliases.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segformer/segformer_aliases.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,39 +10,41 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 
+from keras_cv.src.api_export import keras_cv_export
 from keras_cv.src.models.segmentation.segformer.segformer import SegFormer
 from keras_cv.src.models.segmentation.segformer.segformer_presets import presets
 from keras_cv.src.utils.python_utils import classproperty
 
 ALIAS_DOCSTRING = """SegFormer model.
 
     For transfer learning use cases, make sure to read the
     [guide to transfer learning & fine-tuning](https://keras.io/guides/transfer_learning/).
 
     Args:
         backbone: a KerasCV backbone for feature extraction.
         num_classes: the number of classes for segmentation, including the background class.
 
-    Examples:
+    Example:
     ```python
     input_data = tf.ones(shape=(8, 224, 224, 3))
 
     # Randomly initialized backbone
     backbone = keras_cv.models.MiTBackbone.from_preset("mit_b0_imagenet")
     segformer = keras_cv.models.SegFormer(backbone=backbone, num_classes=19)
     output = model(input_data)
     ```
 """  # noqa: E501
 
 
+@keras_cv_export("keras_cv.models.SegFormerB0")
 class SegFormerB0(SegFormer):
     def __new__(
         cls,
         num_classes,
         **kwargs,
     ):
         # Pack args in kwargs
@@ -63,14 +65,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return cls.presets
 
 
+@keras_cv_export("keras_cv.models.SegFormerB1")
 class SegFormerB1(SegFormer):
     def __new__(
         cls,
         num_classes,
         **kwargs,
     ):
         # Pack args in kwargs
@@ -91,14 +94,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return cls.presets
 
 
+@keras_cv_export("keras_cv.models.SegFormerB2")
 class SegFormerB2(SegFormer):
     def __new__(
         cls,
         num_classes,
         **kwargs,
     ):
         # Pack args in kwargs
@@ -119,14 +123,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return cls.presets
 
 
+@keras_cv_export("keras_cv.models.SegFormerB3")
 class SegFormerB3(SegFormer):
     def __new__(
         cls,
         num_classes,
         **kwargs,
     ):
         # Pack args in kwargs
@@ -147,14 +152,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return cls.presets
 
 
+@keras_cv_export("keras_cv.models.SegFormerB4")
 class SegFormerB4(SegFormer):
     def __new__(
         cls,
         num_classes,
         **kwargs,
     ):
         # Pack args in kwargs
@@ -175,14 +181,15 @@
     @classproperty
     def presets_with_weights(cls):
         """Dictionary of preset names and configurations that include
         weights."""
         return cls.presets
 
 
+@keras_cv_export("keras_cv.models.SegFormerB5")
 class SegFormerB5(SegFormer):
     def __new__(
         cls,
         num_classes,
         **kwargs,
     ):
         # Pack args in kwargs
@@ -238,8 +245,7 @@
 )
 
 setattr(
     SegFormerB5,
     "__doc__",
     ALIAS_DOCSTRING.format(name="SegFormerB5"),
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/segformer_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segformer/segformer_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,8 +89,7 @@
 }
 
 presets = {
     **backbone_presets,  # Add MiTBackbone presets
     **presets_no_weights,
     **presets_with_weights,
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,13 @@
 
 from keras_cv.src.models.segmentation.segment_anything.sam import (
     SegmentAnythingModel,
 )
 from keras_cv.src.models.segmentation.segment_anything.sam_mask_decoder import (
     SAMMaskDecoder,
 )
-from keras_cv.src.models.segmentation.segment_anything.sam_prompt_encoder import (
+from keras_cv.src.models.segmentation.segment_anything.sam_prompt_encoder import (  # noqa: E501
     SAMPromptEncoder,
 )
 from keras_cv.src.models.segmentation.segment_anything.sam_transformer import (
     TwoWayTransformer,
 )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/sam.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,20 +50,20 @@
             generate segmentation masks given the embeddings generated by the
             backbone and the prompt encoder.
 
     References:
         - [Segment Anything paper](https://arxiv.org/abs/2304.02643)
         - [Segment Anything GitHub](https://github.com/facebookresearch/segment-anything)
 
-    Examples:
+    Example:
 
     >>> import numpy as np
-    >>> from keras_cv.models import ViTDetBBackbone
-    >>> from keras_cv.models import SAMPromptEncoder
-    >>> from keras_cv.models import SAMMaskDecoder
+    >>> from keras_cv.src.models import ViTDetBBackbone
+    >>> from keras_cv.src.models import SAMPromptEncoder
+    >>> from keras_cv.src.models import SAMMaskDecoder
 
     Create all the components of the SAM model:
 
     >>> backbone = ViTDetBBackbone()
     >>> prompt_encoder = SAMPromptEncoder()
     >>> mask_decoder = SAMMaskDecoder()
 
@@ -284,8 +284,7 @@
         inputs["labels"] = zeros((B, 0))
     if "boxes" not in inputs:
         inputs["boxes"] = zeros((B, 0, 2, 2))
     if "masks" not in inputs:
         inputs["masks"] = zeros((B, 0, 256, 256, 1))
 
     return inputs
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_layers.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/sam_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,8 +341,7 @@
         config.update(
             {
                 "num_positional_features": self.num_positional_features,
                 "scale": self.scale,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_mask_decoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/sam_mask_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,8 +234,7 @@
 
     @classmethod
     def from_config(cls, config):
         config.update(
             {"transformer": keras.layers.deserialize(config["transformer"])}
         )
         return super().from_config(config)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_presets.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/sam_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,7 @@
             "params": 641_090_864,
             "official_name": "SAM",
             "path": "segment_anything",
         },
         "kaggle_handle": "kaggle://keras/sam/keras/sam_huge_sa1b/2",
     },
 }
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_prompt_encoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/sam_prompt_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,8 +295,7 @@
                 "image_embedding_size": self.image_embedding_size,
                 "input_image_size": self.input_image_size,
                 "mask_in_chans": self.mask_in_chans,
                 "activation": self.activation,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_transformer.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/segmentation/segment_anything/sam_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,8 +149,7 @@
                 "num_heads": self.num_heads,
                 "mlp_dim": self.mlp_dim,
                 "activation": self.activation,
                 "attention_downsample_rate": self.attention_downsample_rate,
             }
         )
         return config
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from keras_cv.src.models.stable_diffusion.clip_tokenizer import SimpleTokenizer
 from keras_cv.src.models.stable_diffusion.decoder import Decoder
 from keras_cv.src.models.stable_diffusion.diffusion_model import DiffusionModel
-from keras_cv.src.models.stable_diffusion.diffusion_model import DiffusionModelV2
+from keras_cv.src.models.stable_diffusion.diffusion_model import (
+    DiffusionModelV2,
+)
 from keras_cv.src.models.stable_diffusion.image_encoder import ImageEncoder
 from keras_cv.src.models.stable_diffusion.noise_scheduler import NoiseScheduler
-from keras_cv.src.models.stable_diffusion.stable_diffusion import StableDiffusion
-from keras_cv.src.models.stable_diffusion.stable_diffusion import StableDiffusionV2
+from keras_cv.src.models.stable_diffusion.stable_diffusion import (
+    StableDiffusion,
+)
+from keras_cv.src.models.stable_diffusion.stable_diffusion import (
+    StableDiffusionV2,
+)
 from keras_cv.src.models.stable_diffusion.text_encoder import TextEncoder
 from keras_cv.src.models.stable_diffusion.text_encoder import TextEncoderV2
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/attention_block.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/attention_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,7 @@
         v = ops.transpose(v, (0, 3, 1, 2))
         v = ops.reshape(v, (-1, c, h * w))
         y = ops.transpose(y, (0, 2, 1))
         x = v @ y
         x = ops.transpose(x, (0, 2, 1))
         x = ops.reshape(x, (-1, h, w, c))
         return self.proj_out(x) + inputs
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/clip_tokenizer.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/clip_tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,8 +209,7 @@
         text = "".join([self.decoder[token] for token in tokens])
         text = (
             bytearray([self.byte_decoder[c] for c in text])
             .decode("utf-8", errors="replace")
             .replace("</w>", " ")
         )
         return text
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/constants.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1089,8 +1089,7 @@
     0.0049491767,
     0.004890135,
     0.0048317118,
     0.004773902,
     0.004716699,
     0.0046600983,
 ]
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/decoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,8 +60,7 @@
 
         if download_weights:
             decoder_weights_fpath = keras.utils.get_file(
                 origin="https://huggingface.co/fchollet/stable-diffusion/resolve/main/kcv_decoder.h5",  # noqa: E501
                 file_hash="ad350a65cc8bc4a80c8103367e039a3329b4231c2469a1093869a345f55b1962",  # noqa: E501
             )
             self.load_weights(decoder_weights_fpath)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/diffusion_model.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/diffusion_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,8 +364,7 @@
 
 
 def td_dot(a, b):
     aa = ops.reshape(a, (-1, a.shape[2], a.shape[3]))
     bb = ops.reshape(b, (-1, b.shape[2], b.shape[3]))
     cc = keras.layers.Dot(axes=(2, 1))([aa, bb])
     return ops.reshape(cc, (-1, a.shape[1], cc.shape[1], cc.shape[2]))
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/image_encoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/image_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,7 @@
 
         if download_weights:
             image_encoder_weights_fpath = keras.utils.get_file(
                 origin="https://huggingface.co/fchollet/stable-diffusion/resolve/main/vae_encoder.h5",  # noqa: E501
                 file_hash="c60fb220a40d090e0f86a6ab4c312d113e115c87c40ff75d11ffcf380aab7ebb",  # noqa: E501
             )
             self.load_weights(image_encoder_weights_fpath)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/noise_scheduler.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/noise_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,8 +213,7 @@
             sqrt_alpha_prod * original_samples
             + sqrt_one_minus_alpha_prod * noise
         )
         return noisy_samples
 
     def __len__(self):
         return self.train_timesteps
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/padded_conv2d.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/padded_conv2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,7 @@
         super().__init__(**kwargs)
         self.padding2d = keras.layers.ZeroPadding2D(padding)
         self.conv2d = keras.layers.Conv2D(filters, kernel_size, strides=strides)
 
     def call(self, inputs):
         x = self.padding2d(inputs)
         return self.conv2d(x)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/resnet_block.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/resnet_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,7 @@
         else:
             self.residual_projection = lambda x: x
 
     def call(self, inputs):
         x = self.conv1(keras.activations.swish(self.norm1(inputs)))
         x = self.conv2(keras.activations.swish(self.norm2(x)))
         return x + self.residual_projection(inputs)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/stable_diffusion.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/stable_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 from keras_cv.src.backend import ops
 from keras_cv.src.backend import random
 from keras_cv.src.models.stable_diffusion.clip_tokenizer import SimpleTokenizer
 from keras_cv.src.models.stable_diffusion.constants import _ALPHAS_CUMPROD
 from keras_cv.src.models.stable_diffusion.constants import _UNCONDITIONAL_TOKENS
 from keras_cv.src.models.stable_diffusion.decoder import Decoder
 from keras_cv.src.models.stable_diffusion.diffusion_model import DiffusionModel
-from keras_cv.src.models.stable_diffusion.diffusion_model import DiffusionModelV2
+from keras_cv.src.models.stable_diffusion.diffusion_model import (
+    DiffusionModelV2,
+)
 from keras_cv.src.models.stable_diffusion.image_encoder import ImageEncoder
 from keras_cv.src.models.stable_diffusion.text_encoder import TextEncoder
 from keras_cv.src.models.stable_diffusion.text_encoder import TextEncoderV2
 
 MAX_PROMPT_LENGTH = 77
 
 
@@ -100,15 +102,15 @@
 
         Args:
             prompt: a string to encode, must be 77 tokens or shorter.
 
         Example:
 
         ```python
-        from keras_cv.models import StableDiffusion
+        from keras_cv.src.models import StableDiffusion
 
         model = StableDiffusion(img_height=512, img_width=512, jit_compile=True)
         encoded_text  = model.encode_text("Tacos at dawn")
         img = model.generate_image(encoded_text)
         ```
         """
         # Tokenize prompt (i.e. starting context)
@@ -163,15 +165,15 @@
             seed: integer which is used to seed the random generation of
                 diffusion noise, only to be specified if `diffusion_noise` is
                 None.
 
         Example:
 
         ```python
-        from keras_cv.models import StableDiffusion
+        from keras_cv.src.models import StableDiffusion
         from keras_core import ops
 
         batch_size = 8
         model = StableDiffusion(img_height=512, img_width=512, jit_compile=True)
         e_tacos = model.encode_text("Tacos at dawn")
         e_watermelons = model.encode_text("Watermelons at dusk")
 
@@ -206,15 +208,19 @@
                 )
             latent = diffusion_noise
         else:
             latent = self._get_initial_diffusion_noise(batch_size, seed)
 
         # Iterative reverse diffusion stage
         num_timesteps = 1000
-        ratio = (num_timesteps - 1) / (num_steps - 1)
+        ratio = (
+            (num_timesteps - 1) / (num_steps - 1)
+            if num_steps > 1
+            else num_timesteps
+        )
         timesteps = (np.arange(0, num_steps) * ratio).round().astype(np.int64)
 
         alphas, alphas_prev = self._get_initial_alphas(timesteps)
         progbar = keras.utils.Progbar(len(timesteps))
         iteration = 0
         for index, timestep in list(enumerate(timesteps))[::-1]:
             latent_prev = latent  # Set aside the previous latent vector
@@ -277,15 +283,15 @@
             )
         return text_embedding
 
     @property
     def image_encoder(self):
         """image_encoder returns the VAE Encoder with pretrained weights.
 
-        Usage:
+        Example:
         ```python
         sd = keras_cv.models.StableDiffusion()
         my_image = np.ones((512, 512, 3))
         latent_representation = sd.image_encoder.predict(my_image)
         ```
         """
         if self._image_encoder is None:
@@ -375,15 +381,15 @@
         jit_compile: bool, whether to compile the underlying models to XLA.
             This can lead to a significant speedup on some systems. Defaults to
             False.
 
     Example:
 
     ```python
-    from keras_cv.models import StableDiffusion
+    from keras_cv.src.models import StableDiffusion
     from PIL import Image
 
     model = StableDiffusion(img_height=512, img_width=512, jit_compile=True)
     img = model.text_to_image(
         prompt="A beautiful horse running through a field",
         batch_size=1,  # How many images to generate at once
         num_steps=25,  # Number of iterations (controls image quality)
@@ -460,15 +466,15 @@
             rounded to the nearest valid value. Defaults to 512.
         jit_compile: bool, whether to compile the underlying models to XLA.
             This can lead to a significant speedup on some systems. Defaults to
             False.
     Example:
 
     ```python
-    from keras_cv.models import StableDiffusionV2
+    from keras_cv.src.models import StableDiffusionV2
     from PIL import Image
 
     model = StableDiffusionV2(img_height=512, img_width=512, jit_compile=True)
     img = model.text_to_image(
         prompt="A beautiful horse running through a field",
         batch_size=1,  # How many images to generate at once
         num_steps=25,  # Number of iterations (controls image quality)
@@ -518,8 +524,7 @@
         if self._diffusion_model is None:
             self._diffusion_model = DiffusionModelV2(
                 self.img_height, self.img_width, MAX_PROMPT_LENGTH
             )
             if self.jit_compile:
                 self._diffusion_model.compile(jit_compile=True)
         return self._diffusion_model
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/text_encoder.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/stable_diffusion/text_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,8 +164,7 @@
 
         attn_output = ops.reshape(
             attn_output, (-1, self.num_heads, tgt_len, self.head_dim)
         )
         attn_output = ops.transpose(attn_output, (0, 2, 1, 3))
         attn_output = ops.reshape(attn_output, (-1, tgt_len, embed_dim))
         return self.out_proj(attn_output)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/task.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             load_weights: Whether to load pre-trained weights into model.
                 Defaults to `None`, which follows whether the preset has
                 pretrained weights available.
             input_shape : input shape that will be passed to backbone
                 initialization, Defaults to `None`.If `None`, the preset
                 value will be used.
 
-        Examples:
+        Example:
         ```python
         # Load architecture and weights from preset
         model = keras_cv.models.{{model_name}}.from_preset(
             "{{example_preset_name}}",
         )
 
         # Load randomly initialized model from preset architecture with weights
@@ -196,8 +196,7 @@
             cls.from_preset.__func__.__doc__ = Task.from_preset.__doc__
             format_docstring(
                 model_name=cls.__name__,
                 example_preset_name=next(iter(cls.presets_with_weights), ""),
                 preset_names='", "'.join(cls.presets),
                 preset_with_weights_names='", "'.join(cls.presets_with_weights),
             )(cls.from_preset.__func__)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/models/utils.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,7 @@
     else:
         adjust = (1 - input_size[0] % 2, 1 - input_size[1] % 2)
     correct = (kernel_size[0] // 2, kernel_size[1] // 2)
     return (
         (correct[0] - adjust[0], correct[0]),
         (correct[1] - adjust[1], correct[1]),
     )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/ops/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from keras_cv.src.ops.iou_3d import iou_3d
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/ops/iou_3d.py` & `keras_cv-0.9.0.dev0/keras_cv/src/ops/iou_3d.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,17 +25,16 @@
     Note that this is implemented using a custom TensorFlow op. If you don't
     have KerasCV installed with custom ops, calling this will fail.
 
     Boxes should have the format CENTER_XYZ_DXDYDZ_PHI. Refer to
     https://github.com/keras-team/keras-cv/blob/master/keras_cv/bounding_box_3d/formats.py
     for more details on supported bounding box formats.
 
-    Sample Usage:
+    Example:
     ```python
     y_true = [[0, 0, 0, 2, 2, 2, 0], [1, 1, 1, 2, 2, 2, 3 * math.pi / 4]]
     y_pred = [[1, 1, 1, 2, 2, 2, math.pi / 4], [1, 1, 1, 2, 2, 2, 0]]
     iou_3d(y_true, y_pred)
     ```
     """
 
     return keras_cv_custom_ops.ops.kcv_pairwise_iou3d(y_true, y_pred)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/point_cloud/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/point_cloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,7 @@
 from keras_cv.src.point_cloud.point_cloud import is_within_any_box3d_v3
 from keras_cv.src.point_cloud.point_cloud import is_within_box2d
 from keras_cv.src.point_cloud.point_cloud import is_within_box3d
 from keras_cv.src.point_cloud.point_cloud import spherical_coordinate_transform
 from keras_cv.src.point_cloud.point_cloud import within_a_frustum
 from keras_cv.src.point_cloud.point_cloud import within_box3d_index
 from keras_cv.src.point_cloud.point_cloud import wrap_angle_radians
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/point_cloud/point_cloud.py` & `keras_cv-0.9.0.dev0/keras_cv/src/point_cloud/point_cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,8 +524,7 @@
 
     in_phi_width = (phi < (center_phi + phi_half_width)) & (
         phi > (center_phi - phi_half_width)
     )
 
     in_r_distance = r > r_distance
     return in_theta_width & in_phi_width & in_r_distance
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/tests/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/models/legacy/object_detection/faster_rcnn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/tests/test_case.py` & `keras_cv-0.9.0.dev0/keras_cv/src/tests/test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,8 +41,7 @@
         super().assertAllLessEqual(x1, x2)
 
 
 def convert_to_numpy(x):
     if ops.is_tensor(x) and not isinstance(x, tf.RaggedTensor):
         return ops.convert_to_numpy(x)
     return x
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/training/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/training/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from keras_cv.src.training.contrastive.contrastive_trainer import ContrastiveTrainer
+from keras_cv.src.training.contrastive.contrastive_trainer import (
+    ContrastiveTrainer,
+)
 from keras_cv.src.training.contrastive.simclr_trainer import SimCLRAugmenter
 from keras_cv.src.training.contrastive.simclr_trainer import SimCLRTrainer
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/training/contrastive/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/training/contrastive/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/training/contrastive/contrastive_trainer.py` & `keras_cv-0.9.0.dev0/keras_cv/src/training/contrastive/contrastive_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             This predicts class labels based on the feature map produced by the
             encoder and is usually a 1 or 2-layer dense MLP.
 
     Returns:
       A `keras.Model` instance.
 
 
-    Usage:
+    Example:
     ```python
     encoder = keras.Sequential(
         [
             DenseNet121Backbone(include_rescaling=False),
             layers.GlobalAveragePooling2D(name="avg_pool"),
         ],
     )
@@ -281,8 +281,7 @@
             "ContrastiveTrainer.call() is not implemented - "
             "please call your model directly."
         )
 
     @staticmethod
     def linear_probe(num_classes, **kwargs):
         return keras.Sequential(keras.layers.Dense(num_classes), **kwargs)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/training/contrastive/simclr_trainer.py` & `keras_cv-0.9.0.dev0/keras_cv/src/training/contrastive/simclr_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,8 +87,7 @@
                         hue_factor=hue_factor,
                     ),
                     rate=color_jitter_rate,
                 ),
             ],
             **kwargs,
         )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/utils/__init__.py` & `keras_cv-0.9.0.dev0/keras_cv/src/utils/__init__.py`

 * *Files identical despite different names*

```diff
@@ -23,8 +23,7 @@
 from keras_cv.src.utils.preprocessing import get_interpolation
 from keras_cv.src.utils.preprocessing import parse_factor
 from keras_cv.src.utils.preprocessing import transform
 from keras_cv.src.utils.preprocessing import transform_value_range
 from keras_cv.src.utils.to_numpy import to_numpy
 from keras_cv.src.utils.train import convert_inputs_to_tf_dataset
 from keras_cv.src.utils.train import scale_loss_for_distribution
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/utils/conditional_imports.py` & `keras_cv-0.9.0.dev0/keras_cv/src/utils/conditional_imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,7 @@
 def assert_pycocotools_installed(symbol_name):
     if pycocotools is None:
         raise ImportError(
             f"{symbol_name} requires the `pycocotools` package. "
             "Please install the package using "
             "`pip install pycocotools`."
         )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/utils/conv_utils.py` & `keras_cv-0.9.0.dev0/keras_cv/src/utils/conv_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,8 +65,7 @@
         error_msg += (
             f" including {unqualified_values}"
             f" that does not satisfy the requirement `{req_msg}`."
         )
         raise ValueError(error_msg)
 
     return value_tuple
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/utils/fill_utils.py` & `keras_cv-0.9.0.dev0/keras_cv/src/utils/fill_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,8 +79,7 @@
     )
     mask_shape = (images_width, images_height)
     is_rectangle = corners_to_mask(corners, mask_shape)
     is_rectangle = tf.expand_dims(is_rectangle, -1)
 
     images = tf.where(is_rectangle, fill_values, images)
     return images
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/utils/preprocessing.py` & `keras_cv-0.9.0.dev0/keras_cv/src/utils/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         original_range: the value range to transform from.
         target_range: the value range to transform to.
         dtype: the dtype to compute the conversion with, defaults to tf.float32.
 
     Returns:
         a new Tensor with values in the target range.
 
-    Usage:
+    Example:
     ```python
     original_range = [0, 1]
     target_range = [0, 255]
     images = keras_cv.utils.preprocessing.transform_value_range(
         images,
         original_range,
         target_range
@@ -389,8 +389,7 @@
             "`constant` or `nearest`. Got `fill_mode` {}. ".format(fill_mode)
         )
     if interpolation not in {"nearest", "bilinear"}:
         raise NotImplementedError(
             "Unknown `interpolation` {}. Only `nearest` and "
             "`bilinear` are supported.".format(interpolation)
         )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/utils/preset_utils.py` & `keras_cv-0.9.0.dev0/keras_cv/src/utils/preset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,8 +212,7 @@
     for cls in inspect.getmro(layer.__class__):
         if cls.__name__ == "Functional":
             functional_cls = cls
     property = functional_cls._layer_checkpoint_dependencies
     functional_cls._layer_checkpoint_dependencies = {}
     layer.load_weights(weights_path)
     functional_cls._layer_checkpoint_dependencies = property
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/utils/python_utils.py` & `keras_cv-0.9.0.dev0/keras_cv/src/utils/python_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,7 @@
         # to swap all double and single brackets in the source docstring.
         doc = "{".join(part.replace("{", "{{") for part in doc.split("{{"))
         doc = "}".join(part.replace("}", "}}") for part in doc.split("}}"))
         obj.__doc__ = doc.format(**replacements)
         return obj
 
     return decorate
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/utils/resource_loader.py` & `keras_cv-0.9.0.dev0/keras_cv/src/utils/resource_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,8 +78,7 @@
             UserWarning,
         )
         abi_warning_already_raised = True
 
 
 def abi_is_compatible():
     return tf.__version__.startswith(TF_VERSION_FOR_ABI_COMPATIBILITY)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/utils/target_gather.py` & `keras_cv-0.9.0.dev0/keras_cv/src/utils/target_gather.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,8 +113,7 @@
                 ) * ops.ones_like(mask, dtype=labels.dtype)
                 return ops.where(mask, masked_targets, targets)
 
     if len(targets_shape) <= 2:
         return _gather_unbatched(targets, indices, mask, mask_val)
     elif len(targets_shape) == 3:
         return _gather_batched(targets, indices, mask, mask_val)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/utils/test_utils.py` & `keras_cv-0.9.0.dev0/keras_cv/src/utils/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,8 +89,7 @@
 
     # Iterate over all keys of the configs and compare each entry exhaustively.
     for key in list(config1.keys()):
         v1, v2 = config1[key], config2[key]
         if not exhaustive_compare(v1, v2):
             return False
     return True
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/utils/to_numpy.py` & `keras_cv-0.9.0.dev0/keras_cv/src/utils/to_numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,7 @@
     if x is None:
         return None
     if isinstance(x, tf.RaggedTensor):
         x = x.to_tensor(-1)
     x = ops.convert_to_numpy(x)
     # Important for consistency when working with visualization utilities
     return np.ascontiguousarray(x)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/utils/train.py` & `keras_cv-0.9.0.dev0/keras_cv/src/utils/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,8 +76,7 @@
     """
 
     if not output_keys:
         output_keys = layer_names
     items = zip(output_keys, layer_names)
     outputs = {key: model.get_layer(name).output for key, name in items}
     return keras.Model(inputs=model.inputs, outputs=outputs)
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/version_check.py` & `keras_cv-0.9.0.dev0/keras_cv/src/version_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,7 @@
         raise RuntimeError(
             "The Tensorflow package version needs to be at least "
             f"{MIN_VERSION} for KerasCV to run. Currently, your TensorFlow "
             f"version is {tf.__version__}. Please upgrade with `$ pip install "
             "--upgrade tensorflow`. You can use `pip freeze` to check "
             "afterwards that everything is ok."
         )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/version_utils.py` & `keras_cv-0.9.0.dev0/keras_cv/src/version_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,13 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from keras_cv.src.api_export import keras_cv_export
 
 # Unique source of truth for the version number.
-__version__ = "0.8.2"
+__version__ = "0.9.0.dev0"
 
 
 @keras_cv_export("keras_cv.version")
 def version():
     return __version__
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/visualization/draw_bounding_boxes.py` & `keras_cv-0.9.0.dev0/keras_cv/src/visualization/draw_bounding_boxes.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,8 +150,7 @@
     line_offset = line_thickness + outline_factor
     static_offset = 3
 
     return (
         x + outline_factor + static_offset,
         y + (2 * font_height) + line_offset + static_offset,
     )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/visualization/plot_bounding_box_gallery.py` & `keras_cv-0.9.0.dev0/keras_cv/src/visualization/plot_bounding_box_gallery.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     legend_handles=None,
     rows=3,
     cols=3,
     **kwargs
 ):
     """Plots a gallery of images with corresponding bounding box annotations.
 
-    Usage:
+    Example:
     ```python
     train_ds = tfds.load(
         "voc/2007", split="train", with_info=False, shuffle_files=True
     )
 
     def unpackage_tfds_inputs(inputs):
         image = inputs["image"]
@@ -178,8 +178,7 @@
         plotted_images,
         value_range,
         legend_handles=legend_handles,
         rows=rows,
         cols=cols,
         **kwargs
     )
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/visualization/plot_image_gallery.py` & `keras_cv-0.9.0.dev0/keras_cv/src/visualization/plot_image_gallery.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     show=None,
     transparent=True,
     dpi=60,
     legend_handles=None,
 ):
     """Displays a gallery of images.
 
-    Usage:
+    Example:
     ```python
     train_ds = tfds.load(
         "cats_vs_dogs",
         split="train",
         with_info=False,
         shuffle_files=True,
     )
@@ -186,8 +186,7 @@
             transparent=transparent,
             dpi=dpi,
         )
         plt.close()
     elif show:
         plt.show()
         plt.close()
-
```

### Comparing `keras-cv-0.8.2/keras_cv/src/visualization/plot_segmentation_mask_gallery.py` & `keras_cv-0.9.0.dev0/keras_cv/src/visualization/plot_segmentation_mask_gallery.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             batched.
         y_pred: (Optional)  a Tensor or NumPy array representing the predicted
             segmentation masks. The predicted segmentation masks should be
             batched.
         kwargs: keyword arguments to propagate to
             `keras_cv.visualization.plot_image_gallery()`.
 
-    Usage:
+    Example:
     ```python
     train_ds = tfds.load(
         "oxford_iiit_pet", split="train", with_info=False, shuffle_files=True
     )
 
     def unpackage_tfds_inputs(inputs):
         image = inputs["image"]
@@ -132,8 +132,7 @@
 
     # Concatenate the images and the masks together.
     plotted_images = np.concatenate(masks_to_contatenate, axis=2)
 
     plot_image_gallery(
         plotted_images, value_range, rows=rows, cols=cols, **kwargs
     )
-
```

### Comparing `keras-cv-0.8.2/keras_cv.egg-info/PKG-INFO` & `keras_cv-0.9.0.dev0/keras_cv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-cv
-Version: 0.8.2
+Version: 0.9.0.dev0
 Summary: Industry-strength computer Vision extensions for Keras.
 Home-page: https://github.com/keras-team/keras-cv
 Author: Keras team
 Author-email: keras-cv@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-cv-0.8.2/keras_cv.egg-info/SOURCES.txt` & `keras_cv-0.9.0.dev0/keras_cv.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,41 +3,43 @@
 setup.py
 keras_cv/__init__.py
 keras_cv.egg-info/PKG-INFO
 keras_cv.egg-info/SOURCES.txt
 keras_cv.egg-info/dependency_links.txt
 keras_cv.egg-info/requires.txt
 keras_cv.egg-info/top_level.txt
-keras_cv/bounding_box/__init__.py
-keras_cv/callbacks/__init__.py
-keras_cv/core/__init__.py
-keras_cv/datasets/__init__.py
-keras_cv/datasets/imagenet/__init__.py
-keras_cv/datasets/pascal_voc/__init__.py
-keras_cv/datasets/pascal_voc/segmentation/__init__.py
-keras_cv/datasets/waymo/__init__.py
-keras_cv/keypoint/__init__.py
-keras_cv/layers/__init__.py
-keras_cv/losses/__init__.py
-keras_cv/metrics/__init__.py
-keras_cv/models/__init__.py
-keras_cv/models/classification/__init__.py
-keras_cv/models/object_detection/__init__.py
-keras_cv/models/retinanet/__init__.py
-keras_cv/models/segmentation/__init__.py
-keras_cv/models/stable_diffusion/__init__.py
-keras_cv/models/yolov8/__init__.py
+keras_cv/api/__init__.py
+keras_cv/api/bounding_box/__init__.py
+keras_cv/api/callbacks/__init__.py
+keras_cv/api/core/__init__.py
+keras_cv/api/datasets/__init__.py
+keras_cv/api/datasets/imagenet/__init__.py
+keras_cv/api/datasets/pascal_voc/__init__.py
+keras_cv/api/datasets/pascal_voc/segmentation/__init__.py
+keras_cv/api/datasets/waymo/__init__.py
+keras_cv/api/keypoint/__init__.py
+keras_cv/api/layers/__init__.py
+keras_cv/api/losses/__init__.py
+keras_cv/api/metrics/__init__.py
+keras_cv/api/models/__init__.py
+keras_cv/api/models/classification/__init__.py
+keras_cv/api/models/feature_extractor/__init__.py
+keras_cv/api/models/object_detection/__init__.py
+keras_cv/api/models/retinanet/__init__.py
+keras_cv/api/models/segmentation/__init__.py
+keras_cv/api/models/stable_diffusion/__init__.py
+keras_cv/api/models/yolov8/__init__.py
+keras_cv/api/visualization/__init__.py
 keras_cv/src/__init__.py
 keras_cv/src/api_export.py
-keras_cv/src/conftest.py
 keras_cv/src/version_check.py
 keras_cv/src/version_utils.py
 keras_cv/src/backend/__init__.py
 keras_cv/src/backend/config.py
-keras_cv/src/backend/keras.py
+keras_cv/src/backend/keras2.py
 keras_cv/src/backend/ops.py
 keras_cv/src/backend/random.py
 keras_cv/src/backend/scope.py
 keras_cv/src/backend/tf_ops.py
 keras_cv/src/bounding_box/__init__.py
 keras_cv/src/bounding_box/converters.py
 keras_cv/src/bounding_box/ensure_tensor.py
@@ -217,21 +219,40 @@
 keras_cv/src/models/backbones/resnet_v1/resnet_v1_aliases.py
 keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone.py
 keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone_presets.py
 keras_cv/src/models/backbones/resnet_v2/__init__.py
 keras_cv/src/models/backbones/resnet_v2/resnet_v2_aliases.py
 keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone.py
 keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone_presets.py
+keras_cv/src/models/backbones/vgg16/__init__.py
+keras_cv/src/models/backbones/vgg16/vgg16_backbone.py
+keras_cv/src/models/backbones/video_swin/__init__.py
+keras_cv/src/models/backbones/video_swin/video_swin_aliases.py
+keras_cv/src/models/backbones/video_swin/video_swin_backbone.py
+keras_cv/src/models/backbones/video_swin/video_swin_backbone_presets.py
+keras_cv/src/models/backbones/video_swin/video_swin_layers.py
 keras_cv/src/models/backbones/vit_det/__init__.py
 keras_cv/src/models/backbones/vit_det/vit_det_aliases.py
 keras_cv/src/models/backbones/vit_det/vit_det_backbone.py
 keras_cv/src/models/backbones/vit_det/vit_det_backbone_presets.py
 keras_cv/src/models/classification/__init__.py
 keras_cv/src/models/classification/image_classifier.py
 keras_cv/src/models/classification/image_classifier_presets.py
+keras_cv/src/models/classification/video_classifier.py
+keras_cv/src/models/classification/video_classifier_presets.py
+keras_cv/src/models/feature_extractor/__init__.py
+keras_cv/src/models/feature_extractor/clip/__init__.py
+keras_cv/src/models/feature_extractor/clip/clip_encoder.py
+keras_cv/src/models/feature_extractor/clip/clip_image_model.py
+keras_cv/src/models/feature_extractor/clip/clip_model.py
+keras_cv/src/models/feature_extractor/clip/clip_presets.py
+keras_cv/src/models/feature_extractor/clip/clip_processor.py
+keras_cv/src/models/feature_extractor/clip/clip_processor_utils.py
+keras_cv/src/models/feature_extractor/clip/clip_text_model.py
+keras_cv/src/models/feature_extractor/clip/clip_tokenizer.py
 keras_cv/src/models/legacy/__init__.py
 keras_cv/src/models/legacy/convmixer.py
 keras_cv/src/models/legacy/convnext.py
 keras_cv/src/models/legacy/darknet.py
 keras_cv/src/models/legacy/mlp_mixer.py
 keras_cv/src/models/legacy/regnet.py
 keras_cv/src/models/legacy/utils.py
@@ -321,9 +342,8 @@
 keras_cv/src/utils/test_utils.py
 keras_cv/src/utils/to_numpy.py
 keras_cv/src/utils/train.py
 keras_cv/src/visualization/__init__.py
 keras_cv/src/visualization/draw_bounding_boxes.py
 keras_cv/src/visualization/plot_bounding_box_gallery.py
 keras_cv/src/visualization/plot_image_gallery.py
-keras_cv/src/visualization/plot_segmentation_mask_gallery.py
-keras_cv/visualization/__init__.py
+keras_cv/src/visualization/plot_segmentation_mask_gallery.py
```

### Comparing `keras-cv-0.8.2/setup.cfg` & `keras_cv-0.9.0.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.2/setup.py` & `keras_cv-0.9.0.dev0/setup.py`

 * *Files identical despite different names*

