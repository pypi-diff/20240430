# Comparing `tmp/keras-cv-0.8.1.dev0.tar.gz` & `tmp/keras-cv-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-cv-0.8.1.dev0.tar", last modified: Mon Jan  8 21:25:20 2024, max compression
+gzip compressed data, was "keras-cv-0.8.2.tar", last modified: Thu Feb  1 00:08:44 2024, max compression
```

## Comparing `keras-cv-0.8.1.dev0.tar` & `keras-cv-0.8.2.tar`

### file list

```diff
@@ -1,407 +1,412 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.609145 keras-cv-0.8.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-01-08 21:25:20.609145 keras-cv-0.8.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.557145 keras-cv-0.8.1.dev0/keras_cv/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.557145 keras-cv-0.8.1.dev0/keras_cv/bounding_box/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/bounding_box/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/core/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/datasets/imagenet/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/datasets/imagenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/datasets/pascal_voc/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/datasets/pascal_voc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/datasets/pascal_voc/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/datasets/pascal_voc/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/datasets/waymo/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/datasets/waymo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/keypoint/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/keypoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/models/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/models/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/models/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/models/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/models/retinanet/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/models/retinanet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/models/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/models/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/models/stable_diffusion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/models/yolov8/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/models/yolov8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.561145 keras-cv-0.8.1.dev0/keras_cv/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.565145 keras-cv-0.8.1.dev0/keras_cv/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/backend/keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/backend/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/backend/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/backend/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/backend/tf_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.565145 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/ensure_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/mask_invalid_detections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/to_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/to_ragged.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/validate_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.565145 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box_3d/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/bounding_box_3d/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.565145 keras-cv-0.8.1.dev0/keras_cv/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/callbacks/pycoco_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/callbacks/waymo_evaluation_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.565145 keras-cv-0.8.1.dev0/keras_cv/src/core/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.569145 keras-cv-0.8.1.dev0/keras_cv/src/core/factor_sampler/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/core/factor_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/core/factor_sampler/constant_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/core/factor_sampler/factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/core/factor_sampler/normal_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/core/factor_sampler/uniform_factor_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.569145 keras-cv-0.8.1.dev0/keras_cv/src/custom_ops/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/custom_ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.569145 keras-cv-0.8.1.dev0/keras_cv/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.569145 keras-cv-0.8.1.dev0/keras_cv/src/datasets/imagenet/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/datasets/imagenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/datasets/imagenet/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.569145 keras-cv-0.8.1.dev0/keras_cv/src/datasets/pascal_voc/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/datasets/pascal_voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/datasets/pascal_voc/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    18974 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/datasets/pascal_voc/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.569145 keras-cv-0.8.1.dev0/keras_cv/src/datasets/waymo/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/datasets/waymo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/datasets/waymo/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/datasets/waymo/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    27677 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/datasets/waymo/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.569145 keras-cv-0.8.1.dev0/keras_cv/src/keypoint/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/keypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/keypoint/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/keypoint/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/keypoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.573145 keras-cv-0.8.1.dev0/keras_cv/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/feature_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/fusedmbconv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/hierarchical_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/mbconv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.573145 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/anchor_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/multi_class_non_max_suppression.py
--rw-r--r--   0 runner    (1001) docker     (127)    21214 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/non_max_suppression.py
--rw-r--r--   0 runner    (1001) docker     (127)    16294 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/roi_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/roi_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/rpn_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.577145 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection_3d/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16712 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection_3d/centernet_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection_3d/heatmap_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection_3d/voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection_3d/voxelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/overlapping_patching_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.581145 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/aug_mix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/auto_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)    22944 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/base_image_augmentation_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/channel_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/cut_mix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/fourier_mix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/grayscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/grid_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/jittered_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/mix_up.py
--rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/posterization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/rand_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_aspect_ratio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_augmentation_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_channel_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_color_degeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_crop_and_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_cutout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_gaussian_blur.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_hue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_jpeg_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)    12287 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_saturation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_sharpness.py
--rw-r--r--   0 runner    (1001) docker     (127)    14063 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_shear.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/repeated_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    15385 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/solarization.py
--rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/vectorized_base_image_augmentation_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.581145 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/base_augmentation_layer_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.585145 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_dropping_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_point_feature_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_dropping_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11154 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/group_points_by_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12343 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/random_copy_paste.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/random_drop_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/swap_background.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.585145 keras-cv-0.8.1.dev0/keras_cv/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/regularization/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/regularization/dropblock_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/regularization/squeeze_excite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/regularization/stochastic_depth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/segformer_multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/spatial_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/vit_det_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/layers/vit_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.585145 keras-cv-0.8.1.dev0/keras_cv/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/losses/centernet_box_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/losses/ciou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/losses/focal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/losses/iou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/losses/penalty_reduced_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/losses/simclr_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/losses/smooth_l1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.585145 keras-cv-0.8.1.dev0/keras_cv/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.585145 keras-cv-0.8.1.dev0/keras_cv/src/metrics/coco/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/metrics/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/metrics/coco/pycoco_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.585145 keras-cv-0.8.1.dev0/keras_cv/src/metrics/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/metrics/object_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/metrics/object_detection/box_coco_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.585145 keras-cv-0.8.1.dev0/keras_cv/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.585145 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.589145 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/csp_darknet/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/csp_darknet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.589145 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/densenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/densenet/densenet_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/densenet/densenet_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/densenet/densenet_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.589145 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.589145 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v1/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.589145 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.589145 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mix_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mix_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mix_transformer/mix_transformer_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.589145 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mobilenet_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.593145 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v1/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v1/resnet_v1_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.593145 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v2/resnet_v2_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    13222 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/test_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.593145 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/vit_det/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/vit_det/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/vit_det/vit_det_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/vit_det/vit_det_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/vit_det/vit_det_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.593145 keras-cv-0.8.1.dev0/keras_cv/src/models/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/classification/image_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/classification/image_classifier_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.593145 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14449 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/convmixer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20273 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/darknet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14410 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/mlp_mixer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.593145 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.593145 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/object_detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/object_detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23894 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/object_detection/faster_rcnn/faster_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    45780 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/regnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    26176 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.597145 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/__internal__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.597145 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/retinanet/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/retinanet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/retinanet/feature_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/retinanet/prediction_head.py
--rw-r--r--   0 runner    (1001) docker     (127)    23044 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/retinanet/retinanet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10678 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/retinanet/retinanet_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/retinanet/retinanet_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.597145 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    24552 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.597145 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/binary_crossentropy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.597145 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_pafpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.601145 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection_3d/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection_3d/center_pillar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection_3d/center_pillar_backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection_3d/center_pillar_backbone_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.601145 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.601145 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.601145 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segformer/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segformer/segformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segformer/segformer_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segformer/segformer_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.601145 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/sam_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/sam_mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/sam_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/sam_prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/sam_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.605145 keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/attention_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/clip_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/diffusion_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/noise_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/padded_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/resnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    20023 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/text_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.605145 keras-cv-0.8.1.dev0/keras_cv/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/ops/iou_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.605145 keras-cv-0.8.1.dev0/keras_cv/src/point_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/point_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18300 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/point_cloud/point_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.605145 keras-cv-0.8.1.dev0/keras_cv/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/tests/test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.605145 keras-cv-0.8.1.dev0/keras_cv/src/training/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.605145 keras-cv-0.8.1.dev0/keras_cv/src/training/contrastive/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/training/contrastive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/training/contrastive/contrastive_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/training/contrastive/simclr_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.609145 keras-cv-0.8.1.dev0/keras_cv/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/utils/conditional_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/utils/conv_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/utils/fill_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14437 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/utils/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/utils/preset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/utils/resource_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/utils/target_gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/utils/to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-01-08 21:25:09.000000 keras-cv-0.8.1.dev0/keras_cv/src/utils/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/version_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.609145 keras-cv-0.8.1.dev0/keras_cv/src/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/visualization/draw_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/visualization/plot_bounding_box_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/visualization/plot_image_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/keras_cv/src/visualization/plot_segmentation_mask_gallery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.609145 keras-cv-0.8.1.dev0/keras_cv/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-01-08 21:25:15.000000 keras-cv-0.8.1.dev0/keras_cv/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 21:25:20.609145 keras-cv-0.8.1.dev0/keras_cv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-01-08 21:25:20.000000 keras-cv-0.8.1.dev0/keras_cv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16191 2024-01-08 21:25:20.000000 keras-cv-0.8.1.dev0/keras_cv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 21:25:20.000000 keras-cv-0.8.1.dev0/keras_cv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-08 21:25:20.000000 keras-cv-0.8.1.dev0/keras_cv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-08 21:25:20.000000 keras-cv-0.8.1.dev0/keras_cv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-01-08 21:25:20.613145 keras-cv-0.8.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-01-08 21:25:08.000000 keras-cv-0.8.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.909271 keras-cv-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-02-01 00:08:44.909271 keras-cv-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-02-01 00:08:33.000000 keras-cv-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.849270 keras-cv-0.8.2/keras_cv/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.849270 keras-cv-0.8.2/keras_cv/bounding_box/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/bounding_box/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/datasets/imagenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/datasets/imagenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/datasets/pascal_voc/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/datasets/pascal_voc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/datasets/pascal_voc/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/datasets/pascal_voc/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/datasets/waymo/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/datasets/waymo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/keypoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/keypoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/retinanet/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/retinanet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/stable_diffusion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.853270 keras-cv-0.8.2/keras_cv/models/yolov8/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/models/yolov8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.857270 keras-cv-0.8.2/keras_cv/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.857270 keras-cv-0.8.2/keras_cv/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/backend/tf_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.857270 keras-cv-0.8.2/keras_cv/src/bounding_box/
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/ensure_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/mask_invalid_detections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/to_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/to_ragged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box/validate_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.857270 keras-cv-0.8.2/keras_cv/src/bounding_box_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/bounding_box_3d/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/callbacks/pycoco_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/callbacks/waymo_evaluation_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/core/factor_sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/core/factor_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/core/factor_sampler/constant_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/core/factor_sampler/factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/core/factor_sampler/normal_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/core/factor_sampler/uniform_factor_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/custom_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/custom_ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/datasets/imagenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/imagenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/imagenet/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18975 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/datasets/waymo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/waymo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/waymo/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/waymo/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27677 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/datasets/waymo/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.861270 keras-cv-0.8.2/keras_cv/src/keypoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/keypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/keypoint/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/keypoint/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/keypoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.865270 keras-cv-0.8.2/keras_cv/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/feature_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/fusedmbconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/hierarchical_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/mbconv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.869270 keras-cv-0.8.2/keras_cv/src/layers/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/anchor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/multi_class_non_max_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21214 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/non_max_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16294 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/rpn_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.869270 keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16712 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/centernet_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/heatmap_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/voxelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/overlapping_patching_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.877270 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/aug_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/auto_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22948 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/base_image_augmentation_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/channel_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/cut_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/fourier_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/grid_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/jittered_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/mix_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/posterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/rand_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_aspect_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_augmentation_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_channel_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_color_degeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_crop_and_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_gaussian_blur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_hue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_jpeg_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12287 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_sharpness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14063 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_shear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/repeated_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15385 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/solarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22644 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing/vectorized_base_image_augmentation_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.877270 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/base_augmentation_layer_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.877270 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_dropping_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_point_feature_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_dropping_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11154 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/group_points_by_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12343 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/random_copy_paste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/random_drop_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/swap_background.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/regularization/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/regularization/dropblock_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/regularization/squeeze_excite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/regularization/stochastic_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/segformer_multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/spatial_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20736 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/vit_det_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/layers/vit_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/centernet_box_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/ciou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/focal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/penalty_reduced_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/simclr_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/losses/smooth_l1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/metrics/coco/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/metrics/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/metrics/coco/pycoco_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/metrics/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/metrics/object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/metrics/object_detection/box_coco_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.881271 keras-cv-0.8.2/keras_cv/src/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.885270 keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.885270 keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/densenet_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/densenet_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/densenet_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.885270 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.885270 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.885270 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.889271 keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/mix_transformer_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.889271 keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.889271 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/resnet_v1_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.889271 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/resnet_v2_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/test_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.889271 keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/vit_det_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/vit_det_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/vit_det_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.889271 keras-cv-0.8.2/keras_cv/src/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/classification/image_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/classification/image_classifier_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.893271 keras-cv-0.8.2/keras_cv/src/models/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14449 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/convmixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20273 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11070 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/darknet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/mlp_mixer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.893271 keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.893271 keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23894 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/faster_rcnn/faster_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45780 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/regnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26176 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/legacy/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.893271 keras-cv-0.8.2/keras_cv/src/models/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/__internal__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.893271 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/feature_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/prediction_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23044 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10678 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/retinanet_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/retinanet_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.897271 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24653 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.897271 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/binary_crossentropy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.897271 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_pafpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.897271 keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/center_pillar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/center_pillar_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/center_pillar_backbone_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.897271 keras-cv-0.8.2/keras_cv/src/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.897271 keras-cv-0.8.2/keras_cv/src/models/segmentation/basnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/basnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/basnet/basnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/basnet/basnet_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.901271 keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.901271 keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/segformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/segformer_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/segformer_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.901271 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.905271 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/clip_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/diffusion_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/noise_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/padded_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/resnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.905271 keras-cv-0.8.2/keras_cv/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/ops/iou_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.905271 keras-cv-0.8.2/keras_cv/src/point_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/point_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18300 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/point_cloud/point_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.905271 keras-cv-0.8.2/keras_cv/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/tests/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.905271 keras-cv-0.8.2/keras_cv/src/training/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.905271 keras-cv-0.8.2/keras_cv/src/training/contrastive/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/training/contrastive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/training/contrastive/contrastive_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/training/contrastive/simclr_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.909271 keras-cv-0.8.2/keras_cv/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/conditional_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/conv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/fill_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14437 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/preset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/resource_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/target_gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/utils/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/version_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/src/version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.909271 keras-cv-0.8.2/keras_cv/src/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/visualization/draw_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/visualization/plot_bounding_box_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/visualization/plot_image_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-02-01 00:08:33.000000 keras-cv-0.8.2/keras_cv/src/visualization/plot_segmentation_mask_gallery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.909271 keras-cv-0.8.2/keras_cv/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-01 00:08:39.000000 keras-cv-0.8.2/keras_cv/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 00:08:44.909271 keras-cv-0.8.2/keras_cv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-02-01 00:08:44.000000 keras-cv-0.8.2/keras_cv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16381 2024-02-01 00:08:44.000000 keras-cv-0.8.2/keras_cv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 00:08:44.000000 keras-cv-0.8.2/keras_cv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-01 00:08:44.000000 keras-cv-0.8.2/keras_cv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-01 00:08:44.000000 keras-cv-0.8.2/keras_cv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-02-01 00:08:44.909271 keras-cv-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-02-01 00:08:33.000000 keras-cv-0.8.2/setup.py
```

### Comparing `keras-cv-0.8.1.dev0/PKG-INFO` & `keras-cv-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-cv
-Version: 0.8.1.dev0
+Version: 0.8.2
 Summary: Industry-strength computer Vision extensions for Keras.
 Home-page: https://github.com/keras-team/keras-cv
 Author: Keras team
 Author-email: keras-cv@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-cv-0.8.1.dev0/README.md` & `keras-cv-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/bounding_box/__init__.py` & `keras-cv-0.8.2/keras_cv/bounding_box/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/datasets/waymo/__init__.py` & `keras-cv-0.8.2/keras_cv/datasets/waymo/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/layers/__init__.py` & `keras-cv-0.8.2/keras_cv/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/losses/__init__.py` & `keras-cv-0.8.2/keras_cv/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/models/__init__.py` & `keras-cv-0.8.2/keras_cv/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from keras_cv.src.models.backbones.vit_det.vit_det_backbone import ViTDetBackbone
 from keras_cv.src.models.classification.image_classifier import ImageClassifier
 from keras_cv.src.models.object_detection.retinanet.retinanet import RetinaNet
 from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_backbone import YOLOV8Backbone
 from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_detector import YOLOV8Detector
 from keras_cv.src.models.object_detection_3d.center_pillar import MultiHeadCenterPillar
 from keras_cv.src.models.object_detection_3d.center_pillar_backbone import CenterPillarBackbone
+from keras_cv.src.models.segmentation.basnet.basnet import BASNet
 from keras_cv.src.models.segmentation.deeplab_v3_plus.deeplab_v3_plus import DeepLabV3Plus
 from keras_cv.src.models.segmentation.segformer.segformer import SegFormer
 from keras_cv.src.models.segmentation.segment_anything.sam import SegmentAnythingModel
 from keras_cv.src.models.segmentation.segment_anything.sam_mask_decoder import SAMMaskDecoder
 from keras_cv.src.models.segmentation.segment_anything.sam_prompt_encoder import SAMPromptEncoder
 from keras_cv.src.models.segmentation.segment_anything.sam_transformer import TwoWayTransformer
 from keras_cv.src.models.stable_diffusion.stable_diffusion import StableDiffusion
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/models/stable_diffusion/__init__.py` & `keras-cv-0.8.2/keras_cv/models/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/__init__.py` & `keras-cv-0.8.2/keras_cv/src/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,10 +37,10 @@
 from keras_cv.src import training
 from keras_cv.src import utils
 from keras_cv.src import visualization
 from keras_cv.src.core import ConstantFactorSampler
 from keras_cv.src.core import FactorSampler
 from keras_cv.src.core import NormalFactorSampler
 from keras_cv.src.core import UniformFactorSampler
-
-__version__ = "0.8.1.dev0"
+from keras_cv.src.version_utils import __version__
+from keras_cv.src.version_utils import version
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/api_export.py` & `keras-cv-0.8.2/keras_cv/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/backend/__init__.py` & `keras-cv-0.8.2/keras_cv/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/backend/config.py` & `keras-cv-0.8.2/keras_cv/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/backend/keras.py` & `keras-cv-0.8.2/keras_cv/src/backend/keras.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/backend/ops.py` & `keras-cv-0.8.2/keras_cv/src/backend/ops.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/backend/random.py` & `keras-cv-0.8.2/keras_cv/src/backend/random.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/backend/scope.py` & `keras-cv-0.8.2/keras_cv/src/backend/scope.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/backend/tf_ops.py` & `keras-cv-0.8.2/keras_cv/src/backend/tf_ops.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/__init__.py` & `keras-cv-0.8.2/keras_cv/src/bounding_box/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/converters.py` & `keras-cv-0.8.2/keras_cv/src/bounding_box/converters.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/ensure_tensor.py` & `keras-cv-0.8.2/keras_cv/src/bounding_box/ensure_tensor.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/formats.py` & `keras-cv-0.8.2/keras_cv/src/bounding_box/formats.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/iou.py` & `keras-cv-0.8.2/keras_cv/src/bounding_box/iou.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/mask_invalid_detections.py` & `keras-cv-0.8.2/keras_cv/src/bounding_box/mask_invalid_detections.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/to_dense.py` & `keras-cv-0.8.2/keras_cv/src/bounding_box/to_dense.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/to_ragged.py` & `keras-cv-0.8.2/keras_cv/src/bounding_box/to_ragged.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/utils.py` & `keras-cv-0.8.2/keras_cv/src/bounding_box/utils.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/bounding_box/validate_format.py` & `keras-cv-0.8.2/keras_cv/src/bounding_box/validate_format.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/bounding_box_3d/__init__.py` & `keras-cv-0.8.2/keras_cv/src/bounding_box_3d/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/bounding_box_3d/formats.py` & `keras-cv-0.8.2/keras_cv/src/bounding_box_3d/formats.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/callbacks/__init__.py` & `keras-cv-0.8.2/keras_cv/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/callbacks/pycoco_callback.py` & `keras-cv-0.8.2/keras_cv/src/callbacks/pycoco_callback.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/callbacks/waymo_evaluation_callback.py` & `keras-cv-0.8.2/keras_cv/src/callbacks/waymo_evaluation_callback.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/conftest.py` & `keras-cv-0.8.2/keras_cv/src/conftest.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/core/__init__.py` & `keras-cv-0.8.2/keras_cv/src/core/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/core/factor_sampler/__init__.py` & `keras-cv-0.8.2/keras_cv/src/core/factor_sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/core/factor_sampler/constant_factor_sampler.py` & `keras-cv-0.8.2/keras_cv/src/core/factor_sampler/constant_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/core/factor_sampler/factor_sampler.py` & `keras-cv-0.8.2/keras_cv/src/core/factor_sampler/factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/core/factor_sampler/normal_factor_sampler.py` & `keras-cv-0.8.2/keras_cv/src/core/factor_sampler/normal_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/core/factor_sampler/uniform_factor_sampler.py` & `keras-cv-0.8.2/keras_cv/src/core/factor_sampler/uniform_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/custom_ops/__init__.py` & `keras-cv-0.8.2/keras_cv/src/custom_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/datasets/__init__.py` & `keras-cv-0.8.2/keras_cv/src/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/datasets/imagenet/__init__.py` & `keras-cv-0.8.2/keras_cv/src/datasets/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/datasets/imagenet/load.py` & `keras-cv-0.8.2/keras_cv/src/datasets/imagenet/load.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/datasets/pascal_voc/__init__.py` & `keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/datasets/pascal_voc/load.py` & `keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/load.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/datasets/pascal_voc/segmentation.py` & `keras-cv-0.8.2/keras_cv/src/datasets/pascal_voc/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 """
 @InProceedings{{BharathICCV2011,
     author = "Bharath Hariharan and Pablo Arbelaez and Lubomir Bourdev and Subhransu Maji and Jitendra Malik",
     title = "Semantic Contours from Inverse Detectors",
     booktitle = "International Conference on Computer Vision (ICCV)",
     year = "2011"}}
 """  # noqa: E501
-SBD_URL = "https://www.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/semantic_contours/benchmark.tgz"  # noqa: E501
+SBD_URL = "https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/semantic_contours/benchmark.tgz"  # noqa: E501
 
 
 # Note that this list doesn't contain the background class. In the
 # classification use case, the label is 0 based (aeroplane -> 0), whereas in
 # segmentation use case, the 0 is reserved for background, so aeroplane maps to
 # 1.
 CLASSES = [
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/datasets/waymo/__init__.py` & `keras-cv-0.8.2/keras_cv/src/datasets/waymo/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/datasets/waymo/load.py` & `keras-cv-0.8.2/keras_cv/src/datasets/waymo/load.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/datasets/waymo/struct.py` & `keras-cv-0.8.2/keras_cv/src/datasets/waymo/struct.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/datasets/waymo/transformer.py` & `keras-cv-0.8.2/keras_cv/src/datasets/waymo/transformer.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/keypoint/__init__.py` & `keras-cv-0.8.2/keras_cv/src/keypoint/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/keypoint/converters.py` & `keras-cv-0.8.2/keras_cv/src/keypoint/converters.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/keypoint/formats.py` & `keras-cv-0.8.2/keras_cv/src/keypoint/formats.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/keypoint/utils.py` & `keras-cv-0.8.2/keras_cv/src/keypoint/utils.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/__init__.py` & `keras-cv-0.8.2/keras_cv/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/augmenter.py` & `keras-cv-0.8.2/keras_cv/src/layers/augmenter.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/feature_pyramid.py` & `keras-cv-0.8.2/keras_cv/src/layers/feature_pyramid.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/fusedmbconv.py` & `keras-cv-0.8.2/keras_cv/src/layers/fusedmbconv.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/hierarchical_transformer_encoder.py` & `keras-cv-0.8.2/keras_cv/src/layers/hierarchical_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/mbconv.py` & `keras-cv-0.8.2/keras_cv/src/layers/mbconv.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/__init__.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/anchor_generator.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection/anchor_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
         if image is not None:
             if len(image.shape) != 3:
                 raise ValueError(
                     "Expected `image` to be a Tensor of rank 3. Got "
                     f"image.shape.rank={len(image.shape)}"
                 )
-            image_shape = image.shape
+            image_shape = tuple(image.shape)
 
         results = {}
         for key, generator in self.anchor_generators.items():
             results[key] = bounding_box.convert_format(
                 generator(image_shape),
                 source="yxyx",
                 target=self.bounding_box_format,
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/box_matcher.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection/box_matcher.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/multi_class_non_max_suppression.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection/multi_class_non_max_suppression.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/non_max_suppression.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection/non_max_suppression.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/roi_align.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_align.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/roi_generator.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_generator.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/roi_pool.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_pool.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/roi_sampler.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection/roi_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/rpn_label_encoder.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection/rpn_label_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection/sampling.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection/sampling.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection_3d/__init__.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection_3d/centernet_label_encoder.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/centernet_label_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection_3d/heatmap_decoder.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/heatmap_decoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection_3d/voxel_utils.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/object_detection_3d/voxelization.py` & `keras-cv-0.8.2/keras_cv/src/layers/object_detection_3d/voxelization.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/overlapping_patching_embedding.py` & `keras-cv-0.8.2/keras_cv/src/layers/overlapping_patching_embedding.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/__init__.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/aug_mix.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/aug_mix.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/auto_contrast.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/auto_contrast.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/base_image_augmentation_layer.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/base_image_augmentation_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,23 +232,23 @@
     def _compute_output_signature(self, inputs):
         fn_output_signature = {
             IMAGES: self.compute_image_signature(inputs[IMAGES])
         }
         bounding_boxes = inputs.get(BOUNDING_BOXES, None)
 
         if bounding_boxes is not None:
-            fn_output_signature[
-                BOUNDING_BOXES
-            ] = self._compute_bounding_box_signature(bounding_boxes)
+            fn_output_signature[BOUNDING_BOXES] = (
+                self._compute_bounding_box_signature(bounding_boxes)
+            )
 
         segmentation_masks = inputs.get(SEGMENTATION_MASKS, None)
         if segmentation_masks is not None:
-            fn_output_signature[
-                SEGMENTATION_MASKS
-            ] = self.compute_image_signature(segmentation_masks)
+            fn_output_signature[SEGMENTATION_MASKS] = (
+                self.compute_image_signature(segmentation_masks)
+            )
 
         keypoints = inputs.get(KEYPOINTS, None)
         if keypoints is not None:
             fn_output_signature[KEYPOINTS] = self._compute_keypoints_signature(
                 keypoints
             )
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/channel_shuffle.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/cut_mix.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/cut_mix.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/equalization.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/equalization.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/fourier_mix.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/fourier_mix.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/grayscale.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/grayscale.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/grid_mask.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/grid_mask.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/jittered_resize.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/jittered_resize.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/mix_up.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/mix_up.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/mosaic.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/mosaic.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/posterization.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/posterization.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/rand_augment.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/rand_augment.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_apply.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_apply.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_aspect_ratio.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_aspect_ratio.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_augmentation_pipeline.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_augmentation_pipeline.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_brightness.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_channel_shift.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_channel_shift.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_choice.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_choice.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_color_degeneration.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_color_degeneration.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_color_jitter.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_color_jitter.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_contrast.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_crop.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_crop_and_resize.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_crop_and_resize.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,18 +268,18 @@
     @classmethod
     def from_config(cls, config):
         if isinstance(config["crop_area_factor"], dict):
             config["crop_area_factor"] = keras.utils.deserialize_keras_object(
                 config["crop_area_factor"]
             )
         if isinstance(config["aspect_ratio_factor"], dict):
-            config[
-                "aspect_ratio_factor"
-            ] = keras.utils.deserialize_keras_object(
-                config["aspect_ratio_factor"]
+            config["aspect_ratio_factor"] = (
+                keras.utils.deserialize_keras_object(
+                    config["aspect_ratio_factor"]
+                )
             )
         return cls(**config)
 
     def _crop_and_resize(self, image, transformation, method=None):
         image = tf.expand_dims(image, axis=0)
         boxes = transformation
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_cutout.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_cutout.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_flip.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_gaussian_blur.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_hue.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_hue.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_jpeg_quality.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_jpeg_quality.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_rotation.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_saturation.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_saturation.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_sharpness.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_sharpness.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_shear.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_shear.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_translation.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/random_zoom.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/repeated_augmentation.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/repeated_augmentation.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/rescaling.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/resizing.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/solarization.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/solarization.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing/vectorized_base_image_augmentation_layer.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing/vectorized_base_image_augmentation_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 import tensorflow as tf
 import tree
 
 from keras_cv.src import bounding_box
 from keras_cv.src.api_export import keras_cv_export
+from keras_cv.src.backend import config
 from keras_cv.src.backend import keras
 from keras_cv.src.backend import ops
 from keras_cv.src.backend import scope
 from keras_cv.src.utils import preprocessing
 
 H_AXIS = -3
 W_AXIS = -2
@@ -408,22 +409,24 @@
         for key in inputs.keys() - result.keys():
             result[key] = inputs[key]
         return result
 
     def call(self, inputs):
         # try to convert a given backend native tensor to TensorFlow tensor
         # before passing it over to TFDataScope
+        is_tf_backend = config.backend() == "tensorflow"
+        is_in_tf_graph = not tf.executing_eagerly()
         contains_ragged = lambda y: any(
             tree.map_structure(
                 lambda x: isinstance(x, (tf.RaggedTensor, tf.SparseTensor)),
                 tree.flatten(y),
             )
         )
         inputs_contain_ragged = contains_ragged(inputs)
-        if not inputs_contain_ragged:
+        if not is_tf_backend and not inputs_contain_ragged:
             inputs = tree.map_structure(
                 lambda x: tf.convert_to_tensor(x), inputs
             )
         with scope.TFDataScope():
             inputs = self._ensure_inputs_are_compute_dtype(inputs)
             inputs, metadata = self._format_inputs(inputs)
             images = inputs[IMAGES]
@@ -439,21 +442,22 @@
                 )
         # convert the outputs to backend native tensors if none of them
         # contain RaggedTensors. Note that if the user passed in Raggeds
         # but the outputs are dense, we still don't want to convert to
         # backend native tensors. This is to avoid breaking TF data
         # pipelines that can't easily be ported to become backend
         # agnostic.
-        if not inputs_contain_ragged and not contains_ragged(outputs):
-            outputs = tree.map_structure(
-                # some layers return None, handle that case when
-                # converting to tensors
-                lambda x: ops.convert_to_tensor(x) if x is not None else x,
-                outputs,
-            )
+        if not is_tf_backend and not is_in_tf_graph:
+            if not inputs_contain_ragged and not contains_ragged(outputs):
+                outputs = tree.map_structure(
+                    # some layers return None, handle that case when
+                    # converting to tensors
+                    lambda x: ops.convert_to_tensor(x) if x is not None else x,
+                    outputs,
+                )
         return outputs
 
     def _format_inputs(self, inputs):
         metadata = {IS_DICT: True, USE_TARGETS: False}
         if tf.is_tensor(inputs):
             # single image input tensor
             metadata[IS_DICT] = False
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/__init__.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/base_augmentation_layer_3d.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/base_augmentation_layer_3d.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_dropping_points.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_dropping_points.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_point_feature_noise.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/frustum_random_point_feature_noise.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_dropping_points.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_dropping_points.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_flip.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_flip.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_rotation.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_scaling.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_scaling.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/global_random_translation.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/global_random_translation.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/group_points_by_bounding_boxes.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/group_points_by_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/random_copy_paste.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/random_copy_paste.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/random_drop_box.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/random_drop_box.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/preprocessing_3d/waymo/swap_background.py` & `keras-cv-0.8.2/keras_cv/src/layers/preprocessing_3d/waymo/swap_background.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/regularization/__init__.py` & `keras-cv-0.8.2/keras_cv/src/layers/regularization/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/regularization/drop_path.py` & `keras-cv-0.8.2/keras_cv/src/layers/regularization/drop_path.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/regularization/dropblock_2d.py` & `keras-cv-0.8.2/keras_cv/src/layers/regularization/dropblock_2d.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/regularization/squeeze_excite.py` & `keras-cv-0.8.2/keras_cv/src/layers/regularization/squeeze_excite.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,18 +114,18 @@
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
     @classmethod
     def from_config(cls, config):
         if isinstance(config["squeeze_activation"], dict):
-            config[
-                "squeeze_activation"
-            ] = keras.saving.deserialize_keras_object(
-                config["squeeze_activation"]
+            config["squeeze_activation"] = (
+                keras.saving.deserialize_keras_object(
+                    config["squeeze_activation"]
+                )
             )
         if isinstance(config["excite_activation"], dict):
             config["excite_activation"] = keras.saving.deserialize_keras_object(
                 config["excite_activation"]
             )
         return cls(**config)
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/regularization/stochastic_depth.py` & `keras-cv-0.8.2/keras_cv/src/layers/regularization/stochastic_depth.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/segformer_multihead_attention.py` & `keras-cv-0.8.2/keras_cv/src/layers/segformer_multihead_attention.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/spatial_pyramid.py` & `keras-cv-0.8.2/keras_cv/src/layers/spatial_pyramid.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/transformer_encoder.py` & `keras-cv-0.8.2/keras_cv/src/layers/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/vit_det_layers.py` & `keras-cv-0.8.2/keras_cv/src/layers/vit_det_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,17 +426,17 @@
             epsilon=self.layer_norm_epsilon
         )
         self.attention = MultiHeadAttentionWithRelativePE(
             num_heads=self.num_heads,
             key_dim=self.project_dim // self.num_heads,
             use_bias=use_bias,
             use_rel_pos=use_rel_pos,
-            input_size=input_size
-            if window_size == 0
-            else (window_size, window_size),
+            input_size=(
+                input_size if window_size == 0 else (window_size, window_size)
+            ),
         )
         self.mlp_block = MLP(
             mlp_dim,
             project_dim,
             num_layers=2,
             activation="gelu",
         )
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/layers/vit_layers.py` & `keras-cv-0.8.2/keras_cv/src/layers/vit_layers.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/losses/__init__.py` & `keras-cv-0.8.2/keras_cv/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/losses/centernet_box_loss.py` & `keras-cv-0.8.2/keras_cv/src/losses/centernet_box_loss.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/losses/ciou_loss.py` & `keras-cv-0.8.2/keras_cv/src/losses/ciou_loss.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/losses/focal.py` & `keras-cv-0.8.2/keras_cv/src/losses/focal.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/losses/giou_loss.py` & `keras-cv-0.8.2/keras_cv/src/losses/giou_loss.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/losses/iou_loss.py` & `keras-cv-0.8.2/keras_cv/src/losses/iou_loss.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/losses/penalty_reduced_focal_loss.py` & `keras-cv-0.8.2/keras_cv/src/losses/penalty_reduced_focal_loss.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/losses/simclr_loss.py` & `keras-cv-0.8.2/keras_cv/src/losses/simclr_loss.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/losses/smooth_l1.py` & `keras-cv-0.8.2/keras_cv/src/losses/smooth_l1.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/metrics/__init__.py` & `keras-cv-0.8.2/keras_cv/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/metrics/coco/__init__.py` & `keras-cv-0.8.2/keras_cv/src/metrics/coco/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/metrics/coco/pycoco_wrapper.py` & `keras-cv-0.8.2/keras_cv/src/metrics/coco/pycoco_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,17 @@
 
 
 def _convert_predictions_to_coco_annotations(predictions):
     coco_predictions = []
     num_batches = len(predictions["source_id"])
     for i in range(num_batches):
         batch_size = predictions["source_id"][i].shape[0]
+        predictions["detection_boxes"][i] = predictions["detection_boxes"][
+            i
+        ].copy()
         for j in range(batch_size):
             max_num_detections = predictions["num_detections"][i][j]
             predictions["detection_boxes"][i][j] = _yxyx_to_xywh(
                 predictions["detection_boxes"][i][j]
             )
             for k in range(max_num_detections):
                 ann = {}
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/metrics/object_detection/__init__.py` & `keras-cv-0.8.2/keras_cv/src/metrics/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/metrics/object_detection/box_coco_metrics.py` & `keras-cv-0.8.2/keras_cv/src/metrics/object_detection/box_coco_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,17 +208,17 @@
 
         def result_fn(self, force=False):
             py_func_result = tf.py_function(
                 self.result_on_host_cpu, inp=[force], Tout=obj.dtype
             )
             result = {}
             for i, key in enumerate(METRIC_NAMES):
-                result[
-                    self.name_prefix() + METRIC_MAPPING[key]
-                ] = py_func_result[i]
+                result[self.name_prefix() + METRIC_MAPPING[key]] = (
+                    py_func_result[i]
+                )
             return result
 
         obj.result = types.MethodType(result_fn, obj)
 
         return obj
 
     def name_prefix(self):
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,14 +186,15 @@
 from keras_cv.src.models.object_detection.retinanet.retinanet import RetinaNet
 from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_backbone import (
     YOLOV8Backbone,
 )
 from keras_cv.src.models.object_detection.yolo_v8.yolo_v8_detector import (
     YOLOV8Detector,
 )
+from keras_cv.src.models.segmentation import BASNet
 from keras_cv.src.models.segmentation import DeepLabV3Plus
 from keras_cv.src.models.segmentation import SAMMaskDecoder
 from keras_cv.src.models.segmentation import SAMPromptEncoder
 from keras_cv.src.models.segmentation import SegmentAnythingModel
 from keras_cv.src.models.segmentation import TwoWayTransformer
 from keras_cv.src.models.segmentation.segformer.segformer_aliases import SegFormer
 from keras_cv.src.models.segmentation.segformer.segformer_aliases import SegFormerB0
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/backbone.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/backbone.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/csp_darknet/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_aliases.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_aliases.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/csp_darknet/csp_darknet_utils.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/csp_darknet/csp_darknet_utils.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/densenet/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/densenet/densenet_aliases.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/densenet_aliases.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/densenet/densenet_backbone.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/densenet_backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,17 +115,17 @@
         x = apply_dense_block(
             x,
             stackwise_num_repeats[-1],
             growth_rate,
             name=f"conv{len(stackwise_num_repeats) + 1}",
         )
 
-        pyramid_level_inputs[
-            f"P{len(stackwise_num_repeats) + 1}"
-        ] = utils.get_tensor_input_name(x)
+        pyramid_level_inputs[f"P{len(stackwise_num_repeats) + 1}"] = (
+            utils.get_tensor_input_name(x)
+        )
         x = keras.layers.BatchNormalization(
             axis=BN_AXIS, epsilon=BN_EPSILON, name="bn"
         )(x)
         x = keras.layers.Activation("relu", name="relu")(x)
 
         # Create model.
         super().__init__(inputs=inputs, outputs=x, **kwargs)
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/densenet/densenet_backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/densenet/densenet_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_lite/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_aliases.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_aliases.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_lite/efficientnet_lite_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v1/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_aliases.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_aliases.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v1/efficientnet_v1_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v2/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_aliases.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_aliases.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/efficientnet_v2/efficientnet_v2_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mix_transformer/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mix_transformer/mix_transformer_aliases.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/mix_transformer_aliases.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/mix_transformer/mix_transformer_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mobilenet_v3/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_aliases.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_aliases.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/mobilenet_v3/mobilenet_v3_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v1/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v1/resnet_v1_aliases.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/resnet_v1_aliases.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,17 +126,17 @@
                 filters=stackwise_filters[stack_index],
                 blocks=stackwise_blocks[stack_index],
                 stride=stackwise_strides[stack_index],
                 block_type=block_type,
                 first_shortcut=(block_type == "block" or stack_index > 0),
                 name=f"v2_stack_{stack_index}",
             )
-            pyramid_level_inputs[
-                f"P{stack_index + 2}"
-            ] = utils.get_tensor_input_name(x)
+            pyramid_level_inputs[f"P{stack_index + 2}"] = (
+                utils.get_tensor_input_name(x)
+            )
 
         # Create model.
         super().__init__(inputs=inputs, outputs=x, **kwargs)
 
         # All references to `self` below this line
         self.pyramid_level_inputs = pyramid_level_inputs
         self.stackwise_filters = stackwise_filters
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v1/resnet_v1_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v2/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v2/resnet_v2_aliases.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/resnet_v2_aliases.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,17 +132,17 @@
                 blocks=stackwise_blocks[stack_index],
                 stride=stackwise_strides[stack_index],
                 dilations=stackwise_dilations[stack_index],
                 block_type=block_type,
                 first_shortcut=(block_type == "block" or stack_index > 0),
                 name=f"v2_stack_{stack_index}",
             )
-            pyramid_level_inputs[
-                f"P{stack_index + 2}"
-            ] = utils.get_tensor_input_name(x)
+            pyramid_level_inputs[f"P{stack_index + 2}"] = (
+                utils.get_tensor_input_name(x)
+            )
 
         x = keras.layers.BatchNormalization(
             axis=BN_AXIS, epsilon=BN_EPSILON, name="post_bn"
         )(x)
         x = keras.layers.Activation("relu", name="post_relu")(x)
 
         # Create model.
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/resnet_v2/resnet_v2_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/test_backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/test_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/vit_det/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/vit_det/vit_det_aliases.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/vit_det_aliases.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/vit_det/vit_det_backbone.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/vit_det_backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,17 +140,17 @@
         for i in range(depth):
             x = WindowedTransformerEncoder(
                 project_dim=embed_dim,
                 mlp_dim=mlp_dim,
                 num_heads=num_heads,
                 use_bias=use_bias,
                 use_rel_pos=use_rel_pos,
-                window_size=window_size
-                if i not in global_attention_indices
-                else 0,
+                window_size=(
+                    window_size if i not in global_attention_indices else 0
+                ),
                 input_size=(img_size // patch_size, img_size // patch_size),
             )(x)
         x = keras.models.Sequential(
             [
                 keras.layers.Conv2D(
                     filters=out_chans, kernel_size=1, use_bias=False
                 ),
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/backbones/vit_det/vit_det_backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/backbones/vit_det/vit_det_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/classification/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/classification/image_classifier.py` & `keras-cv-0.8.2/keras_cv/src/models/classification/image_classifier.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/classification/image_classifier_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/classification/image_classifier_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/convmixer.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/convmixer.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/convnext.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/convnext.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/darknet.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/darknet.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     Returns:
         A `keras.Model` instance.
 """  # noqa: E501
 
 
 @keras.utils.register_keras_serializable(package="keras_cv.models")
 class DarkNet(keras.Model):
-
     """Represents the DarkNet architecture.
 
     The DarkNet architecture is commonly used for detection tasks. It is
     possible to extract the intermediate dark2 to dark5 layers from the model
     for creating a feature pyramid Network.
 
     Reference:
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/mlp_mixer.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/mlp_mixer.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,14 @@
     y = layers.LayerNormalization()(x)
     y = apply_mlp_block(y, channels_mlp_dim, name=f"{name}_channel_mixing")
     return layers.Add()([x, y])
 
 
 @keras.utils.register_keras_serializable(package="keras_cv.models")
 class MLPMixer(keras.Model):
-
     """Instantiates the MLP Mixer architecture.
 
     Args:
       input_shape: tuple denoting the input shape, (224, 224, 3) for example.
       patch_size: integer denoting the size of the patches to be extracted
         from the inputs (16 for extracting 16x16 patches for example).
       num_blocks: integer, number of mixer blocks.
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/object_detection/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/object_detection/faster_rcnn/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/faster_rcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/object_detection/faster_rcnn/faster_rcnn.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/object_detection/faster_rcnn/faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/regnet.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/regnet.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/utils.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/vgg16.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/vgg19.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/vit.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/vit.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/legacy/weights.py` & `keras-cv-0.8.2/keras_cv/src/models/legacy/weights.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/__internal__.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/__internal__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/predict_utils.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/predict_utils.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/retinanet/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/retinanet/feature_pyramid.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/feature_pyramid.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/retinanet/prediction_head.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/prediction_head.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/retinanet/retinanet.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/retinanet.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/retinanet/retinanet_label_encoder.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/retinanet_label_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/retinanet/retinanet_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/retinanet/retinanet_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,17 +174,17 @@
             if stack_id == len(stackwise_depth) - 1:
                 x = apply_spatial_pyramid_pooling_fast(
                     x,
                     pool_size=5,
                     activation=activation,
                     name=f"{stack_name}_spp_fast",
                 )
-            pyramid_level_inputs[
-                f"P{stack_id + 2}"
-            ] = utils.get_tensor_input_name(x)
+            pyramid_level_inputs[f"P{stack_id + 2}"] = (
+                utils.get_tensor_input_name(x)
+            )
 
         super().__init__(inputs=inputs, outputs=x, **kwargs)
         self.pyramid_level_inputs = pyramid_level_inputs
         self.stackwise_channels = stackwise_channels
         self.stackwise_depth = stackwise_depth
         self.include_rescaling = include_rescaling
         self.activation = activation
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -651,23 +651,25 @@
 
     @classmethod
     def from_config(cls, config):
         config["backbone"] = keras.saving.deserialize_keras_object(
             config["backbone"]
         )
         label_encoder = config.get("label_encoder")
-        if label_encoder is not None:
+        if label_encoder is not None and isinstance(label_encoder, dict):
             config["label_encoder"] = keras.saving.deserialize_keras_object(
                 label_encoder
             )
         prediction_decoder = config.get("prediction_decoder")
-        if prediction_decoder is not None:
-            config[
-                "prediction_decoder"
-            ] = keras.saving.deserialize_keras_object(prediction_decoder)
+        if prediction_decoder is not None and isinstance(
+            prediction_decoder, dict
+        ):
+            config["prediction_decoder"] = (
+                keras.saving.deserialize_keras_object(prediction_decoder)
+            )
         return cls(**config)
 
     @classproperty
     def presets(cls):
         """Dictionary of preset names and configurations."""
         return copy.deepcopy({**backbone_presets, **yolo_v8_detector_presets})
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_detector_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_label_encoder.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_label_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_layers.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolo_v8/yolo_v8_layers.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/binary_crossentropy.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/binary_crossentropy.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/layers/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_decoder.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_decoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_head.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_head.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_label_encoder.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_label_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection/yolox/layers/yolox_pafpn.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection/yolox/layers/yolox_pafpn.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection_3d/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection_3d/center_pillar.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/center_pillar.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection_3d/center_pillar_backbone.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/center_pillar_backbone.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/object_detection_3d/center_pillar_backbone_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/object_detection_3d/center_pillar_backbone_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from keras_cv.src.models.segmentation.basnet import BASNet
 from keras_cv.src.models.segmentation.deeplab_v3_plus import DeepLabV3Plus
 from keras_cv.src.models.segmentation.segformer import SegFormer
 from keras_cv.src.models.segmentation.segment_anything import SAMMaskDecoder
 from keras_cv.src.models.segmentation.segment_anything import SAMPromptEncoder
 from keras_cv.src.models.segmentation.segment_anything import SegmentAnythingModel
 from keras_cv.src.models.segmentation.segment_anything import TwoWayTransformer
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segformer/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segformer/segformer.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/segformer.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segformer/segformer_aliases.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/segformer_aliases.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segformer/segformer_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/segformer/segformer_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/sam.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/sam_layers.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_layers.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/sam_mask_decoder.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_mask_decoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/sam_presets.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_presets.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/sam_prompt_encoder.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/segmentation/segment_anything/sam_transformer.py` & `keras-cv-0.8.2/keras_cv/src/models/segmentation/segment_anything/sam_transformer.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/__init__.py` & `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/attention_block.py` & `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/attention_block.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/clip_tokenizer.py` & `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/clip_tokenizer.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/constants.py` & `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/constants.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/decoder.py` & `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/decoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/diffusion_model.py` & `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/diffusion_model.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/image_encoder.py` & `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/image_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/noise_scheduler.py` & `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/noise_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,15 @@
         self.train_timesteps = train_timesteps
 
         if beta_schedule == "linear":
             self.betas = ops.linspace(beta_start, beta_end, train_timesteps)
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
             self.betas = (
-                ops.linspace(
-                    beta_start**0.5, beta_end**0.5, train_timesteps
-                )
+                ops.linspace(beta_start**0.5, beta_end**0.5, train_timesteps)
                 ** 2
             )
         else:
             raise ValueError(f"Invalid beta schedule: {beta_schedule}.")
 
         self.alphas = 1.0 - self.betas
         self.alphas_cumprod = ops.cumprod(self.alphas)
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/padded_conv2d.py` & `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/padded_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/resnet_block.py` & `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/resnet_block.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/stable_diffusion.py` & `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/stable_diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,18 @@
                     ops.expand_dims(diffusion_noise, axis=0), batch_size, axis=0
                 )
             latent = diffusion_noise
         else:
             latent = self._get_initial_diffusion_noise(batch_size, seed)
 
         # Iterative reverse diffusion stage
-        timesteps = np.arange(1, 1000, 1000 // num_steps)
+        num_timesteps = 1000
+        ratio = (num_timesteps - 1) / (num_steps - 1)
+        timesteps = (np.arange(0, num_steps) * ratio).round().astype(np.int64)
+
         alphas, alphas_prev = self._get_initial_alphas(timesteps)
         progbar = keras.utils.Progbar(len(timesteps))
         iteration = 0
         for index, timestep in list(enumerate(timesteps))[::-1]:
             latent_prev = latent  # Set aside the previous latent vector
             t_emb = self._get_timestep_embedding(timestep, batch_size)
             unconditional_latent = self.diffusion_model.predict_on_batch(
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/stable_diffusion/text_encoder.py` & `keras-cv-0.8.2/keras_cv/src/models/stable_diffusion/text_encoder.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/task.py` & `keras-cv-0.8.2/keras_cv/src/models/task.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/models/utils.py` & `keras-cv-0.8.2/keras_cv/src/models/utils.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/ops/__init__.py` & `keras-cv-0.8.2/keras_cv/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/ops/iou_3d.py` & `keras-cv-0.8.2/keras_cv/src/ops/iou_3d.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/point_cloud/__init__.py` & `keras-cv-0.8.2/keras_cv/src/point_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/point_cloud/point_cloud.py` & `keras-cv-0.8.2/keras_cv/src/point_cloud/point_cloud.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/tests/__init__.py` & `keras-cv-0.8.2/keras_cv/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/tests/test_case.py` & `keras-cv-0.8.2/keras_cv/src/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/training/__init__.py` & `keras-cv-0.8.2/keras_cv/src/training/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/training/contrastive/__init__.py` & `keras-cv-0.8.2/keras_cv/src/training/contrastive/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/training/contrastive/contrastive_trainer.py` & `keras-cv-0.8.2/keras_cv/src/training/contrastive/contrastive_trainer.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/training/contrastive/simclr_trainer.py` & `keras-cv-0.8.2/keras_cv/src/training/contrastive/simclr_trainer.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/utils/__init__.py` & `keras-cv-0.8.2/keras_cv/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/utils/conditional_imports.py` & `keras-cv-0.8.2/keras_cv/src/utils/conditional_imports.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/utils/conv_utils.py` & `keras-cv-0.8.2/keras_cv/src/utils/conv_utils.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/utils/fill_utils.py` & `keras-cv-0.8.2/keras_cv/src/utils/fill_utils.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/utils/preprocessing.py` & `keras-cv-0.8.2/keras_cv/src/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/utils/preset_utils.py` & `keras-cv-0.8.2/keras_cv/src/utils/preset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/utils/python_utils.py` & `keras-cv-0.8.2/keras_cv/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/utils/resource_loader.py` & `keras-cv-0.8.2/keras_cv/src/utils/resource_loader.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/utils/target_gather.py` & `keras-cv-0.8.2/keras_cv/src/utils/target_gather.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/utils/test_utils.py` & `keras-cv-0.8.2/keras_cv/src/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/utils/to_numpy.py` & `keras-cv-0.8.2/keras_cv/src/utils/to_numpy.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/utils/train.py` & `keras-cv-0.8.2/keras_cv/src/utils/train.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/version_check.py` & `keras-cv-0.8.2/keras_cv/src/version_check.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/visualization/__init__.py` & `keras-cv-0.8.2/keras_cv/src/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/visualization/draw_bounding_boxes.py` & `keras-cv-0.8.2/keras_cv/src/visualization/draw_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/visualization/plot_bounding_box_gallery.py` & `keras-cv-0.8.2/keras_cv/src/visualization/plot_bounding_box_gallery.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/visualization/plot_image_gallery.py` & `keras-cv-0.8.2/keras_cv/src/visualization/plot_image_gallery.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv/src/visualization/plot_segmentation_mask_gallery.py` & `keras-cv-0.8.2/keras_cv/src/visualization/plot_segmentation_mask_gallery.py`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/keras_cv.egg-info/PKG-INFO` & `keras-cv-0.8.2/keras_cv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-cv
-Version: 0.8.1.dev0
+Version: 0.8.2
 Summary: Industry-strength computer Vision extensions for Keras.
 Home-page: https://github.com/keras-team/keras-cv
 Author: Keras team
 Author-email: keras-cv@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-cv-0.8.1.dev0/keras_cv.egg-info/SOURCES.txt` & `keras-cv-0.8.2/keras_cv.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 keras_cv/models/segmentation/__init__.py
 keras_cv/models/stable_diffusion/__init__.py
 keras_cv/models/yolov8/__init__.py
 keras_cv/src/__init__.py
 keras_cv/src/api_export.py
 keras_cv/src/conftest.py
 keras_cv/src/version_check.py
+keras_cv/src/version_utils.py
 keras_cv/src/backend/__init__.py
 keras_cv/src/backend/config.py
 keras_cv/src/backend/keras.py
 keras_cv/src/backend/ops.py
 keras_cv/src/backend/random.py
 keras_cv/src/backend/scope.py
 keras_cv/src/backend/tf_ops.py
@@ -265,14 +266,17 @@
 keras_cv/src/models/object_detection/yolox/layers/yolox_label_encoder.py
 keras_cv/src/models/object_detection/yolox/layers/yolox_pafpn.py
 keras_cv/src/models/object_detection_3d/__init__.py
 keras_cv/src/models/object_detection_3d/center_pillar.py
 keras_cv/src/models/object_detection_3d/center_pillar_backbone.py
 keras_cv/src/models/object_detection_3d/center_pillar_backbone_presets.py
 keras_cv/src/models/segmentation/__init__.py
+keras_cv/src/models/segmentation/basnet/__init__.py
+keras_cv/src/models/segmentation/basnet/basnet.py
+keras_cv/src/models/segmentation/basnet/basnet_presets.py
 keras_cv/src/models/segmentation/deeplab_v3_plus/__init__.py
 keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus.py
 keras_cv/src/models/segmentation/deeplab_v3_plus/deeplab_v3_plus_presets.py
 keras_cv/src/models/segmentation/segformer/__init__.py
 keras_cv/src/models/segmentation/segformer/segformer.py
 keras_cv/src/models/segmentation/segformer/segformer_aliases.py
 keras_cv/src/models/segmentation/segformer/segformer_presets.py
```

### Comparing `keras-cv-0.8.1.dev0/setup.cfg` & `keras-cv-0.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `keras-cv-0.8.1.dev0/setup.py` & `keras-cv-0.8.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,21 +17,40 @@
 import os
 import pathlib
 
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.dist import Distribution
 
+
+def read(rel_path):
+    here = os.path.abspath(os.path.dirname(__file__))
+    with open(os.path.join(here, rel_path)) as fp:
+        return fp.read()
+
+
+def get_version(rel_path):
+    for line in read(rel_path).splitlines():
+        if line.startswith("__version__"):
+            delim = '"' if '"' in line else "'"
+            return line.split(delim)[1]
+    raise RuntimeError("Unable to find version string.")
+
+
 BUILD_WITH_CUSTOM_OPS = (
     "BUILD_WITH_CUSTOM_OPS" in os.environ
     and os.environ["BUILD_WITH_CUSTOM_OPS"] == "true"
 )
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
+if os.path.exists("keras_cv/version_utils.py"):
+    VERSION = get_version("keras_cv/version_utils.py")
+else:
+    VERSION = get_version("keras_cv/src/version_utils.py")
 
 
 class BinaryDistribution(Distribution):
     """This class is needed in order to create OS specific wheels."""
 
     def has_ext_modules(self):
         return BUILD_WITH_CUSTOM_OPS
@@ -41,14 +60,15 @@
 
 
 setup(
     name="keras-cv",
     description="Industry-strength computer Vision extensions for Keras.",
     long_description=README,
     long_description_content_type="text/markdown",
+    version=VERSION,
     url="https://github.com/keras-team/keras-cv",
     author="Keras team",
     author_email="keras-cv@google.com",
     license="Apache License 2.0",
     install_requires=[
         "packaging",
         "absl-py",
```

