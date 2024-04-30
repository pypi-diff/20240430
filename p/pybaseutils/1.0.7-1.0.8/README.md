# Comparing `tmp/pybaseutils-1.0.7.tar.gz` & `tmp/pybaseutils-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybaseutils-1.0.7.tar", last modified: Mon Apr 29 03:56:10 2024, max compression
+gzip compressed data, was "pybaseutils-1.0.8.tar", last modified: Tue Apr 30 10:01:00 2024, max compression
```

## Comparing `pybaseutils-1.0.7.tar` & `pybaseutils-1.0.8.tar`

### file list

```diff
@@ -1,250 +1,251 @@
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.952406 pybaseutils-1.0.7/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-1.0.7/LICENCE
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3964 2024-04-29 03:56:10.952171 pybaseutils-1.0.7/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-22 02:45:56.000000 pybaseutils-1.0.7/README.md
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.824792 pybaseutils-1.0.7/pybaseutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2024-04-29 03:56:04.000000 pybaseutils-1.0.7/pybaseutils/__init__.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.830153 pybaseutils-1.0.7/pybaseutils/audio/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-1.0.7/pybaseutils/audio/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13844 2023-08-21 03:28:21.000000 pybaseutils-1.0.7/pybaseutils/audio/audio_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1857 2023-07-26 01:11:04.000000 pybaseutils-1.0.7/pybaseutils/audio/pyaudio_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11049 2023-08-09 08:16:14.000000 pybaseutils-1.0.7/pybaseutils/audio/vad_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/pybaseutils/base64_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2333 2023-08-21 01:44:07.000000 pybaseutils-1.0.7/pybaseutils/batch_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.832147 pybaseutils-1.0.7/pybaseutils/build_utils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-20 06:36:23.000000 pybaseutils-1.0.7/pybaseutils/build_utils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6003 2023-09-20 10:26:35.000000 pybaseutils-1.0.7/pybaseutils/build_utils/cython_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2981 2023-12-06 02:32:14.000000 pybaseutils-1.0.7/pybaseutils/build_utils/pyarmor_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.834424 pybaseutils-1.0.7/pybaseutils/cluster/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/pybaseutils/cluster/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/pybaseutils/cluster/kmean.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/pybaseutils/cluster/maxmin_distance.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/pybaseutils/cluster/similarity.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-1.0.7/pybaseutils/color_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-1.0.7/pybaseutils/config_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.846122 pybaseutils-1.0.7/pybaseutils/converter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/pybaseutils/converter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14586 2023-10-16 10:00:40.000000 pybaseutils-1.0.7/pybaseutils/converter/build_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1695 2023-07-11 07:13:11.000000 pybaseutils-1.0.7/pybaseutils/converter/build_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14159 2023-12-18 07:43:36.000000 pybaseutils-1.0.7/pybaseutils/converter/build_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5161 2023-08-18 02:32:51.000000 pybaseutils-1.0.7/pybaseutils/converter/concat_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2576 2024-03-18 08:50:01.000000 pybaseutils-1.0.7/pybaseutils/converter/convert_coco2labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3876 2023-10-17 09:34:43.000000 pybaseutils-1.0.7/pybaseutils/converter/convert_coco2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8994 2023-11-06 09:53:41.000000 pybaseutils-1.0.7/pybaseutils/converter/convert_labelme2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6015 2024-03-12 11:20:45.000000 pybaseutils-1.0.7/pybaseutils/converter/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3366 2023-09-14 06:08:22.000000 pybaseutils-1.0.7/pybaseutils/converter/convert_labelme2yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3823 2023-08-18 02:48:56.000000 pybaseutils-1.0.7/pybaseutils/converter/convert_voc2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2024-03-18 07:31:15.000000 pybaseutils-1.0.7/pybaseutils/converter/convert_voc2labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4163 2023-09-08 10:36:36.000000 pybaseutils-1.0.7/pybaseutils/converter/convert_voc2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9455 2023-08-18 02:51:52.000000 pybaseutils-1.0.7/pybaseutils/converter/convert_voc2yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3468 2023-08-11 05:43:39.000000 pybaseutils-1.0.7/pybaseutils/converter/convert_yolo2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12625 2024-02-04 09:03:56.000000 pybaseutils-1.0.7/pybaseutils/coords_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.849937 pybaseutils-1.0.7/pybaseutils/cvutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-1.0.7/pybaseutils/cvutils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10674 2024-04-29 03:55:20.000000 pybaseutils-1.0.7/pybaseutils/cvutils/corner_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6233 2023-06-21 02:12:33.000000 pybaseutils-1.0.7/pybaseutils/cvutils/monitor.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/pybaseutils/cvutils/mouse_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12675 2024-02-01 07:25:13.000000 pybaseutils-1.0.7/pybaseutils/cvutils/video_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.857294 pybaseutils-1.0.7/pybaseutils/dataloader/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/pybaseutils/dataloader/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    18727 2023-09-26 07:21:19.000000 pybaseutils-1.0.7/pybaseutils/dataloader/base_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7634 2024-03-18 07:07:15.000000 pybaseutils-1.0.7/pybaseutils/dataloader/base_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6286 2024-03-18 07:53:24.000000 pybaseutils-1.0.7/pybaseutils/dataloader/parser_coco_det.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7946 2024-03-18 07:53:24.000000 pybaseutils-1.0.7/pybaseutils/dataloader/parser_coco_ins.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2024-03-18 07:53:24.000000 pybaseutils-1.0.7/pybaseutils/dataloader/parser_coco_kps.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17737 2024-04-17 06:17:13.000000 pybaseutils-1.0.7/pybaseutils/dataloader/parser_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17629 2024-03-18 07:11:47.000000 pybaseutils-1.0.7/pybaseutils/dataloader/parser_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13264 2024-03-18 07:53:24.000000 pybaseutils-1.0.7/pybaseutils/dataloader/parser_yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4360 2023-08-11 05:47:15.000000 pybaseutils-1.0.7/pybaseutils/dataloader/voc_seg_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    39284 2024-03-15 09:42:00.000000 pybaseutils-1.0.7/pybaseutils/file_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.862359 pybaseutils-1.0.7/pybaseutils/filter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.7/pybaseutils/filter/QueueTable.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.7/pybaseutils/filter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.7/pybaseutils/filter/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.7/pybaseutils/filter/kalman_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1785 2023-11-22 02:11:08.000000 pybaseutils-1.0.7/pybaseutils/filter/mean_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1559 2023-11-22 02:10:23.000000 pybaseutils-1.0.7/pybaseutils/filter/motion_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      787 2023-11-22 02:11:08.000000 pybaseutils-1.0.7/pybaseutils/filter/pose_filter.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.863055 pybaseutils-1.0.7/pybaseutils/font_style/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/pybaseutils/font_style/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/pybaseutils/font_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13933 2023-10-08 08:52:58.000000 pybaseutils-1.0.7/pybaseutils/geometry_tools.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5305 2023-11-20 07:29:44.000000 pybaseutils-1.0.7/pybaseutils/heatmap_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)   103608 2024-03-27 03:34:35.000000 pybaseutils-1.0.7/pybaseutils/image_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4480 2023-08-11 03:00:05.000000 pybaseutils-1.0.7/pybaseutils/json_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/pybaseutils/log.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-1.0.7/pybaseutils/logger.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.866853 pybaseutils-1.0.7/pybaseutils/metrics/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/pybaseutils/metrics/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/pybaseutils/metrics/accuracy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/pybaseutils/metrics/average_meter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/pybaseutils/metrics/class_report.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/pybaseutils/metrics/plot_pr.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/pybaseutils/metrics/plot_roc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19252 2023-10-08 08:31:16.000000 pybaseutils-1.0.7/pybaseutils/numpy_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2092 2023-08-17 02:19:40.000000 pybaseutils-1.0.7/pybaseutils/pandas_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-1.0.7/pybaseutils/plot_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.869364 pybaseutils-1.0.7/pybaseutils/pose/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:27:54.000000 pybaseutils-1.0.7/pybaseutils/pose/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3080 2023-11-30 07:45:37.000000 pybaseutils-1.0.7/pybaseutils/pose/bones_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12406 2023-11-13 06:49:34.000000 pybaseutils-1.0.7/pybaseutils/pose/human_pose.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1976 2023-09-08 03:10:04.000000 pybaseutils-1.0.7/pybaseutils/pose/pose_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.871280 pybaseutils-1.0.7/pybaseutils/pycpp/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-1.0.7/pybaseutils/pycpp/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-1.0.7/pybaseutils/pycpp/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/pybaseutils/pycpp/main.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.872489 pybaseutils-1.0.7/pybaseutils/server/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-07-18 02:35:00.000000 pybaseutils-1.0.7/pybaseutils/server/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2004 2023-07-18 03:25:38.000000 pybaseutils-1.0.7/pybaseutils/server/apm_server.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-1.0.7/pybaseutils/setup_config.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1361 2023-12-26 05:59:47.000000 pybaseutils-1.0.7/pybaseutils/singleton_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7501 2023-12-26 07:29:39.000000 pybaseutils-1.0.7/pybaseutils/thread_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/pybaseutils/time_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/pybaseutils/tracemalloc_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-1.0.7/pybaseutils/tracemalloc_utils2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.876992 pybaseutils-1.0.7/pybaseutils/tracking/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.7/pybaseutils/tracking/QueueTable.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.7/pybaseutils/tracking/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.7/pybaseutils/tracking/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.7/pybaseutils/tracking/kalman_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1787 2023-11-28 10:29:05.000000 pybaseutils-1.0.7/pybaseutils/tracking/mean_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1561 2023-11-28 10:29:05.000000 pybaseutils-1.0.7/pybaseutils/tracking/motion_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      869 2023-11-28 10:29:05.000000 pybaseutils-1.0.7/pybaseutils/tracking/pose_filter.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.879921 pybaseutils-1.0.7/pybaseutils/transforms/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/pybaseutils/transforms/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    22405 2023-12-14 09:09:08.000000 pybaseutils-1.0.7/pybaseutils/transforms/affine_transform.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5112 2024-04-28 11:41:39.000000 pybaseutils-1.0.7/pybaseutils/transforms/face_alignment.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7099 2024-04-29 03:50:16.000000 pybaseutils-1.0.7/pybaseutils/transforms/transform_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-1.0.7/pybaseutils/word_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-1.0.7/pybaseutils/worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-1.0.7/pybaseutils/yaml_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.827819 pybaseutils-1.0.7/pybaseutils.egg-info/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3964 2024-04-29 03:56:10.000000 pybaseutils-1.0.7/pybaseutils.egg-info/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6937 2024-04-29 03:56:10.000000 pybaseutils-1.0.7/pybaseutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2024-04-29 03:56:10.000000 pybaseutils-1.0.7/pybaseutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-1.0.7/pybaseutils.egg-info/not-zip-safe
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2024-04-29 03:56:10.000000 pybaseutils-1.0.7/pybaseutils.egg-info/top_level.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2024-04-29 03:56:10.952500 pybaseutils-1.0.7/setup.cfg
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-1.0.7/setup.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.903092 pybaseutils-1.0.7/test_py/
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.905118 pybaseutils-1.0.7/test_py/WebCrawler/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-25 09:17:11.000000 pybaseutils-1.0.7/test_py/WebCrawler/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3615 2023-08-25 09:36:35.000000 pybaseutils-1.0.7/test_py/WebCrawler/search_image.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3183 2023-08-25 09:18:23.000000 pybaseutils-1.0.7/test_py/WebCrawler/search_image_for_baidu.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/test_py/__init__.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.910680 pybaseutils-1.0.7/test_py/aije/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-13 02:52:05.000000 pybaseutils-1.0.7/test_py/aije/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1672 2023-11-10 11:13:57.000000 pybaseutils-1.0.7/test_py/aije/convert_labelme2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1003 2024-03-12 11:20:31.000000 pybaseutils-1.0.7/test_py/aije/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      646 2024-03-15 09:39:47.000000 pybaseutils-1.0.7/test_py/aije/copy_move.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3927 2024-04-15 12:43:54.000000 pybaseutils-1.0.7/test_py/aije/demo_video_aije.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3743 2023-12-12 07:26:52.000000 pybaseutils-1.0.7/test_py/aije/demo_voc_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1948 2024-03-12 11:22:23.000000 pybaseutils-1.0.7/test_py/aije/demo_voc_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2187 2023-10-31 01:05:59.000000 pybaseutils-1.0.7/test_py/aije/video_demo.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.915127 pybaseutils-1.0.7/test_py/audio/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-01 02:27:48.000000 pybaseutils-1.0.7/test_py/audio/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      935 2023-08-04 10:15:41.000000 pybaseutils-1.0.7/test_py/audio/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9241 2023-08-03 04:19:03.000000 pybaseutils-1.0.7/test_py/audio/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1154 2023-08-03 02:53:43.000000 pybaseutils-1.0.7/test_py/audio/main_read.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1269 2023-08-07 09:21:59.000000 pybaseutils-1.0.7/test_py/audio/segment.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    31217 2023-05-10 02:07:39.000000 pybaseutils-1.0.7/test_py/audio/speechbrain_asr_indoor_prod.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4657 2023-08-09 08:17:18.000000 pybaseutils-1.0.7/test_py/audio/speechbrain_demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1296 2023-10-10 06:07:18.000000 pybaseutils-1.0.7/test_py/class_attribute.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-1.0.7/test_py/class_names.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.931993 pybaseutils-1.0.7/test_py/converter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-1.0.7/test_py/converter/AffectNet.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3494 2023-07-19 08:44:04.000000 pybaseutils-1.0.7/test_py/converter/AsianMovie.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3697 2023-08-11 05:35:11.000000 pybaseutils-1.0.7/test_py/converter/BITVehicle2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4581 2023-08-11 05:35:11.000000 pybaseutils-1.0.7/test_py/converter/BSTLD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5581 2023-08-17 02:19:40.000000 pybaseutils-1.0.7/test_py/converter/CCPD.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7029 2023-08-17 02:19:40.000000 pybaseutils-1.0.7/test_py/converter/CCPD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1297 2023-07-13 07:17:07.000000 pybaseutils-1.0.7/test_py/converter/FL3D_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-01 01:02:46.000000 pybaseutils-1.0.7/test_py/converter/FreiHAND2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-18 07:53:20.000000 pybaseutils-1.0.7/test_py/converter/MTFL2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2572 2023-08-11 05:35:11.000000 pybaseutils-1.0.7/test_py/converter/TT100K.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2723 2024-04-28 11:46:31.000000 pybaseutils-1.0.7/test_py/converter/WaterMeters.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/test_py/converter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5514 2023-08-17 02:19:40.000000 pybaseutils-1.0.7/test_py/converter/concat_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      842 2023-10-25 08:51:49.000000 pybaseutils-1.0.7/test_py/converter/convert_coco2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1410 2023-09-08 11:04:11.000000 pybaseutils-1.0.7/test_py/converter/convert_gesture2hand.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10536 2023-11-06 10:11:14.000000 pybaseutils-1.0.7/test_py/converter/convert_labelme2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6727 2023-11-08 03:36:12.000000 pybaseutils-1.0.7/test_py/converter/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      726 2023-07-10 09:58:46.000000 pybaseutils-1.0.7/test_py/converter/fatigue_driving.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2321 2023-08-17 02:19:40.000000 pybaseutils-1.0.7/test_py/converter/fdd_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4726 2023-09-01 07:54:12.000000 pybaseutils-1.0.7/test_py/converter/handpose2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1208 2023-08-17 02:19:40.000000 pybaseutils-1.0.7/test_py/converter/insects_for_aichallenger.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-1.0.7/test_py/converter/tt100k_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7596 2023-08-11 05:35:11.000000 pybaseutils-1.0.7/test_py/converter/ua_detrac2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2798 2024-03-18 08:47:50.000000 pybaseutils-1.0.7/test_py/converter/voc_sbd2labelme.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.937235 pybaseutils-1.0.7/test_py/cython_build/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-21 00:54:56.000000 pybaseutils-1.0.7/test_py/cython_build/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      988 2023-12-06 02:17:29.000000 pybaseutils-1.0.7/test_py/cython_build/build_cython.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1464 2023-12-06 09:27:08.000000 pybaseutils-1.0.7/test_py/cython_build/build_pyarmor.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1836 2023-09-22 03:30:02.000000 pybaseutils-1.0.7/test_py/cython_build/cryptography_demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      164 2023-09-20 00:50:56.000000 pybaseutils-1.0.7/test_py/cython_build/fun_sum.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      197 2023-09-20 00:51:59.000000 pybaseutils-1.0.7/test_py/cython_build/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2167 2023-09-22 01:20:56.000000 pybaseutils-1.0.7/test_py/cython_build/model_des_enctypt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2762 2023-09-22 01:35:52.000000 pybaseutils-1.0.7/test_py/cython_build/model_enctypt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1088 2024-04-28 12:11:12.000000 pybaseutils-1.0.7/test_py/demo1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      864 2023-11-10 09:54:32.000000 pybaseutils-1.0.7/test_py/demo2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      983 2023-09-06 06:55:38.000000 pybaseutils-1.0.7/test_py/demo3.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-1.0.7/test_py/demo_async_await1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-1.0.7/test_py/demo_async_await2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4875 2024-02-04 11:57:57.000000 pybaseutils-1.0.7/test_py/demo_coco_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5184 2023-08-28 09:18:09.000000 pybaseutils-1.0.7/test_py/demo_copy_files.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2169 2023-07-17 09:29:30.000000 pybaseutils-1.0.7/test_py/demo_copy_files_for_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      913 2023-06-28 11:52:23.000000 pybaseutils-1.0.7/test_py/demo_ffmpy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      719 2024-02-20 06:47:57.000000 pybaseutils-1.0.7/test_py/demo_for_pair_file.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1670 2024-03-01 02:07:11.000000 pybaseutils-1.0.7/test_py/demo_for_polygon.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-1.0.7/test_py/demo_for_trt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4613 2023-12-18 07:46:39.000000 pybaseutils-1.0.7/test_py/demo_get_file_list.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      637 2023-11-27 08:52:43.000000 pybaseutils-1.0.7/test_py/demo_gif.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1742 2024-01-12 07:19:32.000000 pybaseutils-1.0.7/test_py/demo_gif_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1125 2024-03-07 10:19:09.000000 pybaseutils-1.0.7/test_py/demo_image_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      825 2023-08-11 06:37:13.000000 pybaseutils-1.0.7/test_py/demo_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/test_py/demo_metrics.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/test_py/demo_mouse.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      972 2023-07-04 07:11:29.000000 pybaseutils-1.0.7/test_py/demo_nii.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2089 2023-08-11 05:35:11.000000 pybaseutils-1.0.7/test_py/demo_pandas.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-1.0.7/test_py/demo_plot.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1056 2024-04-19 09:16:57.000000 pybaseutils-1.0.7/test_py/demo_rename.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-1.0.7/test_py/demo_standard_image .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1174 2023-09-15 08:45:39.000000 pybaseutils-1.0.7/test_py/demo_standard_video .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/test_py/demo_taichi.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      801 2023-10-17 03:30:20.000000 pybaseutils-1.0.7/test_py/demo_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3600 2023-10-17 07:58:27.000000 pybaseutils-1.0.7/test_py/demo_voc_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2914 2023-11-09 03:13:50.000000 pybaseutils-1.0.7/test_py/demo_voc_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-1.0.7/test_py/demo_word_similar.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-1.0.7/test_py/demo_worker1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/test_py/demo_worker2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.939969 pybaseutils-1.0.7/test_py/detector/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-1.0.7/test_py/detector/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1867 2023-08-11 05:35:01.000000 pybaseutils-1.0.7/test_py/detector/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6707 2023-10-17 07:58:27.000000 pybaseutils-1.0.7/test_py/detector/detect_face_person.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6126 2023-08-17 02:19:40.000000 pybaseutils-1.0.7/test_py/detector/predet_labelme.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.942506 pybaseutils-1.0.7/test_py/edit_distance/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-11-08 06:53:33.000000 pybaseutils-1.0.7/test_py/edit_distance/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1359 2023-11-23 06:50:21.000000 pybaseutils-1.0.7/test_py/edit_distance/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5613 2023-11-10 02:24:56.000000 pybaseutils-1.0.7/test_py/edit_distance/text_matching.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8212 2023-11-10 02:30:01.000000 pybaseutils-1.0.7/test_py/edit_distance/text_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.944500 pybaseutils-1.0.7/test_py/flask_demo/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-1.0.7/test_py/flask_demo/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-1.0.7/test_py/flask_demo/func.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-1.0.7/test_py/flask_demo/server.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.947190 pybaseutils-1.0.7/test_py/image_correction/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-1.0.7/test_py/image_correction/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-1.0.7/test_py/image_correction/demo_correction_v1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5603 2024-02-29 06:08:41.000000 pybaseutils-1.0.7/test_py/image_correction/demo_correction_v2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-1.0.7/test_py/image_correction/demo_correction_v3.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-1.0.7/test_py/kafka_worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-1.0.7/test_py/men_tracemalloc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-1.0.7/test_py/performance.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.948458 pybaseutils-1.0.7/test_py/pose/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:28:44.000000 pybaseutils-1.0.7/test_py/pose/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1530 2023-09-11 07:32:44.000000 pybaseutils-1.0.7/test_py/pose/human_pose.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-29 03:56:10.951529 pybaseutils-1.0.7/test_py/registry/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-07 01:10:07.000000 pybaseutils-1.0.7/test_py/registry/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1195 2023-09-07 05:56:01.000000 pybaseutils-1.0.7/test_py/registry/base.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3057 2023-09-07 02:42:07.000000 pybaseutils-1.0.7/test_py/registry/component.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1701 2023-09-07 04:32:01.000000 pybaseutils-1.0.7/test_py/registry/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1093 2023-09-07 05:50:04.000000 pybaseutils-1.0.7/test_py/registry/register.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.228386 pybaseutils-1.0.8/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-1.0.8/LICENCE
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3964 2024-04-30 10:01:00.228038 pybaseutils-1.0.8/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-22 02:45:56.000000 pybaseutils-1.0.8/README.md
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.113769 pybaseutils-1.0.8/pybaseutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2024-04-30 10:00:57.000000 pybaseutils-1.0.8/pybaseutils/__init__.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.119510 pybaseutils-1.0.8/pybaseutils/audio/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-1.0.8/pybaseutils/audio/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13844 2023-08-21 03:28:21.000000 pybaseutils-1.0.8/pybaseutils/audio/audio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1857 2023-07-26 01:11:04.000000 pybaseutils-1.0.8/pybaseutils/audio/pyaudio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11049 2023-08-09 08:16:14.000000 pybaseutils-1.0.8/pybaseutils/audio/vad_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/pybaseutils/base64_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2333 2023-08-21 01:44:07.000000 pybaseutils-1.0.8/pybaseutils/batch_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.121240 pybaseutils-1.0.8/pybaseutils/build_utils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-20 06:36:23.000000 pybaseutils-1.0.8/pybaseutils/build_utils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6003 2023-09-20 10:26:35.000000 pybaseutils-1.0.8/pybaseutils/build_utils/cython_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2981 2023-12-06 02:32:14.000000 pybaseutils-1.0.8/pybaseutils/build_utils/pyarmor_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.123686 pybaseutils-1.0.8/pybaseutils/cluster/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/pybaseutils/cluster/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/pybaseutils/cluster/kmean.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/pybaseutils/cluster/maxmin_distance.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/pybaseutils/cluster/similarity.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-1.0.8/pybaseutils/color_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-1.0.8/pybaseutils/config_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.131940 pybaseutils-1.0.8/pybaseutils/converter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/pybaseutils/converter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14586 2023-10-16 10:00:40.000000 pybaseutils-1.0.8/pybaseutils/converter/build_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1695 2023-07-11 07:13:11.000000 pybaseutils-1.0.8/pybaseutils/converter/build_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14159 2023-12-18 07:43:36.000000 pybaseutils-1.0.8/pybaseutils/converter/build_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5161 2023-08-18 02:32:51.000000 pybaseutils-1.0.8/pybaseutils/converter/concat_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2576 2024-03-18 08:50:01.000000 pybaseutils-1.0.8/pybaseutils/converter/convert_coco2labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3876 2023-10-17 09:34:43.000000 pybaseutils-1.0.8/pybaseutils/converter/convert_coco2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8994 2023-11-06 09:53:41.000000 pybaseutils-1.0.8/pybaseutils/converter/convert_labelme2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6015 2024-03-12 11:20:45.000000 pybaseutils-1.0.8/pybaseutils/converter/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3366 2023-09-14 06:08:22.000000 pybaseutils-1.0.8/pybaseutils/converter/convert_labelme2yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3823 2023-08-18 02:48:56.000000 pybaseutils-1.0.8/pybaseutils/converter/convert_voc2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2024-03-18 07:31:15.000000 pybaseutils-1.0.8/pybaseutils/converter/convert_voc2labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4163 2023-09-08 10:36:36.000000 pybaseutils-1.0.8/pybaseutils/converter/convert_voc2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9455 2023-08-18 02:51:52.000000 pybaseutils-1.0.8/pybaseutils/converter/convert_voc2yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3468 2023-08-11 05:43:39.000000 pybaseutils-1.0.8/pybaseutils/converter/convert_yolo2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12625 2024-02-04 09:03:56.000000 pybaseutils-1.0.8/pybaseutils/coords_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.134232 pybaseutils-1.0.8/pybaseutils/cvutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-1.0.8/pybaseutils/cvutils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10684 2024-04-30 07:58:54.000000 pybaseutils-1.0.8/pybaseutils/cvutils/corner_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6233 2023-06-21 02:12:33.000000 pybaseutils-1.0.8/pybaseutils/cvutils/monitor.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/pybaseutils/cvutils/mouse_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12675 2024-02-01 07:25:13.000000 pybaseutils-1.0.8/pybaseutils/cvutils/video_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.140173 pybaseutils-1.0.8/pybaseutils/dataloader/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/pybaseutils/dataloader/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    18727 2023-09-26 07:21:19.000000 pybaseutils-1.0.8/pybaseutils/dataloader/base_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9083 2024-04-30 09:00:41.000000 pybaseutils-1.0.8/pybaseutils/dataloader/base_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6286 2024-03-18 07:53:24.000000 pybaseutils-1.0.8/pybaseutils/dataloader/parser_coco_det.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7946 2024-03-18 07:53:24.000000 pybaseutils-1.0.8/pybaseutils/dataloader/parser_coco_ins.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2024-03-18 07:53:24.000000 pybaseutils-1.0.8/pybaseutils/dataloader/parser_coco_kps.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17134 2024-04-30 09:13:17.000000 pybaseutils-1.0.8/pybaseutils/dataloader/parser_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    16395 2024-04-30 09:06:38.000000 pybaseutils-1.0.8/pybaseutils/dataloader/parser_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13264 2024-03-18 07:53:24.000000 pybaseutils-1.0.8/pybaseutils/dataloader/parser_yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4360 2023-08-11 05:47:15.000000 pybaseutils-1.0.8/pybaseutils/dataloader/voc_seg_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    39284 2024-03-15 09:42:00.000000 pybaseutils-1.0.8/pybaseutils/file_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.143891 pybaseutils-1.0.8/pybaseutils/filter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.8/pybaseutils/filter/QueueTable.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.8/pybaseutils/filter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.8/pybaseutils/filter/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.8/pybaseutils/filter/kalman_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1785 2023-11-22 02:11:08.000000 pybaseutils-1.0.8/pybaseutils/filter/mean_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1559 2023-11-22 02:10:23.000000 pybaseutils-1.0.8/pybaseutils/filter/motion_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      787 2023-11-22 02:11:08.000000 pybaseutils-1.0.8/pybaseutils/filter/pose_filter.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.144499 pybaseutils-1.0.8/pybaseutils/font_style/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/pybaseutils/font_style/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/pybaseutils/font_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13933 2023-10-08 08:52:58.000000 pybaseutils-1.0.8/pybaseutils/geometry_tools.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5305 2023-11-20 07:29:44.000000 pybaseutils-1.0.8/pybaseutils/heatmap_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)   104090 2024-04-30 07:31:47.000000 pybaseutils-1.0.8/pybaseutils/image_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4756 2024-04-30 08:52:04.000000 pybaseutils-1.0.8/pybaseutils/json_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/pybaseutils/log.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-1.0.8/pybaseutils/logger.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.148381 pybaseutils-1.0.8/pybaseutils/metrics/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/pybaseutils/metrics/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/pybaseutils/metrics/accuracy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/pybaseutils/metrics/average_meter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/pybaseutils/metrics/class_report.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/pybaseutils/metrics/plot_pr.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/pybaseutils/metrics/plot_roc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19252 2023-10-08 08:31:16.000000 pybaseutils-1.0.8/pybaseutils/numpy_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2092 2023-08-17 02:19:40.000000 pybaseutils-1.0.8/pybaseutils/pandas_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-1.0.8/pybaseutils/plot_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.150668 pybaseutils-1.0.8/pybaseutils/pose/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:27:54.000000 pybaseutils-1.0.8/pybaseutils/pose/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3080 2023-11-30 07:45:37.000000 pybaseutils-1.0.8/pybaseutils/pose/bones_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12406 2023-11-13 06:49:34.000000 pybaseutils-1.0.8/pybaseutils/pose/human_pose.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1976 2023-09-08 03:10:04.000000 pybaseutils-1.0.8/pybaseutils/pose/pose_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.152470 pybaseutils-1.0.8/pybaseutils/pycpp/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-1.0.8/pybaseutils/pycpp/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-1.0.8/pybaseutils/pycpp/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/pybaseutils/pycpp/main.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.153648 pybaseutils-1.0.8/pybaseutils/server/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-07-18 02:35:00.000000 pybaseutils-1.0.8/pybaseutils/server/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2004 2023-07-18 03:25:38.000000 pybaseutils-1.0.8/pybaseutils/server/apm_server.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-1.0.8/pybaseutils/setup_config.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1361 2023-12-26 05:59:47.000000 pybaseutils-1.0.8/pybaseutils/singleton_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7501 2023-12-26 07:29:39.000000 pybaseutils-1.0.8/pybaseutils/thread_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/pybaseutils/time_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/pybaseutils/tracemalloc_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-1.0.8/pybaseutils/tracemalloc_utils2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.157938 pybaseutils-1.0.8/pybaseutils/tracking/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.8/pybaseutils/tracking/QueueTable.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.8/pybaseutils/tracking/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.8/pybaseutils/tracking/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.8/pybaseutils/tracking/kalman_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1787 2023-11-28 10:29:05.000000 pybaseutils-1.0.8/pybaseutils/tracking/mean_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1561 2023-11-28 10:29:05.000000 pybaseutils-1.0.8/pybaseutils/tracking/motion_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      869 2023-11-28 10:29:05.000000 pybaseutils-1.0.8/pybaseutils/tracking/pose_filter.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.160403 pybaseutils-1.0.8/pybaseutils/transforms/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/pybaseutils/transforms/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    22405 2023-12-14 09:09:08.000000 pybaseutils-1.0.8/pybaseutils/transforms/affine_transform.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5112 2024-04-28 11:41:39.000000 pybaseutils-1.0.8/pybaseutils/transforms/face_alignment.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7169 2024-04-30 07:42:15.000000 pybaseutils-1.0.8/pybaseutils/transforms/transform_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-1.0.8/pybaseutils/word_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-1.0.8/pybaseutils/worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-1.0.8/pybaseutils/yaml_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.116572 pybaseutils-1.0.8/pybaseutils.egg-info/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3964 2024-04-30 10:01:00.000000 pybaseutils-1.0.8/pybaseutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6972 2024-04-30 10:01:00.000000 pybaseutils-1.0.8/pybaseutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2024-04-30 10:01:00.000000 pybaseutils-1.0.8/pybaseutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-1.0.8/pybaseutils.egg-info/not-zip-safe
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2024-04-30 10:01:00.000000 pybaseutils-1.0.8/pybaseutils.egg-info/top_level.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2024-04-30 10:01:00.228493 pybaseutils-1.0.8/setup.cfg
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-1.0.8/setup.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.181095 pybaseutils-1.0.8/test_py/
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.182708 pybaseutils-1.0.8/test_py/WebCrawler/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-25 09:17:11.000000 pybaseutils-1.0.8/test_py/WebCrawler/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3615 2023-08-25 09:36:35.000000 pybaseutils-1.0.8/test_py/WebCrawler/search_image.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3183 2023-08-25 09:18:23.000000 pybaseutils-1.0.8/test_py/WebCrawler/search_image_for_baidu.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/test_py/__init__.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.187928 pybaseutils-1.0.8/test_py/aije/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-13 02:52:05.000000 pybaseutils-1.0.8/test_py/aije/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1672 2023-11-10 11:13:57.000000 pybaseutils-1.0.8/test_py/aije/convert_labelme2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1003 2024-03-12 11:20:31.000000 pybaseutils-1.0.8/test_py/aije/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      646 2024-03-15 09:39:47.000000 pybaseutils-1.0.8/test_py/aije/copy_move.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3927 2024-04-15 12:43:54.000000 pybaseutils-1.0.8/test_py/aije/demo_video_aije.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3743 2023-12-12 07:26:52.000000 pybaseutils-1.0.8/test_py/aije/demo_voc_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1948 2024-03-12 11:22:23.000000 pybaseutils-1.0.8/test_py/aije/demo_voc_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2187 2023-10-31 01:05:59.000000 pybaseutils-1.0.8/test_py/aije/video_demo.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.192533 pybaseutils-1.0.8/test_py/audio/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-01 02:27:48.000000 pybaseutils-1.0.8/test_py/audio/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      935 2023-08-04 10:15:41.000000 pybaseutils-1.0.8/test_py/audio/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9241 2023-08-03 04:19:03.000000 pybaseutils-1.0.8/test_py/audio/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1154 2023-08-03 02:53:43.000000 pybaseutils-1.0.8/test_py/audio/main_read.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1269 2023-08-07 09:21:59.000000 pybaseutils-1.0.8/test_py/audio/segment.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    31217 2023-05-10 02:07:39.000000 pybaseutils-1.0.8/test_py/audio/speechbrain_asr_indoor_prod.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4657 2023-08-09 08:17:18.000000 pybaseutils-1.0.8/test_py/audio/speechbrain_demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1296 2023-10-10 06:07:18.000000 pybaseutils-1.0.8/test_py/class_attribute.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-1.0.8/test_py/class_names.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.208430 pybaseutils-1.0.8/test_py/converter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-1.0.8/test_py/converter/AffectNet.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3494 2023-07-19 08:44:04.000000 pybaseutils-1.0.8/test_py/converter/AsianMovie.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3697 2023-08-11 05:35:11.000000 pybaseutils-1.0.8/test_py/converter/BITVehicle2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4581 2023-08-11 05:35:11.000000 pybaseutils-1.0.8/test_py/converter/BSTLD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5581 2023-08-17 02:19:40.000000 pybaseutils-1.0.8/test_py/converter/CCPD.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7029 2023-08-17 02:19:40.000000 pybaseutils-1.0.8/test_py/converter/CCPD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1297 2023-07-13 07:17:07.000000 pybaseutils-1.0.8/test_py/converter/FL3D_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-01 01:02:46.000000 pybaseutils-1.0.8/test_py/converter/FreiHAND2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-18 07:53:20.000000 pybaseutils-1.0.8/test_py/converter/MTFL2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2572 2023-08-11 05:35:11.000000 pybaseutils-1.0.8/test_py/converter/TT100K.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3567 2024-04-30 08:17:22.000000 pybaseutils-1.0.8/test_py/converter/WaterMeters1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3275 2024-04-30 08:02:49.000000 pybaseutils-1.0.8/test_py/converter/WaterMeters2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/test_py/converter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5514 2023-08-17 02:19:40.000000 pybaseutils-1.0.8/test_py/converter/concat_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      842 2023-10-25 08:51:49.000000 pybaseutils-1.0.8/test_py/converter/convert_coco2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1410 2023-09-08 11:04:11.000000 pybaseutils-1.0.8/test_py/converter/convert_gesture2hand.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10536 2023-11-06 10:11:14.000000 pybaseutils-1.0.8/test_py/converter/convert_labelme2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6727 2023-11-08 03:36:12.000000 pybaseutils-1.0.8/test_py/converter/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      726 2023-07-10 09:58:46.000000 pybaseutils-1.0.8/test_py/converter/fatigue_driving.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2321 2023-08-17 02:19:40.000000 pybaseutils-1.0.8/test_py/converter/fdd_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4726 2023-09-01 07:54:12.000000 pybaseutils-1.0.8/test_py/converter/handpose2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1208 2023-08-17 02:19:40.000000 pybaseutils-1.0.8/test_py/converter/insects_for_aichallenger.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-1.0.8/test_py/converter/tt100k_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7596 2023-08-11 05:35:11.000000 pybaseutils-1.0.8/test_py/converter/ua_detrac2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2798 2024-03-18 08:47:50.000000 pybaseutils-1.0.8/test_py/converter/voc_sbd2labelme.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.213391 pybaseutils-1.0.8/test_py/cython_build/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-21 00:54:56.000000 pybaseutils-1.0.8/test_py/cython_build/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      988 2023-12-06 02:17:29.000000 pybaseutils-1.0.8/test_py/cython_build/build_cython.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1464 2023-12-06 09:27:08.000000 pybaseutils-1.0.8/test_py/cython_build/build_pyarmor.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1836 2023-09-22 03:30:02.000000 pybaseutils-1.0.8/test_py/cython_build/cryptography_demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      164 2023-09-20 00:50:56.000000 pybaseutils-1.0.8/test_py/cython_build/fun_sum.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      197 2023-09-20 00:51:59.000000 pybaseutils-1.0.8/test_py/cython_build/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2167 2023-09-22 01:20:56.000000 pybaseutils-1.0.8/test_py/cython_build/model_des_enctypt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2762 2023-09-22 01:35:52.000000 pybaseutils-1.0.8/test_py/cython_build/model_enctypt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1151 2024-04-30 08:52:27.000000 pybaseutils-1.0.8/test_py/demo1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      864 2023-11-10 09:54:32.000000 pybaseutils-1.0.8/test_py/demo2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      983 2023-09-06 06:55:38.000000 pybaseutils-1.0.8/test_py/demo3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-1.0.8/test_py/demo_async_await1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-1.0.8/test_py/demo_async_await2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4875 2024-02-04 11:57:57.000000 pybaseutils-1.0.8/test_py/demo_coco_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5184 2023-08-28 09:18:09.000000 pybaseutils-1.0.8/test_py/demo_copy_files.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2169 2023-07-17 09:29:30.000000 pybaseutils-1.0.8/test_py/demo_copy_files_for_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      913 2023-06-28 11:52:23.000000 pybaseutils-1.0.8/test_py/demo_ffmpy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      719 2024-02-20 06:47:57.000000 pybaseutils-1.0.8/test_py/demo_for_pair_file.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1670 2024-03-01 02:07:11.000000 pybaseutils-1.0.8/test_py/demo_for_polygon.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-1.0.8/test_py/demo_for_trt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4613 2023-12-18 07:46:39.000000 pybaseutils-1.0.8/test_py/demo_get_file_list.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      637 2023-11-27 08:52:43.000000 pybaseutils-1.0.8/test_py/demo_gif.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1742 2024-01-12 07:19:32.000000 pybaseutils-1.0.8/test_py/demo_gif_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1125 2024-03-07 10:19:09.000000 pybaseutils-1.0.8/test_py/demo_image_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      825 2023-08-11 06:37:13.000000 pybaseutils-1.0.8/test_py/demo_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/test_py/demo_metrics.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/test_py/demo_mouse.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      972 2023-07-04 07:11:29.000000 pybaseutils-1.0.8/test_py/demo_nii.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2089 2023-08-11 05:35:11.000000 pybaseutils-1.0.8/test_py/demo_pandas.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-1.0.8/test_py/demo_plot.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1056 2024-04-19 09:16:57.000000 pybaseutils-1.0.8/test_py/demo_rename.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-1.0.8/test_py/demo_standard_image .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1174 2023-09-15 08:45:39.000000 pybaseutils-1.0.8/test_py/demo_standard_video .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/test_py/demo_taichi.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      801 2023-10-17 03:30:20.000000 pybaseutils-1.0.8/test_py/demo_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3600 2023-10-17 07:58:27.000000 pybaseutils-1.0.8/test_py/demo_voc_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2914 2023-11-09 03:13:50.000000 pybaseutils-1.0.8/test_py/demo_voc_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-1.0.8/test_py/demo_word_similar.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-1.0.8/test_py/demo_worker1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/test_py/demo_worker2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.215806 pybaseutils-1.0.8/test_py/detector/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-1.0.8/test_py/detector/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1867 2023-08-11 05:35:01.000000 pybaseutils-1.0.8/test_py/detector/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6707 2023-10-17 07:58:27.000000 pybaseutils-1.0.8/test_py/detector/detect_face_person.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6126 2023-08-17 02:19:40.000000 pybaseutils-1.0.8/test_py/detector/predet_labelme.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.217916 pybaseutils-1.0.8/test_py/edit_distance/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-11-08 06:53:33.000000 pybaseutils-1.0.8/test_py/edit_distance/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1359 2023-11-23 06:50:21.000000 pybaseutils-1.0.8/test_py/edit_distance/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5613 2023-11-10 02:24:56.000000 pybaseutils-1.0.8/test_py/edit_distance/text_matching.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8212 2023-11-10 02:30:01.000000 pybaseutils-1.0.8/test_py/edit_distance/text_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.219994 pybaseutils-1.0.8/test_py/flask_demo/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-1.0.8/test_py/flask_demo/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-1.0.8/test_py/flask_demo/func.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-1.0.8/test_py/flask_demo/server.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.222487 pybaseutils-1.0.8/test_py/image_correction/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-1.0.8/test_py/image_correction/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-1.0.8/test_py/image_correction/demo_correction_v1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5603 2024-02-29 06:08:41.000000 pybaseutils-1.0.8/test_py/image_correction/demo_correction_v2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-1.0.8/test_py/image_correction/demo_correction_v3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-1.0.8/test_py/kafka_worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-1.0.8/test_py/men_tracemalloc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-1.0.8/test_py/performance.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.223906 pybaseutils-1.0.8/test_py/pose/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:28:44.000000 pybaseutils-1.0.8/test_py/pose/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1530 2023-09-11 07:32:44.000000 pybaseutils-1.0.8/test_py/pose/human_pose.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:01:00.227342 pybaseutils-1.0.8/test_py/registry/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-07 01:10:07.000000 pybaseutils-1.0.8/test_py/registry/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1195 2023-09-07 05:56:01.000000 pybaseutils-1.0.8/test_py/registry/base.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3057 2023-09-07 02:42:07.000000 pybaseutils-1.0.8/test_py/registry/component.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1701 2023-09-07 04:32:01.000000 pybaseutils-1.0.8/test_py/registry/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1093 2023-09-07 05:50:04.000000 pybaseutils-1.0.8/test_py/registry/register.py
```

### Comparing `pybaseutils-1.0.7/LICENCE` & `pybaseutils-1.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/PKG-INFO` & `pybaseutils-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 1.0.7
+Version: 1.0.8
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENCE
```

### Comparing `pybaseutils-1.0.7/README.md` & `pybaseutils-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/audio/audio_utils.py` & `pybaseutils-1.0.8/pybaseutils/audio/audio_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/audio/pyaudio_utils.py` & `pybaseutils-1.0.8/pybaseutils/audio/pyaudio_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/audio/vad_utils.py` & `pybaseutils-1.0.8/pybaseutils/audio/vad_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/base64_utils.py` & `pybaseutils-1.0.8/pybaseutils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/batch_utils.py` & `pybaseutils-1.0.8/pybaseutils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/build_utils/cython_utils.py` & `pybaseutils-1.0.8/pybaseutils/build_utils/cython_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/build_utils/pyarmor_utils.py` & `pybaseutils-1.0.8/pybaseutils/build_utils/pyarmor_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/cluster/kmean.py` & `pybaseutils-1.0.8/pybaseutils/cluster/kmean.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/cluster/maxmin_distance.py` & `pybaseutils-1.0.8/pybaseutils/cluster/maxmin_distance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/cluster/similarity.py` & `pybaseutils-1.0.8/pybaseutils/cluster/similarity.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/color_utils.py` & `pybaseutils-1.0.8/pybaseutils/color_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/config_utils.py` & `pybaseutils-1.0.8/pybaseutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/build_coco.py` & `pybaseutils-1.0.8/pybaseutils/converter/build_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/build_labelme.py` & `pybaseutils-1.0.8/pybaseutils/converter/build_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/build_voc.py` & `pybaseutils-1.0.8/pybaseutils/converter/build_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/concat_coco.py` & `pybaseutils-1.0.8/pybaseutils/converter/concat_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/convert_coco2labelme.py` & `pybaseutils-1.0.8/pybaseutils/converter/convert_coco2labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/convert_coco2voc.py` & `pybaseutils-1.0.8/pybaseutils/converter/convert_coco2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/convert_labelme2coco.py` & `pybaseutils-1.0.8/pybaseutils/converter/convert_labelme2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/convert_labelme2voc.py` & `pybaseutils-1.0.8/pybaseutils/converter/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/convert_labelme2yolo.py` & `pybaseutils-1.0.8/pybaseutils/converter/convert_labelme2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/convert_voc2coco.py` & `pybaseutils-1.0.8/pybaseutils/converter/convert_voc2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/convert_voc2labelme.py` & `pybaseutils-1.0.8/pybaseutils/converter/convert_voc2labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/convert_voc2voc.py` & `pybaseutils-1.0.8/pybaseutils/converter/convert_voc2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/convert_voc2yolo.py` & `pybaseutils-1.0.8/pybaseutils/converter/convert_voc2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/converter/convert_yolo2voc.py` & `pybaseutils-1.0.8/pybaseutils/converter/convert_yolo2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/coords_utils.py` & `pybaseutils-1.0.8/pybaseutils/coords_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/cvutils/corner_utils.py` & `pybaseutils-1.0.8/pybaseutils/cvutils/corner_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         corners = cv2.approxPolyDP(contour, epsilon, closed=True)
         corners = corners.reshape(-1, 2)
         k += 1
         if log: print(f"k={k},corners={len(corners)},epsilon={epsilon}")
     return corners
 
 
-def get_target_points(src_pts: np.ndarray):
+def get_target_points(src_pts: np.ndarray, method=0):
     """
     根据输入的四个角点，计算其矫正后的目标四个角点,src_pts四个点分布：
         0--(w01)---1
         |          |
       (h03)      (h21)
         |          |
         3--(w23)---2
```

### Comparing `pybaseutils-1.0.7/pybaseutils/cvutils/monitor.py` & `pybaseutils-1.0.8/pybaseutils/cvutils/monitor.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/cvutils/mouse_utils.py` & `pybaseutils-1.0.8/pybaseutils/cvutils/mouse_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/cvutils/video_utils.py` & `pybaseutils-1.0.8/pybaseutils/cvutils/video_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/dataloader/base_coco.py` & `pybaseutils-1.0.8/pybaseutils/dataloader/base_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/dataloader/base_dataset.py` & `pybaseutils-1.0.8/pybaseutils/dataloader/base_dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     @Brief  :
 """
 import os
 import numpy as np
 import cv2
 import glob
 import random
+from pybaseutils import file_utils, json_utils
 
 VOC_NAMES = ["aeroplane", "bicycle", "bird", "boat", "bottle", "bus", "car", "cat",
              "chair", "cow", "diningtable", "dog", "horse", "motorbike", "person",
              "pottedplant", "sheep", "sofa", "train", "tvmonitor"]
 
 COCO_NAMES = ['background', 'person', 'bicycle', 'car', 'motorcycle', 'airplane', 'bus', 'train',
               'truck', 'boat', 'traffic light', 'fire hydrant', 'stop sign',
@@ -33,24 +34,55 @@
     """
     from torch.utils.data import Dataset,DataLoader, ConcatDataset
     """
 
     def __init__(self, **kwargs):
         self.image_ids = []
         self.postfix = "jpg"
+        self.unique = False  # 是否是单一label，如["BACKGROUND", "unique"]
 
     def __getitem__(self, index):
         raise NotImplementedError
 
     def __add__(self, other):
         return ConcatDataset([self, other])
 
     def __len__(self):
         raise NotImplementedError
 
+    def parser_classes(self, class_name):
+        """
+        class_dict = {class_name: i for i, class_name in enumerate(class_name)}
+        :param class_name:
+                    str : class file
+                    list: ["face","person"]
+                    dict: 可以自定义label的id{'BACKGROUND': 0, 'person': 1, 'person_up': 1, 'person_down': 1}
+        :return:
+        """
+        if isinstance(class_name, str):
+            class_name = Dataset.read_files(class_name)
+        elif isinstance(class_name, list) and "unique" in class_name:
+            self.unique = True
+        if isinstance(class_name, list) and len(class_name) > 0:
+            class_dict = {}
+            for i, name in enumerate(class_name):
+                name = name.split(",")
+                for n in name: class_dict[n] = i
+        elif isinstance(class_name, dict) and len(class_name) > 0:
+            class_dict = class_name
+        else:
+            class_dict = None
+        if class_dict:
+            class_dict = json_utils.dict_sort_by_value(class_dict, reverse=False)
+            class_name = {}
+            for n, i in class_dict.items():
+                class_name[i] = "{},{}".format(class_name[i], n) if i in class_name else n
+            class_name = list(class_name.values())
+        return class_name, class_dict
+
     @staticmethod
     def read_files(filename, split=None):
         """
         :param filename:
         :param split:分割
         :return:
         """
```

### Comparing `pybaseutils-1.0.7/pybaseutils/dataloader/parser_coco_det.py` & `pybaseutils-1.0.8/pybaseutils/dataloader/parser_coco_det.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/dataloader/parser_coco_ins.py` & `pybaseutils-1.0.8/pybaseutils/dataloader/parser_coco_ins.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/dataloader/parser_coco_kps.py` & `pybaseutils-1.0.8/pybaseutils/dataloader/parser_coco_kps.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/dataloader/parser_labelme.py` & `pybaseutils-1.0.8/pybaseutils/dataloader/parser_labelme.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,38 +67,14 @@
         print("Dataset num images    :{}".format(len(self.image_ids)))
         # print("Dataset num_classes   :{}".format(self.num_classes))
         print("------" * 10)
 
     def __len__(self):
         return len(self.image_ids)
 
-    def parser_classes(self, class_name):
-        """
-        class_dict = {class_name: i for i, class_name in enumerate(class_name)}
-        :param class_name:
-                    str : class file
-                    list: ["face","person"]
-                    dict: 可以自定义label的id{'BACKGROUND': 0, 'person': 1, 'person_up': 1, 'person_down': 1}
-        :return:
-        """
-        if isinstance(class_name, str):
-            class_name = super().read_files(class_name)
-        elif isinstance(class_name, numbers.Number):
-            class_name = [str(i) for i in range(int(class_name))]
-        elif isinstance(class_name, list) and "unique" in class_name:
-            self.unique = True
-        if isinstance(class_name, list):
-            class_dict = {str(name): str(name) for name in class_name}
-        elif isinstance(class_name, dict):
-            class_dict = class_name
-            class_name = list(class_dict.keys())
-        else:
-            class_dict = None
-        return class_name, class_dict
-
     def get_image_anno_file(self, index):
         """
         :param index:
         :return:
         """
         image_id = self.index2id(index)
         image_file, annotation_file, image_id = self.__get_image_anno_file(self.image_dir,
@@ -183,31 +159,31 @@
         """
         image_id = self.index2id(index)
         image_file, anno_file, image_id = self.get_image_anno_file(image_id)
         annotation, width, height = self.load_annotations(anno_file)
         image = self.read_image(image_file, use_rgb=self.use_rgb)
         shape = image.shape
         boxes, labels, points, groups = self.parser_annotation(annotation, self.class_dict, shape,
-                                                               min_points=self.min_points)
+                                                               min_points=self.min_points, unique=self.unique)
         data = {"image": image, "points": points, "boxes": boxes, "labels": labels, "groups": groups,
                 "image_file": image_file, "anno_file": anno_file, "size": [shape[1], shape[0]]}
         return data
 
     @staticmethod
-    def parser_annotation(annotation: dict, class_dict={}, shape=None, min_points=-1):
+    def parser_annotation(annotation: dict, class_dict={}, shape=None, min_points=-1, unique=False):
         """
         :param annotation:  labelme标注的数据
         :param class_dict:  label映射
         :param shape: 图片shape(H,W,C),可进行坐标点的维度检查，避免越界
         :param min_points: 当标注的轮廓点的个数小于等于min_points，会被剔除；负数不剔除
         :return:
         """
         bboxes, labels, points, groups = [], [], [], []
         for anno in annotation:
-            label = anno["label"]
+            label = "unique" if unique else anno["label"]
             if class_dict:
                 if not label in class_dict:
                     continue
                 if isinstance(class_dict, dict):
                     label = class_dict[label]
             pts = np.asarray(anno["points"], dtype=np.int32)
             if min_points > 0 and len(pts) <= min_points:
@@ -410,16 +386,23 @@
 if __name__ == "__main__":
     from pybaseutils.converter import build_labelme
 
     anno_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-indoor-det/dataset-v1/json"
     anno_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-indoor-det/dataset-v7/json"
     anno_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/使用钳形电流表测量低压线路电流/dataset-v1/json"
     # anno_dir = [anno_dir, anno_dir]
-    # names = None
-    names = ['A相电线','B相电线','C相电线','N相电线']
+    names = ['A相电线', 'B相电线', 'C相电线', 'N相电线']
+
+    anno_dir = "/home/PKing/nasdata/tmp/tmp/水表数字识别/水表数据集/Water-Meter-Det1/train/json"
+    # anno_dir = "/media/PKing/新加卷1/SDK/base-utils/data/coco/json"
+    # # names = ["car", "dog", "person", "unique"]
+    names = ["BG", "unique"]
+    # # names = ["car", "dog", "person"]
+    # # names = ["dog", "car,person"]
+    # # names = {"car": 1, "person": 0}
     dataset = LabelMeDatasets(filename=None,
                               data_root=None,
                               anno_dir=anno_dir,
                               image_dir=None,
                               class_name=names,
                               check=False,
                               phase="val",
```

### Comparing `pybaseutils-1.0.7/pybaseutils/dataloader/parser_voc.py` & `pybaseutils-1.0.8/pybaseutils/dataloader/parser_voc.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         :param anno_dir:
         :param image_dir:
         :param transform:
         :param use_rgb:
         :param shuffle:
         """
         super(VOCDataset, self).__init__()
-        self.unique = False  # 是否是单一label，如["BACKGROUND", "unique"]
         self.class_name, self.class_dict = self.parser_classes(class_name)
         parser = self.parser_paths(filename, data_root, anno_dir, image_dir)
         self.data_root, self.anno_dir, self.image_dir, self.image_ids = parser
         self.seg_dir = seg_dir
         if check or (self.class_dict is None):
             self.image_ids = self.checking(self.image_ids, class_dict=self.class_dict)
         self.transform = transform
@@ -116,43 +115,14 @@
         if not class_dict:
             print("class_name is None, Dataset will auto get class_set :{}".format(class_set))
             self.class_name = class_set
             self.class_dict = {class_name: i for i, class_name in enumerate(class_set)}
         print("have nums image:{},legal image:{}".format(len(image_ids), len(dst_ids)))
         return dst_ids
 
-    def parser_classes(self, class_name):
-        """
-        class_dict = {class_name: i for i, class_name in enumerate(class_name)}
-        :param class_name:
-                    str : class file
-                    list: ["face","person"]
-                    dict: 可以自定义label的id{'BACKGROUND': 0, 'person': 1, 'person_up': 1, 'person_down': 1}
-        :return:
-        """
-        if isinstance(class_name, str):
-            class_name = Dataset.read_files(class_name)
-        elif isinstance(class_name, list) and "unique" in class_name:
-            self.unique = True
-        if isinstance(class_name, list) and len(class_name) > 0:
-            class_dict = {}
-            for i, name in enumerate(class_name):
-                name = name.split(",")
-                for n in name: class_dict[n] = i
-        elif isinstance(class_name, dict) and len(class_name) > 0:
-            class_dict = class_name
-        else:
-            class_dict = None
-        if class_dict:
-            class_name = {}
-            for n, i in class_dict.items():
-                class_name[i] = "{},{}".format(class_name[i], n) if i in class_name else n
-            class_name = list(class_name.values())
-        return class_name, class_dict
-
     def parser_paths(self, filename=None, data_root=None, anno_dir=None, image_dir=None):
         """
         :param filename:
         :param data_root:
         :param anno_dir:
         :param image_dir:
         :return:
@@ -276,15 +246,15 @@
             objects = []
             width = None
             height = None
         objects_list = []
         if not isinstance(objects, list):
             objects = [objects]
         for object in objects:
-            name = str(object["name"]) if not self.unique else "unique"
+            name = "unique" if self.unique else str(object["name"])
             name = "BACKGROUND" if str(object["name"]) == 'BACKGROUND' else name
             if self.class_dict and name not in self.class_dict:
                 continue
             difficult = int(object["difficult"]) if 'difficult' in object else 0
             xmin = float(object["bndbox"]["xmin"])
             xmax = float(object["bndbox"]["xmax"])
             ymin = float(object["bndbox"]["ymin"])
@@ -434,15 +404,17 @@
     image_utils.cv_show_image("image", image, delay=0, use_rgb=use_rgb)
     return image
 
 
 if __name__ == "__main__":
     # from models.transforms import data_transforms
     filename = '/media/PKing/新加卷1/SDK/base-utils/data/coco/file_list.txt'
-    class_name = None
+    # class_name = ["car", "person"]
+    class_name = ["car,person"]
+    # class_name = {"car": 1, "person": 0}
     dataset = VOCDatasets(filename=[filename, filename],
                           data_root=None,
                           image_dir=None,
                           anno_dir=None,
                           class_name=class_name,
                           transform=None,
                           check=False,
```

### Comparing `pybaseutils-1.0.7/pybaseutils/dataloader/parser_yolo.py` & `pybaseutils-1.0.8/pybaseutils/dataloader/parser_yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/dataloader/voc_seg_utils.py` & `pybaseutils-1.0.8/pybaseutils/dataloader/voc_seg_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/file_utils.py` & `pybaseutils-1.0.8/pybaseutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/filter/QueueTable.py` & `pybaseutils-1.0.8/pybaseutils/filter/QueueTable.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/filter/demo.py` & `pybaseutils-1.0.8/pybaseutils/filter/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/filter/kalman_filter.py` & `pybaseutils-1.0.8/pybaseutils/filter/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/filter/mean_filter.py` & `pybaseutils-1.0.8/pybaseutils/filter/mean_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/filter/motion_filter.py` & `pybaseutils-1.0.8/pybaseutils/filter/motion_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/filter/pose_filter.py` & `pybaseutils-1.0.8/pybaseutils/filter/pose_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/font_style/__init__.py` & `pybaseutils-1.0.8/pybaseutils/font_style/__init__.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/font_utils.py` & `pybaseutils-1.0.8/pybaseutils/font_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/geometry_tools.py` & `pybaseutils-1.0.8/pybaseutils/geometry_tools.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/heatmap_utils.py` & `pybaseutils-1.0.8/pybaseutils/heatmap_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/image_utils.py` & `pybaseutils-1.0.8/pybaseutils/image_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2465,15 +2465,15 @@
     xmin = max(0, int(xmin - shift))
     ymin = max(0, int(ymin - shift))
     xmax = min(w, int(xmax + shift))
     ymax = min(h, int(ymax + shift))
     return [xmin, ymin, xmax, ymax]
 
 
-def find_mask_contours(mask, mode=cv2.RETR_LIST, method=cv2.CHAIN_APPROX_NONE):
+def find_mask_contours(mask, max_nums=-1, mode=cv2.RETR_LIST, method=cv2.CHAIN_APPROX_NONE):
     """
     寻找一个二值Mask图像的轮廓
     cv2.findContours(mask，mode, method)
     mask: 输入mask必须是二值Mask图像，注意黑色表示背景，白色表示物体，即在黑色背景里寻找白色物体的轮廓
     mode:
         cv.RETR_LIST: 提取所有轮廓
         cv.RETR_EXTERNAL: 只提取外轮廓（可能有多个外轮廓，只是不提取孔轮廓）
@@ -2481,31 +2481,38 @@
         cv.RETR_CCOMP: 提取所有轮廓，把它们组织成两级结构。
                     第一级是连通域的外边界(external boundaries)，
                     第二级是孔边界(boundaries of holes)。如果在孔中间还有另外的连通域，则被当成另一个外边界
     method:
         CHAIN_APPROX_NONE  :存储所有的轮廓点
         CHAIN_APPROX_SIMPLE:压缩水平，垂直和对角线段，只留下端点,例如矩形轮廓可以用4个点编码。
     :param mask: 输入mask必须是二值Mask图像，注意黑色表示背景，白色表示物体，即在黑色背景里寻找白色物体的轮廓
+    :param max_nums: 按照面积大小进行排序，返回max_nums个轮廓
     :return: contours List[np.ndarray(num_point,2)] 返回二值Mask图像的轮廓
     """
     contours, hierarchy = cv2.findContours(mask, mode=mode, method=method)
     contours = [c.reshape(-1, 2) for c in contours]
+    # contours = sorted(contours, key=lambda c: cv2.contourArea(c), reverse=True)
+    contours = sorted(contours, key=lambda c: len(c), reverse=True)
+    if max_nums > 0:
+        max_nums = min(max_nums, len(contours))
+        contours = contours[0:max_nums]
     return contours
 
 
-def find_minAreaRect(contours, order=False):
+def find_minAreaRect(contours, order=True):
     """
     获得旋转矩形框，即最小外接矩形的四个角点
     :param contours: [shape(n,2),...,]
+    :param order: 对4个点按顺时针方向进行排序:[top-left, top-right, bottom-right, bottom-left]
     :return:
     """
     points = []
     for i in range(len(contours)):
         # 得到最小外接矩形的（中心(x,y), (宽,高), 旋转角度）
-        rotatedRect = cv2.minAreaRect(contours[i])  # [center, wh, angle]==>[Point2f, Size, float]
+        rotatedRect = cv2.minAreaRect(np.array(contours[i],dtype=np.int32))  # [center, wh, angle]==>[Point2f, Size, float]
         pts = cv2.boxPoints(rotatedRect)  # 获取最小外接矩形的4个顶点坐标
         pts = pts[[1, 2, 3, 0], :]
         if order:
             pts = corner_utils.get_order_points(pts)
             # pts2 = corner_utils.order_points_clockwise(pts)
         points.append(pts)
     return points
```

### Comparing `pybaseutils-1.0.7/pybaseutils/json_utils.py` & `pybaseutils-1.0.8/pybaseutils/json_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,25 @@
 class Dict2Obj(object):
     """ dict转类对象"""
 
     def __init__(self, args):
         self.__dict__.update(args)
 
 
+def dict_sort_by_value(data: Dict, reverse=False):
+    """
+    按照字典的value值排序
+    :param src:
+    :param reverse: False 升序
+                    True  降序
+    """
+    dst = dict(sorted(data.items(), key=lambda x: x[1], reverse=reverse))
+    return dst
+
+
 def formatting(content):
     """格式化json数据"""
     info = json.dumps(content, indent=1, separators=(', ', ': '), ensure_ascii=False)
     return info
 
 
 def get_keys_vaules(content, func=None):
@@ -74,14 +85,15 @@
 def set_values(content, keys, values):
     """根据keys路径设置对应的值"""
     for k, v in zip(keys, values):
         content = toolz_assoc_in(content, keys=k, value=v)
         # data = toolz.assoc_in(data, keys=k, value=v)
     return content
 
+
 def set_value(content, key, value):
     """根据keys路径设置对应的值"""
     # content = toolz_assoc_in(content, keys=key, value=value)
     content = toolz.assoc_in(content, keys=key, value=value)
     return content
 
 
@@ -121,14 +133,14 @@
     keys, values = get_keys_vaules(content, func=func)
     for k, v in zip(keys, values):
         print("path={}\t    value={}".format(k, v))
     print("===" * 20)
     # toolz使用toolz工具或得所有keys的值,values1与values的值是一样的
     # values1 = get_values(content, keys=keys)
     # values1 = get_values(content, keys=[['data1', 'image', 1], ['data', 'file', 'file11']])
-    values1 = get_value(None, key=['data', 'image', 1],default={"data"})
+    values1 = get_value(None, key=['data', 'image', 1], default={"data"})
     print(values1)
     print("===" * 20)
     values = list(range(len(values)))
     content = set_values(content, keys=keys, values=values)
     print(formatting(content))
     print("===" * 20)
```

### Comparing `pybaseutils-1.0.7/pybaseutils/log.py` & `pybaseutils-1.0.8/pybaseutils/log.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/logger.py` & `pybaseutils-1.0.8/pybaseutils/logger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/metrics/accuracy.py` & `pybaseutils-1.0.8/pybaseutils/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/metrics/average_meter.py` & `pybaseutils-1.0.8/pybaseutils/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/metrics/class_report.py` & `pybaseutils-1.0.8/pybaseutils/metrics/class_report.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/metrics/plot_pr.py` & `pybaseutils-1.0.8/pybaseutils/metrics/plot_pr.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/metrics/plot_roc.py` & `pybaseutils-1.0.8/pybaseutils/metrics/plot_roc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/numpy_utils.py` & `pybaseutils-1.0.8/pybaseutils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/pandas_utils.py` & `pybaseutils-1.0.8/pybaseutils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/plot_utils.py` & `pybaseutils-1.0.8/pybaseutils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/pose/bones_utils.py` & `pybaseutils-1.0.8/pybaseutils/pose/bones_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/pose/human_pose.py` & `pybaseutils-1.0.8/pybaseutils/pose/human_pose.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/pose/pose_utils.py` & `pybaseutils-1.0.8/pybaseutils/pose/pose_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/pycpp/demo.py` & `pybaseutils-1.0.8/pybaseutils/pycpp/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/pycpp/main.py` & `pybaseutils-1.0.8/pybaseutils/pycpp/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/server/apm_server.py` & `pybaseutils-1.0.8/pybaseutils/server/apm_server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/setup_config.py` & `pybaseutils-1.0.8/pybaseutils/setup_config.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/singleton_utils.py` & `pybaseutils-1.0.8/pybaseutils/singleton_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/thread_utils.py` & `pybaseutils-1.0.8/pybaseutils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/time_utils.py` & `pybaseutils-1.0.8/pybaseutils/time_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/tracemalloc_utils.py` & `pybaseutils-1.0.8/pybaseutils/tracemalloc_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/tracemalloc_utils2.py` & `pybaseutils-1.0.8/pybaseutils/tracemalloc_utils2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/tracking/QueueTable.py` & `pybaseutils-1.0.8/pybaseutils/tracking/QueueTable.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/tracking/demo.py` & `pybaseutils-1.0.8/pybaseutils/tracking/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/tracking/kalman_filter.py` & `pybaseutils-1.0.8/pybaseutils/tracking/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/tracking/mean_filter.py` & `pybaseutils-1.0.8/pybaseutils/tracking/mean_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/tracking/motion_filter.py` & `pybaseutils-1.0.8/pybaseutils/tracking/motion_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/tracking/pose_filter.py` & `pybaseutils-1.0.8/pybaseutils/tracking/pose_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/transforms/affine_transform.py` & `pybaseutils-1.0.8/pybaseutils/transforms/affine_transform.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/transforms/face_alignment.py` & `pybaseutils-1.0.8/pybaseutils/transforms/face_alignment.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/transforms/transform_utils.py` & `pybaseutils-1.0.8/pybaseutils/transforms/transform_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         xmin = min(dst_pts[:, 0])
         ymin = min(dst_pts[:, 1])
         xmax = max(dst_pts[:, 0])
         ymax = max(dst_pts[:, 1])
         tsize = (xmax - xmin, ymax - ymin)
     else:
         tsize = (w, h)
-    if dsize[0] < 0 or dsize[1] < 0:
+    if dsize is None or (dsize[0] < 0 or dsize[1] < 0):
         dsize = tsize
     # 映射居中
     tsize = np.array(tsize)
     dsize = np.array(dsize)
     dst_pts = np.array(dst_pts)
     diff = dsize - tsize
     dst_pts = dst_pts + diff / 2.
@@ -176,23 +176,26 @@
     Minv = Minv[0:2, :]
     return Minv
 
 
 def test_transform(image_file):
     from pybaseutils import image_utils
     src = cv2.imread(image_file)
+    # src[:, :] = 0
     mask = image_utils.get_image_mask(src)
-    contours = image_utils.find_mask_contours(mask)
+    contours = image_utils.find_mask_contours(mask, max_nums=1)
     src_pts = image_utils.find_minAreaRect(contours, order=True)
+    dst = src.copy()
+    dst_pts = []
     if len(src_pts) > 0:
         src_pts = src_pts[0]
-        dst, dst_pts, M, Minv = image_alignment(src, src_pts, dsize=(-1, -1), scale=(1.2, 1.2))
-        src = image_utils.draw_image_contours(src, contours)
-        src = image_utils.draw_landmark(src, [src_pts], color=(255, 0, 0), vis_id=True)
-        dst = image_utils.draw_landmark(dst, [dst_pts], color=(0, 255, 0), vis_id=True)
-        image_utils.cv_show_image("src", src, delay=10)
-        image_utils.cv_show_image("dst", dst, delay=0)
+        dst, dst_pts, M, Minv = image_alignment(dst, src_pts, dsize=(-1, -1), scale=(1.2, 1.2))
+    src = image_utils.draw_image_contours(src, [src_pts])
+    src = image_utils.draw_landmark(src, [src_pts], color=(255, 0, 0), vis_id=True)
+    dst = image_utils.draw_landmark(dst, [dst_pts], color=(0, 255, 0), vis_id=True)
+    image_utils.cv_show_image("src", src, delay=10)
+    image_utils.cv_show_image("dst", dst, delay=0)
 
 
 if __name__ == '__main__':
-    image_file = "../../data/mask/mask5.jpg"
+    image_file = "../../data/mask/mask4.jpg"
     test_transform(image_file)
```

### Comparing `pybaseutils-1.0.7/pybaseutils/word_utils.py` & `pybaseutils-1.0.8/pybaseutils/word_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/worker.py` & `pybaseutils-1.0.8/pybaseutils/worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils/yaml_utils.py` & `pybaseutils-1.0.8/pybaseutils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/pybaseutils.egg-info/PKG-INFO` & `pybaseutils-1.0.8/pybaseutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 1.0.7
+Version: 1.0.8
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENCE
```

### Comparing `pybaseutils-1.0.7/pybaseutils.egg-info/SOURCES.txt` & `pybaseutils-1.0.8/pybaseutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,16 @@
 test_py/converter/BSTLD2voc.py
 test_py/converter/CCPD.py
 test_py/converter/CCPD2voc.py
 test_py/converter/FL3D_dataset.py
 test_py/converter/FreiHAND2coco.py
 test_py/converter/MTFL2voc.py
 test_py/converter/TT100K.py
-test_py/converter/WaterMeters.py
+test_py/converter/WaterMeters1.py
+test_py/converter/WaterMeters2.py
 test_py/converter/__init__.py
 test_py/converter/concat_coco.py
 test_py/converter/convert_coco2voc.py
 test_py/converter/convert_gesture2hand.py
 test_py/converter/convert_labelme2coco.py
 test_py/converter/convert_labelme2voc.py
 test_py/converter/fatigue_driving.py
```

### Comparing `pybaseutils-1.0.7/setup.py` & `pybaseutils-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/WebCrawler/search_image.py` & `pybaseutils-1.0.8/test_py/WebCrawler/search_image.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/WebCrawler/search_image_for_baidu.py` & `pybaseutils-1.0.8/test_py/WebCrawler/search_image_for_baidu.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/aije/convert_labelme2coco.py` & `pybaseutils-1.0.8/test_py/aije/convert_labelme2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/aije/convert_labelme2voc.py` & `pybaseutils-1.0.8/test_py/aije/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/aije/copy_move.py` & `pybaseutils-1.0.8/test_py/aije/copy_move.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/aije/demo_video_aije.py` & `pybaseutils-1.0.8/test_py/aije/demo_video_aije.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/aije/demo_voc_crop.py` & `pybaseutils-1.0.8/test_py/aije/demo_voc_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/aije/demo_voc_vis.py` & `pybaseutils-1.0.8/test_py/aije/demo_voc_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/aije/video_demo.py` & `pybaseutils-1.0.8/test_py/aije/video_demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/audio/demo.py` & `pybaseutils-1.0.8/test_py/audio/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/audio/main.py` & `pybaseutils-1.0.8/test_py/audio/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/audio/main_read.py` & `pybaseutils-1.0.8/test_py/audio/main_read.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/audio/segment.py` & `pybaseutils-1.0.8/test_py/audio/segment.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/audio/speechbrain_asr_indoor_prod.py` & `pybaseutils-1.0.8/test_py/audio/speechbrain_asr_indoor_prod.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/audio/speechbrain_demo.py` & `pybaseutils-1.0.8/test_py/audio/speechbrain_demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/class_attribute.py` & `pybaseutils-1.0.8/test_py/class_attribute.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/class_names.py` & `pybaseutils-1.0.8/test_py/class_names.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/AffectNet.py` & `pybaseutils-1.0.8/test_py/converter/AffectNet.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/AsianMovie.py` & `pybaseutils-1.0.8/test_py/converter/AsianMovie.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/BITVehicle2voc.py` & `pybaseutils-1.0.8/test_py/converter/BITVehicle2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/BSTLD2voc.py` & `pybaseutils-1.0.8/test_py/converter/BSTLD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/CCPD.py` & `pybaseutils-1.0.8/test_py/converter/CCPD.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/CCPD2voc.py` & `pybaseutils-1.0.8/test_py/converter/CCPD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/FL3D_dataset.py` & `pybaseutils-1.0.8/test_py/converter/FL3D_dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/MTFL2voc.py` & `pybaseutils-1.0.8/test_py/converter/MTFL2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/TT100K.py` & `pybaseutils-1.0.8/test_py/converter/TT100K.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/WaterMeters.py` & `pybaseutils-1.0.8/test_py/converter/WaterMeters2.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     @Brief  :
 """
 import os
 import cv2
 import numpy as np
 from tqdm import tqdm
 from pybaseutils import image_utils, file_utils
+from pybaseutils.converter import build_labelme
 from pybaseutils.transforms import transform_utils
 from pybaseutils.converter import build_voc
 
 
 def load_annotation(image_file, lable_file):
     image = image_utils.read_image(image_file)
     annos = file_utils.read_data(lable_file, split=" ", convertNum=False)
@@ -21,40 +22,47 @@
     point = [int(i) for i in annos[0:8]]
     point = np.asarray(point).reshape(-1, 2)
     label = annos[8]
     boxes = image_utils.polygons2boxes([point])
     return image, point, label, boxes
 
 
-def WaterMeters(image_dir, label_dir, out_root, use_align=False, vis=True):
-    if out_root: file_utils.create_dir(out_root)
+def WaterMeters(image_dir, label_dir, out_json, crop_root=None, use_align=False, vis=True, delay=10):
+    if crop_root: file_utils.create_dir(crop_root)
+    if out_json: file_utils.create_dir(out_json)
     file_list = file_utils.get_files_lists(image_dir, sub=True)
     for i, image_name in tqdm(enumerate(file_list)):
         postfix = image_name.split(".")[-1]
         lable_name = image_name.replace(f".{postfix}", ".txt")
+        json_name = image_name.replace(f".{postfix}", ".json")
         image_file = os.path.join(image_dir, image_name)
         lable_file = os.path.join(label_dir, lable_name)
         image, point, label, boxes = load_annotation(image_file, lable_file)
-        if use_align:
+        image_h, image_w = image.shape[:2]
+        if crop_root and use_align:
             dst_pts = transform_utils.get_target_corner_points(point)
             crop, M, Minv = transform_utils.get_image_alignment(image, src_pts=point, dst_pts=dst_pts, dsize=None,
                                                                 method="lstsq")
-            crop_file = os.path.join(out_root, "{}_{:0=5d}_alignment.jpg".format(label, i))
+            crop_file = os.path.join(crop_root, "{}_{:0=5d}_alignment.jpg".format(label, i))
             cv2.imwrite(crop_file, crop)
-        else:
+        elif crop_root:
             crop = image_utils.get_bbox_crop(image, bbox=boxes[0])
-            crop_file = os.path.join(out_root, "{}_{:0=5d}_crop.jpg".format(label, i))
+            crop_file = os.path.join(crop_root, "{}_{:0=5d}_crop.jpg".format(label, i))
             h, w = crop.shape[:2]
             if w > 3 * h: cv2.imwrite(crop_file, crop)
+        json_file = os.path.join(out_json, json_name)
+        build_labelme.maker_labelme(json_file, points=[point], labels=[label],
+                                    image_name=image_name, image_size=(image_w, image_h))
         if vis:
             image = image_utils.draw_image_bboxes_text(image, boxes, boxes_name=[label])
             image = image_utils.draw_key_point_in_image(image, [point], vis_id=True)
-            image_utils.cv_show_image("crop", crop, delay=10)
-            image_utils.cv_show_image("image", image)
+            # image_utils.cv_show_image("crop", crop, delay=10)
+            image_utils.cv_show_image("image", image, delay=delay)
     return
 
 
 if __name__ == '__main__':
-    label_dir = "/home/PKing/nasdata/dataset/tmp/水表数字识别/水表读数自动识别数据集/Water-Meter-v1/zip/val_gts"
-    image_dir = "/home/PKing/nasdata/dataset/tmp/水表数字识别/水表读数自动识别数据集/Water-Meter-v1/zip/val_imgs"
-    out_root = "/home/PKing/nasdata/dataset/tmp/水表数字识别/水表读数自动识别数据集/Water-Meter-v1/labels/val"
-    WaterMeters(image_dir, label_dir, out_root=out_root, vis=False)
+    image_dir = "/home/PKing/nasdata/tmp/tmp/水表数字识别/水表数据集/Water-Meter-Det1/val/images"
+    label_dir = "/home/PKing/nasdata/tmp/tmp/水表数字识别/水表数据集/Water-Meter-Det1/val/labels"
+    crop_root = "/home/PKing/nasdata/tmp/tmp/水表数字识别/水表数据集/Water-Meter-Det1/val/crop"
+    out_json = "/home/PKing/nasdata/tmp/tmp/水表数字识别/水表数据集/Water-Meter-Det1/val/json"
+    WaterMeters(image_dir, label_dir, out_json=out_json, crop_root=None, vis=True)
```

### Comparing `pybaseutils-1.0.7/test_py/converter/concat_coco.py` & `pybaseutils-1.0.8/test_py/converter/concat_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/convert_coco2voc.py` & `pybaseutils-1.0.8/test_py/converter/convert_coco2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/convert_gesture2hand.py` & `pybaseutils-1.0.8/test_py/converter/convert_gesture2hand.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/convert_labelme2coco.py` & `pybaseutils-1.0.8/test_py/converter/convert_labelme2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/convert_labelme2voc.py` & `pybaseutils-1.0.8/test_py/converter/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/fatigue_driving.py` & `pybaseutils-1.0.8/test_py/converter/fatigue_driving.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/fdd_dataset.py` & `pybaseutils-1.0.8/test_py/converter/fdd_dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/handpose2coco.py` & `pybaseutils-1.0.8/test_py/converter/handpose2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/insects_for_aichallenger.py` & `pybaseutils-1.0.8/test_py/converter/insects_for_aichallenger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/tt100k_utils.py` & `pybaseutils-1.0.8/test_py/converter/tt100k_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/ua_detrac2voc.py` & `pybaseutils-1.0.8/test_py/converter/ua_detrac2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/converter/voc_sbd2labelme.py` & `pybaseutils-1.0.8/test_py/converter/voc_sbd2labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/cython_build/build_cython.py` & `pybaseutils-1.0.8/test_py/cython_build/build_cython.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/cython_build/build_pyarmor.py` & `pybaseutils-1.0.8/test_py/cython_build/build_pyarmor.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/cython_build/cryptography_demo.py` & `pybaseutils-1.0.8/test_py/cython_build/cryptography_demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/cython_build/model_des_enctypt.py` & `pybaseutils-1.0.8/test_py/cython_build/model_des_enctypt.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/cython_build/model_enctypt.py` & `pybaseutils-1.0.8/test_py/cython_build/model_enctypt.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo1.py` & `pybaseutils-1.0.8/test_py/demo1.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     @Date   : 2024-02-05 18:19:18
     @Brief  :
 """
 import os
 import cv2
 import numpy as np
 from tqdm import tqdm
-from pybaseutils import image_utils, file_utils
+from pybaseutils import image_utils, file_utils, json_utils
 from pybaseutils.transforms import transform_utils
 from pybaseutils.converter import build_voc
 
 
 def test_transform(image_file):
     src = cv2.imread(image_file)
     mask = image_utils.get_image_mask(src)
@@ -24,9 +24,11 @@
     src = image_utils.draw_landmark(src, [src_pts], color=(255, 0, 0), vis_id=True)
     dst = image_utils.draw_landmark(dst, [dst_pts], color=(0, 255, 0), vis_id=True)
     image_utils.cv_show_image("src", src, delay=10)
     image_utils.cv_show_image("dst", dst, delay=0)
 
 
 if __name__ == '__main__':
-    image_file = "../data/mask/mask5.jpg"
-    test_transform(image_file)
+    src = {"A": 0, "B": 3, "C": 1}
+    dst = json_utils.dict_sort_by_value(src, reverse=True)
+    print(src)
+    print(dst)
```

### Comparing `pybaseutils-1.0.7/test_py/demo2.py` & `pybaseutils-1.0.8/test_py/demo2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo3.py` & `pybaseutils-1.0.8/test_py/demo3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_async_await2.py` & `pybaseutils-1.0.8/test_py/demo_async_await2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_coco_vis.py` & `pybaseutils-1.0.8/test_py/demo_coco_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_copy_files.py` & `pybaseutils-1.0.8/test_py/demo_copy_files.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_copy_files_for_voc.py` & `pybaseutils-1.0.8/test_py/demo_copy_files_for_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_ffmpy.py` & `pybaseutils-1.0.8/test_py/demo_ffmpy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_for_pair_file.py` & `pybaseutils-1.0.8/test_py/demo_for_pair_file.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_for_polygon.py` & `pybaseutils-1.0.8/test_py/demo_for_polygon.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_get_file_list.py` & `pybaseutils-1.0.8/test_py/demo_get_file_list.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_gif.py` & `pybaseutils-1.0.8/test_py/demo_gif.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_gif_video.py` & `pybaseutils-1.0.8/test_py/demo_gif_video.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_image_crop.py` & `pybaseutils-1.0.8/test_py/demo_image_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_labelme.py` & `pybaseutils-1.0.8/test_py/demo_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_metrics.py` & `pybaseutils-1.0.8/test_py/demo_metrics.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_mouse.py` & `pybaseutils-1.0.8/test_py/demo_mouse.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_nii.py` & `pybaseutils-1.0.8/test_py/demo_nii.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_pandas.py` & `pybaseutils-1.0.8/test_py/demo_pandas.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_plot.py` & `pybaseutils-1.0.8/test_py/demo_plot.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_rename.py` & `pybaseutils-1.0.8/test_py/demo_rename.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_standard_image .py` & `pybaseutils-1.0.8/test_py/demo_standard_image .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_standard_video .py` & `pybaseutils-1.0.8/test_py/demo_standard_video .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_taichi.py` & `pybaseutils-1.0.8/test_py/demo_taichi.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_video.py` & `pybaseutils-1.0.8/test_py/demo_video.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_voc_crop.py` & `pybaseutils-1.0.8/test_py/demo_voc_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_voc_vis.py` & `pybaseutils-1.0.8/test_py/demo_voc_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_word_similar.py` & `pybaseutils-1.0.8/test_py/demo_word_similar.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_worker1.py` & `pybaseutils-1.0.8/test_py/demo_worker1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/demo_worker2.py` & `pybaseutils-1.0.8/test_py/demo_worker2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/detector/demo.py` & `pybaseutils-1.0.8/test_py/detector/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/detector/detect_face_person.py` & `pybaseutils-1.0.8/test_py/detector/detect_face_person.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/detector/predet_labelme.py` & `pybaseutils-1.0.8/test_py/detector/predet_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/edit_distance/demo.py` & `pybaseutils-1.0.8/test_py/edit_distance/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/edit_distance/text_matching.py` & `pybaseutils-1.0.8/test_py/edit_distance/text_matching.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/edit_distance/text_utils.py` & `pybaseutils-1.0.8/test_py/edit_distance/text_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/flask_demo/server.py` & `pybaseutils-1.0.8/test_py/flask_demo/server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/image_correction/demo_correction_v1.py` & `pybaseutils-1.0.8/test_py/image_correction/demo_correction_v1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/image_correction/demo_correction_v2.py` & `pybaseutils-1.0.8/test_py/image_correction/demo_correction_v2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/image_correction/demo_correction_v3.py` & `pybaseutils-1.0.8/test_py/image_correction/demo_correction_v3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/kafka_worker.py` & `pybaseutils-1.0.8/test_py/kafka_worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/men_tracemalloc.py` & `pybaseutils-1.0.8/test_py/men_tracemalloc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/performance.py` & `pybaseutils-1.0.8/test_py/performance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/pose/human_pose.py` & `pybaseutils-1.0.8/test_py/pose/human_pose.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/registry/base.py` & `pybaseutils-1.0.8/test_py/registry/base.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/registry/component.py` & `pybaseutils-1.0.8/test_py/registry/component.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/registry/main.py` & `pybaseutils-1.0.8/test_py/registry/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.7/test_py/registry/register.py` & `pybaseutils-1.0.8/test_py/registry/register.py`

 * *Files identical despite different names*

